# QUY TRÌNH QUẢN LÝ THAY ĐỔI 

## 1. Mục tiêu

Đảm bảo mọi thay đổi trong phạm vi, yêu cầu, chi phí, tiến độ hoặc kỹ thuật của dự án đều:
- Được ghi nhận chính thức
- Được phân tích tác động
- Được phê duyệt bởi cấp có thẩm quyền
- Được cập nhật vào tài liệu dự án một cách nhất quán

---

## 2. Phạm vi áp dụng

Áp dụng cho các thay đổi liên quan đến:
- Yêu cầu nghiệp vụ (Business Requirement)
- Phạm vi dự án (Scope)
- Thiết kế hệ thống (Architecture, Database, ETL)
- KPI và chỉ số báo cáo
- Tiến độ và kế hoạch thực hiện

---

## 3. Quy trình quản lý thay đổi

### Bước 1: Gửi yêu cầu thay đổi (Submit Change Request)
- Stakeholder hoặc thành viên dự án tạo Change Request Form.
- Tạo Issue trên GitHub với label: `Change Request`.

### Bước 2: Phân tích tác động (Impact Analysis)
Project Manager phối hợp với team thực hiện:
- Phân tích tác động đến phạm vi
- Phân tích ảnh hưởng đến tiến độ (SPI)
- Phân tích ảnh hưởng đến chi phí (CPI)
- Đánh giá rủi ro phát sinh

### Bước 3: Phê duyệt (Approval)
Thay đổi sẽ được:
- Approved (Phê duyệt)
- Rejected (Từ chối)
- Deferred (Hoãn lại)

Quyết định được ghi nhận trong Issue và biên bản họp.

### Bước 4: Cập nhật tài liệu dự án
Nếu được phê duyệt, cập nhật:
- Project Scope Statement
- WBS / Backlog
- Gantt Chart
- Risk Register
- KPI Definition (nếu liên quan)

### Bước 5: Triển khai và theo dõi
- Thêm vào Sprint tiếp theo
- Theo dõi qua Milestone
- Đánh giá lại SPI, CPI sau khi thực hiện

---

## 4. Biểu mẫu Change Request Form

### CHANGE REQUEST FORM

| Thông tin | Nội dung |
|-----------|----------|
| Mã yêu cầu | CR-01 |
| Ngày yêu cầu | 04/03/2026 |
| Người đề xuất | Stakeholder / PM |
| Mô tả thay đổi | Thêm KPI phân tích theo khu vực địa lý |
| Lý do thay đổi | Nhu cầu báo cáo chi tiết theo vùng |
| Mức độ ưu tiên | High |
| Ảnh hưởng phạm vi | Tăng 2 dashboard |
| Ảnh hưởng tiến độ | +1 tuần |
| Ảnh hưởng chi phí | +3 effort |
| Rủi ro phát sinh | Tăng tải hệ thống |
| Trạng thái | Approved |

---

## 5. Ví dụ áp dụng thực tế trong dự án

Ví dụ: Dashboard không đáp ứng nhu cầu người dùng (Issue R4)

Quy trình thực hiện:
1. Tạo Change Request.
2. Phân tích thấy cần chỉnh sửa cấu trúc dữ liệu.
3. Ảnh hưởng tiến độ: +5 effort.
4. Được PM phê duyệt.
5. Cập nhật:
   - Backlog
   - Milestone
   - Tài liệu thiết kế
6. Theo dõi lại CPI sau Sprint tiếp theo.

---

## 6. Kiểm soát nhất quán tài liệu

Mọi thay đổi sau khi được phê duyệt phải được cập nhật đồng bộ vào:

- README.md
- Tài liệu đặc tả yêu cầu (SRS)
- Risk Log
- Sprint Backlog
- Báo cáo tiến độ

Việc cập nhật được commit rõ ràng trên GitHub với message:

"Update documents after CR-01 approval"

---

## 7. Đánh giá mức độ chuyên nghiệp

Quy trình quản lý thay đổi đảm bảo:

✓ Không thay đổi tự phát  
✓ Có phân tích định lượng (SPI, CPI)  
✓ Có biểu mẫu chuẩn hóa  
✓ Có truy vết (traceability) trên GitHub  
✓ Cập nhật tài liệu nhất quán  

Điều này giúp giảm rủi ro trượt phạm vi (Scope Creep) và kiểm soát dự án một cách có hệ thống.
