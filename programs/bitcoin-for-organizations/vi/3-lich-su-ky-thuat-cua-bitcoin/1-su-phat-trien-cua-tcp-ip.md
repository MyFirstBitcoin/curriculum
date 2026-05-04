# 3.1 Sự phát triển của TCP/IP

Hầu hết chúng ta đều quen thuộc với các giao thức TCP/IP đang được sử dụng ngày nay như là nền tảng cho internet. Nguồn gốc của chúng bắt đầu từ cuối những năm 70 khi các nhà khoa học đang nghiên cứu các thiết kế thay thế cho Arpanet – một mạng lưới còn sớm hơn nữa được Bộ Quốc phòng Hoa Kỳ phát triển nhằm cho phép chia sẻ tài nguyên giữa các máy tính ở xa. TCP/IP trở thành tiêu chuẩn giao thức cho Arpanet vào năm 1983, điều này đã dẫn đến việc nó trở thành mô hình mạng chiếm ưu thế vào cuối những năm 1990 và là nền tảng cho internet mà Bitcoin đang hoạt động ngày nay.


| Mô hình OSI | TCP/IP |
| --- | --- |
| Ứng dụng | Ứng dụng |
| Trình bày | Ứng dụng |
| Phiên | Ứng dụng |
| Vận chuyển | Vận chuyển |
| Mạng | Mạng |
| Liên kết dữ liệu | Liên kết dữ liệu |
| Vật lý | Vật lý |


Cùng thời điểm mô hình TCP/IP được phát triển, một khuôn khổ tương tự nhưng toàn diện hơn cũng đang được Tổ chức Tiêu chuẩn hóa Quốc tế (ISO) và ngành viễn thông (CCITT) phát triển. Quá trình phát triển các giao thức mới hoặc đề xuất thay đổi diễn ra chậm và cồng kềnh hơn so với cách tiếp cận phi tập trung hơn được sử dụng để phát triển TCP/IP, dẫn đến sự thống trị của phương pháp này ngày nay.

##### Yêu cầu thay đổi

Bất kỳ phát triển nào được đề xuất cho các giao thức hiện có hoặc ý tưởng cho giao thức mới đều có thể được đề xuất trong mô hình TCP/IP thông qua một **Yêu cầu thay đổi** quy trình. Những đề xuất này sẽ trải qua một quy trình phê duyệt, được quản lý bởi Nhóm Đặc trách Kỹ thuật Internet (IETF), và sẽ trở thành mã nguồn mở sau khi được phê duyệt để bất kỳ ai cũng có thể triển khai và áp dụng. Một số ví dụ đáng chú ý:

* 1969 RFC 1 Tài liệu hóa cách các gói tin sẽ được gửi trong Arpanet
* 1981 RFC791 định nghĩa giao thức Internet V4 – vẫn được sử dụng rộng rãi ngày nay
* 1982 RFC 821 Giao thức chuyển thư đơn giản (SMTP)
* 1987 Hệ thống tên miền – cách tên miền được phân giải thành địa chỉ IP
* 1999 RDC 2616 Giao thức truyền siêu văn bản – thiết yếu cho việc duyệt web


> **Callout**
>
> Đề xuất cải tiến **Bitcoin** (BIP) tuân theo cách tiếp cận tương tự như RFC, nhưng chỉ tập trung vào việc cải tiến chính Bitcoin thay vì phát triển các giao thức mới hoặc thay thế. Bitcoin cũng vay mượn từ mô hình phân lớp này, và bạn sẽ thấy các giao thức bổ sung được mô tả là lớp hai hoặc ba.


Cũng giống như các lớp cơ sở của mô hình TCP/IP đã thay đổi rất ít trong vài thập kỷ qua, với sự đổi mới diễn ra ở các lớp cao hơn, lớp cơ sở của Bitcoin cũng được kỳ vọng sẽ thay đổi rất chậm ở thời điểm này, với các giải pháp mở rộng như Lightning và Liquid diễn ra ở các lớp trên.

Một ví dụ điển hình về việc các giao thức lớp cơ sở trở nên khó thay đổi theo thời gian là IPv6. Việc dự đoán cạn kiệt không gian địa chỉ trong IPv4 đã tạo ra nhu cầu cho một giao thức mới. Bản dự thảo tiêu chuẩn đầu tiên được tạo ra vào năm 1998, nhưng mãi đến năm 2017 mới được phê duyệt là tiêu chuẩn internet. Dù nó đã giải quyết nhiều vấn đề của IPv4 và có tính tương lai cao hơn nhiều, nhưng việc áp dụng trong ngành vẫn rất chậm. Trong thời gian này, nhiều giao thức mới đã được định nghĩa ở các lớp trên để hỗ trợ đa phương tiện, email, v.v.

##### Các khối xây dựng được Bitcoin sử dụng

Việc tách biệt các vấn đề về khả năng kết nối này cho phép các giao thức được phát triển độc lập với các lớp phía trên và phía dưới nó. Thay vì phải phát minh lại giải pháp cho từng lớp, mạng lưới Bitcoin có thể dựa vào các khả năng cơ bản của mạng được cung cấp ở các lớp vật lý và liên kết dữ liệu.


| Lớp | TCP/IP Gốc |
| --- | --- |
| Ứng dụng | Sử dụng Hệ thống tên miền (DNS) để xác định các nút lân cận. Cổng 8333 báo hiệu giao thức Bitcoin. |
| Vận chuyển | UDP cho giao tiếp FIBRE giữa các thợ đào để giảm độ trễ. TCP cho giao tiếp ngang hàng giữa các nút. |
| Vận chuyển | Định tuyến TOR: Cho phép ẩn danh và bảo mật. Giao thức phát sóng: Định tuyến lưu lượng trên toàn mạng. |
| Liên kết | Hoạt động trên bất kỳ phương tiện nào (ví dụ: Ethernet, Wi-Fi, v.v.) |
| Vật lý | Truyền vật lý qua không dây, Ethernet hoặc các giao diện phần cứng khác. |


##### Bitcoin là một giao thức trung lập để chuyển giá trị giống như HTTPS là một giao thức để truyền thông tin

* **HTTPS**: Trang web bảo mật
* **SMTP**: Gửi Email
* **FTP**: Chuyển tập tin
* **DNS**: Quản lý tên miền
* **BTC**: Lưu trữ và chuyển giá trị

Bitcoin cho phép giá trị được chuyển giao một cách đáng tin cậy và không cần bên thứ ba giữa mọi người hoặc thiết bị qua Internet. Điều này được kỳ vọng sẽ mở ra giá trị to lớn.
