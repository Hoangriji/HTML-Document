# HTML Input Types

## 📄 Giới thiệu
Thẻ `<input>` trong HTML là một phần quan trọng để xây dựng các biểu mẫu (form). Nó cho phép người dùng nhập dữ liệu vào. Tùy vào loại dữ liệu cần nhập, thuộc tính `type` của thẻ `<input>` sẽ quyết định cách trình duyệt hiển thị và xử lý dữ liệu đó.

---

## 📊 Các Loại Input Thường Dùng

### 1. `type="text"` ✏️
**Mô tả**: Dùng để nhập văn bản ngắn như tên, địa chỉ.

**Cú pháp**:
```html
<label for="name">Tên:</label>
<input type="text" id="name" name="name" placeholder="Nhập tên của bạn">
```

---

### 2. `type="password"` 🔐
**Mô tả**: Nhập mật khẩu, hiển thị bằng dấu * hoặc •.

**Cú pháp**:
```html
<label for="password">Mật khẩu:</label>
<input type="password" id="password" name="password">
```

---

### 3. `type="email"` 📧
**Mô tả**: Nhập địa chỉ email, trình duyệt sẽ kiểm tra định dạng.

**Cú pháp**:
```html
<label for="email">Email:</label>
<input type="email" id="email" name="email">
```

---

### 4. `type="number"` 1⃣
**Mô tả**: Chỉ chấp nhận số, có thể đặt giá trị nhỏ nhất (min) và lớn nhất (max).

**Cú pháp**:
```html
<label for="age">Tuổi:</label>
<input type="number" id="age" name="age" min="18" max="60">
```

---

### 5. `type="date"` 📅
**Mô tả**: Hiển thị bảng chọn ngày.

**Cú pháp**:
```html
<label for="dob">Ngày sinh:</label>
<input type="date" id="dob" name="dob">
```

---

### 6. `type="radio"` 🔘
**Mô tả**: Chọn một trong nhiều tùy chọn.

**Cú pháp**:
```html
<label>Giới tính:</label>
<input type="radio" id="male" name="gender" value="male">
<label for="male">Nam</label>
<input type="radio" id="female" name="gender" value="female">
<label for="female">Nữ</label>
```

---

### 7. `type="checkbox"` ☑️
**Mô tả**: Chọn nhiều tùy chọn.

**Cú pháp**:
```html
<label>Sở thích:</label>
<input type="checkbox" id="sports" name="hobby" value="sports">
<label for="sports">Thể thao</label>
<input type="checkbox" id="music" name="hobby" value="music">
<label for="music">Âm nhạc</label>
```

---

### 8. `type="file"` 📂
**Mô tả**: Cho phép tải tệp lên từ máy tính.

**Cú pháp**:
```html
<label for="avatar">Chọn ảnh đại diện:</label>
<input type="file" id="avatar" name="avatar">
```

---

### 9. `type="color"` 🎨
**Mô tả**: Chọn màu từ bảng màu.

**Cú pháp**:
```html
<label for="favcolor">Chọn màu yêu thích:</label>
<input type="color" id="favcolor" name="favcolor">
```

---

### 10. `type="submit"` 📤
**Mô tả**: Nút để gửi dữ liệu form.

**Cú pháp**:
```html
<button type="submit">Gửi</button>
```

---

### 11. `type="reset"` ↺
**Mô tả**: Đặt lại toàn bộ form về giá trị mặc định.

**Cú pháp**:
```html
<input type="reset" value="Đặt lại">
```

---

### 12. `type="tel"` ☎️
**Mô tả**: Nhập số điện thoại. Trên thiết bị di động sẽ hiện bàn phím số.

**Cú pháp**:
```html
<label for="phone">Số điện thoại:</label>
<input type="tel" id="phone" name="phone">
```

---

### 13. `type="url"` 🔗
**Mô tả**: Nhập địa chỉ URL, trình duyệt có thể kiểm tra định dạng.

**Cú pháp**:
```html
<label for="website">Website:</label>
<input type="url" id="website" name="website">
```

---

### 14. `type="range"` 🌐
**Mô tả**: Tạo một thanh trượt giá trị.

**Cú pháp**:
```html
<label for="volume">Âm lượng:</label>
<input type="range" id="volume" name="volume" min="0" max="100">
```

---

## 📝 Câu Hỏi Trắc Nghiệm

1. 📧 Thuộc tính `type="email"` sẽ kiểm tra điều gì?
  - A. Định dạng email hợp lệ
  - B. Địa chỉ IP
  - C. Mật khẩu
  - D. Họ tên người dùng

2. 🔐 Để nhập mật khẩu, bạn dùng loại input nào?
  - A. text
  - B. password
  - C. hidden
  - D. email

3. 🔘 Loại input nào phù hợp để chọn giới tính?
  - A. text
  - B. checkbox
  - C. radio
  - D. select

4. ☑️ Input nào có thể chọn nhiều hơn một giá trị?
  - A. radio
  - B. text
  - C. email
  - D. checkbox

5. 🌐 Loại input nào hiển thị một thanh trượt?
  - A. number
  - B. date
  - C. range
  - D. tel

6. 📤 `type="submit"` dùng để làm gì?
  - A. Gửi form
  - B. Xóa dữ liệu
  - C. Tải tệp
  - D. Hiển thị màu

7. 📂 Input nào sử dụng để tải tệp từ máy tính?
  - A. image
  - B. file
  - C. link
  - D. media

8. ☎️ `type="tel"` khác `type="text"` ở điểm nào?
  - A. Tự động định dạng email
  - B. Có thể nhập màu sắc
  - C. Dùng để nhập URL
  - D. Trên điện thoại sẽ hiển thị bàn phím số

9. 📅 Để chọn ngày sinh, nên dùng `type` nào?
  - A. text
  - B. date
  - C. month
  - D. datetime

10. 🎨 Loại input nào giúp chọn màu sắc?
  - A. range
  - B. image
  - C. color
  - D. file

---
## 💻 Bài Tập Thực Hành

**Yêu cầu**: Tạo một form HTML có các trường:
- Họ tên
- Email
- Mật khẩu
- Ngày sinh
- Giới tính (radio)
- Sở thích (checkbox)
- Màu yêu thích
- Ảnh đại diện (file)
- Nút gửi và đặt lại form

**Gợi ý mẫu**:
```html
<form>
  <label for="fullname">Họ tên:</label>
  <input type="text" id="fullname" name="fullname"><br>

  <label for="email">Email:</label>
  <input type="email" id="email" name="email"><br>

  <label for="password">Mật khẩu:</label>
  <input type="password" id="password" name="password"><br>

  <label for="dob">Ngày sinh:</label>
  <input type="date" id="dob" name="dob"><br>

  <label>Giới tính:</label>
  <input type="radio" id="male" name="gender" value="male">
  <label for="male">Nam</label>
  <input type="radio" id="female" name="gender" value="female">
  <label for="female">Nữ</label><br>

  <label>Sở thích:</label>
  <input type="checkbox" id="music" name="hobby" value="music">
  <label for="music">Âm nhạc</label>
  <input type="checkbox" id="sports" name="hobby" value="sports">
  <label for="sports">Thể thao</label><br>

  <label for="favcolor">Màu yêu thích:</label>
  <input type="color" id="favcolor" name="favcolor"><br>

  <label for="avatar">Ảnh đại diện:</label>
  <input type="file" id="avatar" name="avatar"><br>

  <button type="submit">Gửi</button>
  <input type="reset" value="Đặt lại">
</form>
```

---

## ✅ Đáp Án Trắc Nghiệm

| Câu | Đáp án | Giải thích |
|-----|--------|-------------|
| 1   | A      | `email` sẽ kiểm tra định dạng hợp lệ như `abc@gmail.com` |
| 2   | B      | `password` hiển thị dấu * để bảo mật |
| 3   | C      | `radio` phù hợp khi chỉ chọn 1 trong nhiều lựa chọn |
| 4   | D      | `checkbox` cho phép chọn nhiều mục |
| 5   | C      | `range` tạo thanh trượt giá trị |
| 6   | A      | `submit` dùng để gửi form |
| 7   | B      | `file` dùng để upload tệp |
| 8   | D      | `tel` hiện bàn phím số trên thiết bị di động |
| 9   | B      | `date` dùng để chọn ngày |
| 10  | C      | `color` hiển thị bảng chọn màu |

---

**📅 Tham khảo thêm tại**: [W3Schools HTML Input Types](https://www.w3schools.com/html/html_form_input_types.asp)
