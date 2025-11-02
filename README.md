# cryptography-lab
Xây dựng bài lab về mã hoá đường cong trên nền tảng labtainer

Tài liệu này cung cấp hướng dẫn chi tiết các bước cần thiết để tải môi trường, thực hiện và nộp bài thực hành (lab) trên hệ thống SecLab dành cho sinh viên Học viện Công nghệ Bưu chính Viễn thông.

1. Công tác Chuẩn bị

Trước khi bắt đầu, sinh viên cần đảm bảo các yêu cầu sau:

Máy tính cá nhân: Cần thiết để cài đặt và chạy môi trường ảo.

Phần mềm ảo hóa: Đã cài đặt một trong hai phần mềm: VMware Workstation Player/Pro hoặc VirtualBox.

Tài khoản SecLab: Đã được cấp tài khoản đăng nhập hệ thống. Thông thường, tên đăng nhập và mật khẩu mặc định là Mã Sinh Viên (viết hoa).

2. Tải và Cài đặt Môi trường Thực hành

Bước 1: Tải tệp môi trường ảo:

Đối với người dùng VMware: Truy cập đường dẫn được cung cấp trong tài liệu hướng dẫn (SecLab-HDSD_SV_V1.pdf, trang 13-14) để tải tệp .ova.


Đối với người dùng VirtualBox: Truy cập đường dẫn tương ứng được cung cấp trong tài liệu hướng dẫn (SecLab-HDSD_SV_V1.pdf, trang 13-14) để tải tệp .ova.


Bước 2: Import máy ảo: Khởi chạy phần mềm ảo hóa (VMware hoặc VirtualBox), sử dụng chức năng "Import" hoặc "Open" để nhập tệp .ova vừa tải về.

Bước 3: Khởi động máy ảo: Chạy máy ảo vừa import. Giao diện hệ điều hành Ubuntu sẽ hiển thị khi khởi động thành công.

3. Quy trình Thực hiện Bài Thực hành


Bước 1: Đăng nhập Cổng SecLab: Mở trình duyệt web và truy cập địa chỉ https://seclab.ptit.edu.vn. Đăng nhập bằng tài khoản đã được cấp. Nếu đây là lần đăng nhập đầu tiên, hệ thống sẽ yêu cầu thay đổi mật khẩu mặc định.




Bước 2: Truy cập Bài Thực hành: Sau khi đăng nhập, điều hướng đến mục "Bài tập" (để luyện tập) hoặc "Cuộc thi" (nếu tham gia ca thực hành/thi có giới hạn thời gian). Tìm và chọn bài thực hành cần thực hiện để xem chi tiết yêu cầu đề bài.





Bước 3: Mở Terminal trên Máy ảo: Trong môi trường máy ảo Ubuntu đang chạy, mở ứng dụng Terminal.

Bước 4: Khởi động Môi trường Lab: Tại cửa sổ Terminal, nhập lệnh sau, thay thế <tên_bài_lab> bằng mã hoặc tên chính xác của bài thực hành được ghi trên SecLab:


labtainer <tên_bài_lab> Ví dụ: labtainer nmap-discovery  Hệ thống sẽ tiến hành tải và thiết lập môi trường riêng cho bài thực hành này. Quá trình này có thể mất vài phút.



Bước 5: Nhập Mã Sinh Viên: Khi môi trường lab khởi động và hiển thị yêu cầu "Please enter your e-mail address:", sinh viên bắt buộc phải nhập chính xác Mã Sinh Viên của mình (viết HOA). Đây là bước quan trọng để hệ thống ghi nhận kết quả bài làm.

Bước 6: Thực hiện Yêu cầu: Dựa vào nội dung đề bài hiển thị trên trang web SecLab, sinh viên thực hiện các thao tác và lệnh cần thiết trong môi trường máy ảo (các cửa sổ Terminal mới có thể xuất hiện tùy theo bài lab).

4. Kiểm tra Kết quả trong Quá trình Thực hiện

Trong khi làm bài, sinh viên có thể kiểm tra tiến độ hoàn thành các yêu cầu bằng cách mở cửa sổ Terminal student@ubuntu và thực thi lệnh:


checkwork 

Kết quả trả về sẽ cho biết những phần nào đã được hệ thống ghi nhận là hoàn thành (thường được đánh dấu bằng ký tự 'Y'). Sinh viên có thể thực hiện lệnh này nhiều lần.


5. Hoàn thành và Nộp Bài Thực hành

Bước 1: Kết thúc Bài Thực hành (Tùy chọn): Sau khi hoàn thành tất cả yêu cầu, sinh viên có thể nhập lệnh stoplab <tên_bài_lab> tại Terminal student@ubuntu để dừng môi trường lab.


Bước 2: Tìm tệp Kết quả: Tệp chứa kết quả bài thực hành sẽ được tự động lưu vào thư mục labtainer_xfer trên màn hình Desktop của máy ảo Ubuntu. Tên tệp thường có dạng liên quan đến tên bài lab và Mã Sinh Viên.

Bước 3: Nộp tệp Kết quả: Quay lại trang web SecLab, truy cập vào đúng bài thực hành vừa hoàn thành. Sử dụng chức năng "Chọn tệp" (hoặc nút tương tự) để tải lên tệp kết quả từ thư mục labtainer_xfer. Nhấn nút "Nộp bài" để gửi kết quả lên hệ thống chấm điểm.



Bước 4: Kiểm tra Trạng thái: Sau khi nộp, hệ thống sẽ chấm bài tự động. Kết quả "AC" (Accepted) hoặc trạng thái hoàn thành (ví dụ, bài tập chuyển sang màu xanh) xác nhận bài làm đã được chấp nhận. Sinh viên có thể xem lại lịch sử nộp bài trong mục "Lịch sử" hoặc "Trạng thái giải bài".





Lưu ý: Ngay cả sau khi đã dùng lệnh stoplab, sinh viên vẫn có thể kiểm tra lại kết quả chi tiết bằng lệnh checkwork <tên_bài_lab>
