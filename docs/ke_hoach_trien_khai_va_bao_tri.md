# KẾ HOẠCH TRIỂN KHAI, CHUYỂN GIAO & BẢO TRÌ
## Dự án: InsightDash – RetailPro

---

# 1. Mục tiêu

- Đảm bảo hệ thống được triển khai ổn định sau khi hoàn tất UAT.
- Đào tạo người dùng cuối sử dụng hiệu quả.
- Thiết lập quy trình chuyển giao chính thức.
- Xây dựng kế hoạch bảo trì và SLA rõ ràng.

---

# 2. Kế hoạch triển khai (Deployment Plan)

## 2.1 Điều kiện Go-Live

Hệ thống chỉ được triển khai khi:

- Hoàn tất 100% UAT
- Không còn lỗi mức Critical/High
- Stakeholder ký biên bản nghiệm thu
- Backup dữ liệu hoàn tất

---

## 2.2 Các bước triển khai

1. Backup toàn bộ database
2. Deploy phiên bản production
3. Kiểm tra smoke test sau deploy
4. Kiểm tra phân quyền
5. Thông báo Go-Live chính thức

---

## 2.3 Thời gian triển khai

- Thực hiện ngoài giờ hành chính (20:00 – 23:00)
- Có đội hỗ trợ trực trong 48 giờ đầu

---

# 3. Kế hoạch đào tạo người dùng cuối

## 3.1 Đối tượng đào tạo

- Quản lý kinh doanh
- Trưởng phòng Marketing
- Quản lý cửa hàng

---

## 3.2 Nội dung đào tạo

| Nội dung | Thời lượng |
|----------|------------|
| Giới thiệu hệ thống | 30 phút |
| Hướng dẫn sử dụng Dashboard | 60 phút |
| Thực hành lọc & phân tích dữ liệu | 60 phút |
| Hỏi đáp | 30 phút |

---

## 3.3 Hình thức đào tạo

- Training trực tiếp hoặc online
- Cung cấp tài liệu hướng dẫn (User Guide PDF)
- Video hướng dẫn sử dụng

---

## 3.4 Tiêu chí hoàn thành đào tạo

- 100% người dùng tham gia
- Người dùng thực hiện được các thao tác cơ bản
- Không còn thắc mắc lớn

---

# 4. Quy trình chuyển giao (Handover Process)

## 4.1 Tài liệu bàn giao

- Test Plan
- UAT Sign-off
- Risk Register
- Change Log
- Source Code
- Database Schema
- User Guide

---

## 4.2 Biên bản bàn giao

Bao gồm:

- Phiên bản hệ thống
- Ngày bàn giao
- Danh sách tài liệu
- Trạng thái hệ thống
- Chữ ký xác nhận hai bên

---

# 5. Kế hoạch bảo trì (Maintenance Plan)

## 5.1 Các loại bảo trì

| Loại bảo trì | Mô tả |
|--------------|-------|
| Corrective | Sửa lỗi phát sinh |
| Adaptive | Điều chỉnh theo thay đổi môi trường |
| Perfective | Cải thiện hiệu năng |
| Preventive | Bảo trì phòng ngừa |

---

# 6. SLA (Service Level Agreement – Giả định)

## 6.1 Phân loại mức độ sự cố

| Mức độ | Mô tả | Thời gian phản hồi | Thời gian xử lý |
|--------|-------|-------------------|-----------------|
| Critical | Hệ thống không hoạt động | ≤ 1 giờ | ≤ 4 giờ |
| High | Lỗi chức năng quan trọng | ≤ 2 giờ | ≤ 8 giờ |
| Medium | Lỗi nhỏ | ≤ 4 giờ | ≤ 2 ngày |
| Low | Yêu cầu cải tiến | ≤ 1 ngày | Theo kế hoạch |

---

## 6.2 Cam kết hệ thống

- Uptime ≥ 99%
- Backup dữ liệu hàng ngày
- Lưu trữ backup tối thiểu 30 ngày
- Kiểm tra bảo mật định kỳ hàng tháng

---

# 7. Kế hoạch hỗ trợ sau triển khai

- Hỗ trợ 24/7 trong tuần đầu
- Hỗ trợ giờ hành chính sau tuần đầu
- Kênh hỗ trợ: Email / Ticket system

---

# 8. Quy trình tiếp nhận yêu cầu thay đổi sau Go-Live

1. Người dùng gửi yêu cầu
2. Ghi nhận vào Change Log
3. Phân tích tác động
4. Trình phê duyệt
5. Triển khai theo quy trình Change Management

---

# 9. Kết luận

Kế hoạch triển khai và bảo trì đảm bảo hệ thống InsightDash được vận hành ổn định, người dùng được đào tạo đầy đủ, có quy trình chuyển giao rõ ràng và có SLA cụ thể để duy trì chất lượng dịch vụ lâu dài.
