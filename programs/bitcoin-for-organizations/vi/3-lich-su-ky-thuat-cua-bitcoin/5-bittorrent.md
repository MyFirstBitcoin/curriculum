# 3.5 BitTorrent

Một dự án khác đã đóng vai trò quan trọng trong việc hình thành các loại tiền mã hóa trước khi bitcoin ra đời là BitTorrent.

Năm 2001, Bram Cohen đã phát hành một thiết kế cho một giao thức có tên là BitTorrent, được tạo ra để vận hành một hệ thống chia sẻ tệp ngang hàng (peer-to-peer). Anh bắt đầu làm việc tại một công ty tên là MojoNation, được thành lập để cho phép mọi người chia nhỏ các tệp tin bảo mật thành các phần được mã hóa và phân phối trên các máy tính chạy phần mềm này. Một bản sao của tệp sẽ được tải xuống đồng thời từ nhiều máy tính khác nhau. Mặc dù cuối cùng dự án này thất bại, nó đã đưa Cohen đến với lĩnh vực chia sẻ tệp, nơi anh quyết định mình có thể tạo ra một giao thức tốt hơn, bao gồm các yếu tố sau:

* Swarm: một cộng đồng các máy tính đang tải xuống hoặc tải lên nội dung
* Tracker: một công cụ chuyên dụng hoạt động tương tự như một công cụ tìm kiếm, nhưng theo dõi các tệp nằm trong swarm. Điều này giúp người dùng dễ dàng xem và truy cập bất kỳ tệp nào họ cần
* Phần mềm BitTorrent client: được cài đặt trên máy tính để truy cập tracker. Lưu ý rằng swarm là nơi duy nhất các tệp thực sự được lưu trữ
* Một cơ chế khuyến khích, trong đó người dùng tham gia mạng lưới với vai trò chia sẻ tệp sẽ được tải xuống nhanh hơn

Những điểm tương đồng với Bitcoin:

* Cả hai giao thức đều hoạt động theo mô hình ngang hàng (peer-to-peer)
* Thiết kế phi tập trung
* Các tệp BitTorrent và sổ cái Bitcoin đều được phân phối trên toàn mạng lưới
* Nguồn gốc mã nguồn mở (BitTorrent sau này trở thành phần mềm mã nguồn đóng)
