# KẾ HOẠCH KIỂM THỬ CHI TIẾT (DETAILED TEST PLAN)
## Dự án: InsightDash – RetailPro

---

# 1. Mục tiêu kiểm thử

- Đảm bảo hệ thống hoạt động đúng yêu cầu nghiệp vụ.
- Đảm bảo dữ liệu hiển thị chính xác.
- Phát hiện và xử lý lỗi trước khi triển khai.
- Đảm bảo hệ thống đạt yêu cầu về hiệu năng và bảo mật.
- Đảm bảo người dùng chấp nhận hệ thống (UAT).

---

# 2. Phạm vi kiểm thử

## 2.1 Bao gồm

- Dashboard tổng quan
- Báo cáo doanh thu
- Báo cáo sản phẩm
- Báo cáo khách hàng
- Bộ lọc theo thời gian
- Phân quyền người dùng

## 2.2 Không bao gồm

- Hệ thống POS bên ngoài
- Hạ tầng máy chủ vật lý

---

# 3. Các loại hình kiểm thử

| Loại kiểm thử | Mô tả | Người thực hiện |
|---------------|-------|------------------|
| Unit Testing | Kiểm tra từng module riêng lẻ | Developer |
| Integration Testing | Kiểm tra tích hợp dữ liệu từ POS, Website, CRM | Data Engineer |
| System Testing | Kiểm tra toàn bộ hệ thống | QA |
| Performance Testing | Đánh giá tốc độ phản hồi | QA |
| Security Testing | Kiểm tra phân quyền và bảo mật | QA |
| UAT | Kiểm thử chấp nhận người dùng | Stakeholder |

---

# 4. Test Cases mẫu cho chức năng quan trọng

---

# 4.1 Test Case – Xem Dashboard doanh thu

## TC-01: Hiển thị doanh thu đúng (Trường hợp thành công)

- Mục tiêu: Kiểm tra hiển thị KPI doanh thu
- Điều kiện tiên quyết: Người dùng đã đăng nhập
- Bước thực hiện:
  1. Truy cập Dashboard
  2. Chọn khoảng thời gian "Tháng 01/2026"
- Kết quả mong đợi:
  - Doanh thu hiển thị đúng theo dữ liệu trong database
  - Không xuất hiện lỗi

---

## TC-02: Không đăng nhập (Trường hợp thất bại)

- Mục tiêu: Kiểm tra bảo mật truy cập
- Bước thực hiện:
  1. Truy cập URL Dashboard khi chưa đăng nhập
- Kết quả mong đợi:
  - Hệ thống chuyển hướng về trang Login
  - Không hiển thị dữ liệu

---

# 4.2 Test Case – Bộ lọc theo thời gian

## TC-03: Lọc theo ngày hợp lệ (Success)

- Bước thực hiện:
  1. Chọn ngày từ 01/01/2026 đến 31/01/2026
  2. Nhấn Apply
- Kết quả mong đợi:
  - Dữ liệu cập nhật đúng theo khoảng thời gian

---

## TC-04: Lọc với ngày không hợp lệ (Failure)

- Bước thực hiện:
  1. Chọn ngày bắt đầu > ngày kết thúc
- Kết quả mong đợi:
  - Hiển thị thông báo lỗi
  - Không thực hiện truy vấn

---

# 4.3 Test Case – Phân quyền người dùng

## TC-05: Manager xem đúng dữ liệu khu vực (Success)

- Điều kiện: Đăng nhập với quyền Manager
- Kết quả mong đợi:
  - Chỉ hiển thị dữ liệu khu vực được phân quyền

---

## TC-06: User cố truy cập dữ liệu Admin (Failure)

- Bước thực hiện:
  1. Đăng nhập với tài khoản User
  2. Truy cập trang quản trị
- Kết quả mong đợi:
  - Hiển thị thông báo "Access Denied"
  - Không truy cập được

---

# 4.4 Test Case – Hiệu năng

## TC-07: Tải Dashboard với dữ liệu lớn

- Điều kiện: Database có >= 100.000 bản ghi
- Kết quả mong đợi:
  - Thời gian tải < 3 giây
  - Không crash

---

# 4.5 Test Case – Bảo mật

## TC-08: Kiểm tra SQL Injection (Failure Case)

- Bước thực hiện:
  1. Nhập ' OR 1=1 -- vào ô đăng nhập
- Kết quả mong đợi:
  - Không đăng nhập thành công
  - Không lỗi hệ thống

---

# 5. Tiêu chí nghiệm thu

Hệ thống được nghiệm thu khi:

- 100% Test Case mức Critical & High đạt
- Không còn lỗi nghiêm trọng
- Hiệu năng đạt yêu cầu (<3 giây)
- Phân quyền hoạt động chính xác
- Stakeholder ký xác nhận UAT

---

# 6. Quy trình xử lý lỗi

1. Ghi nhận lỗi vào Bug Log
2. Phân loại mức độ
3. Giao Developer xử lý
4. Retest
5. Đóng lỗi khi xác nhận đạt

---

# 7. Kết luận

Kế hoạch kiểm thử đảm bảo hệ thống InsightDash được kiểm tra toàn diện cả về chức năng và phi chức năng, bao gồm các trường hợp thành công và thất bại, trước khi triển khai chính thức.
