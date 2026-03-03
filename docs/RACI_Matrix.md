# MA TRẬN PHÂN CÔNG TRÁCH NHIỆM (RACI)
Dự án: InsightDash – RetailPro

## 1. Danh sách vai trò

- PM: Quản lý dự án
- BA: Phân tích nghiệp vụ
- DE: Kỹ sư dữ liệu (Data Engineer)
- BI: Lập trình viên Dashboard (BI Developer)
- QA: Kiểm thử hệ thống

---

## 2. Ma trận RACI chi tiết

| Công việc | PM | BA | DE | BI | QA |
|------------|----|----|----|----|----|
| Thu thập yêu cầu | A | R | C | | |
| Xác định KPIs | A | R | C | C | |
| Thiết kế mô hình dữ liệu | C | A | R | | |
| Xây dựng ETL | | C | R | | A |
| Kiểm tra chất lượng dữ liệu | | | R | | A |
| Xây dựng Dashboard | C | A | | R | |
| Kiểm thử hệ thống | A | | C | C | R |
| Triển khai & đào tạo | R | A | | C | |

---

## 3. Giải thích

R (Responsible): Người trực tiếp thực hiện  
A (Accountable): Người chịu trách nhiệm cuối cùng  
C (Consulted): Người được tham vấn  
I (Informed): Người được thông báo  

---

## 4. Nhận xét quản lý nhân sự

- Không có công việc nào có 2 Accountable.
- Mỗi nhiệm vụ có ít nhất 1 Responsible.
- PM chịu trách nhiệm cuối cùng về tiến độ và ngân sách.
- BA chịu trách nhiệm về nghiệp vụ.
- DE đảm bảo chất lượng dữ liệu.
- BI đảm bảo giao diện trực quan.
- QA đảm bảo chất lượng đầu ra.
