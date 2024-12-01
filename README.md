# LapTrinhMang
Giới thiệu phần mềm phát video trong mạng LAN
Phần mềm phát video trong mạng LAN là một ứng dụng cho phép một máy tính trong mạng nội bộ (LAN) phát video trực tiếp (livestream), và các máy khác trong cùng mạng có thể tham gia để xem. Điều này tương tự như tính năng phát trực tiếp, nhưng chỉ giới hạn trong mạng nội bộ, giúp tiết kiệm băng thông internet và phù hợp với các môi trường như văn phòng, lớp học, hoặc các sự kiện nhỏ.

Mô hình hoạt động:
Máy phát: Chọn tệp video hoặc sử dụng camera để phát trực tiếp nội dung.
Các máy xem: Kết nối vào nhóm phát (group stream) và nhận luồng video.
Phương thức giao tiếp: Sử dụng giao thức UDP hoặc multicast để truyền tải dữ liệu video, đảm bảo tốc độ và giảm độ trễ.
Chức năng chính
1. Máy phát (Broadcast Server)
Chọn tệp video từ ổ cứng hoặc phát trực tiếp từ camera.
Hỗ trợ các định dạng video phổ biến như MP4, AVI, MKV.
Tùy chỉnh chất lượng video (độ phân giải, tốc độ bit).
Hỗ trợ nhiều luồng phát (multi-stream) cùng lúc.
Gửi thông báo tới các máy trong mạng LAN khi bắt đầu phát video.
2. Máy xem (Client Viewer)
Hiển thị danh sách các luồng video hiện có trong mạng LAN.
Kết nối nhanh chóng vào luồng phát.
Tùy chỉnh kích thước cửa sổ video hoặc xem toàn màn hình.
Tự động đồng bộ thời gian nếu bị giật hoặc mất khung hình.
3. Quản lý nhóm phát
Tạo nhóm phát với quyền riêng tư (public hoặc private group).
Đặt mật khẩu bảo vệ cho luồng phát.
Quản lý người tham gia (kick, block user nếu cần).
4. Cài đặt chung
Tích hợp codec để hỗ trợ nhiều định dạng video.
Tùy chỉnh port và giao thức mạng (UDP, multicast hoặc TCP).
Kiểm tra tình trạng kết nối (ping, tốc độ mạng).
Ưu điểm
Dễ sử dụng: Không yêu cầu cấu hình mạng phức tạp.
Tiết kiệm tài nguyên: Sử dụng băng thông mạng LAN, không cần internet.
Tốc độ cao: Truyền phát video nhanh với độ trễ thấp.

1. VLC Media Player
Tính năng nổi bật:
Phát video trực tiếp qua giao thức HTTP, UDP, hoặc RTP.
Hỗ trợ hầu hết các định dạng video (MP4, MKV, AVI, FLV...).
Giao diện thân thiện và dễ sử dụng.
Cách hoạt động:
Cấu hình trên máy chủ:
Mở VLC > Chọn Media > Stream.
Thêm file video cần phát > Nhấn Stream.
Chọn giao thức (HTTP, UDP, hoặc RTP).
Thiết lập địa chỉ IP và cổng (ví dụ: 192.168.1.100:8080).
Trên máy khách:
Mở VLC > Chọn Media > Open Network Stream.
Nhập URL phát (ví dụ: http://192.168.1.100:8080).
Máy khách sẽ nhận được luồng video.
2. Plex Media Server
Tính năng nổi bật:
Tích hợp phát video trong mạng LAN và từ xa qua internet.
Tự động tổ chức và gắn nhãn các file video.
Ứng dụng hỗ trợ đa nền tảng (Windows, macOS, iOS, Android).
Cách hoạt động:
Cài đặt Plex Server trên máy chủ:
Tải về và cài đặt Plex từ trang chủ Plex.
Thêm thư viện video.
Truy cập từ máy khách:
Mở ứng dụng Plex trên thiết bị máy khách hoặc trình duyệt.
Đăng nhập và kết nối với server trong mạng LAN.
Máy khách sẽ xem được danh sách video và phát trực tiếp.
3. Kodi (XBMC)
Tính năng nổi bật:
Tích hợp tính năng phát nội dung qua giao thức DLNA/UPnP.
Hỗ trợ nhiều plugin mở rộng.
Giao diện thân thiện và hỗ trợ tùy chỉnh.
Cách hoạt động:
Thiết lập trên máy chủ:
Cài đặt Kodi > Vào Settings > Services > UPnP/DLNA.
Bật Share video and music libraries through UPnP.
Truy cập từ máy khách:
Mở Kodi trên máy khách > Chọn Videos > Add Videos.
Tìm kiếm server trong mạng LAN và chọn video cần phát.
4. Serviio
Tính năng nổi bật:
Hỗ trợ phát video qua DLNA cho TV thông minh, điện thoại, và PC.
Tự động chuyển đổi định dạng file không tương thích.
Tích hợp tính năng bảo vệ mật khẩu cho thư viện.
Cách hoạt động:
Cài đặt Serviio trên máy chủ:
Tải về từ Serviio.
Thêm thư viện video cần phát.
Truy cập từ máy khách:
Dùng ứng dụng DLNA/UPnP client hoặc TV thông minh để dò tìm server trong mạng LAN.

https://github.com/user-attachments/assets/fb9f15aa-7d38-4b86-b124-4a6d680ce869
