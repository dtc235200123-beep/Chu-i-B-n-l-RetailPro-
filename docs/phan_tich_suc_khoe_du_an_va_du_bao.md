# PHÂN TÍCH SỨC KHỎE DỰ ÁN VÀ DỰ BÁO HOÀN THÀNH

## 1. Mục tiêu

Phân tích tình trạng thực tế dự án dựa trên dữ liệu quản lý tiến độ, hiệu suất và chi phí để xác định:
- “Sức khỏe” dự án hiện tại (Project Health)
- Dự báo thời gian và chi phí hoàn thành
- Nguyên nhân sai lệch so với kế hoạch

---

## 2. Chỉ số đánh giá

### 2.1. Planned Value (PV)

Giá trị kế hoạch theo kế hoạch ban đầu (giả sử biểu diễn theo giờ công tích lũy).

### 2.2. Earned Value (EV)

Giá trị đạt được theo khối lượng công việc đã hoàn thành (dựa trên số task closed).

### 2.3. Actual Cost (AC)

Chi phí thực tế đã sử dụng (quy đổi theo giờ làm hoặc điểm tài nguyên).

---

## 3. Phân tích “Sức khỏe dự án”

### 3.1. Tình trạng tiến độ

Sử dụng chỉ số **SPI (Schedule Performance Index)**:

- SPI = 1 → Hoàn thành đúng tiến độ
- SPI > 1 → Nhanh hơn kế hoạch
- SPI < 1 → Chậm hơn kế hoạch

**Kết quả phân tích:**

- Ở cuối giai đoạn hiện tại, PV = 320, EV = 320 → SPI = 1  
→ Dự án về tổng thể hoàn thành đúng kế hoạch.

**Nhận xét:** Dự án có giai đoạn giữa **SPI < 1** do trễ tiến độ ETL, nhưng sau khi xử lý rủi ro và tăng tốc đóng Issue, tiến độ được phục hồi.

---

### 3.2. Tình trạng chi phí

Sử dụng chỉ số **CPI (Cost Performance Index)**:

- CPI = 1 → Chi phí trong kiểm soát
- CPI < 1 → Chi phí vượt dự kiến
- CPI > 1 → Sử dụng hiệu quả hơn dự kiến

**Kết quả phân tích:**

- CUối giai đoạn phân tích: EV = 320, AC = 320  
→ CPI = 1

**Nhận xét:** Dự án kiểm soát chi phí hiệu quả, không phát sinh vượt ngân sách dự kiến.

---

## 4. Dự báo thời gian và chi phí hoàn thành

Sử dụng các công thức trong Earned Value Management:

### 4.1. ETC (Estimate To Complete)

ETC là chi phí cần để hoàn thành phần còn lại:

Trong đó:
- BAC = Tổng ngân sách ban đầu (giả sử 320 giờ)
- EV = 320
- CPI = 1

→ ETC = (320 - 320) / 1 = 0  
→ Không còn chi phí dự kiến phát sinh thêm.

---

### 4.2. EAC (Estimate At Completion)

EAC là ước tính chi phí khi hoàn tất toàn bộ dự án:

Thay số:  
→ EAC = 320 + 0 = 320

**Nhận xét:** Dự án sẽ kết thúc với chi phí bằng đúng kế hoạch ban đầu nếu không có thay đổi thêm.

---

## 5. Nguyên nhân sai lệch

### 5.1. Chậm tiến độ giữa kỳ

- Giai đoạn ETL gặp dữ liệu đầu vào không nhất quán → phát sinh bug, mất thời gian kiểm tra.
- Điều này khiến SPI trong giai đoạn đó giảm (<1).
- Sau khi có buổi trao đổi với Nhóm kỹ thuật và xử lý dữ liệu mẫu → tiến độ cải thiện.

**Bài học:** Cần đánh giá kỹ chất lượng dữ liệu đầu vào ngay từ đầu.

---

### 5.2. Khối lượng công việc phát sinh

- Phát sinh thay đổi yêu cầu KPI (CR-001) → tăng yêu cầu công việc → cần tinh chỉnh kế hoạch.

**Bài học:** Quy trình Change Request cần phân tích kĩ và gắn trực tiếp vào Board/Milestone.

---

## 6. Đánh giá tổng thể

- SPI ≈ 1 → tiến độ tổng thể ổn định
- CPI ≈ 1 → kiểm soát chi phí hiệu quả
- Không còn rủi ro nghiêm trọng tồn đọng

=> Dự án có “sức khỏe tốt”, tiến độ và chi phí đều nằm trong phạm vi kiểm soát.

---

## 7. Khuyến nghị để tăng hiệu quả

- Theo dõi ước lượng dữ liệu real-time dựa trên số Issue đóng theo tuần → cập nhật Burndown chart hàng tuần
- Tăng cường kiểm thử sớm để tránh sai lệch dữ liệu phát sinh
- Đẩy mạnh giao tiếp nội bộ để giảm rủi ro do hiểu sai yêu cầu

---
