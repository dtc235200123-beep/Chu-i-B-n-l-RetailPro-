# PHÂN TÍCH CHỈ SỐ KPI ĐÁNH GIÁ SỨC KHỎE DỰ ÁN
Dự án: InsightDash – RetailPro
Thời điểm đánh giá: Cuối tuần 6

---

## 1. Thông số cơ bản

BAC (Budget at Completion) = 51.000.000 VNĐ  
PV (Planned Value) = 38.000.000 VNĐ  
EV (Earned Value) = 34.000.000 VNĐ  
AC (Actual Cost) = 40.000.000 VNĐ  

---

## 2. Các chỉ số hiệu suất

### 2.1 SPI

SPI = EV / PV  
SPI = 34 / 38 = **0,89**

Ý nghĩa:
- SPI = 1 → Đúng tiến độ
- SPI > 1 → Nhanh hơn kế hoạch
- SPI < 1 → Chậm tiến độ

→ SPI = 0,89 cho thấy dự án chỉ hoàn thành 89% khối lượng kế hoạch tại thời điểm báo cáo.
Dự án đang chậm tiến độ 11%.

---

### 2.2 CPI

CPI = EV / AC  
CPI = 34 / 40 = **0,85**

Ý nghĩa:
- CPI = 1 → Đúng ngân sách
- CPI > 1 → Tiết kiệm chi phí
- CPI < 1 → Vượt ngân sách

→ CPI = 0,85 nghĩa là mỗi 1 đồng chi ra chỉ tạo ra 0,85 đồng giá trị.
Dự án đang vượt chi phí 15%.

---

### 2.3 CV

CV = EV - AC  
CV = 34 - 40 = -6 triệu

→ Giá trị âm cho thấy dự án vượt ngân sách 6 triệu tại thời điểm đánh giá.

---

### 2.4 SV

SV = EV - PV  
SV = 34 - 38 = -4 triệu

→ Dự án chậm tiến độ tương đương 4 triệu giá trị công việc.

---

## 3. Dự báo tương lai

### EAC

EAC = BAC / CPI  
EAC = 51 / 0,85 ≈ 60 triệu

→ Nếu không điều chỉnh, tổng chi phí có thể tăng lên 60 triệu.

---

### ETC

ETC = EAC - AC  
ETC = 60 - 40 = 20 triệu

→ Cần thêm 20 triệu để hoàn thành dự án.

---

## 4. Đánh giá "Sức khỏe" dự án

| Chỉ số | Giá trị | Đánh giá |
|--------|----------|-----------|
| SPI | 0,89 | Cảnh báo |
| CPI | 0,85 | Nguy hiểm |
| CV | -6 triệu | Vượt chi phí |
| SV | -4 triệu | Trễ tiến độ |

Kết luận:
Dự án đang ở trạng thái "Cảnh báo đỏ" về chi phí và "Cảnh báo vàng" về tiến độ.

---

## 5. Hành động điều chỉnh đề xuất

- Cắt giảm các tính năng không cốt lõi
- Tăng cường kiểm soát thay đổi yêu cầu
- Tối ưu quy trình xử lý dữ liệu
- Phân bổ lại nguồn lực cho Sprint 4
- Theo dõi CPI hàng tuần thay vì 2 tuần

---
* Phân tích “Sức khỏe” dự án
1️ Đánh giá hiện tại

PV = 38 triệu

EV = 34 triệu

AC = 40 triệu

BAC = 51 triệu

 SPI = EV / PV = 0.89

→ Dự án chậm tiến độ ~11%

 CPI = EV / AC = 0.85

→ Dự án vượt chi phí

 Kết luận: Dự án đang ở trạng thái cảnh báo (trễ và tốn chi phí hơn kế hoạch).

2️ Dự báo hoàn thành (Forecast)
 EAC = BAC / CPI = 51 / 0.85 ≈ 60 triệu

→ Nếu không điều chỉnh, tổng chi phí có thể lên ~60 triệu.

 ETC = EAC − AC = 60 − 40 = 20 triệu

→ Cần thêm khoảng 20 triệu để hoàn thành.

3️ Nguyên nhân sai lệch

R1: Dữ liệu đầu vào không đồng nhất → ETL kéo dài

R3: Trễ tiến độ xử lý ETL

R5: Dashboard cần tối ưu hiệu năng

R6: Phối hợp giữa các bên chưa hiệu quả

4️ Nhận định tổng thể

Dự án đang chậm tiến độ và vượt chi phí do rủi ro kỹ thuật (ETL, dữ liệu) và thay đổi yêu cầu. Tuy nhiên, nếu kiểm soát phạm vi và tối ưu nguồn lực trong giai đoạn cuối, dự án vẫn có khả năng hoàn thành đúng mục tiêu chiến lược.

## 6. Kết luận quản trị

Việc áp dụng các chỉ số SPI, CPI và EVM giúp nhóm đánh giá khách quan tình trạng dự án thay vì cảm tính.
Dựa trên các chỉ số này, nhóm có cơ sở dữ liệu định lượng để đưa ra quyết định điều chỉnh kế hoạch.
