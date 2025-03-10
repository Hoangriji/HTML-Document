# 🎯 ID và CLASS trong HTML
## 📌 1. Định nghĩa và Khái niệm
### Trong HTML, `id` và `class` là hai thuộc tính quan trọng được sử dụng để gán định danh (identifier) cho các phần tử trên trang web. Chúng giúp tổ chức và quản lý các phần tử dễ dàng hơn, đồng thời là cầu nối giữa HTML với CSS và JavaScript.
- 🆔 ID là :
  - ✔️Là định danh duy nhất trong tài liệu HTML.
  - ✔️ Mỗi phần tử chỉ có một `id` và không được trùng lặp với bất kỳ phần tử nào khác.
  - ✔️ Được sử dụng khi cần thao tác với một phần tử duy nhất trong CSS hoặc JavaScript.
- 🏷 CLASS là gì :
  - ✔️ Có thể được gán cho nhiều phần tử khác nhau.
  - ✔️ Dùng để nhóm các phần tử có chung thuộc tính, giúp dễ dàng áp dụng CSS hoặc xử lý bằng JavaScript.
  - ✔️ Một phần tử có thể có nhiều  `class`.
## 🔍 2. Phân biệt `id` và `class`
| Đặc điểm | `id` | `class` |
|----------|------|---------|
|Độ duy nhất|✅ Chỉ có một trong tài liệu HTMl|❌ Có thể gán cho nhiều phần tử|
|Mục đích|🎯 Xác định phần tử duy nhất|📌 Nhóm các phần tử có cùng đặc điểm|
|Cách sử dụng|🔎 Dùng để định dạng hoặc xử lý riêng một phần tử|🏗 Dùng để định dạng hoặc xử lý nhiều phần tử cùng loại|
|Cú pháp CSS|`#ten-id {}`|`.ten-class {}`|
|Cú pháp JavaScript|`document.getElementById("id")`|`document.getElementsByClassName("class")`|
## 🎨 3. Tầm quan trọng của id và class
### 🎨 Trong CSS
- `id`: Thường được sử dụng khi chỉ muốn áp dụng một kiểu duy nhất cho một phần tử.
- `class`: Được sử dụng để áp dụng cùng một kiểu cho nhiều phần tử.
### 📌 Ví dụ:
```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <style>
        #header {
            background-color: 🔵 blue;
            color: ⚪ white;
            text-align: center;
            padding: 10px;
        }
        .box {
            width: 200px;
            height: 100px;
            background-color: 🎨 lightgray;
            margin: 10px;
            text-align: center;
            line-height: 100px;
        }
    </style>
</head>
<body>
    <div id="header"> 📢 Đây là Header</div>
    <div class="box">📦 Hộp 1</div>
    <div class="box">📦 Hộp 2</div>
</body>
</html>
```
### ✅ Kết quả: 
- `#header` chỉ áp dụng cho phần tử `div` duy nhất có `id="header"`.
- `.box` áp dụng cho cả `div class="box"` (Hộp 1 & Hộp 2).
### ⚡  Trong JavaScript
- `id`: Dùng để chọn một phần tử duy nhất.
- `class`: Dùng khi cần chọn nhiều phần tử có chung đặc điểm.
### 📌 Ví dụ:
```html
<!DOCTYPE html>
<html lang="vi">
<head>
    <style>
        .btn {
            padding: 10px;
            background-color: 🟢 green;
            color: ⚪ white;
            border: none;
            cursor: pointer;
        }
    </style>
</head>
<body>

    <button id="uniqueBtn">Click ID</button>
    <button class="btn">Click Class 1</button>
    <button class="btn">Click Class 2</button>

    <script>
        // 🎯 Sử dụng ID để thay đổi nội dung nút
        document.getElementById("uniqueBtn").addEventListener("click", function() {
            this.innerHTML = "Đã Click!";
        });

        // 🔄 Sử dụng Class để thay đổi tất cả nút có cùng class
        let buttons = document.getElementsByClassName("btn");
        for (let i = 0; i < buttons.length; i++) {
            buttons[i].addEventListener("click", function() {
                this.style.backgroundColor = "red";
            });
        }
    </script>

</body>
</html>
```
### ✅ Kết quả::
- Khi bấm vào nút có `id="uniqueBtn"`, ✔️ nội dung nút sẽ thay đổi.
- Khi bấm vào các nút có `class="btn"`, màu nền sẽ đổi thành 🔴 đỏ.
## ⚖️ 4. Cú pháp và cách sử dụng hợp lý:
|Trường hợp sử dụng|`id`|`class`|
|------------------|----|-------|
|Khi cần thao tác với một phần tử duy nhất|✅|❌|
|Khi muốn áp dụng kiểu cho nhiều phần tử|❌|✅|
|Khi dùng với JavaScript để lấy một phần tử|✅ (`getElementById`)|❌|
|Khi dùng với JavaScript để lấy nhiều phần tử|❌|✅ (`getElementsByClassName`)|
#### 📌 Nguyên tắc sử dụng hợp lý:
- Dùng `id` khi chỉ có một phần tử cần xử lý.
- Dùng `class` khi có nhiều phần tử có chung kiểu hoặc chức năng.
- Không nên dùng `id` cho nhiều phần tử vì sẽ gây lỗi khi sử dụng với JavaScript.
## 🔥 5. Tổng kết
#### ✅ id là duy nhất, dùng để thao tác với một phần tử.
#### ✅ class có thể áp dụng cho nhiều phần tử, giúp nhóm các phần tử có chung đặc điểm.
#### ✅ Kết hợp id và class sẽ giúp tối ưu hóa code, tăng hiệu suất làm việc và dễ dàng bảo trì website.


## 6. Quy chuẩn đặt tên ID và Class <span style="color: red;">(Quan Trọng)</span>


### 6.1 Tại sao cần có quy chuẩn đặt tên?
Việc đặt tên ID và Class theo quy chuẩn giúp:
- **Đồng nhất**: Giúp mã nguồn dễ đọc, dễ bảo trì, tránh xung đột giữa các thành viên trong nhóm.
- **Tránh trùng lặp, xung đột**: ID cần duy nhất, còn Class có thể tái sử dụng nhưng cần có ý nghĩa rõ ràng.
- **Dễ mở rộng và bảo trì**: Khi dự án phát triển, quy chuẩn giúp dễ mở rộng hơn mà không làm rối code.
- **Hỗ trợ tìm kiếm và sửa lỗi nhanh**: Khi cần chỉnh sửa CSS hoặc JavaScript, các tên có quy chuẩn sẽ giúp tìm và sửa lỗi dễ dàng hơn.

---

### 6.2 Quy tắc đặt tên ID và Class
#### a. Đặt tên có ý nghĩa
Tên ID và Class nên phản ánh chức năng hoặc nội dung của phần tử thay vì hình thức trình bày.

✅ **Ví dụ tốt**:
```html
<header class="main-header"></header>
<nav class="primary-navigation"></nav>
<button id="submit-button">Gửi</button>
```

❌ **Ví dụ không nên**:
```html
<div class="box"></div> <!-- Không rõ nghĩa -->
<span id="red-text">Cảnh báo</span> <!-- Gắn với màu sắc, không nên -->
```

#### b. Sử dụng chữ thường và phân tách bằng dấu gạch ngang (-)

✅ **Ví dụ tốt**:
```html
<div class="user-profile"></div>
<div id="main-header"></div>
```

❌ **Ví dụ không nên**:
```html
<div class="UserProfile"></div> <!-- Viết hoa không thống nhất -->
<div class="main_header"></div> <!-- Dùng dấu gạch dưới không đồng nhất -->
```

#### c. Không dùng ký tự đặc biệt, dấu cách hoặc số ở đầu
- Không dùng khoảng trắng, dấu đặc biệt (*, $, @, !, ...).
- Không bắt đầu bằng số.

✅ **Ví dụ tốt**:
```html
<div class="sidebar-menu"></div>
```

❌ **Ví dụ không nên**:
```html
<div class="side bar menu"></div> <!-- Có dấu cách -->
<div id="123button"></div> <!-- Bắt đầu bằng số -->
```

#### d. Tránh trùng với tên thẻ HTML hoặc từ khóa JavaScript

✅ **Ví dụ tốt**:
```html
<div class="custom-button"></div>
```

❌ **Ví dụ không nên**:
```html
<div class="button"></div> <!-- Có thể gây xung đột với thẻ <button> -->
```

---

### 6.3 Quy tắc đặt tên ID
- **Duy nhất trên toàn bộ trang**: ID chỉ nên sử dụng khi cần định danh một phần tử duy nhất.
- **Sử dụng cho mục tiêu cụ thể**: ID nên dùng cho phần tử quan trọng như tiêu đề chính, biểu mẫu, liên kết nội bộ.

✅ **Ví dụ tốt**:
```html
<h1 id="page-title">Trang chủ</h1>
<form id="contact-form"></form>
```

❌ **Ví dụ không nên**:
```html
<div id="box"></div> <!-- Không rõ nghĩa -->
```

---

### 6.4 Quy tắc đặt tên Class
- **Có thể tái sử dụng**: Class được dùng khi nhiều phần tử cần có cùng kiểu dáng hoặc hành vi.
- **Không đặt theo màu sắc, kích thước trực tiếp**: Tránh gắn với thuộc tính trình bày.

✅ **Ví dụ tốt**:
```html
<p class="error-message">Lỗi đăng nhập</p>
<button class="btn-primary">Đăng ký</button>
```

❌ **Ví dụ không nên**:
```html
<p class="red-text">Lỗi đăng nhập</p> <!-- Gắn trực tiếp với màu sắc -->
<button class="big-button">Đăng ký</button> <!-- Gắn với kích thước -->
```

---

### 6.5 Quy chuẩn đặt tên theo phương pháp BEM
BEM (Block-Element-Modifier) là phương pháp đặt tên phổ biến trong dự án lớn.

#### a. Cấu trúc BEM
- **Block**: Thành phần chính, độc lập.
- **Element**: Thành phần con của Block.
- **Modifier**: Biến thể hoặc trạng thái của Block hoặc Element.

✅ **Ví dụ tốt**:
```html
<div class="menu">
  <ul class="menu__list">
    <li class="menu__item menu__item--active">Trang chủ</li>
    <li class="menu__item">Giới thiệu</li>
  </ul>
</div>
```

---

### 6.6 Kiểm tra tính hợp lệ của ID và Class
- ID và Class phải bắt đầu bằng chữ cái hoặc dấu gạch dưới (_).
- Không chứa khoảng trắng hoặc ký tự đặc biệt (trừ dấu gạch ngang - hoặc gạch dưới _).
- Có thể sử dụng công cụ như **Stylelint, ESLint** để kiểm tra tự động.

✅ **Ví dụ hợp lệ**:
```html
<div id="main-content"></div>
<div class="container-fluid"></div>
```

❌ **Ví dụ không hợp lệ**:
```html
<div id="123content"></div> <!-- Bắt đầu bằng số -->
<div class="content area"></div> <!-- Chứa khoảng trắng -->
```
---
### 6.7 Tổng kết
- **ID chỉ dùng khi cần định danh duy nhất, tránh lạm dụng.**
- **Class nên được tái sử dụng, không đặt theo màu sắc hay trình bày.**
- **Sử dụng phương pháp BEM để có cấu trúc rõ ràng.**
- **Tuân thủ quy chuẩn giúp mã nguồn dễ đọc, bảo trì và mở rộng.**
- **Việc đặt chuẩn rất quan trọng đặt biệt là khi làm việc nhóm nên phải chú ý tuân thủ theo quy tắc đặt của dự án**

---
## BÀI TẬP CỦNG CỐ KIẾN THỨC

##### Câu hỏi 1: Trong HTML, thuộc tính `id` được sử dụng để: 

a. Định dạng một phần tử duy nhất trong tài liệu HTML.<br>
b. Áp dụng một kiểu dáng CSS chung cho nhiều phần tử.<br>
c. Tạo liên kết đến một trang web khác.<br>
d. Không có chức năng gì.<br>

##### Câu hỏi 2: Trong CSS, khi sử dụng `id`, ký tự nào sẽ được dùng để chọn phần tử `có` id đó? 

a. `.`.<br>
b. `#`.<br>
c. `@`.<br>
d. `*`.<br>

##### Câu hỏi 3: Chọn câu đúng về sự khác nhau giữa id và class: 

a. `id` có thể được sử dụng nhiều lần, còn `class` chỉ được sử dụng một lần duy nhất.<br>
b. `class` có thể được áp dụng cho nhiều phần tử, còn id chỉ được áp dụng cho một phần tử duy nhất.<br>
c. `class` có độ ưu tiên cao hơn `id` trong CSS.<br>
d. `id` không thể sử dụng trong CSS.<br>

##### Câu hỏi 4: Xem đoạn mã sau và chọn câu trả lời đúng: 

``` html
<div id="my-element">
    Nội dung 1
</div>

<div id="my-element">
    Nội dung 2
</div>
```

a. Mỗi `id` chỉ định dạng một phần tử duy nhất, nên không thể có 2 phần tử cùng `id="my-element"`.<br>
b. `id` có thể lặp lại mà không có vấn đề gì.<br>
c. Cần phải thay đổi thẻ `<div>` để không bị lỗi.<br>
d. Không có lỗi cú pháp nào trong đoạn mã này.<br>

##### Câu hỏi 5: Đoạn mã sau có một lỗi khi áp dụng class trong CSS. Chọn câu trả lời đúng:

```html
<div class="highlight">
    Nội dung
</div>

<div class="highlight">
    Nội dung khác
</div>
```
```css
.highlight{
    font-weight: bold;
}

```

a. `class` không thể có dấu cách.<br>
b. `class` cần phải được sử dụng cho các phần tử khác nhau.<br>
c. Không có lỗi cú pháp nào trong mã trên.<br>
d. Bạn cần thêm dấu `#` trong CSS để chọn đúng `class`.<br>

##### Câu hỏi 6: Đoạn mã JavaScript dưới đây có mục đích gì?

```javascript
const element = document.getElementById('unique-id');
element.textContent = 'nội dung mới!';
```

a. Thay đổi nội dung văn bản của tất cả các phần tử có `id="unique-id"`.<br>
b. Thay đổi nội dung văn bản của phần tử có `id="unique-id"`.<br>
c. Tạo một phần tử mới có `id="unique-id"`.<br>
d. Đổi màu của tất cả các phần tử có `id="unique-id"`.<br>

##### Câu hỏi 7: Điền vào chỗ trống còn thiếu trong đoạn mã sau:

```html
<div class="header">Đây là phần đầu trang</div>
```
```css
________ {
  color: red;
}
```
##### Câu hỏi 8: Điền vào chỗ trống còn thiếu trong đoạn mã sau: 

```html
<div class="header" id="header-style">
```
```css
#_______ {
    border: 1px solid black;
    font-size: 20px;
}
```

##### Câu hỏi 9: Giả sử bạn muốn thay đổi màu sắc của tất cả các nút trong một trang web (ví dụ: tất cả các phần tử `<button>`), bạn sẽ sử dụng `id` hay `class`?

a. Sử dụng `id`.<br>
b. Sử dụng `class`.

##### Câu hỏi 10: Giả sử bạn muốn thay đổi màu nền của phần tử header duy nhất trên trang (ví dụ: `<header>`), bạn sẽ sử dụng id hay class?

a. Sử dụng `id`<br>
b. Sử dụng `class`

---

#### Đáp án: 
1. a. Đánh dấu một phần tử HTML duy nhất trên trang.<br>
2. b. `#`<br>
3. b. `class` có thể được áp dụng cho nhiều phần tử còn `id` chỉ được áp dụng cho một phần tử duy nhất.<br>
4. a. Mỗi `id` chỉ định dạng một phần tử duy nhất, nên không thể có 2 phần tử cùng `id="my-element"`.<br>
5. c. Không có lỗi cú pháp nào trong mã trên.<br>
6. b. Thay đổi nội dung văn bản của phần tử có `id="unique-id"`.<br>
7. *Đáp án:* `.header`.<br>
8. *Đáp án:* `header-style`.<br>
9. b. Sử dụng `class`.<br>
    > *Giải thích:*
    > - Sử dụng `class` khi bạn muốn thay đổi nhiều phần tử giống nhau.<br>
    > - `id` chỉ dùng cho một phần tử duy nhất trên trang.
10. a. Sử dụng `id`.<br>
    > *Giải thích: Sử dụng `id` khi bạn muốn chọn phần tử duy nhất trên trang (như một phần tử `header` duy nhất).