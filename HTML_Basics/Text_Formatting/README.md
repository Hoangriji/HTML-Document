# 📝 HTML Text Formatting

## 📌 1. Giới thiệu
HTML Text Formatting là cách sử dụng các thẻ HTML để định dạng văn bản trên trang web, giúp nội dung dễ đọc, rõ ràng và nhấn mạnh những phần quan trọng. Các thẻ định dạng có thể giúp in đậm, in nghiêng, gạch chân, tạo trích dẫn, chỉ số, đánh dấu văn bản, v.v

---

## 🧩 2. Các Thẻ Định Dạng Văn Bản Trong HTML

### 🔸 2.1 `<b>` và `<strong>` – In đậm
- **Cú pháp:**
```html
<b>Văn bản in đậm</b>
<strong>Văn bản quan trọng</strong>
```
- **Ghi chú:**
  - `<b>`: dùng để làm nổi bật mà không mang ý nghĩa đặc biệt.
  - `<strong>`: mang ý nghĩa nhấn mạnh nội dung.

### 🔸 2.2 `<i>` và `<em>` – In nghiêng
- **Cú pháp:**
```html
<i>Văn bản in nghiêng</i>
<em>Văn bản nhấn mạnh</em>
```
- **Ghi chú:**
  - `<i>`: in nghiêng không mang ý nghĩa đặc biệt.
  - `<em>`: nhấn mạnh nội dung, có thể ảnh hưởng đến cách đọc của trình đọc màn hình.

### 🔸 2.3 `<u>` – Gạch chân
- **Cú pháp:**
```html
<u>Văn bản gạch chân</u>
```
- **Ghi chú:** Có thể dùng để nhấn mạnh hoặc để phân biệt.

### 🔸 2.4 `<s>` và `<del>` – Gạch ngang (Xoá)
- **Cú pháp:**
```html
<s>Văn bản gạch ngang</s>
<del>Văn bản bị xóa</del>
```
- **Ghi chú:**
  - `<s>`: văn bản không còn chính xác hoặc hợp lệ.
  - `<del>`: văn bản bị xóa (thường dùng trong chỉnh sửa).

### 🔸 2.5 `<mark>` – Đánh dấu văn bản
- **Cú pháp:**
```html
<mark>Văn bản được đánh dấu</mark>
```
- **Ghi chú:** Dùng để làm nổi bật đoạn văn.

### 🔸 2.6 `<small>` – Văn bản nhỏ hơn
- **Cú pháp:**
```html
<small>Văn bản kích thước nhỏ</small>
```
- **Ghi chú:** Dùng cho chú thích hoặc thông tin phụ.

### 🔸 2.7 `<sub>` và `<sup>` – Chỉ số dưới và chỉ số trên
- **Cú pháp:**
```html
H<sub>2</sub>O
X<sup>2</sup>
```
- **Ghi chú:**
  - `<sub>`: chỉ số dưới (thường dùng trong công thức hoá học).
  - `<sup>`: chỉ số trên (thường dùng trong toán học).

### 🔸 2.8 `<blockquote>` và `<q>` – Trích dẫn
- **Cú pháp:**
```html
<blockquote>Đây là một đoạn trích dẫn dài.</blockquote>
<q>Đây là trích dẫn ngắn.</q>
```
- **Ghi chú:**
  - `<blockquote>`: trích dẫn đoạn văn dài, thường lùi vào lề.
  - `<q>`: trích dẫn ngắn, hiển thị trong dấu ngoặc kép.

---

## ❓ 3. Câu Hỏi Trắc Nghiệm

1. 🧐 Thẻ nào dùng để thể hiện văn bản quan trọng?
    - A. `<b>`
    - B. `<strong>`
    - C. `<i>`
    - D. `<u>`

2. 🧐 Thẻ nào được dùng để hiển thị văn bản bị xoá?
    - A. `<s>`
    - B. `<del>`
    - C. `<strike>`
    - D. Cả A và B

3. 🧐 Kết quả của đoạn mã sau là gì?
```html
<mark>Hello</mark>
```
    - A. In đậm chữ Hello
    - B. Gạch chân chữ Hello
    - C. Tô màu nền chữ Hello
    - D. In nghiêng chữ Hello

4. 🧐 `<em>` và `<i>` khác nhau ở điểm nào?
    - A. Không có gì khác
    - B. `<em>` mang ý nghĩa nhấn mạnh
    - C. `<i>` mang nghĩa đặc biệt
    - D. `<em>` không được hỗ trợ

5. 🧐 Thẻ nào được dùng để hiển thị chỉ số dưới?
    - A. `<sup>`
    - B. `<sub>`
    - C. `<low>`
    - D. `<min>`

6. 🧐 Thẻ `<small>` có tác dụng gì?
    - A. Làm văn bản in nghiêng
    - B. Làm văn bản nhỏ hơn bình thường
    - C. Làm văn bản đậm hơn
    - D. Không có tác dụng gì

7. 🧐 Kết quả của đoạn mã `<q>Trích dẫn</q>` là gì?
    - A. Không hiển thị gì
    - B. Hiển thị “Trích dẫn”
    - C. Hiển thị < Trích dẫn >
    - D. Hiển thị trong dấu ngoặc kép

8. 🧐 Thẻ nào thường dùng trong công thức hoá học?
    - A. `<sub>`
    - B. `<sup>`
    - C. `<strong>`
    - D. `<blockquote>`

9. 🧐 Cặp thẻ nào là để định dạng trích dẫn dài?
    - A. `<q>`
    - B. `<blockquote>`
    - C. `<quote>`
    - D. `<cite>`

10. 🧐 Thẻ `<b>` khác gì so với `<strong>`?
    - A. `<b>` nhấn mạnh hơn
    - B. `<strong>` mang ngữ nghĩa quan trọng hơn
    - C. Không có sự khác biệt
    - D. `<b>` không còn được dùng nữa

---

## 🧪 4. Bài Tập Thực Hành

### 📘 Yêu cầu:
Tạo một đoạn HTML hiển thị nội dung sau, sử dụng đúng các thẻ định dạng văn bản:

"Phương trình nổi tiếng là E = mc^2. Đây là một <trích dẫn> nổi tiếng trong vật lý. Hãy nhớ rằng <strong>kiến thức</strong> là sức mạnh."

### 💡 Gợi ý:
- Dùng `<sup>` cho mũ 2
- Dùng `<blockquote>` cho trích dẫn
- Dùng `<strong>` cho nhấn mạnh

### 🧾 Mẫu HTML tham khảo:
```html
<p>Phương trình nổi tiếng là E = mc<sup>2</sup>.</p>
<blockquote>Đây là một trích dẫn nổi tiếng trong vật lý.</blockquote>
<p>Hãy nhớ rằng <strong>kiến thức</strong> là sức mạnh.</p>
```

---

## ✅ 5. Đáp Án Trắc Nghiệm

| 📌 Câu | ✅ Đáp án |
|-------|-----------|
| 1     | B         |
| 2     | D         |
| 3     | C         |
| 4     | B         |
| 5     | B         |
| 6     | B         |
| 7     | D         |
| 8     | A         |
| 9     | B         |
| 10    | B         |

