# Khắc phục & Hoàn thiện Phân loại Cấp độ Prompting

## Phần 1: Phân tích vấn đề
* **Dòng 1, 2, 5:** Đang phân loại sai thành Few-shot/One-shot ➔ Thực tế là **Zero-shot** (0 ví dụ mẫu).
* **Dòng 4:** Đang phân loại sai thành Zero-shot ➔ Thực tế là **Few-shot** (có 3 mẫu).
* **Dòng 3 & 6:** Phân loại đúng là **One-shot** (có đúng 1 mẫu minh họa).

---

## Phần 2: Bảng chuẩn hóa

| STT | Nội dung Câu lệnh (Prompt) | Phân loại đúng | Số lượng ví dụ mẫu |
| :---: | :--- | :---: | :---: |
| **1** | "Phân loại đánh giá sau là Tích cực hay Tiêu cực..." | **Zero-shot** | 0 |
| **2** | "Hãy viết hoa tiêu đề sau theo phong cách công nghệ." | **Zero-shot** | 0 |
| **3** | "Đổi thông số sau: 'RAM 16GB'. Mẫu: 'RAM 8GB' -> ..." | **One-shot** | 1 |
| **4** | "Phân loại cảm xúc: Mẫu 1... Mẫu 2... Mẫu 3... Input..." | **Few-shot** | 3 |
| **5** | "Viết lại email thông báo bảo hành xong cho khách..." | **Zero-shot** | 0 |
| **6** | "Dịch mã lỗi sang tiếng Việt. Ví dụ: 'Err_404'... Input..." | **One-shot** | 1 |