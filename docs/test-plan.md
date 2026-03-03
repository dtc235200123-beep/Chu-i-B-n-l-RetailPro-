# KẾ HOẠCH KIỂM THỬ DỰ ÁN DASHBOARD

## 1. Mục tiêu kiểm thử

Đảm bảo hệ thống Dashboard:
- Hoạt động đúng yêu cầu nghiệp vụ
- Số liệu chính xác
- Hiệu năng ổn định
- Đảm bảo bảo mật dữ liệu
- Được người dùng chấp nhận trước khi bàn giao

---

# 2. Kiểm thử chức năng (Functional Testing)

## 2.1 Phạm vi kiểm thử

- Kiểm tra hiển thị KPI doanh thu
- Kiểm tra KPI sản phẩm bán chạy
- Kiểm tra KPI khách hàng
- Kiểm tra bộ lọc theo ngày/tháng/năm
- Kiểm tra xuất dữ liệu (nếu có)

## 2.2 Tiêu chí đạt

- Số liệu hiển thị khớp 100% với dữ liệu gốc
- Không có lỗi giao diện
- Không xảy ra lỗi hệ thống

---

# 3. Kiểm thử phi chức năng (Non-functional Testing)

## 3.1 Kiểm thử hiệu năng (Performance Testing)

Mục tiêu:
- Dashboard tải trong ≤ 3 giây với dữ liệu hiện tại
- Không bị treo khi truy vấn dữ liệu lớn

Cách kiểm tra:
- Đo thời gian load trang
- Kiểm tra truy vấn SQL

Tiêu chí đạt:
- Thời gian phản hồi < 3 giây
- Không lỗi timeout

---

## 3.2 Kiểm thử bảo mật (Security Testing)

Phạm vi:
- Kiểm tra phân quyền truy cập
- Kiểm tra truy cập trái phép
- Kiểm tra bảo mật dữ liệu nhạy cảm

Tiêu chí đạt:
- Người dùng không được truy cập dữ liệu ngoài quyền hạn
- Không lộ thông tin quan trọng
- Không có lỗi SQL Injection cơ bản

---

# 4. Kế hoạch Kiểm thử Chấp nhận Người dùng (UAT)

## 4.1 Mục tiêu

Đảm bảo Dashboard đáp ứng nhu cầu thực tế của Ban lãnh đạo và bộ phận kinh doanh trước khi bàn giao chính thức.

## 4.2 Người tham gia

- Project Manager
- Business Analyst
- Đại diện Ban lãnh đạo

## 4.3 Quy trình UAT

1. Trình bày Dashboard
2. Người dùng thao tác trực tiếp
3. Ghi nhận phản hồi
4. Tổng hợp lỗi (nếu có)
5. Chỉnh sửa và xác nhận lại

## 4.4 Tiêu chí nghiệm thu

- 100% KPI hiển thị đúng yêu cầu
- Không còn lỗi nghiêm trọng (Critical/High)
- Người dùng xác nhận hài lòng
- Có biên bản nghiệm thu

---

# 5. Tài liệu bàn giao sau kiểm thử

- Biên bản UAT
- Danh sách lỗi đã xử lý
- Phiên bản Dashboard cuối cùng
- Commit xác nhận bàn giao trên GitHub

---

# 6. Kết luận

Việc thực hiện kiểm thử toàn diện bao gồm kiểm thử chức năng, phi chức năng và UAT giúp đảm bảo hệ thống đạt chất lượng cao, đáp ứng yêu cầu nghiệp vụ và sẵn sàng triển khai thực tế.
