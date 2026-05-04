# 3.0 Giới thiệu

> **Info – Tóm tắt Sách Trắng Bitcoin**
>
> **Một phiên bản tiền điện tử hoàn toàn ngang hàng** sẽ cho phép các khoản thanh toán trực tuyến được gửi trực tiếp từ người này sang người khác mà không cần thông qua một tổ chức tài chính.**Chữ ký số cung cấp một phần giải pháp**, nhưng lợi ích chính sẽ bị mất nếu vẫn cần một **bên thứ ba đáng tin cậy** để ngăn chặn việc chi tiêu hai lần. Chúng tôi đề xuất một giải pháp cho vấn đề chi tiêu hai lần bằng cách sử dụng một **mạng ngang hàng**. **Mạng sẽ đánh dấu thời gian cho các giao dịch** bằng cách băm chúng vào một chuỗi liên tục của **bằng chứng công việc dựa trên hàm băm,** tạo thành một bản ghi không thể thay đổi nếu không thực hiện lại **bằng chứng công việc**. Chuỗi dài nhất không chỉ là bằng chứng về trình tự các sự kiện đã được xác nhận, mà còn là bằng chứng rằng nó xuất phát từ nhóm sức mạnh xử lý lớn nhất. Miễn là phần lớn sức mạnh xử lý được kiểm soát bởi các nút không hợp tác để tấn công mạng, họ sẽ tạo ra chuỗi dài nhất và vượt qua những kẻ tấn công.**Bản thân mạng lưới yêu cầu cấu trúc tối thiểu. Các thông điệp được phát sóng dựa trên nỗ lực tốt nhất, và các nút có thể rời khỏi hoặc tham gia lại mạng bất cứ lúc nào**, chấp nhận chuỗi bằng chứng công việc dài nhất như là bằng chứng về những gì đã xảy ra trong thời gian họ vắng mặt.


Bitcoin không xuất hiện một cách ngẫu nhiên mà được xây dựng dựa trên thành quả của nhiều người trong các thập kỷ trước đó. Phần này sẽ khám phá nền tảng của internet mà Bitcoin dựa vào, cũng như các nghiên cứu và phát triển được ghi nhận trong sách trắng.

Vào những năm 70, một nhóm cá nhân đã nhận thấy chính phủ Hoa Kỳ, đặc biệt là, đang cố gắng hạn chế quyền truy cập vào mật mã học, và họ đã nỗ lực để đảm bảo công nghệ này sẽ được phổ biến cho tất cả mọi người nhằm bảo vệ quyền riêng tư trực tuyến. Một số người tiên phong này cũng tập trung vào tiềm năng của một hệ thống 'tiền tệ lành mạnh' kỹ thuật số có thể được sử dụng để lưu trữ và trao đổi giá trị trên internet mới nổi. Friedrich Hayek – một nhà đóng góp hàng đầu cho kinh tế học Áo – đã hình dung ra một loại tiền tệ lý tưởng dựa trên cạnh tranh thị trường tự do từ trước thời internet, nhưng ông cho rằng điều đó là không khả thi về mặt kỹ thuật và chính trị. Bên cạnh quyền riêng tư kỹ thuật số, nhóm này, sau này phát triển thành Cypherpunks, đã cố gắng hiện thực hóa tầm nhìn của Hayek về tiền kỹ thuật số, nhưng những nỗ lực này đều thất bại cho đến khi Satoshi công bố ý tưởng của mình trên danh sách thư điện tử.

* Giao thức TCP/IP (1976)
* Giao thức cho Hệ mật mã Khóa công khai - Ralph Merkle (1980)
* Digicash - David Chaum (1989)
* Đánh dấu thời gian kỹ thuật số (những năm 90)
* Hashcash - Adam Back (1997)
* BitTorrent - Bram Cohen (2001)
* POW có thể tái sử dụng - Hal Finney (2004)
* Sách Trắng Bitcoin - Satoshi Nakamoto (2008)

Một ảnh hưởng quan trọng đến sự phát triển của Bitcoin là sự xuất hiện của phong trào Cypherpunk vào những năm 1990. Họ đã phát triển nhiều công nghệ mật mã, bao gồm mật mã khóa công khai để cho phép người dùng giao tiếp và chia sẻ thông tin một cách an toàn, riêng tư. Nhiều phát triển được mô tả ở đây và những người tham gia đều là thành viên của nhóm này.

Nhu cầu về tiền kỹ thuật số cũng đã được nhận ra và nhiều nỗ lực đã được thực hiện để tạo ra nó, nhưng đều có những hạn chế khiến chúng không thành công. Sự thiên tài của Satoshi Nakamoto là đã kết hợp những khả năng này lại, cùng với một số đổi mới của riêng mình, xây dựng trên đó để tạo ra giao thức Bitcoin như ngày nay. Trong các phần tiếp theo, chúng ta sẽ khám phá một số phát triển này và giải thích cách chúng đã giúp định hình thiết kế của Bitcoin. Chúng ta cũng sẽ thảo luận về những mảnh ghép còn thiếu mà Satoshi đã giải quyết được.
