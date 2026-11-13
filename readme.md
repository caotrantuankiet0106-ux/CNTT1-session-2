# Khắc phục lỗi khai báo biến số trong prompt mẫu

## Bước 1: Phân tích lỗi
* **Nguyên nhân:** Dùng lẫn lộn ngoặc vuông `[language]` và ngoặc nhọn `{audience}` khiến hệ thống tự động hóa và AI không nhận diện được đồng nhất ranh giới biến số, dễ dẫn đến lỗi thay thế dữ liệu.

---

## Bước 2: Đồng bộ biến số (Prompt chuẩn hóa)
```text
Hãy viết một bài chia sẻ về Cấu trúc Prompt Tiêu chuẩn & Định dạng bằng ngôn ngữ [NGÔN_NGỮ]. Dành cho đối tượng [ĐỐI_TƯỢNG].