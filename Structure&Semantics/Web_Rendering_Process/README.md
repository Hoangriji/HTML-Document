# Quá Trình Render Web

Khi bạn nhập một đường link và nhấn Enter, trình duyệt sẽ bắt đầu quá trình hiển thị trang web. Quá trình này bao gồm nhiều giai đoạn phức tạp, từ việc tải dữ liệu từ server đến khi trang web được hiển thị đầy đủ trên màn hình.

---

## **Quá Trình Render Web Là Gì?**

Render web là quá trình:
1. Trình duyệt nhận dữ liệu HTML, CSS, và JavaScript từ server.
2. Phân tích và xử lý các dữ liệu đó để hiển thị nội dung lên màn hình.
3. Gồm nhiều giai đoạn từ **parse HTML**, tải tài nguyên, đến tính toán bố cục và vẽ nội dung.

---

## **Các Giai Đoạn Chính Của Quá Trình Render**

### **1. Parse HTML → Tạo DOM Tree**

- Trình duyệt đọc HTML và tạo cây DOM (Document Object Model) từ các thẻ trong file HTML.

#### **Ví dụ HTML:**
```html
<!DOCTYPE html>
<html>
  <head>
    <title>Trang web đầu tiên</title>
  </head>
  <body>
    <h1>Xin chào!</h1>
    <p>Đây là một đoạn văn bản.</p>
  </body>
</html>
```

#### **Cấu trúc DOM Tree:**
```plaintext
html
├── head
│   └── title
└── body
    ├── h1
    └── p
```

---

### **2. Load External Resources (CSS/JS)**

- Khi trình duyệt gặp các thẻ `<link>` hoặc `<script>`, nó sẽ tải các tài nguyên bên ngoài (CSS/JavaScript).

#### **Ví dụ:**
```html
<link rel="stylesheet" href="style.css">
<script src="main.js" defer></script>
<script src="analytics.js" async></script>
```

#### **Cách hoạt động:**
- **`defer`**: JavaScript được tải song song nhưng thực thi sau khi HTML đã parse xong.
- **`async`**: JavaScript được tải song song và thực thi ngay khi tải xong (không chờ HTML parse xong).

---

### **3. Parse CSS → Tạo CSSOM Tree**

- CSS được phân tích cú pháp và chuyển thành CSSOM Tree (CSS Object Model), mô tả mối quan hệ giữa selector và style.

#### **Ví dụ CSS:**
```css
body {
  background-color: #f9f9f9;
}

h1 {
  color: blue;
  font-size: 24px;
}
```

#### **Cấu trúc CSSOM Tree:**
```plaintext
body {
  background-color: #f9f9f9;
}

h1 {
  color: blue;
  font-size: 24px;
}
```

---

### **4. Thực Thi JavaScript**

- JavaScript được parse, compile, và execute. Nó có thể thay đổi DOM hoặc CSSOM.

#### **Ví dụ:**
```html
<script>
  document.addEventListener('DOMContentLoaded', function () {
    document.querySelector('h1').textContent = 'Chào bạn!';
  });
</script>
```

#### **Lưu ý:**
- **`DOMContentLoaded`**: Chạy khi DOM đã sẵn sàng.
- **`window.onload`**: Chạy khi tất cả tài nguyên (ảnh, JS, CSS) đã tải xong.

---

### **5. Merge DOM + CSSOM → Render Tree**

- Tạo Render Tree bằng cách kết hợp DOM và CSSOM, nhưng bỏ qua các phần tử `display: none`.

#### **Ví dụ:**
```html
<p style="display: none;">Sẽ bị bỏ qua</p>
<p style="visibility: hidden;">Vẫn chiếm chỗ nhưng không hiển thị</p>
```

#### **Lưu ý:**
- `display: none`: Không có trong Render Tree.
- `visibility: hidden` và `opacity: 0`: Vẫn có mặt trong Render Tree.

---

### **6. Tính Toán Layout và Paint**

- Trình duyệt tính toán kích thước, vị trí của các phần tử (Layout) và vẽ chúng lên màn hình (Paint).

#### **Ví dụ CSS:**
```css
div {
  width: 100px;
  height: 100px;
  background: red;
}
```

➡️ Trình duyệt sẽ xác định vị trí div trên màn hình và hiển thị hình vuông đỏ tương ứng.

---

## **Sơ Đồ Quá Trình Render**

Dưới đây là sơ đồ minh họa quá trình render web:

```plaintext
1. Nhập URL → Gửi yêu cầu đến server
       ↓
2. Nhận HTML từ server
       ↓
3. Parse HTML → Tạo DOM Tree
       ↓
4. Tải tài nguyên (CSS/JS)
       ↓
5. Parse CSS → Tạo CSSOM Tree
       ↓
6. Thực thi JS → Cập nhật DOM/CSSOM
       ↓
7. Merge DOM + CSSOM → Tạo Render Tree
       ↓
8. Tính toán Layout
       ↓
9. Paint (Vẽ nội dung lên màn hình)
```

---

## **Tổng Kết**

| Giai đoạn          | Trình duyệt làm gì                          |
|---------------------|---------------------------------------------|
| 1. Parse HTML       | Tạo DOM Tree                               |
| 2. Load Resources   | Tải CSS/JS                                 |
| 3. Parse CSS        | Tạo CSSOM Tree                             |
| 4. Thực thi JS      | Cập nhật DOM hoặc CSSOM                    |
| 5. Tạo Render Tree  | Kết hợp DOM + CSSOM                        |
| 6. Layout & Paint   | Tính toán kích thước, vị trí và hiển thị   |

---

## **Bài Tập**

### **10 Câu Hỏi Trắc Nghiệm**

1. Giai đoạn nào tạo DOM Tree?
   - A. Parse CSS
   - B. Parse HTML
   - C. Thực thi JavaScript
   - D. Paint

2. CSSOM Tree được tạo ra từ đâu?
   - A. HTML
   - B. CSS
   - C. JavaScript
   - D. Render Tree

3. Thuộc tính nào giúp JavaScript tải song song nhưng thực thi sau khi HTML parse xong?
   - A. async
   - B. defer
   - C. preload
   - D. lazy

4. Render Tree được tạo ra từ?
   - A. DOM + CSSOM
   - B. DOM + JavaScript
   - C. CSSOM + Paint
   - D. Layout + Paint

5. `display: none` có xuất hiện trong Render Tree không?
   - A. Có
   - B. Không

6. Giai đoạn nào tính toán kích thước và vị trí các phần tử?
   - A. Parse HTML
   - B. Layout
   - C. Paint
   - D. Load Resources

7. `DOMContentLoaded` được kích hoạt khi nào?
   - A. Khi DOM sẵn sàng
   - B. Khi tất cả tài nguyên đã tải xong
   - C. Khi Render Tree được tạo
   - D. Khi Paint hoàn tất

8. `window.onload` được kích hoạt khi nào?
   - A. Khi DOM sẵn sàng
   - B. Khi tất cả tài nguyên đã tải xong
   - C. Khi Render Tree được tạo
   - D. Khi Parse HTML hoàn tất

9. Giai đoạn nào thực thi JavaScript?
   - A. Paint
   - B. Load Resources
   - C. Parse HTML
   - D. Thực thi JS

10. Giai đoạn cuối cùng của quá trình render là gì?
    - A. Parse HTML
    - B. Layout
    - C. Paint
    - D. Load Resources

---

### **Bài Tập Thực Hành**

Hãy viết đoạn HTML/CSS đơn giản mô tả một trang web với:
1. Một tiêu đề `<h1>` hiển thị "Chào mừng đến với trang web".
2. Một đoạn văn `<p>` chứa nội dung bất kỳ.
3. Một nút `<button>` có nội dung "Nhấn vào đây!".

---

## **Đáp Án**

### **1. Đáp Án Trắc Nghiệm**

| Câu hỏi | Đáp án |
|---------|--------|
| 1       | B      |
| 2       | B      |
| 3       | B      |
| 4       | A      |
| 5       | B      |
| 6       | B      |
| 7       | A      |
| 8       | B      |
| 9       | D      |
| 10      | C      |

---

### **2. Đáp Án Bài Tập Thực Hành**

```html
<!DOCTYPE html>
<html>
<head>
    <title>Trang Web Đầu Tiên</title>
</head>
<body>
    <h1>Chào mừng đến với trang web</h1>
    <p>Đây là nội dung của trang web demo.</p>
    <button>Nhấn vào đây!</button>
</body>
</html>
```