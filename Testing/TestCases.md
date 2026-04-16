# TÀI LIỆU KIỂM THỬ (TEST CASES SPECIFICATION) - DỰ ÁN HÒA PHÁT

Tài liệu này dùng để xác minh các yêu cầu chức năng từ tầng Use Case đã được cài đặt chính xác.

## 1. UC-01: Quản lý công văn và Phê duyệt online

### Scenario 1: Luồng phê duyệt chuẩn (Happy Path)
* **Mã Test Case:** TC-01
* **Mục tiêu:** Xác nhận lãnh đạo có thể phê duyệt công văn thành công.
* **Tiền điều kiện:** Nhân viên đã gửi một công văn ở trạng thái "Chờ duyệt".
* **Các bước thực hiện:**
    1. Đăng nhập vào hệ thống bằng tài khoản Trưởng phòng/Giám đốc.
    2. Truy cập menu "Danh sách chờ duyệt".
    3. Chọn công văn cần duyệt và nhấn nút "Phê duyệt".
* **Kết quả mong đợi:** Hệ thống thông báo phê duyệt thành công. Trạng thái công văn chuyển sang "Đã phê duyệt". Nhân viên khởi tạo nhận được thông báo qua hệ thống.

### Scenario 2: Từ chối phê duyệt kèm lý do
* **Mã Test Case:** TC-02
* **Mục tiêu:** Kiểm tra chức năng từ chối và phản hồi thông tin.
* **Các bước thực hiện:**
    1. Lãnh đạo chọn công văn chờ duyệt.
    2. Nhấn nút "Từ chối".
    3. Hệ thống yêu cầu nhập lý do, nhập: "Thiếu hồ sơ đính kèm".
    4. Nhấn "Xác nhận".
* **Kết quả mong đợi:** Công văn chuyển sang trạng thái "Bị từ chối" hoặc "Chờ sửa đổi". Người gửi nhìn thấy lý do phản hồi của lãnh đạo.

---

## 2. UC-04: Lưu trữ tài liệu số và Tìm kiếm nhanh

### Scenario 3: Tìm kiếm tài liệu bằng từ khóa
* **Mã Test Case:** TC-03
* **Mục tiêu:** Xác tra khả năng truy xuất dữ liệu từ kho lưu trữ tập trung.
* **Các bước thực hiện:**
    1. Vào mục "Kho tài liệu".
    2. Nhập từ khóa "Hợp đồng thép 2024" vào thanh tìm kiếm.
* **Kết quả mong đợi:** Hệ thống hiển thị danh sách các file có tên hoặc nội dung chứa từ khóa trong vòng dưới 2 giây.

---

## 3. UC-07: Tối ưu công việc bằng AI

### Scenario 4: AI gợi ý lịch họp thông minh
* **Mã Test Case:** TC-04
* **Mục tiêu:** Kiểm tra khả năng tự động phân tích lịch biểu của AI.
* **Các bước thực hiện:**
    1. Chọn chức năng "Tạo lịch họp nhóm".
    2. Thêm danh sách thành viên (Ngát, Ly, Mến, Lập).
    3. Nhấn "AI gợi ý thời gian".
* **Kết quả mong đợi:** AI hiển thị các khung giờ trống mà tất cả thành viên đều không bị trùng lịch.

---

## 4. Kiểm thử yêu cầu phi chức năng (Supplementary Requirements)

### Scenario 5: Kiểm tra bảo mật truy cập (UR-04)
* **Mã Test Case:** TC-05
* **Mục tiêu:** Đảm bảo nhân viên không thể duyệt công văn của chính mình hoặc của người khác.
* **Các bước thực hiện:**
    1. Đăng nhập tài khoản quyền "Nhân viên".
    2. Cố gắng truy cập vào đường dẫn trực tiếp (URL) của trang phê duyệt.
* **Kết quả mong đợi:** Hệ thống hiển thị lỗi "403 Forbidden" hoặc "Bạn không có quyền truy cập".
