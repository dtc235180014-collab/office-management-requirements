# SOFTWARE REQUIREMENTS SPECIFICATION (SRS) - HỆ THỐNG E-OFFICE HÒA PHÁT

Tài liệu này tổng hợp toàn bộ các yêu cầu của hệ thống, được phân loại theo cấu trúc chuẩn IEEE nhằm phục vụ quá trình phân tích và thiết kế theo mô hình V-Model.

## 1. GIỚI THIỆU (INTRODUCTION)
Chi tiết về mục tiêu và phạm vi dự án đã được mô tả tại: **[Vision_Document.md](../Vision/README.md)**.

## 2. CÁC YÊU CẦU CHỨC NĂNG (FUNCTIONAL REQUIREMENTS)
Hệ thống được thiết kế dựa trên các nghiệp vụ cốt lõi của Tập đoàn Hòa Phát. Chi tiết từng chức năng được mô tả qua danh sách Use Case dưới đây:

### 2.1 Quản lý Công văn & Hồ sơ (Module chính)
* **[UC-01]: Tiếp nhận và Phân loại công văn đến** - Hỗ trợ bởi công nghệ AI & OCR.
* **[UC-02]: Khởi tạo và Phát hành công văn đi**.
* **[UC-03]: Quản lý kho tài liệu số và Hồ sơ nội bộ**.

### 2.2 Quy trình Phê duyệt (Workflow)
* **[UC-04]: Thiết lập luồng phê duyệt đa cấp**.
* **[UC-05]: Thực hiện Phê duyệt / Từ chối / Chuyển xử lý hồ sơ**.

### 2.3 Quản lý Hành chính & Tiện ích
* **[UC-06]: Quản lý lịch họp và Đặt phòng họp tập trung**.
* **[UC-07]: Quản lý phiếu đề xuất hành chính (Mua sắm, thanh toán...)**.

### 2.4 Quản trị Hệ thống
* **[UC-08]: Quản lý người dùng và Phân quyền (RBAC)**.
* **[UC-09]: Dashboard báo cáo và Thống kê quản trị cho Lãnh đạo**.

---

## 3. CÁC YÊU CẦU PHI CHỨC NĂNG (SUPPLEMENTARY REQUIREMENTS)
Các tiêu chuẩn về chất lượng hệ thống (UR) được đặc tả chi tiết tại: **[Supplementary_Requirements.md](Supplementary_Requirements.md)**.

### 3.1 Độ tin cậy (Reliability)
* Đảm bảo tính sẵn dùng (Uptime) tối thiểu 99.5%.
* Cơ chế xử lý lỗi (Robustness) và thông báo nhập liệu chính xác.

### 3.2 Hiệu suất (Performance)
* Thời gian phản hồi cho các thao tác tìm kiếm và truy xuất dữ liệu < 2 giây.
* Khả năng chịu tải tối thiểu 1.000 người dùng đồng thời.

### 3.3 Bảo mật (Security)
* Sử dụng giao thức HTTPS để mã hóa đường truyền dữ liệu.
* Xác thực người dùng qua cơ chế SSO và quản lý quyền truy cập nghiêm ngặt.

### 3.4 Khả năng hỗ trợ (Supportability)
* Thiết kế Responsive tương thích với trình duyệt trên PC, Tablet và Smartphone.

---

## 4. MA TRẬN TRUY VẾT (TRACEABILITY)
Để đảm bảo tất cả yêu cầu trên đều được phát triển và kiểm thử, nhóm tham chiếu tại: **[RTM_README.md](../RTM/README.md)**.
