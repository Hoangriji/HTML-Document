# Hướng Dẫn HTML Forms

HTML Forms là một phần quan trọng trong việc xây dựng website, giúp thu thập dữ liệu từ người dùng và gửi đến server. Dưới đây là tài liệu tổng hợp về HTML Forms gồm cấu trúc cơ bản, các thành phần chính, cú pháp và ví dụ cụ thể.

---

## 1. **HTML Forms Là Gì?**

- HTML Forms được sử dụng để thu thập dữ liệu từ người dùng trên website.
- Tương tác với người dùng qua biểu mẫu.
- Dữ liệu nhập vào form có thể được gửi đến server để xử lý.
- Thường được kết hợp với JavaScript để xử lý và kiểm tra dữ liệu trước khi gửi.

---

## 2. **Cấu Trúc Cơ Bản Của HTML Form**

```html
<form action="/submit" method="POST">
    <label for="name">Họ và tên:</label>
    <input type="text" id="name" name="name" required>

    <label for="email">Email:</label>
    <input type="email" id="email" name="email" required>

    <label for="message">Tin nhắn:</label>
    <textarea id="message" name="message"></textarea>

    <button type="submit">Gửi</button>
</form>
```

### Giải thích:
- `<form>`: Bao bọc toàn bộ biểu mẫu, có thuộc tính `action` để chỉ định URL xử lý dữ liệu và `method` để xác định phương thức gửi dữ liệu (`POST` hoặc `GET`).
- `<label>`: Gắn nhãn cho các ô nhập liệu.
- `<input>`: Thành phần nhập dữ liệu, ví dụ: text, email, password,…
- `<textarea>`: Hộp nhập nội dung dài.
- `<button>`: Nút gửi biểu mẫu.

---

## 3. **Các Thành Phần Chính Của HTML Form**

### 3.1 `<input>` – Ô Nhập Dữ Liệu
Dùng để nhập văn bản, email, mật khẩu,...

#### Ví dụ:
```html
<label for="name">Tên:</label>
<input type="text" id="name" name="name" placeholder="Nhập tên">
```

#### Các loại phổ biến:
- `type="text"`: Nhập văn bản.
- `type="email"`: Nhập email.
- `type="password"`: Nhập mật khẩu.
- `type="number"`: Nhập số.
- `type="date"`: Nhập ngày.

---
## **Sự Kết Hợp Giữa `<label>` và `<input>`**

Thẻ `<label>` được sử dụng để gắn nhãn cho các trường nhập liệu (`<input>`) trong form. Việc kết hợp `<label>` với `<input>` giúp cải thiện khả năng truy cập (accessibility) và trải nghiệm người dùng.

### **Cách Kết Hợp**

1. **Sử dụng thuộc tính `for`:**
   - Thuộc tính `for` trong thẻ `<label>` liên kết với thuộc tính `id` của thẻ `<input>`.
   - Khi nhấp vào nhãn `<label>`, con trỏ tự động di chuyển đến trường nhập liệu tương ứng.

   **Ví dụ:**
   ```html
   <label for="name">Họ và tên:</label>
   <input type="text" id="name" name="name">
   ```

2. **Bao bọc `<input>` bên trong `<label>`:**
   - Thẻ `<label>` có thể bao bọc trực tiếp thẻ `<input>`.
   - Không cần sử dụng thuộc tính `for` trong trường hợp này.

   **Ví dụ:**
   ```html
   <label>
       Họ và tên:
       <input type="text" name="name">
   </label>
   ```

### **Tác Dụng Của `<label>`**

- Tăng khả năng truy cập cho người dùng sử dụng trình đọc màn hình (screen reader).
- Cải thiện trải nghiệm người dùng bằng cách nhấn vào nhãn để thao tác nhanh hơn.

---

### 3.2 `<textarea>` – Ô Nhập Văn Bản Dài
Dùng để nhập nội dung dài hơn một dòng.

#### Ví dụ:
```html
<label for="message">Tin nhắn:</label>
<textarea id="message" name="message" rows="4"></textarea>
```

---

### 3.3 `<select>` – Danh Sách Thả Xuống
Cho phép chọn một trong nhiều tùy chọn.

#### Ví dụ:
```html
<label for="gender">Giới tính:</label>
<select id="gender" name="gender">
    <option value="male">Nam</option>
    <option value="female">Nữ</option>
</select>
```

---

### 3.4 `<button>` – Nút Gửi Biểu Mẫu
Dùng để gửi dữ liệu.

#### Ví dụ:
```html
<button type="submit">Gửi</button>
```

---

### 3.5 `<fieldset>` & `<legend>` – Nhóm Các Trường
Dùng để nhóm các ô nhập liệu có liên quan.

#### Ví dụ:
```html
<fieldset>
    <legend>Thông tin cá nhân</legend>
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
</fieldset>
```

---

## 4. **Thuộc Tính Quan Trọng Của Form**

- `action`: Đường dẫn xử lý dữ liệu form.
- `method`: Phương thức gửi dữ liệu, gồm `GET` (dữ liệu nằm trên URL) và `POST` (gửi dữ liệu ngầm).
- `required`: Bắt buộc nhập dữ liệu.
- `placeholder`: Gợi ý nội dung nhập.
- `name`: Tên của trường dữ liệu khi gửi đến server.

---

## 5. **Bài Tập**

### 5.1 Câu Hỏi Trắc Nghiệm
1. Thuộc tính nào dùng để chỉ định URL xử lý dữ liệu form?
   - A. `action`
   - B. `method`
   - C. `placeholder`
   - D. `name`

2. Thuộc tính `required` dùng để làm gì?
   - A. Gợi ý nội dung nhập.
   - B. Bắt buộc nhập dữ liệu.
   - C. Nhóm các trường dữ liệu.
   - D. Thay đổi kiểu dữ liệu gửi.

3. `<textarea>` dùng để:
   - A. Nhập văn bản dài.
   - B. Nhập mật khẩu.
   - C. Hiển thị danh sách thả xuống.
   - D. Nhập số.

4. Thuộc tính nào bắt buộc phải có trong thẻ `<form>`?
   - A. `method`
   - B. `action`
   - C. `name`
   - D. Không bắt buộc

5. `<select>` dùng để:
   - A. Nhập văn bản.
   - B. Chọn một hoặc nhiều tùy chọn.
   - C. Hiển thị nút bấm.
   - D. Hiển thị đoạn văn.

6. Thuộc tính nào xác định phương thức gửi dữ liệu?
   - A. `action`
   - B. `method`
   - C. `name`
   - D. `required`

7. `type="email"` trong `<input>` dùng để:
   - A. Nhập văn bản.
   - B. Nhập ngày.
   - C. Nhập email.
   - D. Nhập số.

8. Thẻ nào dùng để nhóm các trường dữ liệu liên quan?
   - A. `<fieldset>`
   - B. `<group>`
   - C. `<legend>`
   - D. `<div>`

9. Thuộc tính `placeholder` dùng để:
   - A. Tạo nhãn cho ô nhập liệu.
   - B. Bắt buộc nhập dữ liệu.
   - C. Gợi ý nội dung nhập.
   - D. Gửi dữ liệu đến server.

10. Thẻ `<button>` với `type="submit"` dùng để:
    - A. Hiển thị đoạn văn.
    - B. Gửi dữ liệu.
    - C. Nhập dữ liệu.
    - D. Thay đổi kiểu dữ liệu.

---

### 5.2 Bài Tập Tự Luận
Hãy tạo một biểu mẫu HTML với các yêu cầu sau:
- Thu thập thông tin cá nhân: Tên, Email, Số điện thoại.
- Thu thập tin nhắn từ người dùng.
- Sử dụng danh sách thả xuống để chọn quốc gia.
- Nút gửi biểu mẫu.

---

## 6. **Đáp Án**

### 6.1 Đáp Án Trắc Nghiệm
### **Bảng Đáp Án**

| Câu hỏi | Đáp án |
|---------|--------|
| 1       | A      |
| 2       | B      |
| 3       | A      |
| 4       | D      |
| 5       | B      |
| 6       | B      |
| 7       | C      |
| 8       | A      |
| 9       | C      |
| 10      | B      |


### 6.2 Đáp Án Bài Tập Tự Luận
```html
<form action="/submit" method="POST">
    <fieldset>
        <legend>Thông tin cá nhân</legend>
        <label for="name">Tên:</label>
        <input type="text" id="name" name="name" required placeholder="Nhập tên của bạn">

        <label for="email">Email:</label>
        <input type="email" id="email" name="email" required placeholder="Nhập email của bạn">

        <label for="phone">Số điện thoại:</label>
        <input type="tel" id="phone" name="phone" required placeholder="Nhập số điện thoại">
    </fieldset>

    <label for="message">Tin nhắn:</label>
    <textarea id="message" name="message" rows="4" placeholder="Nhập tin nhắn"></textarea>

    <label for="country">Quốc gia:</label>
    <select id="country" name="country">
        <option value="vn">Việt Nam</option>
        <option value="us">Hoa Kỳ</option>
        <option value="jp">Nhật Bản</option>
    </select>

    <button type="submit">Gửi</button>
</form>
```