# PHÂN TÍCH TÌNH HUỐNG XUNG ĐỘT & HƯỚNG XỬ LÝ
## Dự án: InsightDash – RetailPro

---

# 1. Tình huống 1: Hai lập trình viên tranh cãi về giải pháp kỹ thuật

## 1.1 Mô tả tình huống

Trong Sprint 3 (giai đoạn tối ưu hiệu năng Dashboard), hai Developer xảy ra tranh cãi:

- Dev A muốn tối ưu bằng cách thêm index và tối ưu truy vấn SQL.
- Dev B muốn triển khai cache dữ liệu (Redis) để giảm tải truy vấn.

Tranh luận kéo dài 2 ngày, ảnh hưởng tiến độ sprint và làm chậm kế hoạch UAT.

---

## 1.2 Phân tích nguyên nhân

- Cả hai đều tập trung vào giải pháp kỹ thuật, chưa dựa vào mục tiêu dự án.
- Không có tiêu chí đánh giá rõ ràng (performance target).
- Thiếu vai trò điều phối của Project Manager.

Rủi ro phát sinh:
- Trễ Sprint
- Ảnh hưởng Go-live
- Gây mất tinh thần đội nhóm

---

## 1.3 Áp dụng phương pháp giải quyết xung đột

Theo lý thuyết quản lý dự án, có 5 phương pháp:

1. Avoiding (Tránh né)
2. Accommodating (Nhượng bộ)
3. Compromising (Thỏa hiệp)
4. Forcing (Áp đặt)
5. Collaborating (Hợp tác)

Trong tình huống này, phương pháp phù hợp nhất là:

→ **Collaborating (Hợp tác)**

---

## 1.4 Hướng xử lý cụ thể

Bước 1: Tổ chức họp kỹ thuật ngắn (Technical Review Meeting)  
Bước 2: Xác định mục tiêu rõ ràng:
- Dashboard phải tải < 3 giây (theo Test Plan)
- Không tăng chi phí hạ tầng quá mức

Bước 3: Đưa ra tiêu chí đánh giá:
- Độ cải thiện performance
- Độ phức tạp triển khai
- Ảnh hưởng bảo trì

Bước 4: Thực hiện test thử nghiệm cả hai giải pháp trên môi trường staging

Kết quả:
- Tối ưu SQL cải thiện 40%
- Cache cải thiện thêm 20% nữa

Giải pháp cuối cùng:
→ Kết hợp cả hai phương án (tối ưu SQL + cache cho dữ liệu lớn)

---

## 1.5 Kết quả đạt được

- Giữ đúng tiến độ Sprint
- Cải thiện hiệu năng đạt tiêu chí UAT
- Tăng tinh thần hợp tác giữa các thành viên

---

# 2. Tình huống 2: Thành viên chậm tiến độ

## 2.1 Mô tả tình huống

Data Engineer phụ trách xây dựng ETL nhưng trễ 5 ngày so với kế hoạch.

Hệ quả:
- Không có dữ liệu đầy đủ để kiểm thử
- Sprint có nguy cơ trễ
- Ảnh hưởng đến Test Plan và UAT

---

## 2.2 Phân tích nguyên nhân

Sau khi trao đổi riêng (1-1 meeting), phát hiện:

- Khối lượng công việc underestimated
- Phát sinh yêu cầu thay đổi KPI (CR-001)
- Thiếu hỗ trợ từ Developer

---

## 2.3 Áp dụng phương pháp giải quyết

Phương pháp áp dụng:

→ **Problem Solving / Collaborating**
→ Không sử dụng Forcing vì dễ gây áp lực tiêu cực

---

## 2.4 Hướng xử lý

1. Điều chỉnh lại kế hoạch Sprint
2. Chia nhỏ công việc ETL thành các task nhỏ
3. Hỗ trợ thêm 1 Developer trong 3 ngày
4. Cập nhật lại Risk Register (rủi ro trễ tiến độ)
5. Ghi nhận vào Change Log nếu có ảnh hưởng baseline

---

## 2.5 Kết quả

- Hoàn thành ETL sau 3 ngày điều chỉnh
- Sprint chậm 1 ngày nhưng không ảnh hưởng Go-live
- Cập nhật lại baseline hợp lý

---

# 3. Bài học rút ra

- Xung đột kỹ thuật nên xử lý bằng Collaborating.
- Luôn dựa vào mục tiêu dự án thay vì quan điểm cá nhân.
- Theo dõi tiến độ sớm để phát hiện chậm trễ.
- Cập nhật Risk Register khi phát sinh vấn đề.
- Change Management giúp kiểm soát tác động hệ thống.

---

# 4. Kết luận

Việc áp dụng đúng phương pháp giải quyết xung đột giúp:

- Giữ vững tiến độ dự án
- Duy trì tinh thần đội nhóm
- Hạn chế rủi ro lan rộng
- Đảm bảo hoàn thành UAT và Go-live đúng kế hoạch

Tình huống trên cho thấy vai trò quan trọng của Project Manager trong điều phối, lắng nghe và ra quyết định dựa trên mục tiêu chung của dự án.
