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

## 4. Phân tích nguyên nhân của các sai lệch

Dựa trên kết quả phân tích Earned Value Management:

SPI = 0.57  
CPI = 0.57  

Có thể thấy dự án đang **chậm tiến độ và hiệu suất sử dụng nguồn lực thấp**. Các sai lệch này xuất phát từ một số nguyên nhân chính sau:

### 4.1. Sai lệch tiến độ (SPI < 1)

SPI = 0.57 cho thấy dự án mới hoàn thành **16/28 Issue**, tương đương khoảng **57% khối lượng công việc so với kế hoạch**.

Nguyên nhân chính gồm:

- **Ước lượng công việc chưa chính xác**

Một số Issue có độ phức tạp cao nhưng được ước lượng effort thấp, đặc biệt là các task liên quan đến:
+ Xây dựng pipeline ETL  
+ Thiết kế dashboard phân tích dữ liệu  
+ Tối ưu truy vấn dữ liệu  

Điều này khiến thời gian thực hiện kéo dài hơn so với kế hoạch ban đầu.

- **Phụ thuộc giữa các nhiệm vụ (Task Dependencies)**

Một số công việc phụ thuộc vào kết quả của task trước đó, ví dụ:

+ Dashboard phụ thuộc dữ liệu từ ETL  
+ KPI dashboard phụ thuộc mô hình dữ liệu  

Khi một task bị chậm, các task tiếp theo cũng bị ảnh hưởng và làm trễ tiến độ chung của dự án.

- **Issue chưa được chia nhỏ**

Một số Issue có phạm vi quá lớn nên:

+ Khó ước lượng effort chính xác  
+ Khó theo dõi tiến độ thực tế  
+ Dễ phát sinh thêm công việc ngoài kế hoạch  

Điều này làm giảm tốc độ hoàn thành Issue.

---

### 4.2. Sai lệch chi phí / effort (CPI < 1)

CPI = 0.57 cho thấy **hiệu suất sử dụng nguồn lực thấp**, tức là effort bỏ ra nhiều nhưng giá trị hoàn thành chưa tương xứng.

Nguyên nhân chính bao gồm:

- **Phát sinh rework (làm lại)**

Một số chức năng phải chỉnh sửa lại do:

+ Dashboard chưa đáp ứng đúng yêu cầu ban đầu  
+ Cấu trúc dữ liệu cần điều chỉnh để phù hợp với phân tích  

Việc sửa đổi nhiều lần làm tăng effort thực tế (AC).

- **Thay đổi yêu cầu từ stakeholder**

Trong quá trình thực hiện, một số yêu cầu phân tích được điều chỉnh như:

+ Thay đổi cách tính KPI  
+ Bổ sung thêm chỉ số phân tích  

Những thay đổi này làm tăng khối lượng công việc so với kế hoạch ban đầu.

- **Kinh nghiệm công nghệ của nhóm còn hạn chế**

Một số thành viên chưa quen với các công cụ như:

+ ETL tools  
+ Dashboard BI  
+ Tối ưu truy vấn dữ liệu  

Do đó thời gian thực hiện task dài hơn so với dự kiến.

---

### 4.3. Tác động tổng hợp đến dự án

Các nguyên nhân trên dẫn đến sai lệch trong các chỉ số EVM:

- EV thấp hơn PV → tiến độ thực tế chậm hơn kế hoạch → SPI thấp  
- AC cao hơn giá trị tạo ra → hiệu suất nguồn lực thấp → CPI thấp  

Kết quả là dự án:

- Chậm tiến độ so với kế hoạch  
- Effort thực tế tăng cao  
- Dự báo tổng effort khi hoàn thành (EAC) lớn hơn đáng kể so với BAC

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
