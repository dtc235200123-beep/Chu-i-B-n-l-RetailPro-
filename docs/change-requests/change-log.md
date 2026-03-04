# NHẬT KÝ THAY ĐỔI (CHANGE LOG) – DỰ ÁN INSIGHTDASH (RETAILPRO)

Tài liệu này ghi nhận toàn bộ các thay đổi chính thức của dự án InsightDash.  
Mọi thay đổi đều phải được lập thành Yêu cầu thay đổi (Change Request - CR) và được phê duyệt trước khi triển khai.

---

# 1. THÔNG TIN PHIÊN BẢN

| Phiên bản | Ngày phát hành | Mô tả | Liên quan CR | Trạng thái |
|------------|----------------|--------|--------------|------------|
| v1.0 | 01/03/2026 | Hoàn thành Dashboard cơ bản | - | Baseline |
| v1.1 | 16/03/2026 | Bổ sung KPI Tỷ lệ khách hàng quay lại | CR-001 | Đã phê duyệt |

---

# 2. CHI TIẾT THAY ĐỔI

---

## Phiên bản 1.0 – Baseline ban đầu

**Ngày phát hành:** 01/03/2026  

### Nội dung hoàn thành:
- Hoàn thành mô hình dữ liệu ban đầu.
- Xây dựng Dashboard gồm:
  - Doanh thu theo thời gian
  - Doanh thu theo khu vực
  - Top sản phẩm bán chạy
- Thiết lập Sổ đăng ký rủi ro (Risk Register).
- Thiết lập Baseline phạm vi dự án.

**Trạng thái:** Baseline được phê duyệt và làm cơ sở kiểm soát thay đổi.

---

## Phiên bản 1.1 – CR-001

**Mã thay đổi:** CR-001  
**Ngày phê duyệt:** 16/03/2026  
**Người phê duyệt:** Project Manager  

---

### Nội dung thay đổi

- Bổ sung KPI: **Tỷ lệ khách hàng quay lại (Repeat Customer Rate)**.
- Cập nhật Dashboard mục “Customer Analytics”.
- Cập nhật tài liệu:
  - data-model.md
  - risk-register.md
  - project-baseline.md

---

### Phân loại thay đổi

- Loại thay đổi: Nâng cấp chức năng (Functional Enhancement)
- Mức độ ảnh hưởng: Trung bình
- Ảnh hưởng đến: Phạm vi, Tiến độ, Chi phí

---

### Phân tích tác động

| Yếu tố | Mô tả |
|--------|--------|
| Phạm vi | Thêm 1 KPI mới vào Dashboard |
| Tiến độ | Tăng 2 ngày phát triển |
| Chi phí | Tăng 5% ngân sách Sprint 2 |
| Rủi ro | Bổ sung R2 và R3 vào Risk Register |

---

### Triển khai kỹ thuật

- Tạo nhánh: `feature/repeat-customer-kpi`
- Phát triển và kiểm thử trên nhánh riêng.
- Tạo Pull Request để xem xét và phê duyệt.
- Sau khi được phê duyệt mới hợp nhất (merge) vào nhánh chính.
- Không được commit trực tiếp vào nhánh main.

---

### Kết quả sau triển khai

✔ KPI hiển thị chính xác trên Dashboard  
✔ Không ảnh hưởng kiến trúc hệ thống  
✔ Hoàn thành đúng trong Sprint 2  
✔ Không phát sinh lỗi nghiêm trọng  

---

# 3. QUY TẮC QUẢN LÝ THAY ĐỔI

1. Mọi thay đổi phải được ghi nhận bằng Change Request (CR).
2. Phải phân tích tác động trước khi phê duyệt.
3. Phải có quyết định chính thức từ Project Manager.
4. Phải triển khai trên nhánh riêng (branch).
5. Phải có Pull Request và được review trước khi merge.
6. Sau khi triển khai phải cập nhật:
   - Change Log
   - Risk Register
   - Project Baseline (nếu thay đổi phạm vi)

---

# 4. LỊCH SỬ CẬP NHẬT TÀI LIỆU

| Ngày | Tài liệu | Nội dung cập nhật |
|------|----------|------------------|
| 16/03/2026 | data-model.md | Thêm logic tính Repeat Customer Rate |
| 16/03/2026 | risk-register.md | Thêm R2, R3 |
| 16/03/2026 | project-baseline.md | Cập nhật Scope phiên bản 1.1 |

---

# 5. KẾT LUẬN

Tài liệu Change Log giúp:

- Kiểm soát phiên bản rõ ràng.
- Truy vết thay đổi minh bạch.
- Đảm bảo tính nhất quán giữa các tài liệu dự án.
- Thể hiện quy trình quản lý thay đổi chuyên nghiệp.
- Phù hợp với phương pháp quản lý dự án chuẩn (PMI/Agile).

Tất cả thay đổi đều được lưu vết trên GitHub để đảm bảo minh bạch và kiểm soát cấu hình.
