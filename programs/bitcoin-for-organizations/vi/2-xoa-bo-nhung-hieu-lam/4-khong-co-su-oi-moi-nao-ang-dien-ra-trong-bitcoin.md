# 2.4 Không có sự đổi mới nào đang diễn ra trong Bitcoin

> Sự hình thành của hàng ngàn khu rừng nằm trong một hạt sồi.  
_Ralph Waldo Emerson_

Những người chỉ trích thường cố gắng cho rằng Bitcoin là công nghệ 'lỗi thời' hoặc 'đã chết' vì nó không thay đổi giao thức lớp nền thường xuyên như các blockchain cạnh tranh. Lập luận này bỏ qua cả lý do tại sao các thay đổi đối với Bitcoin được áp dụng một cách chậm rãi và lượng đổi mới đang diễn ra để mở rộng mạng lưới ở các lớp cao hơn, như Lightning Network. Nó cũng bỏ qua thực tế rằng nhiều công nghệ linh hoạt và bền bỉ nhất của chúng ta cũng không phát triển nhanh ở lớp nền.

Ví dụ, cũng không có đổi mới nào diễn ra trong Giao thức Điều khiển Truyền tải (TCP), nền tảng của internet. TCP được tạo ra lần đầu vào năm 1974. Lần cuối cùng TCP được cập nhật là vào năm 1982. Nó làm đúng những gì nó cần làm. Nó không hoàn hảo, và vẫn có những tranh luận về việc liệu chúng ta có cần nâng cấp IPv4 để hỗ trợ sự phát triển của internet trong tương lai hay không. Tuy nhiên, nói rằng không có đổi mới nào trên internet kể từ năm 1982 sẽ là một tuyên bố đáng kinh ngạc. Tất cả đổi mới này đều diễn ra 'trên' TCP, chứ không phải 'trong' TCP.

Phần lớn đổi mới đang diễn ra không phải là 'trong' Bitcoin mà là 'trên' Bitcoin. Một ngày nào đó có thể sẽ không còn đổi mới nào 'trong' Bitcoin nữa, và đó nên là mục tiêu chứ không phải là sự chỉ trích, vì điều đó sẽ phản ánh mức độ nền tảng của nó trong việc hỗ trợ nền kinh tế toàn cầu bằng cách cung cấp nền móng cho một loại tiền tệ toàn cầu, trung lập và không cần sự cho phép. Một loại tiền tệ vững chắc cả về mặt kinh tế với nguồn cung cố định và sổ cái bất biến, mà còn vững chắc về mặt công nghệ vì nó không thay đổi và hệ thống đã vận hành liên tục trong nhiều năm không gián đoạn. Bitcoin đã đạt được 100% thời gian hoạt động trong 10 năm qua.

Tuy nhiên, sẽ là một vấn đề nếu không có đổi mới nào diễn ra 'trên' Bitcoin. Hãy cùng nhìn lại điều đó trong 10 năm qua:



#### 'Trong' Bitcoin

Segregated Witness (SegWit) được triển khai vào năm 2017 để bảo vệ khỏi việc thay đổi dữ liệu giao dịch và tăng dung lượng khối. SegWit cũng là bước đệm cần thiết để Lightning và một số sidechain hoạt động hiệu quả.

Taproot được triển khai vào năm 2021 để cho phép gộp và xác thực nhiều chữ ký bằng cách tích hợp chữ ký Schnorr, giới thiệu ngôn ngữ kịch bản để cho phép các chức năng phức tạp hơn và tăng cường quyền riêng tư cũng như khả năng chống kiểm duyệt của các giao dịch.



#### 'Trên' Bitcoin

##### Liquid Sidechain

Sidechain Liquid được triển khai vào năm 2018. Liquid, giống như các sidechain khác, là một sổ cái blockchain riêng biệt được liên kết với blockchain chính của Bitcoin, theo một bộ quy tắc được xác định trước. Những quy tắc này đủ linh hoạt để cho phép chuỗi Liquid phát triển và tích hợp các cải tiến về thiết kế và khả năng mở rộng theo thời gian. Tuy nhiên, liên kết với blockchain Bitcoin đảm bảo tổng nguồn cung 21 triệu bitcoin được nhất quán trên cả hai chuỗi.

Tài sản trong Liquid, L-BTC, được gắn chặt hai chiều với bitcoin trên chuỗi chính. Có những đánh đổi về chi phí, tốc độ, quyền riêng tư và bảo mật khiến L-BTC phù hợp cho một số ứng dụng nhất định. Chi phí, tốc độ và quyền riêng tư đều được cải thiện với L-BTC, đổi lại là phải đặt một phần niềm tin vào các tổ chức tạo nên Liên minh Liquid, những người cùng nhau kiểm soát quy trình đa chữ ký 11 trên 15 để chuyển đổi L-BTC sang bitcoin và ngược lại.

##### Lightning Network

Lightning Network được triển khai vào năm 2018. Lightning được thiết kế như một mạng thanh toán ngang hàng dưới dạng đồ thị các nút kết nối với nhau qua các kênh; nó không phải là một blockchain. Bitcoin được khóa bởi người vận hành nút trên blockchain chính để có thể sử dụng trên Lightning Network, điều này đảm bảo chỉ có bitcoin 'thật' được sử dụng. Các nút sau đó có thể mở các kênh thanh khoản thông qua hợp đồng thông minh đa chữ ký với nhau. Các khoản thanh toán sẽ tìm đường đi qua mạng từ nguồn đến đích, tối ưu hóa chi phí dựa trên yêu cầu rằng phải có đủ thanh khoản theo đúng hướng giữa mỗi bước nút trong tuyến đường. Lightning Network cải thiện đáng kể chi phí, tốc độ và quyền riêng tư, đổi lại là giảm bảo mật (hoặc tăng mức độ tin cậy cần thiết) và tăng độ phức tạp. Tuy nhiên, nó được thiết kế cho các khoản thanh toán hàng ngày với khối lượng lớn, giá trị nhỏ, nên đây được xem là sự đánh đổi rất hợp lý cho hàng triệu giao dịch mỗi ngày (nguồn: River, 2023).

##### Chaumian eCash Mints

Fedimint có thể được xem như một Lightning Network giới hạn trong cộng đồng. Chúng được thiết kế để tận dụng sự tin tưởng vốn có trong một số cộng đồng nhất định (ví dụ: gia đình, làng xóm, nhóm bạn bè) để đơn giản hóa sự phức tạp và tăng cường quyền riêng tư cho người dùng. Đây là các giao thức mã nguồn mở, dạng mô-đun để lưu ký và giao dịch bitcoin trong bối cảnh cộng đồng. Chúng tương thích với chính Lightning Network.

**Cashu** là một token mang giá trị có thể lưu trữ trên thiết bị như điện thoại di động; thiết kế nhằm tái hiện các lợi ích của tiền mặt vật lý nhưng ở dạng kỹ thuật số. Cashu là một ví dụ về Chaumian eCash được xây dựng trên Bitcoin, tăng cường quyền riêng tư, khả năng chống kiểm duyệt và giảm sự phức tạp, đổi lại là phải tin tưởng vào mint eCash đang sử dụng. Các mint Cashu phát hành token eCash, đại diện cho bitcoin, có thể được người dùng chi tiêu mà không tiết lộ danh tính. Cashu tương thích với Lightning Network.

Có khả năng sẽ có nhiều ứng dụng lớp 2 được xây dựng trong tương lai, với nhiều ứng dụng lớp 3 tiếp tục được phát triển trên mỗi ứng dụng đó.

Là một ví dụ về số lượng ứng dụng đáng kinh ngạc được xây dựng trên Lightning, dưới đây là một trích đoạn từ Báo cáo Nghiên cứu Lightning Network của River.

![The Lightning Network Industry Market Map 2023](https://cdn.sanity.io/images/vje9ehw2/staging/a5d3bdf5b343b7ae7e44663cf6e56a76a4bdec2d-501x706.svg)
