# TÀI LIỆU QUẢN LÝ YÊU CẦU - DỰ ÁN E-OFFICE HÒA PHÁT

## 1. Glossary (Thuật ngữ dự án)
| Thuật ngữ | Định nghĩa |
| :--- | :--- |
| **E-Office** | Hệ thống quản lý văn phòng - hành chính điện tử tập trung cho Tập đoàn. |
| **Workflow** | Quy trình luân chuyển và phê duyệt hồ sơ tự động giữa các phòng ban. |
| **OCR** | Công nghệ nhận diện ký tự để chuyển công văn giấy thành dữ liệu số. |
| **AI Suggestion** | Trí tuệ nhân tạo gợi ý sắp xếp lịch họp và phân loại tài liệu tự động. |
| **RTM** | Ma trận truy vết yêu cầu (Requirements Traceability Matrix). |

## 2. Scenarios & Test Cases (Kịch bản & Kiểm thử)
### UC-01: Quản lý công văn và Phê duyệt online
**Scenario 1: Phê duyệt luồng chuẩn (Happy Path)**
- **Test Case TC-01**: Kiểm tra lãnh đạo phê duyệt công văn thành công.
- **Các bước**: 1. Đăng nhập quyền Lãnh đạo -> 2. Chọn CV chờ duyệt -> 3. Nhấn "Duyệt".
- **Kết quả**: Trạng thái chuyển thành "Đã duyệt", hệ thống gửi thông báo cho người tạo.

**Scenario 2: Từ chối và yêu cầu sửa đổi**
- **Test Case TC-02**: Kiểm tra luồng từ chối có kèm lý do.
- **Các bước**: 1. Chọn CV -> 2. Nhấn "Từ chối" -> 3. Nhập lý do "Thiếu chữ ký".
- **Kết quả**: CV trả về trạng thái "Chờ sửa đổi", hiển thị đúng lý do đã nhập.

### UC-07: Tối ưu công việc bằng AI
**Scenario 3: AI gợi ý lịch họp**
- **Test Case TC-03**: Kiểm tra tính năng tự động tìm thời gian trống của các thành viên.
- **Kết quả**: AI hiển thị danh sách 3 khung giờ tối ưu nhất mà không bị trùng lịch.

## 3. Ma trận truy vết yêu cầu (Tầng Test Case)
| Needs ID | Feature ID | Use Case ID | Test Case ID | Trạng thái |
| :--- | :--- | :--- | :--- | :--- |
| N-01 | F-01 | UC-01 | TC-01, TC-02 | Hoàn thành |
| N-03 | F-04 | UC-07 | TC-03 | Đang thực hiện |
