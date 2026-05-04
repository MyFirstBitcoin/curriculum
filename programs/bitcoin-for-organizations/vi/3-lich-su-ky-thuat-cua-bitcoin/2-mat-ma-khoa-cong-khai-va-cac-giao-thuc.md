# 3.2 Mật mã khóa công khai và các giao thức

Ngày nay, Internet và hầu hết các hệ thống máy tính hiện đại đều dựa vào mật mã học, một phương pháp làm mờ thông tin để chỉ người nhận thông tin mới có thể giải mã được. Nền tảng của mật mã học dùng để bảo vệ Bitcoin có thể được truy ngược về những năm 70.

Vấn đề đầu tiên cần giải quyết là – làm thế nào để gửi một bí mật chung qua một môi trường không an toàn.

Điều này lần đầu tiên được nghiên cứu bởi Whitfield Diffie và Martin Hellman.

Vấn đề đặt ra: hai bên – thường được gọi là An và Bình – muốn chia sẻ thông tin bí mật qua một mạng mà người khác có thể nghe lén. Để đạt được điều này, họ đã tạo ra quy trình trao đổi khóa Diffie-Hellman.

Bí mật chung này sau đó có thể được sử dụng làm giá trị hạt giống để tạo ra nhiều khóa đối xứng nhằm mã hóa và giải mã các tin nhắn gửi cho nhau mà không cần chia sẻ khóa công khai.

Vì khóa riêng tư không bao giờ phải chia sẻ, và các khóa khác nhau được sử dụng ở mỗi đầu để mã hóa và giải mã, nên đây được gọi là thuật toán mã hóa bất đối xứng.

Các trường hợp sử dụng:

* An ký một tin nhắn bằng khóa công khai của Bình – người duy nhất có thể giải mã nó bằng khóa riêng tư của mình
* An ký một tin nhắn bằng khóa riêng tư của mình – bằng cách giải mã với khóa công khai của An, bất kỳ ai cũng có thể xác minh rằng tin nhắn được gửi bởi An, mà không cần biết khóa riêng tư của cô ấy
* Kết hợp hai phương pháp này với hai lớp mã hóa, một tin nhắn có thể được gửi mã hóa để chỉ Bình có thể giải mã, và anh ấy có thể xác minh người gửi thực sự là An

Mặc dù không được ghi nhận trên bài báo, Ralph Merkle đã đóng vai trò quan trọng trong việc giúp giải quyết điều mà trước đó được coi là câu đố không thể giải – làm thế nào để thiết lập hoặc tái thiết lập liên lạc riêng tư qua một mạng mở và có thể thù địch.

Phương pháp này tự nó dễ bị tấn công brute force, khi kẻ tấn công có thể lấy các số đã chia sẻ và cuối cùng tạo lại khóa chung nếu có đủ thời gian và tài nguyên, vì vậy nó không phải là câu trả lời hoàn chỉnh nếu chỉ dùng riêng lẻ.

##### Các giao thức cho hệ mật mã khóa công khai

Bên cạnh việc đóng góp vào hệ thống khóa công khai Diffie-Hellman được mô tả ở trên, **Ralph Merkle** tiếp tục đóng góp cho lĩnh vực này trong nhiều năm, và đã đóng vai trò quan trọng trong việc phát triển một số thành phần then chốt được sử dụng bởi Bitcoin.

Hàm băm mật mã là một thuật toán toán học nhận đầu vào với kích thước bất kỳ và xử lý các phép tính phức tạp để trả về một giá trị băm dưới dạng bit, thường được biểu diễn bằng một chuỗi ký tự chữ và số có độ dài cố định sử dụng định dạng thập lục phân.

* Đầu vào có thể có kích thước bất kỳ
* Đầu ra luôn có độ dài cố định và xác định (cùng một đầu vào sẽ tạo ra cùng một giá trị băm mỗi lần)
* Việc xác minh rất dễ dàng nhưng cực kỳ khó để đảo ngược quá trình nhằm xác định đầu vào
* Chỉ cần thay đổi nhỏ dữ liệu cũng hoàn toàn thay đổi đầu ra

![Hash function](https://cdn.sanity.io/images/vje9ehw2/staging/8c3cd5c137d97a023c9230f087b8f2922889cbe0-515x331.svg)

Băm là một phần không thể thiếu của giao thức Bitcoin. SHA-256, được sử dụng trong Bitcoin, do NSA tạo ra và là một ví dụ về thuật toán băm mật mã.

* Mỗi khối trong chuỗi đều được băm để dữ liệu không thể bị thay đổi – đảm bảo tính toàn vẹn của sổ cái phân tán
* Giá trị băm được tạo ra cần đáp ứng tiêu chí ‘Bằng chứng công việc’ để được coi là một khối hợp lệ
* Cây Merkle – bằng cách sử dụng các nhánh và băm của các giá trị băm, cây băm có thể cho phép xác minh các tập dữ liệu lớn với dung lượng lưu trữ tối thiểu
* Chữ ký và khóa dựa trên băm có thể được sử dụng cho ví, địa chỉ và xác thực giao dịch

Việc xác minh phân tán trạng thái blockchain và mô hình sổ cái chỉ ghi bổ sung, chống sửa đổi được thực hiện nhờ vào hàm băm một chiều. Các hàm băm cung cấp phương pháp xác minh sự kiện trên sổ cái công khai như Bitcoin một cách đáng tin cậy, xác định mà không cần mô hình tin cậy tập trung.

Những khả năng mới trong lĩnh vực mật mã học này được các nhà sáng tạo kỳ vọng sẽ mở ra một làn sóng đổi mới mới trong lĩnh vực này.

##### Mật mã đường cong elliptic

Một trong những đổi mới sau này xuất hiện dưới dạng mật mã đường cong elliptic.

Mật mã đường cong elliptic được giới thiệu vào năm 1985 bởi hai nhà khoa học, N. Koblitz và V. Miller. Họ đề xuất ý tưởng sử dụng các điểm được xác định bởi đường cong elliptic thay vì các trường số nguyên tố hữu hạn sao cho giả định bài toán Logarit rời rạc vẫn đúng, như thường được sử dụng trong giao thức trao đổi khóa Diffie-Hellman tiêu chuẩn. Chi tiết về cách hoạt động của nó vượt ra ngoài phạm vi của phần này, nhưng ở mức độ tổng quan, một đường cong elliptic là tập hợp các điểm thỏa mãn một phương trình toán học cụ thể.

Phương trình cho một đường cong elliptic trông như sau:

![Elliptic curve](https://cdn.sanity.io/images/vje9ehw2/staging/a30483f84b1a10c35de9854c9a6fad78fd0cb9b0-451x285.webp)

Điều này có một số tính chất hữu ích:

* Đối xứng theo chiều ngang. Bất kỳ điểm nào trên đường cong đều có thể phản chiếu qua trục x và vẫn nằm trên cùng một đường cong.
* bất kỳ đường thẳng nào không thẳng đứng sẽ cắt đường cong tại tối đa ba điểm.
* Kích thước khóa nhỏ gọn là điều cần thiết để lưu trữ và truyền tải khóa công khai hiệu quả trên blockchain.

Những tính chất này có thể được sử dụng để tạo cặp khóa theo cách tương tự như thuật toán Diffie-Hellman. Bitcoin sử dụng ECDSA, viết tắt của Elliptic Curve Digital Signature Algorithm. Đây là một quy trình sử dụng đường cong elliptic và trường hữu hạn để “ký” dữ liệu theo cách mà bên thứ ba có thể xác minh tính xác thực của chữ ký trong khi người ký vẫn giữ quyền duy nhất tạo ra chữ ký đó. Với bitcoin, dữ liệu được ký là giao dịch chuyển quyền sở hữu.

Phần 'hữu hạn' tương tự như cách dùng 'mod' trong Diffie-Hellman, nơi đầu ra của phương trình được chia lấy phần dư để đảm bảo nó nằm trong một phạm vi số nhất định.
