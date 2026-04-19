# Ma trận Truy vết Yêu cầu (Requirements Traceability Matrix - RTM)
**Dự án:** Hệ thống quản lý văn phòng – hành chính cho Tập đoàn Hòa Phát  
**Nhóm 11**  
**Thành viên thực hiện:** Lương Thị Mến  
**Cập nhật:** Tháng 4/2026

## 1. Trace From (Truy vết nguồn gốc yêu cầu)

| Needs | Mô tả ngắn gọn | Liên kết chính |
|-------|----------------|---------------|
| N1 | Chuẩn hóa quy trình hành chính | FE-01, FE-02, FE-04 → UC-01, UC-02 |
| N2 | Tăng tốc độ xử lý công việc | FE-01, FE-04, FE-05 → UC-01, UC-02, UC-03 |
| N3 | Minh bạch hóa quy trình | FE-07, FE-19, FE-20 → UC-04 |
| N4 | Quản lý dữ liệu tập trung | FE-08, FE-09, FE-10 → UC-05, UC-06 |
| N5 | Kiểm soát trách nhiệm | FE-04, FE-05, FE-21 → UC-02, UC-03 |
| N6 | Theo dõi tiến độ thời gian thực | FE-07, FE-19, FE-20 → UC-04 |
| N7 | Giảm sai sót nghiệp vụ | FE-04, FE-16 → UC-09 |
| N8 | Phối hợp nội bộ hiệu quả | FE-12, FE-14, FE-15 → UC-07, UC-08 |
| N9 | Hỗ trợ ra quyết định | FE-16, FE-17, FE-19 → UC-09, UC-10 |
| N10 | Giảm giấy tờ thủ công | FE-01, FE-02, FE-08 → UC-01, UC-05 |
| N11 | Tuân thủ quy định pháp luật | FE-06, FE-21 → UC-02, UC-03 |
| N12 | Bảo mật thông tin | FE-06, FE-21 → UC-01, UC-05 |
| N13 | Tìm kiếm tài liệu nhanh | FE-11, FE-17 → UC-06 |
| N14 | Làm việc linh hoạt | FE-13, FE-22 → UC-04, UC-07 |
| N15 | Sẵn sàng mở rộng | FE-23, FE-24 → UC-05 |

## 2. Trace To (Truy vết triển khai)

| Use Case | Features chính | Supplementary Requirements | Test Cases |
|----------|----------------|-----------------------------|------------|
| UC-01 | FE-01, FE-02, FE-03, FE-25 | UR-01, UR-03, UR-04 | TC01, TC02 |
| UC-02 | FE-04, FE-05, FE-06, FE-21 | UR-01, UR-02, UR-03, UR-04 | TC03 |
| UC-03 | FE-04, FE-05, FE-10 | UR-01, UR-03 | - |
| UC-04 | FE-07, FE-19, FE-20 | UR-02, UR-03 | - |
| UC-05 | FE-08, FE-09, FE-10, FE-24 | UR-04 | - |
| UC-06 | FE-11, FE-17 | UR-02, UR-03 | - |
| UC-07 | FE-12, FE-18 | UR-03 | - |
| UC-08 | FE-14, FE-15 | UR-02, UR-03 | - |
| UC-09 | FE-16 | UR-02, UR-04 | - |
| UC-10 | FE-17 | UR-02, UR-03 | - |

## 3. Kết luận Traceability
- Mọi Needs đều được ánh xạ xuống Features và Use Cases.
- Tất cả Use Cases đều được liên kết với Supplementary Requirements (UR-01 đến UR-04).
- Toàn bộ yêu cầu được quản lý trên **GitHub Project "Requirement Lifecycle & Traceability - Nhóm 11"** với 7 trạng thái vòng đời.

**Công cụ sử dụng:** GitHub Issues + GitHub Projects
