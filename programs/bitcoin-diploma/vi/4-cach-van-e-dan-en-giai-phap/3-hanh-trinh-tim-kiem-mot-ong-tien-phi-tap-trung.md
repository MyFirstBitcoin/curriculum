# 4.3 Hành Trình Tìm Kiếm Một Đồng Tiền Phi Tập Trung

Chúng ta đã chứng kiến quá trình các ngân hàng và chính phủ dần kiểm soát tiền tệ trong suốt lịch sử, dẫn đến hệ thống tiền pháp định như ngày nay cùng những hậu quả tai hại cho xã hội. Tuy nhiên, sự xuất hiện của các công nghệ mới như mã hóa và internet đã cho phép những ý tưởng mới xuất hiện, chẳng hạn như tiền kỹ thuật số độc lập — không bị chính phủ can thiệp, mở và ai cũng có thể tiếp cận. Hãy cùng khám phá hành trình của những người dẫn đầu phong trào cách mạng này: các Cypherpunks.

#### Các Cypherpunks

> Máy tính có thể được sử dụng như một công cụ để giải phóng và bảo vệ con người, thay vì kiểm soát họ.  
_Hal Finney_

Nửa sau thế kỷ 20 chứng kiến sự xuất hiện của những công nghệ mạnh mẽ mới như máy tính cá nhân và internet. Những đổi mới này bắt đầu thay đổi cách con người giao tiếp, chia sẻ thông tin và tổ chức xã hội.

Một số nhà tư tưởng và lập trình viên nhận ra rằng các công nghệ này có thể gia tăng tự do cá nhân hoặc cho phép chính phủ và các tập đoàn dễ dàng giám sát, kiểm soát con người hơn.

Nhóm này được biết đến với tên gọi Cypherpunks. Họ tin rằng mật mã học, tức việc sử dụng mã toán học để bảo vệ thông tin, có thể bảo vệ tự do cá nhân trong thời đại số.

Các Cypherpunks đã phát triển những công cụ giúp bảo vệ quyền riêng tư trên mạng, bảo mật liên lạc và cho phép mọi người tương tác trên internet mà không cần dựa vào các tổ chức tập trung.

Một trong những mục tiêu chính của họ là tạo ra một dạng tiền kỹ thuật số mà mọi người có thể sử dụng mà không bị ngân hàng hay chính phủ kiểm soát. Bitcoin sau này đã được tạo ra như một giải pháp cho vấn đề này.


> **Definition – Định nghĩa về một tương lai kiểu orwell**
>
> **Tương lai kiểu orwell** đề cập đến một xã hội phản địa đàng, nơi một thế lực quyền lực, thường là chính phủ, kiểm soát chặt chẽ cuộc sống của người dân. Trong thế giới đó, công dân luôn bị theo dõi, thông tin bị thao túng và việc lên tiếng chống lại những người cầm quyền có thể dẫn đến trừng phạt. Quyền tự do cá nhân bị hạn chế, và sự thật thường bị bóp méo để duy trì quyền kiểm soát dân chúng.


Những nhân vật chủ chốt trong phong trào Cypherpunk bao gồm Eric Hughes, Timothy C. May và John Gilmore. Năm 1992, Eric Hughes đã viết _Tuyên ngôn Cypherpunk_, trong đó lập luận rằng mọi người nên có quyền riêng tư và kiểm soát cuộc sống số của mình.

Các Cypherpunks tin rằng mật mã học có thể bảo vệ cá nhân trên mạng. Năm 1991, Phil Zimmermann đã tạo ra PGP (Pretty Good Privacy), một công cụ cho phép mọi người gửi email được mã hóa để chỉ người nhận dự định mới đọc được.

Họ tin rằng mã hóa, kết hợp với internet và máy tính, có thể cho phép mọi người giao tiếp và tương tác trực tuyến mà không cần dựa vào các tổ chức trung gian.

Tuy nhiên, vẫn còn một vấn đề lớn chưa được giải quyết: thế giới vẫn thiếu một loại tiền kỹ thuật số phi tập trung mà mọi người có thể tự do sử dụng trên internet.

#### Hệ thống Tập trung và Phi tập trung

##### Hệ thống Tập trung

Trong một hệ thống tập trung, mọi thứ đều xoay quanh một cơ quan chính, giống như một tòa nhà cao tầng trong thành phố. Cơ quan này kiểm soát cách toàn bộ hệ thống vận hành. Hãy nghĩ đến các ngân hàng truyền thống như một ví dụ, nơi một nhóm nhỏ đưa ra mọi quyết định.

###### Vấn đề của Hệ thống Tập trung

* **Điểm yếu tập trung**: Nếu cơ quan trung tâm gặp sự cố, cả hệ thống có thể sụp đổ.
* **Kiểm soát**: Một nhóm nhỏ ở trên cùng nắm toàn bộ quyền lực và kiểm soát, thường dẫn đến các quyết định có lợi cho họ thay vì cho tất cả mọi người.
* **Kém hiệu quả và nhiều trung gian**: Giống như tắc đường trong thành phố, hệ thống tập trung có thể trở nên chậm chạp và tốn kém do có quá nhiều bên trung gian không cần thiết.
* **Thiếu tự chủ**: Mọi người có thể không được tự quyết định tài chính của mình; tất cả đều do cơ quan trung tâm quyết định.
* **Kiểm duyệt và hạn chế**: Giống như một số khu vực trong thành phố có thể bị chặn lại, hệ thống tập trung có thể chặn hoặc hạn chế quyền truy cập vào một số nguồn lực tài chính.
* **Khó mở rộng**: Khi nhiều người cần dịch vụ tài chính hơn, hệ thống tập trung có thể gặp khó khăn trong việc đáp ứng.
* **Rủi ro bảo mật**: Sự cố ở cơ quan trung tâm có thể khiến cả hệ thống gặp rủi ro bị tấn công mạng.
* **Thiếu minh bạch và niềm tin**: Cách vận hành bên trong của hệ thống tập trung có thể rất khó hiểu, khiến mọi người khó tin tưởng.


> **Light**
>
> Năm 2022, trong các cuộc biểu tình ôn hòa ở Canada, các ngân hàng đã đóng băng tài khoản của người biểu tình, cho thấy một cơ quan trung tâm có thể kiểm soát quyền truy cập tài chính như thế nào.


##### Hệ thống Phi tập trung

Hãy tưởng tượng một hệ thống phi tập trung giống như một khu rừng. Mỗi cái cây là một phần riêng biệt, và cả khu rừng là hệ thống. Khác với thành phố chỉ có một điểm trung tâm, hệ thống phi tập trung bền vững hơn và vẫn có thể hoạt động ngay cả khi một phần bị hỏng.

###### Lợi ích của Hệ thống Phi tập trung

* **Tăng khả năng phục hồi và độ tin cậy**: Không có điểm yếu tập trung, hệ thống trở nên mạnh mẽ ngay cả khi có sự cố xảy ra.
* **Tăng cường bảo mật**: Với mã hóa/bảo vệ phù hợp, hệ thống phi tập trung chống lại sự kiểm soát từ một cơ quan duy nhất tốt hơn.
* **Chủ quyền lớn hơn**: Mọi người có nhiều quyền kiểm soát hơn đối với tiền, dữ liệu và lựa chọn của mình.
* **Minh bạch hơn**: Ai cũng nhìn thấy cùng một thông tin, giúp hệ thống trở nên đáng tin cậy hơn.
* **Không cần cấp phép và không giới hạn**: Bất kỳ ai cũng có thể tham gia hoặc góp phần.
* **Cơ hội bình đẳng**: Mọi người đều có cơ hội công bằng để đóng góp và lên tiếng.
* **Tăng cường quyền riêng tư**: Dữ liệu được phân phối giữa nhiều người tham gia và phần lớn là ẩn danh, giúp các hệ thống phi tập trung riêng tư hơn.

Mặc dù các hệ thống phi tập trung có nhiều ưu điểm, việc ra quyết định chung có thể hơi phức tạp. Nó đòi hỏi mọi người phải hợp tác cùng nhau.

Trong một thế giới có cả hệ thống tập trung và phi tập trung, tất cả đều xoay quanh việc ai nắm giữ quyền lực. Hệ thống tập trung trao quyền cho một nhóm nhỏ, trong khi hệ thống phi tập trung phân tán quyền lực, cho phép mọi người đều có tiếng nói. Sự chuyển dịch quyền lực này sẽ mang lại một tương lai công bằng hơn, nơi nhiều người cùng ảnh hưởng đến hệ thống định hình cuộc sống của họ.


> **Light**
>
> Mạng Tor tạo ra một hệ thống phi tập trung, nơi mọi người có thể ẩn danh khi trực tuyến và mạng lưới này rất khó bị ngăn chặn hoặc kiểm duyệt.


#### Lược sử về các loại tiền kỹ thuật số

Một trong những ý tưởng then chốt được các Cypherpunk bàn luận là **tiền điện tử**. Họ tin rằng tiền nên được tách khỏi sự kiểm soát của chính phủ để mọi người có thể tự do và riêng tư gửi, nhận thanh toán trực tuyến.

Nhà mật mã học tiên phong **Minh** đã tạo ra một trong những hệ thống tiền điện tử đầu tiên bằng cách sử dụng mật mã để làm cho giao dịch an toàn và riêng tư. Tuy nhiên, hệ thống của anh ấy vẫn dựa vào một **cơ quan trung ương** để vận hành, điều này có nghĩa là nó có thể thất bại hoặc kiểm duyệt giao dịch.

Trong những thập kỷ tiếp theo, nhiều Cypherpunk đã cố gắng thiết kế một dạng tiền kỹ thuật số không phụ thuộc vào cơ quan trung ương. Dù họ đã đưa ra nhiều đổi mới quan trọng, nhưng không hệ thống nào giải quyết được tất cả các thách thức cần thiết cho một loại tiền kỹ thuật số an toàn, phi tập trung và dễ sử dụng rộng rãi.

Những nỗ lực này đã giúp chỉ ra những điều còn thiếu sót. Sau đó, ai đó đã phát triển dựa trên các ý tưởng này và cuối cùng tạo ra một hệ thống tiền kỹ thuật số phi tập trung hoạt động thực sự.

###### Tài nguyên


[▶ Xem video này để khám phá câu chuyện về các Cypherpunk!](https://www.youtube.com/watch?v=9vM0oIEhMag)
