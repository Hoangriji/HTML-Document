# Hướng Dẫn HTML Semantic và Layout Elements

## **HTML Semantic Elements Là Gì?**

Semantic elements trong HTML là các thẻ có ý nghĩa rõ ràng về nội dung bên trong. Chúng giúp trình duyệt và công cụ tìm kiếm hiểu trang web tốt hơn, cải thiện SEO và khả năng truy cập.

### **Lợi Ích Của Semantic Elements**
- **Dễ đọc, dễ hiểu:** Cấu trúc rõ ràng hơn cho người phát triển và trình duyệt.
- **Tối ưu SEO:** Công cụ tìm kiếm dễ dàng lập chỉ mục nội dung.
- **Cải thiện khả năng truy cập:** Hỗ trợ tốt hơn cho người dùng sử dụng trình đọc màn hình.

---

## **Các HTML Semantic Elements Quan Trọng**

### **1. `<header>` – Phần Đầu Trang**
Dùng để chứa logo, tiêu đề, hoặc menu điều hướng.

#### **Cách Chèn Logo trong `<header>`**
Bạn có thể chèn logo vào `<header>` bằng cách sử dụng thẻ `<img>`.

#### **Ví dụ:**
```html
<header>
    <img src="logo.png" alt="Logo Website" width="100">
    <h1>Website Của Tôi</h1>
</header>
```

**Giải thích:**
- **`<img>`**: Sử dụng để hiển thị hình ảnh logo.
  - `src`: Đường dẫn đến tệp hình ảnh.
  - `alt`: Văn bản thay thế mô tả logo (hữu ích khi hình ảnh không tải được hoặc dành cho trình đọc màn hình).
  - `width`: Đặt kích thước cho logo.

---

### **2. `<nav>` – Thanh Điều Hướng**
Dùng để chứa các liên kết điều hướng.

#### **Ví dụ:**
```html
<nav>
    <a href="#">Trang chủ</a> | <a href="#">Giới thiệu</a> | <a href="#">Liên hệ</a>
</nav>
```

---

### **3. `<section>` – Chia Nội Dung Thành Từng Phần**
Dùng để phân chia nội dung thành các phần logic.

#### **Ví dụ:**
```html
<section>
    <h2>Giới thiệu</h2>
    <p>Đây là nội dung chính.</p>
</section>
```

---

### **4. `<article>` – Nội Dung Độc Lập**
Dùng cho các bài viết, tin tức, hoặc nội dung độc lập.

#### **Ví dụ:**
```html
<article>
    <h2>Bài Viết Mới Nhất</h2>
    <p>Đây là nội dung bài viết...</p>
</article>
```

---

### **5. `<aside>` – Thông Tin Bên Lề**
Dùng cho các nội dung không phải chính, như quảng cáo, danh mục, hoặc thông tin bên lề.

#### **Ví dụ:**
```html
<aside>
    <p>Quảng cáo & Tin tức</p>
</aside>
```

---

### **6. `<footer>` – Phần Chân Trang**
Dùng để chứa thông tin bản quyền, liên hệ, hoặc các liên kết cuối trang.

#### **Ví dụ:**
```html
<footer>
    <p>&copy; 2025 Website Của Tôi</p>
</footer>
```

---

### **So Sánh Semantic vs. Non-Semantic Elements**

| **Non-Semantic** | **Semantic**        |
|-------------------|---------------------|
| `<div>`          | `<header>`          |
| `<span>`         | `<nav>`             |
| Không rõ nội dung | Cung cấp ý nghĩa rõ ràng |

---

## **HTML Layout Elements Là Gì?**

HTML Layout Elements giúp tổ chức và xây dựng bố cục trang web một cách trực quan, hợp lý.

### **Thẻ Quan Trọng Trong Layout**
- **`<header>`**: Phần đầu trang.
- **`<nav>`**: Thanh điều hướng.
- **`<section>`**: Phân chia nội dung.
- **`<article>`**: Nội dung độc lập.
- **`<aside>`**: Nội dung bên lề.
- **`<footer>`**: Phần chân trang.
- **`<div>` và `<span>`**: Nhóm và định dạng nội dung.

---

## **Ví Dụ HTML Layout Cơ Bản**

```html
<header>
    <img src="logo.png" alt="Logo Website" width="100">
    <h1>Website Của Tôi</h1>
</header>
<nav>
    <a href="#">Trang chủ</a> | <a href="#">Giới thiệu</a> | <a href="#">Liên hệ</a>
</nav>
<section>
    <h2>Giới thiệu</h2>
    <p>Đây là nội dung chính.</p>
</section>
<aside>
    <p>Thông tin bên lề.</p>
</aside>
<footer>
    <p>&copy; 2025 Website Của Tôi</p>
</footer>
```

---

## **Bài Tập**

### **10 Câu Hỏi Trắc Nghiệm**

1. Thẻ `<header>` thường được sử dụng để làm gì?
   - A. Chứa nội dung bài viết.
   - B. Chứa thông tin chân trang.
   - C. Chứa logo và tiêu đề.
   - D. Chứa thông tin bên lề.

2. Thẻ `<nav>` thường chứa gì?
   - A. Các đoạn văn bản.
   - B. Các liên kết điều hướng.
   - C. Hình ảnh.
   - D. Quảng cáo.

3. Thẻ nào dùng để phân chia nội dung thành các phần logic?
   - A. `<footer>`
   - B. `<nav>`
   - C. `<section>`
   - D. `<header>`

4. `<article>` được sử dụng khi nào?
   - A. Khi nhóm các nội dung liên quan.
   - B. Khi nội dung độc lập như bài viết hoặc tin tức.
   - C. Khi hiển thị thanh điều hướng.
   - D. Khi hiển thị thông tin bên lề.

5. Thẻ nào dùng để hiển thị quảng cáo hoặc thông tin bên lề?
   - A. `<aside>`
   - B. `<header>`
   - C. `<footer>`
   - D. `<article>`

6. Semantic elements giúp cải thiện điều gì?
   - A. Tăng tốc độ tải trang.
   - B. Hỗ trợ SEO và khả năng truy cập.
   - C. Thay đổi kiểu chữ.
   - D. Chèn hình ảnh.

7. Thẻ nào không phải là semantic element?
   - A. `<div>`
   - B. `<header>`
   - C. `<nav>`
   - D. `<footer>`

8. Thẻ `<section>` được dùng để:
   - A. Hiển thị đoạn văn bản dài.
   - B. Phân chia nội dung thành các phần.
   - C. Hiển thị nội dung bên lề.
   - D. Tạo liên kết điều hướng.

9. Phần `<footer>` thường chứa gì?
   - A. Tiêu đề chính.
   - B. Nội dung bài viết.
   - C. Thông tin bản quyền và liên hệ.
   - D. Quảng cáo.

10. Semantic elements có tác dụng gì trong SEO?
    - A. Tăng tốc độ tải trang.
    - B. Giúp công cụ tìm kiếm hiểu nội dung trang web.
    - C. Chèn hình ảnh dễ dàng hơn.
    - D. Làm đẹp giao diện.

---

### **Bài Tập Thực Hành**
Hãy tạo một bố cục HTML cơ bản với các yêu cầu sau:
1. Phần đầu trang (header) chứa logo và tiêu đề trang.
2. Thanh điều hướng (nav) với 3 liên kết: Trang chủ, Giới thiệu, Liên hệ.
3. Nội dung chính (section) bao gồm một bài viết (article) với tiêu đề và nội dung.
4. Thông tin bên lề (aside) với nội dung tùy ý.
5. Phần chân trang (footer) chứa thông tin bản quyền.

---

## **Đáp Án**

### **1. Đáp Án Trắc Nghiệm**

| Câu hỏi | Đáp án |
|---------|--------|
| 1       | C      |
| 2       | B      |
| 3       | C      |
| 4       | B      |
| 5       | A      |
| 6       | B      |
| 7       | A      |
| 8       | B      |
| 9       | C      |
| 10      | B      |

### **2. Đáp Án Bài Thực Hành**

```html
<header>
    <img src="logo.png" alt="Logo Website" width="100">
    <h1>Logo Website</h1>
    <p>Tiêu đề trang</p>
</header>
<nav>
    <a href="#">Trang chủ</a> | <a href="#">Giới thiệu</a> | <a href="#">Liên hệ</a>
</nav>
<section>
    <article>
        <h2>Tiêu đề Bài Viết</h2>
        <p>Nội dung bài viết...</p>
    </article>
</section>
<aside>
    <p>Thông tin bên lề...</p>
</aside>
<footer>
    <p>&copy; 2025 Website Của Tôi</p>
</footer>
```