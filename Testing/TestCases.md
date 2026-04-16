# TÀI LIỆU KỊCH BẢN KIỂM THỬ CHI TIẾT (TEST CASE SPECIFICATION)

Dài liệu này mô tả chi tiết các kịch bản kiểm thử nhằm đảm bảo hệ thống e-Office Hòa Phát vận hành đúng theo yêu cầu nghiệp vụ đã phân tích.

---

### 1. TC01: Thêm công văn mới đầy đủ thông tin
* **Yêu cầu liên quan:** SR01 (Khởi tạo dữ liệu)
* **Tiền điều kiện:** Người dùng đã đăng nhập vào hệ thống với quyền nhân viên văn phòng.
* **Các bước thực hiện:**
    1. Truy cập vào chức năng "Tạo mới công văn".
    2. Nhập đầy đủ các trường: Tiêu đề, Số hiệu, Ngày ban hành.
    3. Đính kèm tệp tin tài liệu (định dạng .pdf hoặc .docx).
    4. Nhấn nút "Lưu".
* **Kết quả mong đợi (Expected Result):** Hệ thống thông báo "Thêm mới thành công". Công văn mới xuất hiện ở đầu danh sách quản lý.

---

### 2. TC02: Thêm công văn nhưng bỏ trống số công văn
* **Yêu cầu liên quan:** SR01 (Kiểm soát dữ liệu đầu vào)
* **Tiền điều kiện:** Đang ở màn hình thêm mới công văn.
* **Các bước thực hiện:**
    1. Nhập tiêu đề và đính kèm tệp tin.
    2. **Để trống** ô "Số công văn".
    3. Nhấn nút "Lưu".
* **Kết quả mong đợi (Expected Result):** Hệ thống báo lỗi nhập liệu (ô Số công văn hiển thị cảnh báo màu đỏ) và không cho phép lưu bản ghi.

---

### 3. TC03: Thực hiện click phê duyệt công văn
* **Yêu cầu liên quan:** SR02 (Luồng phê duyệt)
* **Tiền điều kiện:** Có công văn đang ở trạng thái "Chờ phê duyệt" và người dùng đăng nhập với quyền Lãnh đạo.
* **Các bước thực hiện:**
    1. Tìm chọn công văn có trạng thái "Chờ phê duyệt".
    2. Kiểm tra thông tin chi tiết của công văn.
    3. Nhấn vào nút **"Phê duyệt"**.
* **Kết quả mong đợi (Expected Result):** Trạng thái công văn thay đổi từ "Chờ phê duyệt" sang **"Đã phê duyệt"**. Hệ thống ghi nhận thời gian và người phê duyệt.

---

### 4. TC05: Tìm kiếm tài liệu bằng từ khóa
* **Yêu cầu liên quan:** SR04 (Tra cứu dữ liệu)
* **Tiền điều kiện:** Hệ thống đã có dữ liệu công văn lưu trữ.
* **Các bước thực hiện:**
    1. Truy cập thanh tìm kiếm tại màn hình danh sách tài liệu.
    2. Nhập từ khóa liên quan đến tiêu đề hoặc nội dung tài liệu (Ví dụ: "Hòa Phát").
    3. Nhấn phím Enter hoặc nút "Tìm kiếm".
* **Kết quả mong đợi (Expected Result):** Hệ thống hiển thị danh sách tài liệu phù hợp với từ khóa đã nhập. Các tài liệu không liên quan sẽ bị ẩn đi.

---

### 5. Ghi chú bổ sung
* Các kịch bản trên được thiết kế để bao phủ các luồng nghiệp vụ chính (Happy Path) và luồng ngoại lệ (Exception Path).
* Dữ liệu kiểm thử được sử dụng dựa trên hồ sơ thực tế của dự án e-Office Hòa Phát.
