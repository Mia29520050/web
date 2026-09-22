# Bài tập Buổi 4: Design System & Responsive Web Design

Thư mục này tổng hợp toàn bộ các hoạt động từ **Buổi 3** và tích hợp đầy đủ 4 hoạt động thực hành của **Buổi 4**.

---

## 4 Hoạt động thực hành Buổi 4 đã thực hiện:

### 1. HĐ 1 — 30 phút: Bảng mã màu thông minh
- Định nghĩa các biến CSS (`CSS Variables`) tại `:root` cho:
  - Màu chính: `--color-primary: #2563eb`
  - Màu phụ: `--color-secondary: #4f46e5`
  - 3 mức xám:
    - Xám đậm: `--color-gray-dark: #1f2937`
    - Xám trung bình: `--color-gray-medium: #6b7280`
    - Xám nhạt: `--color-gray-light: #e5e7eb`
  - Nền trang: `--color-bg: #f5f7fb` và bề mặt `--color-surface: #ffffff`
- Áp dụng xuyên suốt vào giao diện Portfolio từ tuần 3.

### 2. HĐ 2 — 60 phút: Responsive Portfolio
- Bố cục mặc định trên Desktop là **2 cột** (`grid-template-columns: 260px 1fr` gồm Sidebar + Main).
- Sử dụng `@media (max-width: 767px)` để chuyển thành **1 cột** trên màn hình điện thoại di động:
  ```css
  @media (max-width: 767px) {
      .portfolio-wrapper {
          grid-template-columns: 1fr;
          grid-template-areas:
              "header"
              "sidebar"
              "main"
              "footer";
      }
      .projects {
          grid-template-columns: 1fr;
      }
  }
  ```

### 3. HĐ 3 — 30 phút: Breakpoint Challenge: Khu vực "Dịch vụ"
- Bố cục khu vực "Dịch vụ" với CSS Grid:
  - **Desktop (>1024px):** 4 cột (`repeat(4, 1fr)`)
  - **Tablet (768px - 1024px):** 2 cột (`repeat(2, 1fr)`)
  - **Mobile (<768px):** 1 cột (`1fr`)

### 4. HĐ 4 — 30 phút: Design System Refactoring
- Trích xuất toàn bộ mã màu và khoảng cách cố định (hard-coded) thành biến CSS tại `:root`:
  - Biến khoảng cách theo tỉ lệ chuẩn `8px`: `--space-1` (8px), `--space-2` (16px), `--space-3` (24px), `--space-4` (32px), `--space-5` (40px).
  - Tối ưu hóa shorthand properties và loại bỏ CSS dư thừa.

---

## Tích hợp toàn bộ hoạt động Buổi 3:
1. **Hoạt động 1:** Kỹ thuật căn giữa tuyệt đối bằng Flexbox (`justify-content: center; align-items: center;`) và bố cục CSS Grid 3 cột.
2. **Hoạt động 2:** Portfolio với hệ thống lưới tổng thể (`grid-template-areas`), danh sách Kỹ năng tự co giãn Flexbox wrap và danh sách Dự án CSS Grid.
3. **Hoạt động 3:** Checklist Debug và Refactor CSS theo tiêu chuẩn Design System.

---

## Hướng dẫn xem kết quả:
Mở file [index.html](file:///D:/bài%20tập/Bài%20tập%20buổi%204/index.html) bằng trình duyệt web bất kỳ hoặc bấm phím `F12` để kiểm tra độ tương thích responsive trên các kích thước màn hình khác nhau.
