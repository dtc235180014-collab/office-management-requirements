# CHI TIẾT KỊCH BẢN KIỂM THỬ (TEST CASES & SCENARIOS)

Dưới đây là các kịch bản kiểm thử chi tiết nhằm xác minh các yêu cầu nghiệp vụ (Business Requirements) của hệ thống e-Office Hòa Phát.

---

### TC01: Thêm công văn mới đầy đủ thông tin
* **Mã yêu cầu (Requirement):** BR-01 (SR01)
* **Kịch bản chi tiết (Scenario):**
    1. Người dùng đăng nhập với quyền Nhân viên, chọn "Khởi tạo công văn".
    2. Nhập Tiêu đề, Số hiệu công văn và chọn loại văn bản.
    3. Đính kèm tệp tin tài liệu (định dạng PDF/Docx).
    4. Nhấn nút "Lưu hệ thống".
* **Kết quả mong đợi:** Công văn được lưu thành công, hiển thị tại danh sách "Quản lý công văn" và trạng thái là "Chờ duyệt".

---

### TC02: Thêm công văn nhưng bỏ trống số công văn (Kiểm thử lỗi)
* **Mã yêu cầu (Requirement):** BR-01 (SR01)
* **Kịch bản chi tiết (Scenario):**
    1. Tại màn hình "Khởi tạo công văn", nhân viên nhập tiêu đề nhưng để trống ô "Số hiệu".
    2. Nhấn nút "Lưu hệ thống".
* **Kết quả mong đợi:** Hệ thống báo lỗi "Trường dữ liệu bắt buộc không được để trống" và không lưu bản ghi vào cơ sở dữ liệu.

---

### TC03: Thực hiện click phê duyệt công văn
* **Mã yêu cầu (Requirement):** BR-06 (SR02)
* **Kịch bản chi tiết (Scenario):**
    1. Lãnh đạo đăng nhập, mở danh sách công văn "Chờ duyệt".
    2. Chọn công văn cần xử lý và nhấn nút "Phê duyệt".
    3. Thực hiện ký số điện tử theo yêu cầu của hệ thống.
* **Kết quả mong đợi:** Trạng thái công văn chuyển sang "Đã phê duyệt", thông báo đẩy (Fe-14) được gửi tới người khởi tạo.

---

### TC05: Tìm kiếm tài liệu bằng từ khóa
* **Mã yêu cầu (Requirement):** BR-04 (SR04)
* **Kịch bản chi tiết (Scenario):**
    1. Truy cập thanh tìm kiếm thông minh tại màn hình chính.
    2. Nhập từ khóa dựa trên Metadata (Ví dụ: "Hòa Phát", "Công văn 2026").
    3. Nhấn phím Enter hoặc nút "Tìm kiếm".
* **Kết quả mong đợi:** Hệ thống hiển thị chính xác danh sách các tài liệu có chứa từ khóa trong nội dung hoặc Metadata.
