# 8.1 Bảo mật thông qua Mật mã học

> Điều mà Bitcoin mang lại cho chúng ta là một cam kết chắc chắn: chương trình sẽ thực thi chính xác như đã được chỉ định.  
_Andreas M. Antonopoulos_

#### Mật mã khóa công khai/khóa riêng


> **Definition – Định nghĩa về Mật mã học**
>
> **Mật mã học** là việc biến thông tin thành một bí mật mà chỉ những người phù hợp mới có thể đọc được.


* **Mã hóa** là quá trình biến thông tin thành dạng mã hóa để chỉ người có khóa đúng mới có thể đọc được.
* **Giải mã** là quá trình biến thông tin đã mã hóa trở lại thành dạng có thể đọc được.

Trong mật mã học truyền thống, hai người muốn liên lạc riêng tư phải chia sẻ trước cùng một khóa bí mật, tương tự như một mật khẩu chung. Một người sử dụng khóa này để mã hóa tin nhắn trước khi gửi đi, và người kia sử dụng cùng khóa đó để giải mã và đọc tin nhắn.

Vấn đề với hệ thống này là cả hai người phải chia sẻ trước khóa bí mật. Nếu ai đó khác có được khóa này, họ có thể đọc bất kỳ tin nhắn nào bị chặn lại.

Bitcoin giải quyết vấn đề này bằng một phương pháp khác gọi là mật mã khóa công khai, nơi người dùng không cần phải chia sẻ khóa bí mật trước.

Mật mã khóa công khai/khóa riêng giải quyết vấn đề chia sẻ bí mật. Thay vì chia sẻ mật khẩu, mỗi người có hai khóa: một khóa công khai và một khóa riêng.

* **khóa công khai** có thể chia sẻ với bất kỳ ai.
* **khóa riêng** phải luôn được giữ bí mật.

Nếu Minh muốn gửi gì đó cho An, Minh có thể sử dụng khóa công khai của An. Chỉ An mới có thể mở khóa bằng khóa riêng của mình. Ngay cả khi ai đó chặn được tin nhắn, họ cũng không thể đọc hoặc sử dụng nó nếu không có khóa riêng.

Trong Bitcoin, hệ thống này được sử dụng để tạo chữ ký số. Chữ ký số chứng minh rằng chủ sở hữu của khóa riêng đã phê duyệt giao dịch, tương tự như việc ký tên vào một tài liệu. Đây là điều giúp các giao dịch Bitcoin trở nên an toàn và có thể xác minh mà không cần tin tưởng bên thứ ba.

Giao dịch Bitcoin liên quan đến việc chuyển quyền sở hữu bitcoin từ một địa chỉ sang một địa chỉ khác.

Mã hóa được sử dụng để đảm bảo rằng chỉ người thực sự sở hữu bitcoin mới có quyền gửi tiền của mình cho người khác. Nó đảm bảo tài sản của họ được bảo vệ khỏi những kẻ xấu.

Như một biện pháp bảo vệ bổ sung, mỗi giao dịch Bitcoin tự động nhận được một chữ ký số DUY NHẤT. Chữ ký số duy nhất này được hỗ trợ bởi công nghệ chống giả mạo giúp mạng lưới xác minh rằng chủ sở hữu thực sự của bitcoin, chứ không phải ai khác, đã gửi chúng.


> **Dark**
>
> Mỗi người dùng có hai khóa: một **khóa riêng**, được **giữ bí mật**, và một **khóa công khai** có thể được **chia sẻ với người khác**. **Khóa riêng** đóng vai trò như một hình thức nhận dạng và bằng chứng sở hữu, xác nhận: “Địa chỉ này thuộc về tôi và tôi kiểm soát nó.”


###### Cách một giao dịch Bitcoin hoạt động

1. **Tạo giao dịch**: Người dùng bắt đầu một giao dịch Bitcoin bằng cách nhập các thông tin như địa chỉ người nhận và số lượng bitcoin muốn gửi.
1. **Tạo chữ ký số**: Người gửi tạo ra một **chữ ký số** duy nhất bằng **khóa riêng** của mình. Chữ ký này là một mã duy nhất xác minh tính xác thực của giao dịch.
1. **Phát sóng giao dịch**: Giao dịch đã được ký sẽ được phát lên mạng lưới Bitcoin, thể hiện ý định chuyển quyền sở hữu bitcoin từ người gửi sang người nhận.
1. **Xác minh trên mạng lưới**: Các nút trên mạng lưới Bitcoin nhận giao dịch và sử dụng **khóa công khai** để xác minh tính xác thực của chữ ký. của giao dịch. Đồng thời, họ sử dụng **khóa công khai** để xác minh **chữ ký số**.
1. **Xác nhận trên mạng lưới Bitcoin**: Nếu việc xác minh thành công, giao dịch sẽ được thêm vào sổ cái, đóng vai trò là bản ghi an toàn, minh bạch của tất cả các giao dịch. Khi đã được xác nhận, quyền sở hữu bitcoin sẽ chính thức được chuyển từ người gửi sang người nhận.


> **Callout – Tóm tắt**
>
> **chữ ký số**, được tạo bằng **khóa riêng** của người gửi, chứng minh rằng giao dịch đã được chủ sở hữu bitcoin cho phép. Mạng lưới Bitcoin sau đó có thể xác minh bằng chứng này và ghi lại giao dịch.


#### Giải thích về Hàm băm

Xin đừng cảm thấy sợ hãi bởi các thuật ngữ kỹ thuật và khái niệm toán học phía trước. Chúng tôi hiểu rằng không phải ai cũng yêu thích toán học, nhưng bạn có thể sẽ ngạc nhiên khi thấy rằng ngay cả những ý tưởng phức tạp nhất cũng có thể nắm bắt được nếu bạn cố gắng một chút.


> **Definition – Định nghĩa về hàm số**
>
> Một **hàm số** giống như một chiếc máy nhận thông tin và biến nó thành một thứ mới. Thông tin bạn đưa vào hàm gọi là **đầu vào**. Thông tin mới mà hàm tạo ra gọi là **đầu ra**. Hàm số giúp máy tính thực hiện các nhiệm vụ và giải quyết vấn đề.


##### Hàm số là gì?

Hàm số là một tập hợp các hướng dẫn nhận đầu vào và tạo ra đầu ra. Bạn có thể hình dung nó như một công thức nấu ăn: bạn làm theo các bước với những nguyên liệu nhất định, và bạn luôn nhận được kết quả dự đoán được.

Trong Bitcoin, các hàm số được sử dụng để xử lý và xác minh giao dịch. Khi ai đó gửi bitcoin, các hàm mật mã giúp kiểm tra tính hợp lệ của giao dịch, xác nhận người gửi có đủ tiền và cập nhật số dư trên sổ cái Bitcoin. Khi đã được xác minh và thêm vào một khối, giao dịch sẽ trở thành một phần của bản ghi vĩnh viễn trên blockchain.

##### Hàm một chiều là gì?

Hàm một chiều là một loại hàm đặc biệt rất dễ tính toán theo một chiều nhưng cực kỳ khó đảo ngược. Ví dụ, xay các nguyên liệu thành sinh tố thì dễ, nhưng bạn không thể tách sinh tố trở lại thành các nguyên liệu ban đầu.

Bảo mật của Bitcoin dựa vào các hàm một chiều. Chúng được sử dụng trong mật mã khóa công khai và khóa riêng, cho phép mọi người chia sẻ khóa công khai mà vẫn giữ bí mật khóa riêng. Dù khóa công khai có thể nhìn thấy, không thể suy ra khóa riêng từ đó. Đây chính là điều làm cho các giao dịch Bitcoin an toàn.

##### Hàm băm là gì?

Một **hàm băm** giống như một chiếc máy mã hóa bí mật. Nó nhận một thông điệp và biến nó thành một mã.

###### Cách hoạt động của Hàm băm trong giao dịch Bitcoin

Trong Bitcoin, mỗi giao dịch đều được chuyển thành một hàm băm trước khi được thêm vào blockchain. Hàm băm là một dấu vân tay số duy nhất của giao dịch. Nếu ai đó cố thay đổi dù chỉ một phần nhỏ của giao dịch, hàm băm sẽ thay đổi hoàn toàn. Điều này giúp mạng lưới dễ dàng phát hiện sự can thiệp.

###### Vai trò của Hàm băm trong bảo mật Bitcoin

Hàm băm giúp bảo vệ mạng lưới Bitcoin bằng cách làm cho các giao dịch dễ xác minh và không thể bị thay đổi một cách lặng lẽ. Vì mỗi giao dịch có một hàm băm riêng biệt, mạng lưới có thể nhanh chóng phát hiện nếu có điều gì đó bị thay đổi.

Một hàm băm nhận dữ liệu và chuyển nó thành một chuỗi ký tự và số cố định gọi là hàm băm. Cùng một đầu vào sẽ luôn tạo ra cùng một hàm băm, nhưng chỉ cần thay đổi nhỏ ở đầu vào sẽ tạo ra kết quả hoàn toàn khác. Tính chất này cho phép máy tính kiểm tra dữ liệu có bị thay đổi hay không.


> **Definition – Định nghĩa về Hàm băm**
>
> **Hàm băm** giống như tạo dấu vân tay cho dữ liệu số. Đó là quá trình lấy một thông điệp số và biến nó thành một mã có độ dài cố định, đóng vai trò là định danh duy nhất. Cũng như dấu vân tay nhận diện một người, hàm băm nhận diện một thông điệp số.


**đầu ra**, hay hàm băm, luôn có cùng độ dài, bất kể thông tin gốc dài bao nhiêu. Bitcoin sử dụng một số loại hàm băm cụ thể gọi là **SHA-256** và **RIPEMD160**.

Một vài ví dụ dưới đây:

* Hàm băm SHA256 của chuỗi **xin chào thế giới**
  * `b94d27b9934d3e08a52e52d7da7dabfac484efe37a5380ee9088f7ace2efcde9`
* Băm SHA256 của chuỗi **xin chào thế giới.**
  * `7ddb227315f423250fc67f3be69c544628dffe41752af91c50ae0a9c49faeb87`
  * Hãy chú ý rằng chỉ một thay đổi nhỏ trong đầu vào cũng làm thay đổi hoàn toàn đầu ra so với lần đầu tiên
* Băm SHA256 của tệp iso có thể tải về **Ubuntu 18.10**
  * `7b9f670c749f797a0f7481d619ce8807edac052c97e1a0df3b130c95efae4765`
  * Đầu vào này là một tệp rất lớn nhưng đầu ra vẫn có độ dài cố định như nhau

Bạn cũng có thể hình dung việc băm giống như một bản nhạc ghi lại tinh thần của một bản nhạc. Cũng như bản nhạc là đại diện duy nhất cho một giai điệu, giá trị băm là đại diện duy nhất cho một dữ liệu.

Bằng cách so sánh bản nhạc với màn trình diễn thực tế, một nhạc sĩ có thể xác định xem màn trình diễn có chính xác không. Tương tự, bằng cách so sánh giá trị băm của dữ liệu nhận được với giá trị băm gốc, bạn có thể xác định xem dữ liệu có bị thay đổi trong quá trình truyền không.

Cũng như chỉ một sai lệch nhỏ trong màn trình diễn âm nhạc có thể làm nó nghe khác đi, chỉ một thay đổi nhỏ nhất đối với dữ liệu gốc cũng sẽ tạo ra một giá trị băm khác. Điều này làm cho việc băm trở thành một công cụ mạnh mẽ để đảm bảo tính toàn vẹn và xác thực của giao dịch Bitcoin.

Quá trình mã hóa **khóa công khai** thông qua việc băm được sử dụng để tăng cường bảo mật thông tin bằng cách chuyển đổi nó thành một định dạng cố định, không thể đọc được. Bitcoin sử dụng các thuật toán SHA-256 và RIPEMD160 để tạo ra địa chỉ công khai. Kết quả đầu ra là một định danh duy nhất cho **khóa công khai** và giúp đảm bảo tính toàn vẹn cũng như bảo mật cho các giao dịch được lưu trữ trên sổ cái. Bằng cách mã hóa thông tin như vậy, sẽ khó hơn cho những người không được phép truy cập và thay đổi dữ liệu.

##### Các tính chất của hàm băm

* **Tính xác định**: Cùng một nguyên liệu luôn tạo ra cùng một ly sinh tố. Tương tự, cùng một dữ liệu sẽ luôn tạo ra cùng một giá trị băm.
* **Kháng ảnh ngược**: Nếu bạn chỉ có ly sinh tố, bạn không thể biết chính xác các loại trái cây đã được dùng. Tương tự, nếu bạn chỉ có giá trị băm, bạn không thể xác định được dữ liệu gốc.
* **Hiệu ứng lở tuyết**: Chỉ cần thay đổi một phần nhỏ của nguyên liệu cũng tạo ra một ly sinh tố hoàn toàn khác. Trong băm, một thay đổi rất nhỏ trong dữ liệu sẽ tạo ra một giá trị băm hoàn toàn khác.
* **Kháng va chạm**: Rất khó để tìm hai bộ nguyên liệu khác nhau mà lại tạo ra đúng cùng một ly sinh tố. Tương tự, rất khó xảy ra trường hợp hai dữ liệu khác nhau lại tạo ra cùng một giá trị băm.
* **Dễ kiểm tra nhanh**: Làm sinh tố rất nhanh, và dễ dàng kiểm tra kết quả là một ly sinh tố. Hàm băm tính toán nhanh và ai cũng có thể kiểm tra dễ dàng.

#### Hoạt động: Tạo giá trị băm SHA 256


https://tools.keycdn.com/sha256-online-generator

_SHA256 Online Generator_


Bạn tò mò về cách hoạt động của hàm băm? Hãy quét mã QR để tạo ngay giá trị băm SHA256 từ bất kỳ từ, câu hoặc dữ liệu nào bạn chọn. Hàm băm giống như dấu vân tay kỹ thuật số: chúng chỉ đi một chiều, nghĩa là một khi đã băm thì không thể đảo ngược lại. Hãy thử và tự mình trải nghiệm nhé!
