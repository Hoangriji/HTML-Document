# Hướng Dẫn Sử Dụng Visual Studio Code Để Viết HTML

Nếu bạn muốn viết **HTML** một cách chuyên nghiệp và hiệu quả, **Visual Studio Code** (*VS Code*) là một trong những trình soạn thảo tốt nhất mà bạn nên sử dụng.

### Vậy tại sao nên chọn VS Code để viết HTML?
Không phải ngẫu nhiên mà Visual Studio Code được các lập trình viên ưa chuộng sử dụng. Visual Studio Code mang rất nhiều ưu điểm vượt trội so với bất kỳ IDE nào khác:

- [x] Là **phần mềm miễn phí**
- [x] Hỗ trợ đa nền tảng: Linux, Mac, Windows,...
- [x] Hỗ trợ đa ngôn ngữ: C/C++, C#, JavaScript, JSON, Visual Basic, HTML, CSS,...
- [x] Ít dung lượng
- [x] Tính năng mạnh mẽ
- [x] Intellisense chuyên nghiệp
- [x] Giao diện tối giản và thân thiện
- [x] Kiến trúc mạnh mẽ và người dùng có thể khai thác mở rộng

Chính vì vậy ứng dụng chuyên biên tập, soạn thảo code này trở nên phổ biến nhất hiện nay. Với việc không ngừng cải tiến và áp dụng rất nhiều các công nghệ mới, Visual Studio Code đã được các lập trình viên chứng minh độ hiệu quả trong việc lập trình. 

### Các Bước Cài Đặt Visual Studio Code

🛠 Bước 1: Tải và cài đặt VS Code từ trang chủ 👉 [Visual Studio Code](https://code.visualstudio.com/)
🛠 Bước 2: Tạo một thư mục dự án mới bằng cách chọn `File` → `New Folder`→ Đặt tên thư mục theo tên dự án
🛠 Bước 3: Vào VS Code, tạo một file HTML mới bằng cách vào `File` → `New File` rồi lưu lại với tên `index.html`

→ *Video hướng dẫn chi tiết:* [*Cách tải Visual Studio Code*](https://youtu.be/xrHn-WQhbhE?si=TLetwogqnp_mPbEq)

##### Viết các câu lệnh HTML đầu tiên trong VS Code

Mở file `index.html` (*hoặc tên file bạn đã lưu*) và nhập đoạn code sau:

``` html
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Trang HTML Đầu Tiên</title>
</head>
<body>
    <h1>Chào mừng bạn đến với VS Code!</h1>
    <p>Đây là trang HTML đầu tiên của bạn.</p>
</body>
</html>
```

Mẹo hay: Bạn có thể gõ `!` rồi nhấn `Enter`, VS Code sẽ tự động tạo một bộ khung HTML đầy đủ cho bạn! 🚀

##### Cách Chạy File HTML Trong Trình Duyệt

🔹 **Cách 1:** Mở thủ công

Nhấn chuột phải vào file `index.html` và chọn `Open with` → Chọn trình duyệt bạn muốn xem.

🔹 **Cách 2:** Dùng *Extension Live Server* (*Khuyên dùng*)
- Bước 1: Vào `Extensions` (*Ctrl + Shift + X*), tìm `Live Server` và cài đặt.
- Bước 2️: Mở file `index.html`, nhấn chuột phải và chọn `Open with Live Server`.
- Bước 3️: Trình duyệt sẽ tự động mở trang web, và mỗi lần bạn chỉnh sửa, trang sẽ tự động cập nhật!

##### Một Số Extension Hữu Ích Cho HTML trên VS Code

| Extentions | Usage |
| :--- | :--- |
| HTML CSS Support | Gợi ý code HTML và CSS tốt hơn |
| Prettier | Giúp format code đẹp hơn |
| Auto Rename Tag | Tự động đổi tên thẻ HTML khi bạn sửa |
| Live Server | Xem trước trang web trực tiếp |