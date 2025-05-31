# 📜 HTML Attributes

## 🔹 HTML Attributes Là Gì?

HTML Attributes (thuộc tính HTML) cung cấp thông tin bổ sung cho các thẻ HTML. Chúng giúp điều khiển cách nội dung hiển thị và hoạt động trên trang web.


---

## 🔹 Danh Sách Các HTML Attributes Phổ Biến (Cú pháp + Ví dụ)

### 📌 Thuộc tính điều hướng:

#### `href`
- **Cú pháp:** `<a href="URL">Nội dung</a>`
- **Ví dụ:**
```html
<a href="https://example.com">Trang chủ</a>
```

#### `target`# Hướng Dẫn Về HTML Attributes

## 🔹 HTML Attributes Là Gì?

HTML Attributes (thuộc tính HTML) cung cấp thông tin bổ sung cho các thẻ HTML. Chúng giúp điều khiển cách nội dung hiển thị và hoạt động trên trang web.

### ✅ Cú pháp:
- Luôn được khai báo trong thẻ mở.
- Có giá trị nằm trong dấu ngoặc kép (`" "`).
- Một thẻ có thể có nhiều thuộc tính.

### 🧩 Ví dụ cơ bản:
```html
<a href="https://www.google.com/" target="_blank">Truy cập Google</a>
```
- `href`: Xác định đường dẫn liên kết.
- `target="_blank"`: Mở liên kết trong tab mới.

---

## 🔹 Danh Sách Các HTML Attributes Phổ Biến (Cú pháp + Ví dụ + Giải thích)

### 📌 Thuộc tính điều hướng:

#### `href` (Xác định địa chỉ URL mà thẻ `<a>` sẽ liên kết đến)
- **Cú pháp:** `<a href="URL">Nội dung</a>`
- **Ví dụ:**
```html
<a href="https://example.com">Trang chủ</a>
```

#### `target` (Xác định nơi hiển thị liên kết được mở, ví dụ: tab mới)
- **Cú pháp:** `<a target="_blank">...</a>`
- **Ví dụ:**
```html
<a href="https://example.com" target="_blank">Mở tab mới</a>
```

#### `download` (Cho phép người dùng tải tệp về khi nhấp vào liên kết)
- **Cú pháp:** `<a href="file.pdf" download>...</a>`
- **Ví dụ:**
```html
<a href="report.pdf" download>Tải về báo cáo</a>
```

#### `rel` (Xác định mối quan hệ giữa tài liệu hiện tại và tài liệu được liên kết)
- **Cú pháp:** `<a rel="nofollow">...</a>`
- **Ví dụ:**
```html
<a href="https://example.com" rel="noopener">Liên kết an toàn</a>
```

---

### 🖼️ Thuộc tính hình ảnh:

#### `src` (Đường dẫn tới tệp hình ảnh)
- **Cú pháp:** `<img src="link">`
- **Ví dụ:**
```html
<img src="image.jpg" alt="Mô tả ảnh">
```

#### `alt` (Văn bản thay thế nếu hình ảnh không hiển thị; hỗ trợ truy cập và SEO)
- **Cú pháp:** `<img alt="mô tả">`
- **Ví dụ:**
```html
<img src="logo.png" alt="Logo công ty">
```

#### `width` và `height` (Xác định chiều rộng và chiều cao của hình ảnh)
- **Cú pháp:** `<img width="100" height="100">`
- **Ví dụ:**
```html
<img src="icon.png" width="64" height="64">
```

#### `loading` (Tối ưu hiệu suất bằng cách trì hoãn tải hình ảnh - lazy loading)
- **Cú pháp:** `<img loading="lazy">`
- **Ví dụ:**
```html
<img src="large.jpg" loading="lazy" alt="Ảnh lớn">
```

---

### 🖋️ Thuộc tính văn bản:

#### `title` (Hiển thị chú giải khi di chuột qua phần tử)
- **Cú pháp:** `<p title="Gợi ý">Nội dung</p>`
- **Ví dụ:**
```html
<p title="Thông tin thêm">Di chuột vào tôi</p>
```

#### `lang` (Xác định ngôn ngữ của nội dung)
- **Cú pháp:** `<p lang="en">Text</p>`
- **Ví dụ:**
```html
<p lang="fr">Bonjour le monde</p>
```

#### `dir` (Xác định hướng văn bản: ltr, rtl)
- **Cú pháp:** `<p dir="rtl">Text</p>`
- **Ví dụ:**
```html
<p dir="rtl">نص باللغة العربية</p>
```

#### `style` (Áp dụng CSS trực tiếp lên phần tử HTML)
- **Cú pháp:** `<element style="property: value">`
- **Ví dụ:**
```html
<p style="color: red; font-size: 18px;">Đoạn văn</p>
```

---

### 🆔 Thuộc tính định danh:

#### `id` (Xác định phần tử duy nhất, dùng cho CSS, JavaScript)
- **Cú pháp:** `<element id="unique">`
- **Ví dụ:**
```html
<div id="header">Phần đầu trang</div>
```

#### `class` (Gán phần tử vào một hoặc nhiều lớp CSS)
- **Cú pháp:** `<element class="ten-lop">`
- **Ví dụ:**
```html
<p class="text-primary">Đoạn văn</p>
```

---

### 🎛️ Thuộc tính cho biểu mẫu:

#### `type` (Xác định loại trường nhập liệu)
- **Cú pháp:** `<input type="text">`
- **Ví dụ:**
```html
<input type="email">
```

#### `name` (Gán tên cho trường nhập, gửi dữ liệu đi)
- **Cú pháp:** `<input name="email">`
- **Ví dụ:**
```html
<input type="text" name="username">
```

#### `value` (Giá trị mặc định được hiển thị)
- **Cú pháp:** `<input value="nội dung">`
- **Ví dụ:**
```html
<input type="text" value="Mặc định">
```

#### `placeholder` (Gợi ý nội dung người dùng cần nhập)
- **Cú pháp:** `<input placeholder="gợi ý">`
- **Ví dụ:**
```html
<input type="text" placeholder="Nhập họ tên">
```

#### `required` (Bắt buộc nhập dữ liệu vào trường)
- **Cú pháp:** `<input required>`
- **Ví dụ:**
```html
<input type="text" required>
```

#### `readonly` (Trường nhập không thể chỉnh sửa)
- **Cú pháp:** `<input readonly>`
- **Ví dụ:**
```html
<input type="text" value="Chỉ đọc" readonly>
```

#### `disabled` (Trường bị vô hiệu hóa, không tương tác được)
- **Cú pháp:** `<input disabled>`
- **Ví dụ:**
```html
<input type="text" value="Không hoạt động" disabled>
```

#### `checked` (Được chọn sẵn với checkbox/radio)
- **Cú pháp:** `<input type="checkbox" checked>`
- **Ví dụ:**
```html
<input type="checkbox" checked> Tôi đồng ý
```

#### `maxlength` (Giới hạn số ký tự tối đa)
- **Cú pháp:** `<input maxlength="số">`
- **Ví dụ:**
```html
<input type="text" maxlength="10">
```

#### `min`, `max`, `step` (Giới hạn giá trị số và bước nhảy)
- **Cú pháp:** `<input type="number" min="0" max="10" step="2">`
- **Ví dụ:**
```html
<input type="number" min="1" max="100" step="5">
```

#### `autocomplete` (Cho phép trình duyệt tự động điền thông tin)
- **Cú pháp:** `<input autocomplete="on|off">`
- **Ví dụ:**
```html
<input type="text" autocomplete="on">
```

---

### 🧭 Các thuộc tính đa mục đích:

#### `hidden` (Ẩn phần tử khỏi hiển thị mà không xoá khỏi DOM)
- **Cú pháp:** `<element hidden>`
- **Ví dụ:**
```html
<p hidden>Nội dung này bị ẩn</p>
```

#### `tabindex` (Thiết lập thứ tự khi nhấn phím Tab)
- **Cú pháp:** `<element tabindex="số">`
- **Ví dụ:**
```html
<input type="text" tabindex="1">
```

#### `draggable` (Cho phép kéo thả phần tử)
- **Cú pháp:** `<element draggable="true">`
- **Ví dụ:**
```html
<div draggable="true">Kéo tôi</div>
```

#### `spellcheck` (Bật/tắt kiểm tra chính tả trong nội dung)
- **Cú pháp:** `<element spellcheck="true|false">`
- **Ví dụ:**
```html
<p spellcheck="true">Kiểm tra chính tả</p>
```

#### `contenteditable` (Cho phép chỉnh sửa nội dung trực tiếp trong trình duyệt)
- **Cú pháp:** `<element contenteditable="true">`
- **Ví dụ:**
```html
<div contenteditable="true">Bạn có thể chỉnh sửa nội dung này</div>
```

---


## 🔥 Kết Luận

HTML Attributes giúp trang web trở nên linh hoạt, tương tác và dễ kiểm soát hơn. Hãy luyện tập thường xuyên để nắm vững cách sử dụng nhé!

🔗 Link tham khảo: [HTML Attributes - W3Schools](https://www.w3schools.com/html/html_attributes.asp)

---

## ❓ 10 Câu Hỏi Trắc Nghiệm Ôn Tập

1. Thuộc tính `href` được sử dụng với thẻ nào sau đây?
    a) `<img>`  
    b) `<a>`  
    c) `<p>`  
    d) `<div>`

2. `target="_blank"` có tác dụng gì?
    a) Mở liên kết trong cùng tab  
    b) Mở liên kết trong cửa sổ mới  
    c) Mở liên kết trong tab mới  
    d) Không có tác dụng gì

3. Thuộc tính nào dùng để hiển thị gợi ý nhập liệu trong ô input?
    a) `value`  
    b) `alt`  
    c) `placeholder`  
    d) `title`

4. `style="color: red;"` có tác dụng gì?
    a) Thay đổi kích thước văn bản  
    b) Làm văn bản nghiêng  
    c) Đặt màu văn bản là đỏ  
    d) Không có tác dụng

5. `alt` là thuộc tính dành cho thẻ nào?
    a) `<a>`  
    b) `<p>`  
    c) `<img>`  
    d) `<input>`

6. `id` khác `class` ở điểm nào?
    a) `id` dùng được nhiều lần, `class` thì không  
    b) `id` là duy nhất, `class` có thể lặp lại  
    c) Cả hai giống nhau  
    d) `class` không dùng trong HTML

7. Thuộc tính `src` dùng để làm gì?
    a) Thêm liên kết  
    b) Chèn hình ảnh hoặc tài nguyên  
    c) Tạo input  
    d) Không có tác dụng

8. Thẻ nào KHÔNG sử dụng được thuộc tính `href`?
    a) `<a>`  
    b) `<link>`  
    c) `<img>`  
    d) `<area>`

9. `title` hiển thị nội dung ở đâu?
    a) Trên đầu trình duyệt  
    b) Dưới chân trang  
    c) Khi di chuột vào phần tử  
    d) Không hiển thị

10. Thuộc tính nào sau đây không phải của thẻ `<input>`?
    a) `type`  
    b) `placeholder`  
    c) `src`  
    d) `value`

---

## 🧪 Bài Tập Thực Hành

### Đề bài:
Tạo một biểu mẫu HTML có chứa:
- Một ô nhập tên (bắt buộc nhập).
- Một ô nhập email với gợi ý "Nhập email của bạn".
- Một ô nhập số có giới hạn từ 1 đến 100 và bước nhảy là 5.
- Một checkbox được chọn sẵn.
- Một nút gửi.

### Hướng dẫn làm:
1. Sử dụng thẻ `<form>` để bao toàn bộ nội dung.
2. Dùng `<input type="text" required>` cho tên.
3. Dùng `<input type="email" placeholder="Nhập email của bạn">` cho email.
4. Dùng `<input type="number" min="1" max="100" step="5">` cho số.
5. Dùng `<input type="checkbox" checked>` cho checkbox.
6. Dùng `<button type="submit">Gửi</button>` để tạo nút gửi.

### Bài mẫu:
```html
<form>
  <label>Họ tên:</label>
  <input type="text" required><br><br>

  <label>Email:</label>
  <input type="email" placeholder="Nhập email của bạn"><br><br>

  <label>Chọn số:</label>
  <input type="number" min="1" max="100" step="5"><br><br>

  <label>
    <input type="checkbox" checked> Tôi đồng ý
  </label><br><br>

  <button type="submit">Gửi</button>
</form>
```


---

## ✅ Đáp Án Câu Hỏi Trắc Nghiệm

| Câu hỏi | Đáp án đúng |
|---------|--------------|
| 1       | b            |
| 2       | c            |
| 3       | c            |
| 4       | c            |
| 5       | c            |
| 6       | b            |
| 7       | b            |
| 8       | c            |
| 9       | c            |
| 10      | c            |

