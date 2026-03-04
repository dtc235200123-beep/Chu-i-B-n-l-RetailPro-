# SỔ ĐĂNG KÝ RỦI RO (RISK REGISTER)  
## Dự án: InsightDash – RetailPro

---

## Thang đo đánh giá

- Xác suất: Thấp / Trung bình / Cao  
- Ảnh hưởng: Thấp / Trung bình / Cao  
- Mức độ rủi ro: Được đánh giá dựa trên Xác suất + Ảnh hưởng  

---

## Danh sách rủi ro

| ID | Rủi ro | Nguyên nhân | Xác suất | Ảnh hưởng | Mức độ rủi ro | Chiến lược | Biện pháp xử lý | Người phụ trách | Trạng thái | Ngày cập nhật |
|----|--------|------------|----------|------------|---------------|------------|----------------|------------------|------------|---------------|
| R1 | Dữ liệu đầu vào không chính xác | Lỗi nhập liệu từ hệ thống POS | Trung bình | Cao | Cao | Giảm thiểu | Kiểm tra và làm sạch dữ liệu trước khi phân tích | Data Engineer | Đang theo dõi | 01/03/2026 |
| R2 | KPI định nghĩa không thống nhất | Thiếu xác nhận giữa các phòng ban | Trung bình | Cao | Cao | Giảm thiểu | Tổ chức họp xác nhận định nghĩa KPI trước khi triển khai | Business Analyst | Đang theo dõi | 01/03/2026 |
| R3 | Truy vấn dữ liệu chậm | Dữ liệu lớn, chưa tối ưu index | Trung bình | Trung bình | Trung bình | Giảm thiểu | Tối ưu truy vấn và bổ sung index | Data Engineer | Đang theo dõi | 01/03/2026 |
| R4 | Trễ tiến độ Sprint | Phát sinh thay đổi phạm vi (Change Request) | Trung bình | Trung bình | Trung bình | Giảm thiểu | Quản lý backlog chặt chẽ và đánh giá tác động trước khi phê duyệt | Project Manager | Đang theo dõi | 01/03/2026 |
| R5 | Người dùng không hiểu Dashboard | Thiếu hướng dẫn sử dụng | Thấp | Trung bình | Thấp | Giảm thiểu | Xây dựng tài liệu hướng dẫn và demo cho người dùng | Business Analyst | Chưa xảy ra | 01/03/2026 |
| R6 | Mất dữ liệu | Lỗi hệ thống hoặc backup không đầy đủ | Thấp | Cao | Trung bình | Giảm thiểu | Thiết lập cơ chế backup định kỳ | Data Engineer | Đang theo dõi | 01/03/2026 |
| R7 | KPI mới gây sai lệch số liệu | Định nghĩa KPI chưa rõ ràng | Trung bình | Cao | Cao | Giảm thiểu | Xác nhận định nghĩa và kiểm thử dữ liệu trước khi đưa vào Dashboard | Business Analyst | Đang theo dõi | 16/03/2026 |
| R8 | Thay đổi yêu cầu liên tục | Stakeholder thay đổi nhu cầu phân tích | Trung bình | Trung bình | Trung bình | Giảm thiểu | Áp dụng quy trình Change Management chính thức | Project Manager | Đang theo dõi | 16/03/2026 |
| R9 | Lỗi tích hợp dữ liệu | Dữ liệu từ nhiều nguồn (POS, Website) không đồng nhất | Trung bình | Cao | Cao | Giảm thiểu | Chuẩn hóa dữ liệu trong quá trình ETL | Data Engineer | Đang theo dõi | 01/03/2026 |
| R10 | Bảo mật dữ liệu khách hàng | Phân quyền truy cập chưa chặt chẽ | Thấp | Cao | Trung bình | Giảm thiểu | Thiết lập phân quyền và kiểm soát truy cập | Project Manager | Đang theo dõi | 01/03/2026 |

---

# Cập nhật liên quan đến CR-001

- Bổ sung rủi ro R7 do thay đổi KPI.
- Đánh giá lại R2 khi có KPI mới.
- Cập nhật ngày theo dõi: 16/03/2026.

---

# Kết luận

Sổ đăng ký rủi ro được cập nhật xuyên suốt vòng đời dự án.  
Mọi Change Request đều phải đánh giá tác động đến rủi ro và cập nhật tài liệu này để đảm bảo kiểm soát rủi ro hiệu quả.
