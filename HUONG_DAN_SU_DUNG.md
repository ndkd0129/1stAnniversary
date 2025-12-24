# HƯỚNG DẪN SỬ DỤNG - NOEL 3D PRO & ANNIVERSARY

Chào mừng bạn đến với ứng dụng Tương tác 3D Noel & Anniversary! Dưới đây là hướng dẫn chi tiết cách sử dụng và tùy biến.

## 1. Cách Sử Dụng (Người Dùng Xem)

### Thao tác Cơ bản
-   **Xoay Hũ Tuyết:** Nhấn giữ chuột trái và kéo (trên máy tính) hoặc vuốt ngón tay (trên điện thoại).
-   **Phóng to / Thu nhỏ:** Lăn chuột giữa.

### Các Chế độ Hiển thị
1.  **Chế độ Mặc định (Hũ Tuyết):**
    -   Hiển thị hũ cầu tuyết 3D xoay tròn.
2.  **Chế độ Xem Ảnh (Gallery Mode):**
    -   **Cách vào:** Click chuột trái (hoặc chạm nhẹ) vào màn hình một lần. Camera sẽ zoom vào các tấm ảnh Polaroid.
    -   **Cách thoát:** Click/chạm lại lần nữa để quay về chế độ Hũ Tuyết.
3.  **Chế độ Pháo Hoa (Anniversary Mode):**
    -   **Cách kích hoạt:**
        -   **Trên máy tính:** Khi đang ở **Chế độ Xem Ảnh**, nhấn **Chuột Phải** (Right Click) hoặc nhấn phím **Enter**.
        -   **Trên điện thoại:** Nhấn giữ lâu vào màn hình.
    -   **Hiệu ứng:** Màn hình chuyển sang nền tối, chữ "Happy 1st Anniversary" & tên "Khâyy Du ❤️ Mỹ Thoee" hiện ra cùng pháo hoa.
    -   **Thoát:** Nhấn **Enter** hoặc chạm vào màn hình.

---

## 2. Hướng Dẫn Tùy Biến (Dành cho Admin/Dev)

### A. Thay Đổi Ảnh Kỷ Niệm
1.  Chuẩn bị **28 tấm ảnh** đẹp nhất của bạn.
2.  Đổi tên các file ảnh thành số thứ tự từ `1` đến `28` (ví dụ: `1.jpg`, `2.png`, `15.jpeg`...).
    -   *Lưu ý:* Mã nguồn hỗ trợ cả đuôi `.png`, `.jpg`, `.jpeg`.
3.  Copy và ghi đè toàn bộ ảnh vào thư mục `images/` của dự án.
    -   *Lời khuyên:* Nên dùng ảnh tỉ lệ dọc hoặc vuông để hiển thị đẹp nhất trong khung Polaroid. Chế độ hiển thị hiện tại là **Full Cover** (Tràn viền) nên ảnh sẽ tự động được cắt chỉnh cho vừa khung.

### B. Thay Đổi Nhạc Nền
1.  Chuẩn bị file nhạc bạn thích (định dạng `.mp3`).
2.  Đổi tên file thành `audio.mp3`.
3.  Copy đè vào thư mục gốc của dự án (nơi chứa file `index.html`).

### C. Sửa Tên & Lời Chúc
Mở file `index.html` bằng phần mềm chỉnh sửa code (Notepad, VS Code...) và tìm các dòng sau để sửa:

1.  **Sửa Tên hiển thị:**
    -   Tìm dòng: `<div class="sm-line-names">Khâyy Du ... Mỹ Thoee</div>` (khoảng dòng 459).
    -   Thay nội dung tên bạn muốn vào giữa các thẻ `<div>`.

2.  **Sửa Lời Chúc (Anniversary):**
    -   Tìm các dòng chứa chữ `Happy`, `1st`, `Anniversary` (gần dòng 456-458) để sửa nội dung text.

3.  **Sửa Lời Bài Hát (Subtitle):**
    -   Tìm đoạn `const LYRICS_DATA` (trong phần `<script>`, khoảng dòng 416).
    -   Sửa thời gian (`time`) và nội dung lời bài hát (`text`) tương ứng.

---

## 3. Một số Lưu ý Kỹ thuật
-   **Chất lượng ảnh:** Dự án đã được tối ưu hiển thị ảnh chất lượng cao (High DPI).
-   **Hiệu ứng:** Nếu máy tính yếu, có thể cảm thấy hơi giật nhẹ do hiệu ứng đổ bóng và ánh sáng (Bloom).
-   **Font chữ:** Dự án sử dụng font `Montserrat` và `Playfair Display` được nhúng trực tiếp từ Google Fonts, cần có kết nối Internet để hiển thị đúng font đẹp nhất.

Chúc bạn có những giây phút kỷ niệm thật ý nghĩa! ❤️
