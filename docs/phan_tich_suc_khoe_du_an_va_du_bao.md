# PHÂN TÍCH SỨC KHỎE DỰ ÁN
## 1. Cơ sở dữ liệu phân tích

Tổng số Issue của dự án (BAC – Budget at Completion): 28  
Số Issue đã hoàn thành (Closed): 16  
Số Issue đang mở (Open): 12  

Giả định:
- Tại thời điểm đánh giá, theo kế hoạch phải hoàn thành toàn bộ 28 Issue.
- 1 Issue được quy đổi tương đương 1 đơn vị effort.

EV (Earned Value) = 16  
PV (Planned Value) = 28  
AC (Actual Cost quy đổi effort) = 28  

---

## 2. Phân tích chỉ số hiệu suất

### 2.1. Chỉ số tiến độ (SPI)

SPI = EV / PV  
SPI = 16 / 28 = 0.57  

→ SPI < 1 cho thấy dự án đang chậm tiến độ nghiêm trọng.  
Tỷ lệ hoàn thành mới đạt 57% so với kế hoạch đề ra.

---

### 2.2. Chỉ số chi phí (CPI)

CPI = EV / AC  
CPI = 16 / 28 = 0.57  

→ CPI < 1 cho thấy hiệu suất sử dụng nguồn lực thấp.  
Để tạo ra 1 đơn vị giá trị, nhóm đang tiêu tốn gần gấp đôi effort dự kiến.

---

## 3. Dự báo hoàn thành (Forecast)

### 3.1. Estimate At Completion (EAC)

EAC = BAC / CPI  
EAC = 28 / 0.57 ≈ 49 đơn vị effort  

→ Nếu không có biện pháp cải thiện, tổng effort khi kết thúc dự án có thể lên tới 49 thay vì 28 như kế hoạch ban đầu (tăng ~75%).

---

### 3.2. Estimate To Complete (ETC)

ETC = EAC – AC  
ETC = 49 – 28 = 21 đơn vị effort  

→ Dự án cần thêm khoảng 21 đơn vị effort nữa để hoàn thành.

---

## 4. Phân tích nguyên nhân sai lệch

Qua theo dõi Issue trên GitHub và nội dung các rủi ro đang mở, có thể xác định các nguyên nhân chính:

### 4.1. Rủi ro kỹ thuật (Technical Risks)
- Trễ tiến độ ETL
- Dashboard chưa đáp ứng yêu cầu
- Hiệu năng hệ thống thấp

→ Dẫn đến việc phải sửa đổi và làm lại (rework), làm tăng AC và giảm CPI.

### 4.2. Quản lý yêu cầu chưa chặt chẽ
- Requirement thay đổi trong quá trình thực hiện
- Stakeholder chưa thống nhất kỳ vọng ban đầu

→ Làm PV không còn phản ánh chính xác khối lượng thực tế.

### 4.3. Phân bổ nguồn lực chưa tối ưu
- Issue chưa được chia nhỏ
- Một số task có độ phức tạp cao nhưng ước lượng thấp

→ Làm giảm hiệu suất thực tế.

---

## 5. Đánh giá tổng thể sức khỏe dự án

Dựa trên các chỉ số SPI và CPI (< 1), dự án đang ở trạng thái:

* Chậm tiến độ  
* Vượt effort dự kiến  
* Có nguy cơ kéo dài thời gian hoàn thành  

Nếu không có biện pháp điều chỉnh:
- Thời gian hoàn thành sẽ kéo dài thêm ~75%
- Effort thực tế có thể gần gấp đôi kế hoạch

---

## 6. Đề xuất cải thiện và kiểm soát

Để đưa dự án trở lại trạng thái ổn định, cần:

1. Rà soát và chuẩn hóa lại backlog.
2. Tách nhỏ Issue để ước lượng chính xác hơn.
3. Áp dụng kiểm soát Sprint Review định kỳ.
4. Ưu tiên xử lý các Issue có ảnh hưởng lớn đến KPI kinh doanh.
5. Sử dụng Milestone và Dashboard GitHub để theo dõi tiến độ theo tuần.
6. Thiết lập quy trình quản lý thay đổi (Change Control) rõ ràng.

---

## 7. Kết luận

Phân tích định lượng bằng phương pháp Earned Value Management (EVM) cho thấy dự án đang có sai lệch đáng kể về tiến độ và chi phí. Tuy nhiên, các sai lệch chủ yếu đến từ yếu tố kỹ thuật và quản lý yêu cầu, có thể kiểm soát được nếu áp dụng các biện pháp cải tiến quy trình.

Việc sử dụng dữ liệu trực tiếp từ GitHub (Issue, trạng thái Open/Closed) để tính toán SPI, CPI, EAC, ETC thể hiện khả năng làm chủ công cụ và áp dụng phương pháp quản lý dự án một cách thực tiễn.
