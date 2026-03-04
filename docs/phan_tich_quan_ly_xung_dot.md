# PHÂN TÍCH XUNG ĐỘT & GIẢI PHÁP DUY TRÌ HIỆU SUẤT ĐỘI NHÓM
## Dự án: InsightDash – RetailPro

---

# 1. Bối cảnh dự án

Dự án InsightDash đang ở giai đoạn Sprint 3 (tối ưu hiệu năng trước UAT). 
Áp lực tiến độ cao vì phải đảm bảo:

- Dashboard tải < 3 giây (theo Test Plan)
- Hoàn thành trước mốc UAT
- Không ảnh hưởng kế hoạch Go-live

Trong bối cảnh này, hai tình huống xung đột xảy ra.

---

# 2. Tình huống 1: Tranh cãi kỹ thuật giữa hai Developer

## 2.1 Mô tả tình huống

Dev A: đề xuất tối ưu SQL & index  
Dev B: đề xuất triển khai caching (Redis)

Tranh luận kéo dài, trở nên căng thẳng, ảnh hưởng tiến độ Sprint và tinh thần nhóm.

---

## 2.2 Phân tích chiều sâu (Góc độ kỹ năng mềm)

### 1. Gốc rễ xung đột

- Cả hai đều muốn bảo vệ chuyên môn của mình.
- Cảm giác “ý tưởng của mình tốt hơn”.
- Áp lực deadline khiến giao tiếp trở nên căng thẳng.
- Thiếu tiêu chí đánh giá khách quan.

### 2. Yếu tố tâm lý

- Nhu cầu được công nhận (Recognition)
- Cái tôi chuyên môn (Professional Ego)
- Áp lực thành tích trước UAT

Nếu xử lý sai cách (Forcing hoặc né tránh):
→ Có thể gây mất động lực lâu dài
→ Hình thành chia rẽ nội bộ

---

## 2.3 Áp dụng mô hình giải quyết xung đột

Theo Thomas–Kilmann Conflict Mode Instrument:

- Avoiding → Không phù hợp
- Competing (Forcing) → Gây tổn hại quan hệ
- Compromising → Giải pháp trung bình
- Collaborating → Phù hợp nhất

→ Chọn **Collaborating (Hợp tác)**

---

## 2.4 Hướng xử lý ngắn hạn (Giải quyết vấn đề trước mắt)

1. Tổ chức Technical Review Meeting trung lập
2. PM đóng vai trò điều phối, không phán xét
3. Xác định mục tiêu chung: 
   - Đạt performance target
   - Giữ tiến độ Sprint
4. Thống nhất tiêu chí đánh giá:
   - Tốc độ cải thiện
   - Độ phức tạp bảo trì
   - Chi phí hạ tầng

5. Cho phép thử nghiệm song song trên môi trường staging

Kết quả:
- SQL optimization cải thiện 40%
- Cache cải thiện thêm 20%

Quyết định:
→ Kết hợp hai giải pháp

---

## 2.5 Giải pháp dài hạn (Duy trì gắn kết & hiệu suất)

- Thiết lập quy trình Technical Decision Framework rõ ràng
- Áp dụng rule: “Data-driven decision”
- Tổ chức retrospective cuối Sprint
- Khuyến khích văn hóa: tranh luận về ý tưởng, không công kích cá nhân
- Ghi nhận đóng góp của cả hai

Kết quả lâu dài:
- Tăng sự tôn trọng chuyên môn lẫn nhau
- Cải thiện văn hóa phản biện tích cực
- Tăng chất lượng quyết định kỹ thuật

---

# 3. Tình huống 2: Thành viên chậm tiến độ

## 3.1 Mô tả

Data Engineer trễ 5 ngày trong việc xây dựng ETL.
Nguy cơ ảnh hưởng:

- System Testing
- UAT
- Go-live timeline

---

## 3.2 Phân tích nguyên nhân sâu

Qua 1-1 meeting (Active Listening):

- Công việc bị underestimate
- Phát sinh Change Request (CR-001)
- Cảm thấy quá tải nhưng không dám báo sớm

Yếu tố tâm lý:
- Sợ bị đánh giá kém năng lực
- Áp lực deadline
- Thiếu hỗ trợ kỹ thuật

---

## 3.3 Kỹ năng mềm được áp dụng

1. Active Listening
2. Empathy (Thấu cảm)
3. Coaching thay vì khiển trách
4. Problem-solving mindset

Không sử dụng:
- Forcing
- Blaming

---

## 3.4 Giải pháp ngắn hạn

- Chia nhỏ task ETL
- Phân bổ thêm 1 Developer hỗ trợ
- Điều chỉnh nhẹ Sprint backlog
- Cập nhật Risk Register
- Thông báo minh bạch với Stakeholder

Kết quả:
- Hoàn thành sau 3 ngày điều chỉnh
- Không ảnh hưởng Go-live

---

## 3.5 Giải pháp dài hạn

- Áp dụng Workload Review mỗi Sprint
- Tạo môi trường an toàn để báo sớm rủi ro
- Thiết lập rule: “Không phạt người báo rủi ro sớm”
- Theo dõi capacity planning thực tế

Hiệu quả dài hạn:

- Giảm burnout
- Tăng sự tin tưởng
- Cải thiện dự báo tiến độ chính xác hơn

---

# 4. Liên kết với các phần quản lý dự án khác

| Vấn đề | Công cụ quản lý đã sử dụng |
|--------|----------------------------|
| Tranh cãi kỹ thuật | Technical Review + Data-driven decision |
| Chậm tiến độ | Risk Register cập nhật |
| Thay đổi yêu cầu | Change Management |
| Đảm bảo chất lượng | Test Plan & UAT |
| Duy trì tinh thần | Retrospective & Coaching |

---

# 5. Bài học về lãnh đạo & kỹ năng mềm

- Xung đột không phải là tiêu cực nếu được quản lý tốt.
- Lắng nghe quan trọng hơn phản biện tức thì.
- Quyết định nên dựa trên dữ liệu thay vì cái tôi.
- Minh bạch giúp giảm căng thẳng.
- Văn hóa an toàn tâm lý (Psychological Safety) giúp duy trì hiệu suất lâu dài.

---

# 6. Kết luận

Việc xử lý xung đột trong dự án InsightDash không chỉ giải quyết vấn đề trước mắt (tiến độ, hiệu năng) mà còn:

- Củng cố sự tin tưởng giữa các thành viên
- Nâng cao chất lượng quyết định kỹ thuật
- Tăng động lực làm việc
- Duy trì hiệu suất bền vững
- Giảm rủi ro tái diễn xung đột trong tương lai

Điều này thể hiện vai trò quan trọng của Project Manager không chỉ là người quản lý tiến độ, mà còn là người lãnh đạo, điều phối và xây dựng văn hóa đội nhóm tích cực.
