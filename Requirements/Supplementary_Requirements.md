# SUPPLEMENTARY REQUIREMENTS DOCUMENT (DỰ ÁN E-OFFICE HÒA PHÁT)

## Mục đích
Mục đích của tài liệu này là xác định và mô tả các yêu cầu bổ sung của hệ thống Quản lý Văn phòng – Hành chính cho Công ty Cổ phần Tập đoàn Hòa Phát mà không thể mô tả đầy đủ trong các Use Case. Các yêu cầu bổ sung tập trung vào các yếu tố chất lượng của hệ thống như hiệu năng, bảo mật, độ tin cậy, khả năng mở rộng, khả năng bảo trì, khả năng tích hợp và các ràng buộc kỹ thuật cần thiết để hệ thống vận hành hiệu quả trong môi trường doanh nghiệp quy mô lớn.

## Phạm vi
Tài liệu này cung cấp các hướng dẫn và yêu cầu cho việc xây dựng, triển khai và vận hành hệ thống Quản lý Văn phòng – Hành chính, bao gồm:
1. Quản lý công văn đến, công văn đi và hồ sơ nội bộ. 
2. Quản lý quy trình đề xuất, phê duyệt điện tử nhiều cấp. 
3. Quản lý lịch họp, lịch làm việc và đặt phòng họp. 
4. Quản lý kho tài liệu điện tử tập trung. 
5. Quản trị người dùng, phân quyền và bảo mật dữ liệu. 
6. Các chức năng hỗ trợ thông minh bằng AI.

## Định nghĩa, Các từ viết tắt và Các ký hiệu
* **Admin:** Quản trị viên hệ thống. 
* **Workflow:** Quy trình xử lý nghiệp vụ tự động. 
* **RBAC:** Role-Based Access Control – Phân quyền theo vai trò. 
* **AI:** Artificial Intelligence – Trí tuệ nhân tạo. 
* **KPI:** Chỉ số đánh giá hiệu quả công việc. 
* **SSO:** Single Sign-On – Đăng nhập một lần. 
* **Audit Log:** Nhật ký ghi nhận thao tác người dùng. 

## Tài liệu tham khảo 
[1] Managing Software Requirements: A Unified Approach.  
[2] Software & Systems Requirements Engineering: In Practice.  
[3] Requirements Engineering.  
[4] IEEE Recommended Practice for Software Requirements Specifications.

## Tổng quan
Tài liệu này mô tả chi tiết các yêu cầu bổ sung của dự án gồm:
1. Các yêu cầu phi chức năng liên quan đến chất lượng vận hành của hệ thống. 
2. Các tiêu chuẩn kỹ thuật cần tuân thủ trong quá trình phát triển và triển khai. 
3. Các ràng buộc về bảo mật, hiệu năng và khả năng mở rộng. 
4. Các yêu cầu giao diện và tích hợp với các hệ thống khác. 
5. Các tiêu chí đánh giá mức độ hoàn thiện của hệ thống.

## Chức năng
Không có yêu cầu chức năng bổ sung ngoài các Use Case đã được mô tả trong tài liệu Use Case Specification.

## Khả năng sử dụng
* **Khả năng truy cập:** Người dùng có thể truy cập hệ thống thông qua trình duyệt web nội bộ; hỗ trợ từ máy tính để bàn, laptop, máy tính bảng và điện thoại thông minh. Chỉ người dùng được cấp tài khoản mới có quyền truy cập. 
* **Tính dễ sử dụng:** Giao diện ngôn ngữ tiếng Việt rõ ràng, thống nhất. Các chức năng chính được bố trí theo nhóm nghiệp vụ dễ tìm kiếm. Người dùng mới có thể thực hiện các thao tác cơ bản sau tối đa 01 buổi hướng dẫn. Các biểu mẫu nhập liệu có hướng dẫn và thông báo lỗi cụ thể. 
* **Tính lao động:** Hệ thống giúp giảm thời gian xử lý công văn, đề xuất và phê duyệt thủ công; giảm khối lượng giấy tờ và công việc nhập liệu lặp lại; tăng khả năng phối hợp giữa các phòng ban.

## Khả năng kiểm thử
* Hệ thống phải cho phép kiểm thử độc lập từng module chức năng. 
* Giao diện không chứa các thành phần cản trở kiểm thử tự động. 
* Có môi trường kiểm thử riêng trước khi triển khai chính thức. 
* Các lỗi phát sinh trong kiểm thử phải được ghi nhận và xử lý đầy đủ. 

## Khả năng thích nghi
* Hệ thống có thể triển khai tại nhiều chi nhánh, nhà máy khác nhau. 
* Có thể cấu hình quy trình phê duyệt phù hợp từng đơn vị. 
* Có thể bổ sung phân hệ mới trong tương lai mà không ảnh hưởng hệ thống hiện tại.

## Khả năng bảo trì
* Mã nguồn được tổ chức theo module rõ ràng; có tài liệu kỹ thuật cho các chức năng chính. 
* Có cơ chế ghi log lỗi để hỗ trợ xử lý sự cố. 
* Việc nâng cấp phiên bản không làm mất dữ liệu hiện có.

## Độ tin cậy
* **Khả năng sẵn dùng:** Hệ thống có thể sử dụng tối thiểu **99.5%** thời gian trong giờ làm việc. Có cơ chế giám sát tình trạng hoạt động hệ thống. 
* **Độ mạnh:** Khi người dùng nhập dữ liệu sai định dạng, hệ thống phải thông báo lỗi rõ ràng. Hệ thống không được dừng đột ngột khi nhận dữ liệu không hợp lệ. 
* **Tính chính xác:** Thông tin công văn, lịch họp, trạng thái phê duyệt phải chính xác và nhất quán. Mỗi hồ sơ có mã định danh duy nhất. 
* **Khả năng phục hồi:** Có cơ chế sao lưu dữ liệu tự động hằng ngày. Có thể phục hồi dữ liệu khi xảy ra sự cố hệ thống. 
* **Dung thứ lỗi:** Khi một phân hệ phụ gặp lỗi, các phân hệ chính vẫn phải hoạt động nếu có thể. Hệ thống cần hạn chế lỗi dây chuyền. 
* **Tính an toàn:** Dữ liệu nội bộ phải được bảo vệ khỏi mất mát hoặc truy cập trái phép. Các thao tác xóa dữ liệu quan trọng phải có xác nhận. 
* **Tính an ninh:** Tài khoản quản trị phải sử dụng xác thực mạnh. Người dùng chỉ truy cập được chức năng theo quyền hạn được cấp. Toàn bộ giao tiếp mạng phải sử dụng **HTTPS**. 
* **Tính đúng đắn:** Sau khi triển khai, hệ thống không được tồn tại lỗi nghiêm trọng gây dừng toàn bộ hoạt động. Các lỗi nhỏ phải được xử lý trong các bản cập nhật tiếp theo. 

## Hiệu suất
* **Thời gian phản hồi:** Trung bình cho thao tác thông thường < 3 giây; thời gian tìm kiếm công văn hoặc tài liệu < 2 giây. 
* **Thời gian khôi phục:** Trong trường hợp lỗi máy chủ, hệ thống có thể phục hồi dịch vụ trong vòng 30 phút. Thời gian xử lý lỗi nghiêm trọng không quá 4 giờ làm việc. 
* **Thời gian khởi động/tắt:** Hệ thống hoàn tất khởi động trong vòng 5 phút. 
* **Khả năng chứa đựng/công suất:** Hệ thống hỗ trợ tối thiểu **3000 người dùng đồng thời**. Có khả năng mở rộng lên số lượng người dùng lớn hơn khi cần. 
* **Sự tận dụng tài nguyên:** Tài nguyên máy chủ phải được tối ưu để tránh lãng phí CPU, RAM và lưu trữ. Dữ liệu cũ có thể lưu trữ sang kho dữ liệu dự phòng.

## Khả năng hỗ trợ
* Hệ thống hỗ trợ kiểm thử tự động, kiểm thử hồi quy và có thể triển khai trên nhiều môi trường khác nhau. 
* Có dashboard giám sát lỗi và hiệu năng. 
* Tương thích: Chrome, Edge, Firefox phiên bản mới; hỗ trợ Windows, macOS. 
* Có thể cấu hình quy trình phê duyệt, vai trò người dùng, thông báo hệ thống. 
* Các bản cập nhật được triển khai phía máy chủ, không yêu cầu cài đặt lại phía người dùng. 
* Việc cài đặt mới được thực hiện tập trung tại máy chủ. 
* Hệ thống ghi nhận số lượng người dùng, số hồ sơ xử lý, dung lượng dữ liệu sử dụng. 
* Khả năng sử dụng lại các module: đăng nhập, thông báo, phân quyền. 
* Khả năng tương tác: Tích hợp với ERP, HRM, Email nội bộ, chữ ký số. 
* Khả năng kiểm toán: Nhật ký thao tác người dùng (Audit Log) phải được lưu đầy đủ để phục vụ kiểm tra. 
* Hỗ trợ tiếng Việt và có thể mở rộng thêm tiếng Anh trong tương lai. 

## Các ràng buộc về thiết kế 
* Hệ thống được xây dựng theo mô hình **Web-based Application**. 
* Kiến trúc phân lớp hoặc microservices tùy quy mô triển khai. 
* Cơ sở dữ liệu tập trung. 
* Có khả năng mở rộng tích hợp AI trong tương lai.

## Các yêu cầu cài đặt/triển khai
* Có môi trường Development, Testing và Production riêng biệt. 
* Máy chủ đáp ứng yêu cầu CPU, RAM, lưu trữ phù hợp số lượng người dùng. 
* Có cơ chế sao lưu dữ liệu định kỳ và kế hoạch khôi phục thảm họa.

## Tài liệu người dùng trực tuyến và trợ giúp
* Có tài liệu hướng dẫn sử dụng cho nhân viên và quản trị viên (PDF/Video). 
* Có mục trợ giúp trực tuyến tích hợp sẵn trong hệ thống. 

## Các yêu cầu về giao diện
* **Giao diện người dùng:** Dashboard trực quan, thanh tìm kiếm nhanh, thông báo thời gian thực. 
* **Giao diện phần cứng:** Máy tính văn phòng, laptop, điện thoại thông minh, máy scan tài liệu. 
* **Giao diện phần mềm:** Email nội bộ, ERP, HRM, Chữ ký số. 
* **Giao diện giao tiếp:** HTTP/HTTPS, REST API, SMTP Email Notification.
