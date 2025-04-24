# Hướng Dẫn HTML Block và Inline Elements

## **HTML Block và Inline Elements Là Gì?**

### **1. Block Elements (Phần Tử Khối)**

Block elements là các phần tử HTML chiếm toàn bộ chiều rộng của container (khối chứa nó) và luôn bắt đầu trên một dòng mới. Chúng thường được sử dụng để định dạng bố cục trang web, như các phần, đoạn văn, hoặc tiêu đề.

#### **Đặc điểm:**
- Chiếm toàn bộ chiều rộng của container.
- Luôn bắt đầu trên một dòng mới.
- Có thể chứa các block elements khác hoặc inline elements.
- Thường được sử dụng để tạo bố cục trang.

#### **Ví dụ Block Elements phổ biến:**
```html
<div>Đây là một phần tử block</div>
<p>Đây là một đoạn văn</p>
<h1>Đây là tiêu đề lớn</h1>
```

#### **Cách Sử Dụng:**
Block elements được dùng để tổ chức bố cục trang, nhóm nội dung, hoặc tạo phần.

---

### **2. Inline Elements (Phần Tử Nội Tuyến)**

Inline elements là các phần tử HTML chỉ chiếm không gian cần thiết để hiển thị nội dung của chúng và không bắt đầu trên một dòng mới. Chúng thường được sử dụng để định dạng văn bản.

#### **Đặc điểm:**
- Chỉ chiếm không gian vừa đủ với nội dung bên trong.
- Không bắt đầu trên một dòng mới.
- Không thể chứa block elements.
- Thường được sử dụng để định dạng văn bản.

#### **Ví dụ Inline Elements phổ biến:**
```html
<span>Đây là một phần tử inline</span>
<a href="#">Đây là một liên kết</a>
<strong>Đây là văn bản in đậm</strong>
```

#### **Cách Sử Dụng:**
Inline elements thường được dùng để chỉnh sửa hoặc định dạng nội dung chi tiết trong đoạn văn.

---

### **3. So Sánh Block vs Inline Elements**

| **Đặc điểm**                      | **Block Elements**         | **Inline Elements**         |
|------------------------------------|----------------------------|-----------------------------|
| **Chiếm toàn bộ chiều rộng**       | Có                         | Không                       |
| **Bắt đầu dòng mới**               | Có                         | Không                       |
| **Chứa được block elements khác** | Có                         | Không                       |
| **Chủ yếu dùng để**                | Định dạng bố cục           | Định dạng nội dung văn bản  |

---

## **Kết Hợp Block và Inline Elements**

Block và Inline elements có thể kết hợp với nhau để tạo nên cấu trúc nội dung phức tạp.

#### **Ví dụ:**
```html
<div>
    <h2>Tiêu đề</h2>
    <p>Đây là một đoạn văn có <strong>chữ in đậm</strong> và <a href="#">một liên kết</a>.</p>
</div>
```

**Giải thích:**
- `<div>`: Phần tử block chứa toàn bộ cấu trúc.
- `<h2>`: Tiêu đề (block element).
- `<p>`: Đoạn văn (block element).
- `<strong>`: Văn bản in đậm (inline element).
- `<a>`: Liên kết (inline element).

---

## **Bài Tập**

### **10 Câu Hỏi Trắc Nghiệm**

1. Block elements có đặc điểm nào sau đây?
   - A. Không chiếm toàn bộ chiều rộng.
   - B. Không bắt đầu dòng mới.
   - C. Chiếm toàn bộ chiều rộng và bắt đầu dòng mới.
   - D. Chỉ dùng để định dạng văn bản.

2. Inline elements có thể chứa block elements không?
   - A. Có.
   - B. Không.

3. Thẻ `<div>` thuộc loại nào?
   - A. Inline element.
   - B. Block element.

4. Thẻ `<span>` thuộc loại nào?
   - A. Inline element.
   - B. Block element.

5. Inline elements thường được sử dụng để:
   - A. Tạo bố cục trang web.
   - B. Định dạng văn bản.
   - C. Tạo các khối nội dung.

6. Block elements có thể chứa inline elements không?
   - A. Có.
   - B. Không.

7. Thẻ `<h1>` thuộc loại nào?
   - A. Inline element.
   - B. Block element.

8. Thẻ nào sau đây KHÔNG phải là block element?
   - A. `<div>`
   - B. `<p>`
   - C. `<a>`
   - D. `<h2>`

9. Thẻ nào sau đây là inline element?
   - A. `<strong>`
   - B. `<div>`
   - C. `<p>`
   - D. `<h1>`

10. Kết hợp block và inline elements có thể giúp:
    - A. Tạo cấu trúc nội dung phức tạp.
    - B. Làm cho trang web tải nhanh hơn.
    - C. Tăng tốc độ xử lý trình duyệt.

---

### **Bài Tập Thực Hành**

Hãy tạo một đoạn HTML gồm:
1. Một khối `<div>` chứa:
   - Một tiêu đề `<h1>` với nội dung "Giới thiệu".
   - Một đoạn văn `<p>` với nội dung tùy ý, trong đó có:
     - Một chữ in đậm sử dụng `<strong>`.
     - Một liên kết sử dụng `<a>`.

---

## **Đáp Án**

### **1. Đáp Án Trắc Nghiệm**

| Câu hỏi | Đáp án |
|---------|--------|
| 1       | C      |
| 2       | B      |
| 3       | B      |
| 4       | A      |
| 5       | B      |
| 6       | A      |
| 7       | B      |
| 8       | C      |
| 9       | A      |
| 10      | A      |

### **2. Đáp Án Bài Tập Thực Hành**

```html
<div>
    <h1>Giới thiệu</h1>
    <p>
        Đây là một đoạn văn có <strong>chữ in đậm</strong> và 
        <a href="#">một liên kết</a>.
    </p>
</div>
```