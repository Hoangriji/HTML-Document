## HTML Entities và Ký tự đặc biệt

### 1. HTML Entities là gì?

#### Khái niệm

HTML Entities là các mã đặc biệt giúp hiển thị ký tự mà HTML thường sử dụng làm cú pháp hoặc các ký tự không có sẵn trên bàn phím. Điều này giúp đảm bảo nội dung hiển thị đúng cách mà không làm ảnh hưởng đến mã HTML.

Ví dụ: Nếu bạn muốn hiển thị dấu "<" hoặc ">" mà không làm trình duyệt hiểu nhầm là thẻ HTML, bạn cần sử dụng `&lt;` và `&gt;`.

**Ví dụ minh họa:**

```html
<p>Hiển thị dấu nhỏ hơn và lớn hơn: <br>
       5 &lt; 10 và 10 &gt; 5
</p>
```

**Kết quả hiển thị:**

```
Hiển thị dấu nhỏ hơn và lớn hơn:
5 < 10 và 10 > 5
```

### 2. Một số HTML Entities phổ biến

#### a. Ký tự đặc biệt

- `&lt;` → < (Dấu bé hơn)
- `&gt;` → > (Dấu lớn hơn)
- `&amp;` → & (Dấu và)
- `&quot;` → " (Dấu nháy kép)
- `&apos;` → ' (Dấu nháy đơn)

#### b. Dấu bản quyền và tiền tệ

- `&copy;` → © (Bản quyền)
- `&reg;` → ® (Đã đăng ký)
- `&euro;` → € (Euro)
- `&yen;` → ¥ (Yên Nhật)
- `&pound;` → £ (Bảng Anh)
- `&cent;` → ¢ (Xu Mỹ)
- `&dollar;` → \$ (Đô la)

#### c. Khoảng trắng đặc biệt

- `&nbsp;` → Khoảng trắng không thể phá vỡ
- `&ensp;` → Khoảng trắng vừa
- `&emsp;` → Khoảng trắng dài
- `&thinsp;` → Khoảng trắng mỏng

#### d. Một số ký hiệu toán học

- `&plusmn;` → ± (Cộng trừ)
- `&times;` → × (Nhân)
- `&divide;` → ÷ (Chia)
- `&radic;` → √ (Căn bậc hai)
- `&sum;` → ∑ (Tổng)
- `&infin;` → ∞ (Vô cực)

#### e. Ký tự mũi tên

- `&larr;` → ← (Mũi tên trái)
- `&rarr;` → → (Mũi tên phải)
- `&uarr;` → ↑ (Mũi tên lên)
- `&darr;` → ↓ (Mũi tên xuống)
- `&harr;` → ↔ (Mũi tên trái phải)

### 3. Khi nào cần dùng HTML Entities?

- Khi muốn hiển thị các ký tự đặc biệt mà không bị trình duyệt hiểu sai.
- Khi nhập nội dung chứa dấu `&`, `<`, `>` để tránh lỗi HTML hoặc lỗi cú pháp.
- Khi cần tạo khoảng trắng hoặc ký tự đặc biệt không có trên bàn phím.
- Khi mã hóa nội dung đầu vào từ người dùng nhằm tránh các lỗ hổng bảo mật như **XSS (Cross-Site Scripting)**.

### 4. Cách sử dụng HTML Entities hiệu quả

- **Dùng HTML Entities để mã hóa nội dung động:** Khi nhập nội dung từ người dùng, việc mã hóa các ký tự đặc biệt giúp tránh lỗi hiển thị hoặc rủi ro bảo mật.
- **Kiểm tra khả năng hiển thị trên nhiều trình duyệt:** Không phải tất cả trình duyệt đều hỗ trợ đầy đủ mọi HTML Entity, do đó nên kiểm tra kỹ trước khi sử dụng.
- **Sử dụng mã Unicode thay cho HTML Entities khi cần thiết:** Thay vì sử dụng `&copy;`, bạn có thể sử dụng mã Unicode `&#169;` hoặc `&#xA9;`.

**Ví dụ:**

```html
&#169; (thập phân) tương đương với &copy;
&#xA9; (hex) tương đương với &copy;
```

### 5. Công cụ hỗ trợ làm việc với HTML Entities

- **HTML Entities Reference:** Các trang web như [w3schools](https://www.w3schools.com/charsets/ref_html_entities.asp) hoặc [unicode-table](https://unicode-table.com/) giúp tra cứu nhanh các HTML Entities.
- **HTML Escape Tools:** Các công cụ trực tuyến giúp tự động chuyển đổi ký tự sang HTML Entities.
- **Trình duyệt Developer Tools:** Hỗ trợ kiểm tra nhanh cách hiển thị của HTML Entities.

### 6. Tóm tắt

Việc sử dụng HTML Entities giúp đảm bảo nội dung hiển thị chính xác, đặc biệt khi làm việc với ký tự đặc biệt và bảo mật dữ liệu đầu vào. Khi xây dựng trang web hoặc làm việc với HTML, hãy luôn lưu ý đến việc sử dụng đúng cách HTML Entities để tránh các lỗi không mong muốn.

---
# Các Thuộc Tính Nâng Cao Trong HTML

HTML không chỉ cung cấp các thuộc tính cơ bản mà còn hỗ trợ nhiều thuộc tính nâng cao, giúp tăng cường khả năng tương tác và linh hoạt cho trang web. Dưới đây là một số thuộc tính nâng cao quan trọng mà bạn nên biết:

## 1. Thuộc tính `data-*`
### a. Khái niệm
Thuộc tính `data-*` cho phép bạn lưu trữ thông tin tùy chỉnh trong các phần tử HTML mà không ảnh hưởng đến cấu trúc hoặc kiểu dáng của trang. Các thuộc tính này bắt đầu bằng tiền tố `data-` và được sử dụng để gắn dữ liệu tùy chỉnh vào các phần tử HTML.

### b. Cú pháp
```html
<element data-key="value"></element>
```

### c. Ví dụ
```html
<div data-user-id="12345" data-role="admin">Người dùng: Admin</div>
```

## 2. Thuộc tính `contenteditable`
### a. Khái niệm
Cho phép chỉnh sửa nội dung trực tiếp trên trình duyệt.

### b. Ví dụ
```html
<p contenteditable="true">Bạn có thể chỉnh sửa đoạn văn này.</p>
```

## 3. Thuộc tính `hidden`
### a. Khái niệm
Thuộc tính `hidden` được sử dụng để ẩn một phần tử mà không cần CSS.

### b. Ví dụ
```html
<p hidden>Đoạn văn này bị ẩn.</p>
```

## 4. Thuộc tính `spellcheck`
### a. Khái niệm
Cho phép kiểm tra lỗi chính tả trong các nội dung nhập vào.

### b. Ví dụ
```html
<textarea spellcheck="true">Nhập văn bản...</textarea>
```

## 5. Thuộc tính `draggable`
### a. Khái niệm
Xác định liệu một phần tử có thể được kéo và thả hay không.

### b. Ví dụ
```html
<img src="image.jpg" draggable="true">
```

## 6. Thuộc tính `accesskey`
### a. Khái niệm
Định nghĩa phím tắt để truy cập nhanh đến một phần tử.

### b. Ví dụ
```html
<button accesskey="s">Lưu</button>
```

## 7. Thuộc tính `tabindex`
### a. Khái niệm
Xác định thứ tự tab của các phần tử khi điều hướng bằng bàn phím.

### b. Ví dụ
```html
<input type="text" tabindex="1">
<input type="text" tabindex="3">
<input type="text" tabindex="2">
```

## Tổng kếtkết
Việc sử dụng các thuộc tính nâng cao này giúp tối ưu trải nghiệm người dùng và làm cho trang web của bạn linh hoạt hơn.

---
# 📘 BÀI TẬP: HTML ENTITIES & CÁC THUỘC TÍNH NÂNG CAO TRONG HTML

## 🔹 Phần 1: HTML Entities

### 📝 Câu hỏi trắc nghiệm
> **Chọn đáp án đúng nhất**

1. **HTML Entities dùng để làm gì?**
   - A. Giúp hiển thị các ký tự đặc biệt trong HTML
   - B. Tăng tốc độ tải trang web
   - C. Giảm kích thước file HTML
   - D. Làm cho HTML dễ đọc hơn

2. **Ký tự `&gt;` sẽ hiển thị như thế nào trên trình duyệt?**
   - A. @
   - B. >
   - C. <
   - D. &

3. **Ký tự nào đại diện cho dấu nháy kép trong HTML Entities?**
   - A. `&apos;`
   - B. `&quot;`
   - C. `&dblquote;`
   - D. `&quote;`

4. **`&nbsp;` có tác dụng gì trong HTML?**
   - A. Tạo một dấu xuống dòng
   - B. Tạo một khoảng trắng không thể bị phá vỡ
   - C. Tạo một dòng kẻ ngang
   - D. Hiển thị dấu “&” trên trang web

5. **Khi nào cần sử dụng HTML Entities?**
   - A. Khi muốn hiển thị ký tự đặc biệt mà không ảnh hưởng đến cú pháp HTML
   - B. Khi muốn tối ưu SEO cho trang web
   - C. Khi viết CSS để trang trí văn bản
   - D. Khi muốn tăng tốc độ tải trang

### ✍️ Bài tập tự luận
Viết một đoạn HTML hiển thị nội dung sau:
- "Chào mừng bạn đến với khóa học HTML & CSS!"
- "5 < 10 và 10 > 5 là một sự thật hiển nhiên."
- "Dấu nháy kép: \" và Dấu nháy đơn: ' "

**Yêu cầu:**
- Sử dụng HTML Entities để đảm bảo nội dung hiển thị đúng.

📌 **Gợi ý đoạn HTML:**
```html
<p>Chào mừng bạn đến với khóa học HTML &amp; CSS!</p>
<p>5 &lt; 10 và 10 &gt; 5 là một sự thật hiển nhiên.</p>
<p>Dấu nháy kép: &quot; và Dấu nháy đơn: &apos;</p>
```

---

## 🔹 Phần 2: Các Thuộc Tính Nâng Cao trong HTML

### 📝 Câu hỏi trắc nghiệm
> **Chọn đáp án đúng nhất**

6. **Thuộc tính `data-*` trong HTML dùng để làm gì?**
   - A. Lưu trữ dữ liệu tùy chỉnh trong HTML
   - B. Tạo hiệu ứng động
   - C. Thay thế JavaScript
   - D. Định dạng nội dung văn bản

7. **Giá trị nào dưới đây giúp phần tử HTML có thể chỉnh sửa trực tiếp trên trình duyệt?**
   - A. `editable="yes"`
   - B. `contenteditable="true"`
   - C. `edit-mode="on"`
   - D. `modifiable="true"`

8. **Thuộc tính `hidden` có tác dụng gì?**
   - A. Ẩn một phần tử HTML nhưng vẫn chiếm không gian trên trang
   - B. Ẩn một phần tử HTML mà không chiếm không gian trên trang
   - C. Làm mờ phần tử HTML
   - D. Tăng kích thước phần tử

9. **Thuộc tính `spellcheck` dùng để kiểm tra lỗi chính tả trong phần tử nào sau đây?**
   - A. `<div>`
   - B. `<img>`
   - C. `<input>`
   - D. `<span>`

10. **Nếu muốn cho phép kéo thả một hình ảnh, ta cần sử dụng thuộc tính nào?**
    - A. `draggable="false"`
    - B. `movable="true"`
    - C. `draggable="true"`
    - D. `drag="enable"`

### ✍️ Bài tập tự luận
Viết một đoạn HTML có các yêu cầu sau:
- Một `<div>` hiển thị số user ID bằng cách sử dụng thuộc tính `data-user-id`.
- Một đoạn văn có thể chỉnh sửa nội dung trực tiếp trên trình duyệt.
- Một ô nhập liệu kiểm tra lỗi chính tả.
- Một hình ảnh có thể kéo thả được.
- Một đoạn văn bản bị ẩn bằng thuộc tính `hidden`.

📌 **Gợi ý đoạn HTML:**
```html
<div data-user-id="12345">User ID: 12345</div>
<p contenteditable="true">Click vào đây để chỉnh sửa nội dung</p>
<input type="text" spellcheck="true" placeholder="Nhập nội dung có kiểm tra lỗi chính tả...">
<img src="image.jpg" draggable="true" alt="Ảnh có thể kéo thả">
<p hidden>Đây là nội dung bị ẩn.</p>
```

📌 **Hướng dẫn:**
- Dán đoạn code vào file `.html` và chạy trên trình duyệt để kiểm tra kết quả.
- Thử chỉnh sửa nội dung của `<p contenteditable="true">` và kiểm tra tính năng kéo thả của ảnh.

---

## ✅ Đáp án & Giải thích

| Câu | Đáp án | Giải thích |
|----|--------|------------|
| 1  | A      | HTML Entities giúp hiển thị ký tự đặc biệt mà HTML thường sử dụng làm cú pháp. |
| 2  | B      | `&gt;` đại diện cho dấu `>` trong HTML. |
| 3  | B      | `&quot;` là HTML Entity cho dấu nháy kép. |
| 4  | B      | `&nbsp;` tạo một khoảng trắng không thể bị phá vỡ. |
| 5  | A      | Dùng khi cần hiển thị các ký tự đặc biệt mà không ảnh hưởng đến mã HTML. |
| 6  | A      | `data-*` lưu trữ thông tin tùy chỉnh mà không ảnh hưởng đến HTML tiêu chuẩn. |
| 7  | B      | `contenteditable="true"` giúp chỉnh sửa nội dung trực tiếp. |
| 8  | B      | `hidden` ẩn phần tử mà không chiếm không gian trên trang. |
| 9  | C      | `spellcheck="true"` dùng cho các thẻ nhập liệu như `<input>`. |
| 10 | C      | `draggable="true"` cho phép kéo thả phần tử. |
