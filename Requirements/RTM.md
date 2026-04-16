# MA TRẬN TRUY VẾT YÊU CẦU (RTM) - DỰ ÁN E-OFFICE HÒA PHÁT

Tài liệu này dùng để quản lý sự liên kết giữa các tầng yêu cầu trong mô hình Kim tự tháp: Needs -> Features -> Use Cases -> Test Cases.

## 1. Ma trận truy vết chức năng (Functional RTM)

| Needs ID | Feature ID | Use Case ID | Test Case ID | Trạng thái phê duyệt |
| :--- | :--- | :--- | :--- | :--- |
| **N-01** (Số hóa quy trình) | **F-01** (Workflow) | **UC-01** (Phê duyệt online) | TC-01, TC-02 | [Approved] |
| **N-01** (Số hóa quy trình) | **F-01** (Workflow) | **UC-02** (Theo dõi trạng thái) | TC-01 | [Approved] |
| **N-02** (Kho dữ liệu số) | **F-02** (Lưu trữ) | **UC-04** (Lưu trữ hồ sơ) | TC-03 | [Approved] |
| **N-02** (Kho dữ liệu số) | **F-03** (Tìm kiếm) | **UC-05** (Tra cứu tài liệu) | TC-03 | [Approved] |
| **N-03** (Tối ưu bằng AI) | **F-04** (AI gợi ý) | **UC-07** (AI nhắc lịch) | TC-04 | [Pending] |
| **N-03** (Tối ưu bằng AI) | **F-04** (AI gợi ý) | **UC-08** (AI phân loại file) | TC-04 | [Pending] |

## 2. Truy vết yêu cầu phi chức năng (Supplementary Requirements)

| Supplementary ID | Nội dung yêu cầu | Test Case ID | Ghi chú |
| :--- | :--- | :--- | :--- |
| **UR-01** (Hiệu năng) | Tìm kiếm tài liệu phải hiển thị kết quả < 2s. | TC-03 | Quan trọng |
| **UR-02** (Khả dụng) | Hoạt động tốt trên trình duyệt Chrome, Edge. | TC-01 | Đồng bộ |
| **UR-03** (Tin cậy) | Hệ thống hoạt động 24/7. | N/A | Server-side |
| **UR-04** (Bảo mật) | Phân quyền truy cập theo chức danh (Lãnh đạo/Nhân viên). | TC-05 | Bắt buộc |

---

## 3. Nhật ký phê duyệt (Approval Log)
*Đây là bằng chứng cho việc Phiên bản hóa và Phê duyệt yêu cầu theo chuẩn GitHub.*

- **Phiên bản 1.0**: Khởi tạo kho yêu cầu (Người thực hiện: Nhóm sinh viên).
- **Trạng thái**: Đã phê duyệt nội bộ bởi Trưởng nhóm (Ngát).
- **Cơ chế phê duyệt**: Thông qua Pull Request trên GitHub.
