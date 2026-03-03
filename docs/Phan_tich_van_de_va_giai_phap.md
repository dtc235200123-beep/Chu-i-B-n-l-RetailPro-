# PHÂN TÍCH VẤN ĐỀ & GIẢI PHÁP KHẮC PHỤC
Dự án: InsightDash – RetailPro

---

## 1. Vấn đề 1: Dữ liệu đầu vào không đồng nhất

### Nguyên nhân:
- Dữ liệu POS và Website sử dụng định dạng khác nhau
- Thiếu chuẩn hóa mã sản phẩm

### Tác động:
- Làm chậm tiến độ ETL
- Sai lệch báo cáo doanh thu

### Giải pháp:
- Thêm bước Data Validation trong ETL
- Xây dựng bảng chuẩn hóa mã sản phẩm
- Thiết lập quy trình kiểm tra dữ liệu tự động

### Điều chỉnh kế hoạch:
- Bổ sung 3 ngày xử lý dữ liệu
- Điều chuyển 1 thành viên hỗ trợ Data Engineer

---

## 2. Vấn đề 2: Thay đổi yêu cầu từ khách hàng

### Nguyên nhân:
- Sau khi xem dashboard demo, khách hàng yêu cầu thêm chỉ số mới

### Tác động:
- Phát sinh thêm 5 biểu đồ
- Nguy cơ trễ Sprint 3

### Giải pháp:
- Áp dụng quy trình Change Request
- Đánh giá tác động trước khi chấp nhận thay đổi
- Loại bỏ các tính năng ít ưu tiên

### Điều chỉnh kế hoạch:
- Tăng ngân sách dự phòng 5%
- Gia hạn Sprint 3 thêm 2 ngày

---

## 3. Vấn đề 3: Nguy cơ vượt ngân sách

### Dấu hiệu:
- CPI = 0.85 (<1)

### Tác động:
- Dự kiến vượt ngân sách 9 triệu

### Giải pháp:
- Tối ưu truy vấn dữ liệu
- Giảm họp không cần thiết
- Tái phân bổ nguồn lực

### Điều chỉnh:
- Cắt giảm 10% chi phí kiểm thử ngoài giờ
- Tập trung hoàn thành tính năng cốt lõi

---

## 4. Kết luận quản trị

Nhóm không chỉ nhận diện rủi ro mà còn:
- Phân tích nguyên nhân gốc
- Đánh giá tác động
- Đề xuất hành động cụ thể
- Điều chỉnh kế hoạch phù hợp

Điều này giúp giảm thiểu ảnh hưởng tiêu cực đến tiến độ và ngân sách dự án.
## Đánh giá mức độ rủi ro

| Rủi ro | Xác suất | Ảnh hưởng | Mức độ |
|--------|----------|-----------|--------|
| Dữ liệu sai lệch | Cao | Cao | Nghiêm trọng |
| Thay đổi yêu cầu | Trung | Cao | Cao |
| Trễ tiến độ | Trung | Trung | Trung bình |
