# SỔ THEO DÕI RỦI RO (RISK REGISTER)
Dự án: InsightDash – RetailPro
Cập nhật: Tuần 6

---

## 1. Bảng tổng hợp rủi ro

| ID | Mô tả rủi ro | Nguyên nhân | Xác suất | Ảnh hưởng | Mức độ | Risk Owner | Chiến lược | Trạng thái |
|----|--------------|-------------|----------|------------|---------|------------|------------|------------|
| R1 | Dữ liệu không đồng nhất | Nguồn POS & Website khác chuẩn | Cao | Cao | Nghiêm trọng | Data Engineer | Giảm thiểu | Đang xử lý |
| R2 | Thay đổi yêu cầu khách hàng | Demo phát sinh yêu cầu mới | Trung | Cao | Cao | PM | Kiểm soát thay đổi | Đang theo dõi |
| R3 | Trễ tiến độ Sprint 3 | ETL kéo dài | Trung | Trung | Trung bình | PM | Tái phân bổ nguồn lực | Đang xử lý |
| R4 | Vượt ngân sách | CPI < 1 | Trung | Cao | Cao | PM | Kiểm soát chi phí | Cảnh báo |
| R5 | Thành viên nghỉ đột xuất | Lý do cá nhân | Thấp | Cao | Trung bình | PM | Kế hoạch dự phòng | Theo dõi |

---

## 2. Thang đánh giá

Xác suất:
- Thấp (1)
- Trung (2)
- Cao (3)

Ảnh hưởng:
- Thấp (1)
- Trung (2)
- Cao (3)

Mức độ = Xác suất x Ảnh hưởng

---

## 3. Chiến lược ứng phó rủi ro

- Tránh (Avoid)
- Giảm thiểu (Mitigate)
- Chuyển giao (Transfer)
- Chấp nhận (Accept)

---

## 4. Phân tích chuyên sâu

### R1 – Dữ liệu không đồng nhất
- Điểm rủi ro: 3 x 3 = 9 (Cao nhất)
- Tác động trực tiếp đến ETL và Dashboard
- Giải pháp: Thêm bước Data Validation & chuẩn hóa mã sản phẩm

### R2 – Thay đổi yêu cầu
- Có thể làm tăng EAC
- Áp dụng quy trình Change Request bắt buộc

### R4 – Vượt ngân sách
- CPI = 0.85
- Dự báo EAC = 60 triệu
- Cần theo dõi hàng tuần

---

## 5. Quy trình cập nhật Risk Register

- Cập nhật hàng tuần trong họp dự án
- Risk Owner chịu trách nhiệm báo cáo
- PM tổng hợp và cập nhật vào GitHub

---

## 6. Kết luận

Risk Register giúp dự án:
- Chủ động thay vì phản ứng
- Giảm tác động dây chuyền
- Minh bạch trách nhiệm (Risk Owner rõ ràng)
- Kiểm soát tốt tiến độ và chi phí
