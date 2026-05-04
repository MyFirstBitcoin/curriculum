# 6.2 Giới thiệu về Ví

Không giống như tiền vật lý, bitcoin thực chất không nằm trong ví Bitcoin. Thay vào đó, chúng tồn tại trên sổ cái phân tán mà mạng lưới Bitcoin liên tục xác minh và bảo mật. Vậy, làm thế nào bạn có thể sở hữu bitcoin?

Bạn chỉ thực sự sở hữu bitcoin khi bạn kiểm soát các khóa riêng tư cho phép bạn ký giao dịch và chuyển quyền sở hữu bitcoin của mình cho người khác. Đây chính là hành động gửi bitcoin.

Hãy cùng xem hai khái niệm mà chúng ta nhắc đến khi sử dụng thuật ngữ **ví**:

* Một khóa riêng chủ, giống như mật khẩu, từ đó các khóa công khai của bạn, giống như địa chỉ email, được tạo ra. Bạn có thể chia sẻ địa chỉ công khai với người khác để nhận và gửi bitcoin, nhưng tuyệt đối không bao giờ được chia sẻ khóa riêng tư!
* Giao diện trên điện thoại hoặc máy tính dùng để tương tác với mạng lưới Bitcoin, kiểm tra số dư bitcoin, gửi và nhận giao dịch, cũng như phát giao dịch lên mạng. Các loại ví khác nhau, cùng với ưu điểm và nhược điểm của chúng, sẽ được trình bày ở các phần tiếp theo.

#### Ví tự quản lý và ví lưu ký

Trước khi đi sâu vào các loại ví Bitcoin khác nhau và đặc điểm của chúng, hãy làm rõ sự khác biệt quan trọng giữa ví tự quản lý và ví lưu ký. Mỗi loại đều có lợi ích, rủi ro và mức độ kiểm soát bitcoin khác nhau. Tự quản lý nghĩa là người dùng giữ khóa riêng và thực sự kiểm soát bitcoin của mình; còn với ví lưu ký, một bên thứ ba giữ bitcoin thay cho người dùng.


| Loại | Kiểm soát | Lợi ích | Rủi ro |
| --- | --- | --- | --- |
| Tự quản lý | Người dùng | Kiểm soát hoàn toàn tài sản và giao dịch, không cần phê duyệt hay bị đóng băng tài khoản, không bị kiểm soát bởi công ty hay chính phủ, được bảo vệ khỏi việc bị tịch thu. | Không thể khôi phục nếu mất cụm từ khôi phục, toàn bộ trách nhiệm thuộc về người dùng. |
| Lưu ký | Nhà cung cấp bên thứ ba | Dễ dàng khôi phục nếu mất quyền truy cập, hỗ trợ khách hàng thuận tiện hơn. | Tài sản được kết nối Internet, dễ bị tấn công hơn. Bên lưu ký có thể đóng băng tài khoản. |


Trong ví tự quản lý (còn gọi là ví không lưu ký), bạn là người duy nhất giữ khóa ví và bạn có toàn quyền kiểm soát những gì ra vào. Ngược lại, với ví lưu ký, người khác giữ khóa riêng, cho phép họ toàn quyền di chuyển bất kỳ bitcoin nào mà nhà cung cấp đó kiểm soát thay cho bạn.

* Tự quản lý giống như bạn tự làm ngân hàng cho chính mình. Các giao dịch không bị kiểm soát và giám sát
* Tự quản lý đảm bảo rằng bên thứ ba không thể tịch thu bitcoin của bạn.
* Tự quản lý mang lại sự yên tâm trong những thời điểm bất ổn, vì bạn biết bitcoin của mình được an toàn.

Việc chọn đúng loại ví phù hợp với nhu cầu của từng người là rất quan trọng. Đôi khi, mọi người khó phân biệt được mình đang cài đặt ví tự quản lý hay ví lưu ký. Bảng dưới đây cho thấy sự khác biệt trong quá trình cài đặt.


| Loại | Bước 1: Chọn | Bước 2: Cài đặt | Bước 3: Tạo | Bước 4: Bảo mật |
| --- | --- | --- | --- | --- |
| Tự quản lý | Chọn ví tự quản lý | Làm theo hướng dẫn của ví | Tạo cụm từ khôi phục | Lưu trữ cụm từ khôi phục ở nơi an toàn |
| Lưu ký | Chọn ví lưu ký | Làm theo hướng dẫn của ví | Tạo tài khoản | Không áp dụng |


“**Không giữ khóa, không giữ tiền**” là một câu nói phổ biến trong cộng đồng người nắm giữ bitcoin. Nó ám chỉ rằng nếu bạn không kiểm soát trực tiếp các khóa riêng tư liên kết với ví Bitcoin của mình, bạn không thực sự sở hữu số bitcoin đó.

Ai truy cập được khóa riêng tư của bạn thì người đó sở hữu bitcoin của bạn. Vì vậy, việc bảo vệ chúng khỏi những ánh mắt tò mò là vô cùng quan trọng! Chúng ta sẽ tìm hiểu một số cách để làm điều đó ở phần sau của cuốn sách.

Trong phần tiếp theo, chúng ta sẽ chỉ nói về ví tự quản lý, nơi người dùng sở hữu khóa và có toàn quyền kiểm soát bitcoin của mình.

Đừng lo nếu bạn thấy mọi thứ có vẻ phức tạp hoặc chưa hiểu hết — đây là một hành trình, và bạn sẽ hiểu rõ hơn khi bắt đầu sử dụng Bitcoin!

#### Các loại ví Bitcoin khác nhau

Nơi khóa riêng tư của bạn được tạo ra và lưu trữ sẽ quyết định cách chúng ta mô tả các loại ví Bitcoin. Nếu khóa nằm trên điện thoại thông minh của bạn, đó là **ví di động**. Nếu chúng được lưu trữ an toàn trên một thiết bị chuyên dụng, đó là một **ví cứng**.


| Loại | Mô tả | Ưu điểm | Nhược điểm | Người dùng ví dụ |
| --- | --- | --- | --- | --- |
| Ví trực tuyến | Truy cập thông qua trình duyệt web | Có thể truy cập từ bất kỳ thiết bị nào có kết nối internet | Kém an toàn hơn vì có thể bị hack hoặc xâm nhập | Cần truy cập ví thường xuyên và không có nhiều tiền để lưu trữ |
| Ví di động | Cài đặt trên thiết bị di động | Dễ sử dụng | Có thể bị mất nếu thiết bị bị đánh cắp hoặc bị hack | Cần thực hiện giao dịch khi di chuyển và không có nhiều tiền để lưu trữ |
| Ví máy tính | Cài đặt trên máy tính để bàn | Tiện lợi và có thể truy cập từ bất cứ đâu | Có thể bị hack nếu máy tính bị nhiễm phần mềm độc hại | Muốn lưu trữ số lượng lớn bitcoin và quen sử dụng máy tính để bàn |
| Ví cứng | Thiết bị vật lý lưu trữ bitcoin ngoại tuyến | An toàn hơn ví trực tuyến và có thể sử dụng ngoại tuyến | Tiền có thể không thể khôi phục được | Muốn lưu trữ số lượng lớn bitcoin và sẵn sàng trả thêm để tăng bảo mật |


Vì khóa có thể được chuyển từ thiết bị này sang thiết bị khác, nên “trạng thái” của ví Bitcoin của bạn không cố định. Ví dụ, nếu tôi tạo khóa ví trên máy tính và sau đó chuyển chúng sang điện thoại, thì “ví máy tính” sẽ trở thành “ví di động”.

Khi nói đến việc lưu trữ bitcoin của bạn, không chỉ là ai kiểm soát khóa — còn có nhiều rủi ro khác cần cân nhắc. Đó là lý do tại sao bạn nên tìm một giải pháp lưu trữ vừa an toàn vừa tiện lợi. Khi bạn phân tích các điểm mạnh yếu của các loại ví khác nhau, bạn sẽ nhận ra không có loại ví nào là hoàn hảo cho mọi nhu cầu.

##### Những điều cần cân nhắc khi chọn ví

* **Bảo mật**: Đảm bảo ví có các biện pháp bảo mật mạnh mẽ.
* **Quyền riêng tư**: Xem xét liệu ví có yêu cầu thông tin cá nhân hay không.
* **Dễ sử dụng**: Chọn ví dễ sử dụng và dễ thao tác.
* **Tương thích**: Đảm bảo ví tương thích với thiết bị của bạn.
* **Phí**: So sánh phí của các ví khác nhau.
* **Uy tín**: Kiểm tra uy tín của nhà phát triển để đảm bảo họ đáng tin cậy.
* **Kiểm soát**: Một số ví cho phép bạn kiểm soát nhiều hơn đối với khóa riêng tư của mình.

##### Mã nguồn mở và mã nguồn đóng

Một yếu tố quan trọng khác cần lưu ý khi chọn ví Bitcoin là biết ứng dụng hoặc phần mềm đó có phải mã nguồn mở hay không. Điều này quan trọng vì các dự án mã nguồn mở cho phép cộng đồng kiểm tra mã nguồn và tiếp tục phát triển dự án nếu nhóm phát triển dừng lại. Cũng giống như mã nguồn của Bitcoin hoàn toàn mở để mọi người kiểm tra, sử dụng và chỉnh sửa, mã nguồn của ví bạn dùng để quản lý bitcoin cũng nên như vậy.

#### Hoạt động: Thảo luận và đánh giá các loại ví Bitcoin

https://bitcoin.org/en/choose-your-wallet

Truy cập trang web sau: [https://bitcoin.org/en/choose-your-wallet](https://bitcoin.org/en/choose-your-wallet)

Hãy sử dụng kiến thức mới về ví Bitcoin của bạn để chọn ra loại ví phù hợp nhất với nhu cầu của mình dựa trên các tiêu chí mà chúng ta đã thảo luận hôm nay.
