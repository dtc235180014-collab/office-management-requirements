# 1 CHI TIẾT KỊCH BẢN KIỂM THỬ (TEST CASES & SCENARIOS)

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
## 2. Kiểm thử Yêu cầu Phi chức năng (Non-Functional)

### TC-SEC-01: Kiểm tra bảo mật giao thức HTTPS
* **Mục đích:** Đảm bảo toàn bộ dữ liệu truyền tải được mã hóa theo mục 3.3.11.
* **Yêu cầu liên quan:** UR-03 (Security - HTTPS).
* **Các bước thực hiện:**
    1. Mở trình duyệt, nhập địa chỉ hệ thống bằng `http://[tên-miền-hệ-thống]`.
    2. Quan sát thanh địa chỉ của trình duyệt.
* **Kết quả mong đợi:** Hệ thống tự động chuyển hướng sang `https://`. Xuất hiện biểu tượng ổ khóa an toàn.

### TC-PERF-01: Kiểm tra hiệu suất phản hồi tìm kiếm
* **Mục đích:** Đảm bảo tốc độ truy xuất dữ liệu theo mục 3.3.12.
* **Yêu cầu liên quan:** UR-01 (Performance).
* **Các bước thực hiện:**
    1. Đăng nhập vào hệ thống với vai trò nhân viên.
    2. Truy cập kho lưu trữ công văn (dữ liệu mẫu > 1000 bản ghi).
    3. Nhập từ khóa tìm kiếm và nhấn Enter.
* **Kết quả mong đợi:** Danh sách kết quả hiển thị trong thời gian **< 2 giây**.

### TC-REL-01: Kiểm tra tính đúng đắn và độ mạnh (Robustness)
* **Mục đích:** Xác minh khả năng xử lý dữ liệu sai định dạng theo mục 3.3.11.
* **Yêu cầu liên quan:** UR-02 (Reliability - Robustness).
* **Các bước thực hiện:**
    1. Chọn chức năng "Tải lên công văn đến".
    2. Chọn tệp tin có định dạng không được phép (ví dụ: `.exe`, `.dll`).
    3. Nhấn nút "Lưu".
* **Kết quả mong đợi:** Hệ thống không bị treo, hiển thị thông báo: "Định dạng tệp không hợp lệ. Chỉ chấp nhận .pdf, .doc, .docx".

---

## 3. Kiểm thử Chức năng Đặc biệt (Functional)

### TC-AI-01: Kiểm tra phân loại công văn bằng AI
* **Mục đích:** Xác minh tính năng hỗ trợ thông minh theo mục 3.3.2.
* **Yêu cầu liên quan:** BR-06 (AI Integration).
* **Các bước thực hiện:**
    1. Tải lên một văn bản nội bộ có nội dung về "Quy định an toàn lao động".
    2. Kiểm tra phần gợi ý "Loại văn bản" do AI đề xuất.
* **Kết quả mong đợi:** Hệ thống tự động gợi ý nhãn "Quy định/Hướng dẫn" với độ chính xác cao.

### TC-RBAC-01: Kiểm tra phân quyền truy cập (Access Control)
* **Mục đích:** Đảm bảo tính an toàn dữ liệu nội bộ Hòa Phát theo mục 3.3.11.
* **Yêu cầu liên quan:** UR-03 (Security - RBAC).
* **Các bước thực hiện:**
    1. Đăng nhập bằng tài khoản "Nhân viên văn phòng".
    2. Cố gắng truy cập đường dẫn URL dành cho "Quản trị viên" (ví dụ: `/admin/settings`).
* **Kết quả mong đợi:** Hệ thống từ chối truy cập và hiển thị thông báo lỗi "403 Forbidden" hoặc chuyển hướng về trang chủ.

---

## 4. Kiểm thử Khả năng Phục hồi (Recoverability)

### TC-REL-02: Kiểm tra khôi phục dữ liệu từ bản sao lưu
* **Mục đích:** Xác minh cam kết phục hồi dịch vụ trong 30-60 phút theo mục 3.3.12.
* **Yêu cầu liên quan:** UR-06 (Recoverability).
* **Các bước thực hiện:**
    1. Giả lập tình huống xóa nhầm dữ liệu trong môi trường Testing.
    2. Thực hiện lệnh khôi phục từ bản Backup gần nhất.
* **Kết quả mong đợi:** Dữ liệu được khôi phục đầy đủ và hệ thống hoạt động lại bình thường.
