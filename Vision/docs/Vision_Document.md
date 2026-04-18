#  VISION DOCUMENT - HỆ THỐNG E-OFFICE HÒA PHÁT

## Giới thiệu

### a. Mục đích
* Định nghĩa phạm vi của hệ thống Quản lý Văn phòng – Hành chính cho Tập đoàn Hòa Phát.
* Xác định các nhu cầu nghiệp vụ và ràng buộc của hệ thống.
* Thống nhất nhận thức giữa nhóm phát triển và các bên liên quan về mục tiêu dự án.
* Làm cơ sở xây dựng các tài liệu Use Case, Supplementary Requirements và thiết kế hệ thống.
* Định hướng triển khai hệ thống phục vụ chuyển đổi số quản trị nội bộ doanh nghiệp.

### b. Phạm vi
* Đề tài hướng đến đối tượng sử dụng là các phòng ban hành chính – văn phòng trong doanh nghiệp quy mô lớn, nhiều chi nhánh.
* Hệ thống phục vụ quản lý công văn, hồ sơ nội bộ, lịch họp, quy trình phê duyệt và kho tài liệu số.
* Cho phép vận hành tập trung tại trụ sở chính, công ty thành viên, nhà máy và chi nhánh.
* Hỗ trợ truy cập qua môi trường web nội bộ hoặc cloud riêng doanh nghiệp.

### c. Tài liệu tham khảo
* [1] Peter Zielczynski, *Requirements Management Using IBM Rational RequisitePro*, IBM Press, 2008.
* [2] Dean Leffingwell, Don Widrig, *Managing Software Requirements: A Unified Process*, Addison Wesley, 1999.
* [3] Axel van Lamsweerde, *Requirements Engineering: From System Goals to UML Models to Software Specifications*, Wiley, 2009.
* [4] Hull, Jackson, Dick, *Requirements Engineering*, Springer, 2005.

### d. Tổng quan
Tài liệu Vision mô tả tổng quan các vấn đề nghiệp vụ hiện tại trong công tác quản trị hành chính doanh nghiệp và giải pháp hệ thống được đề xuất. Tài liệu cũng trình bày các nhóm người dùng, nhu cầu chính và các chức năng cốt lõi của hệ thống, làm cơ sở cho các giai đoạn phân tích và thiết kế tiếp theo.

---

## Vai trò

### a. Cơ hội nghiệp vụ
Việc số hóa quy trình hành chính tại Hòa Phát sẽ giúp:
* Giảm phụ thuộc giấy tờ thủ công.
* Tăng tốc độ xử lý hồ sơ.
* Kiểm soát quy trình minh bạch.
* Hỗ trợ quản lý tập trung nhiều đơn vị.
* Giảm chi phí vận hành và tăng hiệu quả phối hợp giữa các phòng ban.

### b. Phát biểu vấn đề
Hiện trạng quản lý hành chính còn tồn tại nhiều bất cập:
* Công văn xử lý rời rạc qua giấy tờ hoặc email.
* Khó theo dõi tiến độ hồ sơ và chậm phê duyệt do quy trình thủ công.
* Khó truy vết người xử lý và tài liệu phân tán nhiều nơi.
* Lãnh đạo thiếu báo cáo tổng hợp tức thời.

### c. Phát biểu về vai trò của sản phẩm
Hệ thống giúp:
* Chuẩn hóa nghiệp vụ hành chính nội bộ và quản lý công văn tập trung.
* Tự động hóa quy trình phê duyệt và tăng khả năng giám sát của lãnh đạo.
* Giảm thất lạc hồ sơ và tạo nền tảng chuyển đổi số lâu dài.

---

## Các mô tả người dùng và Stakeholder

### a. Các thuật ngữ nghiệp vụ
* **Công văn đến:** Văn bản gửi từ bên ngoài vào doanh nghiệp.
* **Công văn đi:** Văn bản do doanh nghiệp phát hành ra ngoài.
* **Phiếu đề xuất:** Hồ sơ yêu cầu nội bộ như mua sắm, sửa chữa, thanh toán.
* **Workflow:** Chuỗi bước xử lý hồ sơ tự động.
* **Kho tài liệu số:** Nơi lưu trữ tập trung tài liệu điện tử.
* **Phê duyệt đa cấp:** Hồ sơ cần nhiều cấp quản lý xác nhận.

### b. Mô tả Stakeholder
| Stakeholder | Mô tả |
| :--- | :--- |
| **Ban lãnh đạo** | Xem báo cáo, phê duyệt hồ sơ quan trọng. |
| **Phòng Hành chính** | Quản lý công văn, lịch họp, hồ sơ. |
| **Trưởng phòng** | Kiểm tra và duyệt hồ sơ thuộc đơn vị. |
| **Nhân viên** | Tạo đề xuất, tra cứu thông tin. |
| **Bộ phận CNTT** | Quản trị hệ thống, hỗ trợ kỹ thuật. |
| **Nhóm phát triển** | Phân tích, thiết kế, lập trình, kiểm thử. |

---

## Tổng quan về sản phẩm

### a. Viễn cảnh sản phẩm
Hệ thống là nền tảng quản trị nội bộ tập trung dành cho doanh nghiệp nhiều phòng ban và nhiều cơ sở hoạt động. Người dùng truy cập qua trình duyệt web trên máy tính hoặc thiết bị di động.

### b. Tóm tắt khả năng
* Quản lý công văn đến / đi và hồ sơ nội bộ.
* Quy trình phê duyệt điện tử và đặt lịch họp/phòng họp.
* Kho tài liệu tập trung, Dashboard quản trị và tìm kiếm nhanh.
* Phân quyền người dùng, báo cáo thống kê và hỗ trợ AI phân loại hồ sơ.

---

## Các đặc trưng sản phẩm

### STRQ1: Quản lý công văn
* FEAT1: Tiếp nhận công văn đến | FEAT2: Tạo công văn đi
* FEAT3: Theo dõi trạng thái xử lý | FEAT4: Tìm kiếm công văn

### STRQ2: Quản lý hồ sơ nội bộ
* FEAT5: Tạo phiếu đề xuất | FEAT6: Đính kèm tài liệu | FEAT7: Theo dõi tiến độ hồ sơ

### STRQ3: Phê duyệt điện tử
* FEAT8: Thiết lập luồng duyệt nhiều cấp | FEAT9: Phê duyệt / từ chối hồ sơ | FEAT10: Ghi nhận lịch sử xử lý

### STRQ4: Quản lý lịch họp
* FEAT11: Tạo lịch họp | FEAT12: Mời thành viên | FEAT13: Đặt phòng họp | FEAT14: Nhắc lịch tự động

### STRQ5: Quản lý người dùng
* FEAT15: Tạo tài khoản | FEAT16: Phân quyền theo vai trò | FEAT17: Khóa / mở tài khoản

### STRQ6: Báo cáo quản trị
* FEAT18: Thống kê theo trạng thái | FEAT19: Báo cáo phòng ban | FEAT20: Dashboard lãnh đạo

### STRQ7: Hỗ trợ AI
* FEAT21: OCR tài liệu scan | FEAT22: Phân loại hồ sơ tự động | FEAT23: Gợi ý mức ưu tiên xử lý

---

## Các ràng buộc
* Hệ thống phải dễ sử dụng, bảo mật dữ liệu nội bộ tuyệt đối.
* Hỗ trợ mở rộng số lượng người dùng lớn, có khả năng sao lưu và phục hồi.
* Tương thích trình duyệt phổ biến, dễ bảo trì và nâng cấp.

---

## Các yêu cầu sản phẩm khác

### a. Yêu cầu chức năng
Bao gồm quản lý công văn, hồ sơ, phê duyệt, lịch họp, tài liệu số, người dùng, báo cáo, tìm kiếm và hỗ trợ AI.

### b. Yêu cầu phi chức năng
* **Hiệu năng:** Thời gian phản hồi trung bình < 3 giây; hỗ trợ tối thiểu 1.000 người dùng đồng thời.
* **Độ tin cậy:** Hoạt động ổn định 24/7; sao lưu dữ liệu tự động hằng ngày.
* **Bảo mật:** Kết nối bảo mật HTTPS.
* **Tương thích:** Hoạt động tốt trên máy tính, máy tính bảng và điện thoại.
