# Hướng Dẫn HTML Tables

## **HTML Tables Là Gì?**

HTML Tables được sử dụng để hiển thị dữ liệu dưới dạng bảng, giúp nội dung dễ đọc, được tổ chức khoa học và dễ dàng so sánh.

---

## **Cấu Trúc Bảng Cơ Bản**

### **Các Thành Phần Chính Của Bảng**
- **`<table>`**: Định nghĩa bảng.
- **`<tr>`**: Định nghĩa một hàng trong bảng.
- **`<th>`**: Định nghĩa tiêu đề cột (ô tiêu đề).
- **`<td>`**: Định nghĩa ô dữ liệu (ô thông thường).

---

### **Ví Dụ Cơ Bản**

#### **Tạo Bảng Đơn Giản**
```html
<table border="1">
    <tr>
        <th>Tên</th>
        <th>Tuổi</th>
        <th>Thành phố</th>
    </tr>
    <tr>
        <td>Hưng</td>
        <td>25</td>
        <td>Hà Nội</td>
    </tr>
    <tr>
        <td>Linh</td>
        <td>23</td>
        <td>TP.HCM</td>
    </tr>
</table>
```

**Giải thích:**
- `<th>`: Tiêu đề của các cột (Tên, Tuổi, Thành phố).
- `<tr>`: Tạo hàng trong bảng.
- `<td>`: Hiển thị dữ liệu trong từng ô.

---

### **Hợp Nhất Cột và Hàng**
HTML Tables cho phép bạn hợp nhất nhiều cột hoặc hàng bằng thuộc tính `colspan` và `rowspan`.

#### **Ví Dụ Sử Dụng `colspan` và `rowspan`**
```html
<table border="1">
    <tr>
        <th colspan="2">Họ và Tên</th>
        <th>Tuổi</th>
    </tr>
    <tr>
        <td colspan="2">Trần Tuấn Hưng</td>
        <td>25</td>
    </tr>
    <tr>
        <td rowspan="2">Linh</td>
        <td>23</td>
        <td>TP.HCM</td>
    </tr>
</table>
```

**Giải thích:**
- `colspan="2"`: Gộp hai cột thành một ô.
- `rowspan="2"`: Gộp hai hàng thành một ô.

---

## **Lợi Ích Khi Sử Dụng HTML Tables**
- **Hiển thị dữ liệu trực quan**: Tổ chức dữ liệu dạng bảng dễ đọc và so sánh.
- **Sắp xếp dữ liệu khoa học**: Hỗ trợ phân nhóm thông tin.
- **Tích hợp dễ dàng**: Có thể kết hợp với các công nghệ khác như CSS để làm đẹp hoặc JavaScript để tương tác.

---

## **Bài Tập**

### **10 Câu Hỏi Trắc Nghiệm**

1. Phần tử nào dùng để định nghĩa bảng trong HTML?
   - A. `<table>`
   - B. `<tr>`
   - C. `<td>`
   - D. `<th>`

2. Phần tử nào dùng để tạo hàng trong bảng?
   - A. `<table>`
   - B. `<tr>`
   - C. `<td>`
   - D. `<th>`

3. Phần tử nào dùng để định nghĩa ô tiêu đề (header cell)?
   - A. `<table>`
   - B. `<tr>`
   - C. `<td>`
   - D. `<th>`

4. Phần tử nào dùng để định nghĩa ô dữ liệu thông thường?
   - A. `<table>`
   - B. `<tr>`
   - C. `<td>`
   - D. `<th>`

5. Thuộc tính nào được sử dụng để gộp hai cột thành một ô?
   - A. `colspan`
   - B. `rowspan`
   - C. `merge`
   - D. `combine`

6. Thuộc tính nào được sử dụng để gộp hai hàng thành một ô?
   - A. `colspan`
   - B. `rowspan`
   - C. `merge`
   - D. `combine`

7. Trong đoạn mã dưới đây, số lượng hàng (rows) của bảng là bao nhiêu?
   ```html
   <table>
       <tr>
           <th>Tên</th>
           <th>Tuổi</th>
       </tr>
       <tr>
           <td>Hưng</td>
           <td>25</td>
       </tr>
       <tr>
           <td>Linh</td>
           <td>23</td>
       </tr>
   </table>
   ```
   - A. 2
   - B. 3
   - C. 4
   - D. 5

8. Thuộc tính nào giúp tạo đường viền cho bảng?
   - A. `border`
   - B. `style`
   - C. `width`
   - D. `padding`

9. Trong HTML Tables, thẻ `<tr>` có thể chứa phần tử nào?
   - A. `<table>`
   - B. `<th>` và `<td>`
   - C. `<div>`
   - D. `<span>`

10. Kết hợp `<th>` và `<td>` trong bảng giúp:
    - A. Làm đẹp bảng.
    - B. Trình bày dữ liệu trực quan hơn.
    - C. Tăng tốc độ tải trang.
    - D. Làm cho bảng tương tác tốt hơn.

---

### **Bài Tập Thực Hành**

Hãy tạo một bảng HTML với các yêu cầu sau:
1. Tiêu đề bảng: "Danh Sách Sinh Viên".
2. Có 3 cột: Tên, Tuổi, Điểm Trung Bình.
3. Có 3 hàng dữ liệu:
   - Hàng 1: Nguyễn Văn A, 20, 8.5
   - Hàng 2: Trần Thị B, 21, 9.0
   - Hàng 3: Lê Văn C, 22, 7.5

---

## **Đáp Án**

### **1. Đáp Án Trắc Nghiệm**

| Câu hỏi | Đáp án |
|---------|--------|
| 1       | A      |
| 2       | B      |
| 3       | D      |
| 4       | C      |
| 5       | A      |
| 6       | B      |
| 7       | B      |
| 8       | A      |
| 9       | B      |
| 10      | B      |

---

### **2. Đáp Án Bài Tập Thực Hành**

```html
<table border="1">
    <caption>Danh Sách Sinh Viên</caption>
    <tr>
        <th>Tên</th>
        <th>Tuổi</th>
        <th>Điểm Trung Bình</th>
    </tr>
    <tr>
        <td>Nguyễn Văn A</td>
        <td>20</td>
        <td>8.5</td>
    </tr>
    <tr>
        <td>Trần Thị B</td>
        <td>21</td>
        <td>9.0</td>
    </tr>
    <tr>
        <td>Lê Văn C</td>
        <td>22</td>
        <td>7.5</td>
    </tr>
</table>
```