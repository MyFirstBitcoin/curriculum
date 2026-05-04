# 6.4 Nhận và Gửi Giao Dịch

Một giao dịch Bitcoin là việc chuyển quyền sở hữu bitcoin sang một chủ sở hữu mới. Lưu ý rằng không phải các đồng tiền thực sự được chuyển đi, mà là quyền sở hữu của chúng: nói cách khác, là quyền sử dụng chúng. Mỗi khi một giao dịch được chấp nhận vào một khối, tất cả các nút trong mạng sẽ cập nhật bản sao sổ cái công khai của mình để phản ánh sự thay đổi quyền sở hữu. Ở khía cạnh này, một giao dịch Bitcoin giống với giao dịch bất động sản (hoặc tài sản khác) hơn là giao dịch tiền mặt.

Để "gửi" bitcoin, người gửi ký một thông điệp bằng khóa riêng của mình, thông báo cho mạng rằng chủ sở hữu hợp pháp của bitcoin đã chuyển quyền sở hữu sang người nhận.

Bitcoin giờ sẽ được liên kết với địa chỉ của người nhận, trao cho họ quyền sở hữu bitcoin, để chỉ chủ sở hữu mới có thể sử dụng chúng bằng khóa riêng của mình.

Các giao dịch Bitcoin mới được khởi tạo từ các ví trên khắp thế giới, nhưng không có bộ xử lý thanh toán trung tâm. Thay vào đó, các thợ đào cạnh tranh để ghi lại các giao dịch vào sổ cái.

Giả sử Nam nợ Linh 0,5 BTC và sẵn sàng trả lại cho cô ấy. Cả hai đều có ví điện tử.

1. Linh chia sẻ địa chỉ của mình với Nam.
1. Nam sử dụng phần mềm ví của mình để tạo giao dịch, bao gồm địa chỉ của Linh, số lượng cần chuyển (0,5 BTC), và một khoản phí cho thợ đào. Phí càng cao thì càng có khả năng thợ đào sẽ đưa giao dịch vào khối tiếp theo.
1. Sau khi ký giao dịch, nó được phát lên mạng, nơi các nút xác minh. Họ kiểm tra xem Nam có đủ tiền và là chủ sở hữu hợp pháp của số bitcoin muốn sử dụng hay không. Nếu không, họ sẽ từ chối giao dịch ngay lập tức.
1. Khi giao dịch được xác minh, các thợ đào sẽ quyết định có thêm giao dịch vào khối tiếp theo hay không, thường dựa trên mức phí đã chọn. Khi giao dịch được đưa vào một khối, nó sẽ được thêm vào blockchain và số tiền sẽ được chuyển đến địa chỉ của Linh.
1. Quyền sở hữu đã được chuyển cho Linh. Cô ấy giờ có thể sử dụng khóa riêng của mình để sử dụng số tiền này.

_Điều quan trọng cần lưu ý là khi giao dịch đã hoàn tất, nó không thể bị đảo ngược._


> **Note – Cách một giao dịch Bitcoin hoạt động**
>
> 1. Ai đó yêu cầu thực hiện giao dịch
> 1. Giao dịch được phát tới các máy tính ngang hàng (nút)
> 1. Thợ đào xác minh giao dịch
> 1. Các giao dịch được kết hợp để tạo thành một khối dữ liệu
> 1. Khối mới được thêm vào blockchain hiện có
> 1. Giao dịch đã hoàn tất



> **Note – Nhận giao dịch Bitcoin**
>
> Để nhận bitcoin, bạn cần cung cấp cho người gửi một địa chỉ công khai Bitcoin. Đây là một chuỗi ký tự và số duy nhất đại diện cho ví của bạn và được dùng để xác định nó trên mạng Bitcoin.
>
> Bạn có thể tìm địa chỉ công khai của mình bằng cách mở ví Bitcoin và tìm tùy chọn “Nhận” hoặc “Nạp” bitcoin.
>
> Sau đó, bạn có thể chia sẻ địa chỉ Bitcoin của mình bằng một trong các cách sau:
>
> 1. **Sao chép và dán địa chỉ**: Bạn có thể sao chép địa chỉ bằng cách bôi đen và nhấn "Sao chép", sau đó dán vào email hoặc tin nhắn.
> 1. **Chia sẻ liên kết tới ví Bitcoin của bạn**: Một số ví Bitcoin cho phép bạn tạo liên kết tới ví để chia sẻ với người gửi. Họ có thể nhấp vào liên kết để truy cập ví của bạn và gửi bitcoin.
> 1. **Chia sẻ mã QR**: Nếu người gửi có điện thoại thông minh với ứng dụng ví Bitcoin, họ có thể quét mã QR để lấy địa chỉ Bitcoin của bạn.


Khi người gửi đã có địa chỉ của bạn, họ có thể gửi bitcoin cho bạn bằng cách nhập địa chỉ và số lượng muốn gửi. Bitcoin sau đó sẽ được chuyển từ ví của họ sang ví của bạn.

Giao dịch được xác nhận bởi Mạng lưới Bitcoin và thường mất khoảng 10 phút. Để an toàn hơn, nên chờ hai lần xác nhận, mất khoảng 20 phút.


> **Note – Gửi giao dịch Bitcoin**
>
> Để gửi bitcoin, bạn cần một số thứ: một ví Bitcoin, địa chỉ công khai của người nhận và số lượng bitcoin bạn muốn gửi.
>
> 1. Mở ví Bitcoin của bạn.
> 1. Đi tới nút “Gửi” và dán địa chỉ của người nhận vào trường "Đến". Ngoài ra, bạn cũng có thể quét mã QR nếu người nhận cung cấp.
> 1. Nhập số lượng bitcoin bạn muốn gửi vào trường “Số lượng”.
> 1. Kiểm tra kỹ địa chỉ của người nhận và số lượng cần gửi. Hãy nhớ rằng các giao dịch không thể đảo ngược!
> 1. Trước khi nhấn “Xác nhận và Gửi”, chúng tôi khuyên bạn nên kiểm tra lại thông tin giao dịch một lần nữa để đảm bảo bạn đang gửi đúng số lượng bitcoin đến đúng địa chỉ.
> 1. Phát giao dịch lên mạng và chờ mạng xác nhận giao dịch.
>
> Giờ bạn đã biết cách đánh giá, lựa chọn và thiết lập một ví Bitcoin tự quản lý. Việc gửi và nhận bitcoin trên mạng Bitcoin được gọi là các giao dịch “on-chain”. Điều này là vì các giao dịch diễn ra trên mạng chính của Bitcoin và được ghi lại trên blockchain.
>
> Các giao dịch on-chain là cách an toàn nhất để giao dịch với bitcoin nhờ sự xác minh phi tập trung của mạng lưới.
>
> Tuy nhiên, các giao dịch on-chain chậm hơn và có thể đắt hơn đáng kể so với các lựa chọn khác (chúng ta sẽ thảo luận ở Phần 7) do phí thợ đào.


#### Hoạt động: Giao dịch thực tế

https://qr.myfirstbitcoin.org/transactions.pdf

**Đây là một bài tập hợp tác đơn giản hóa các vai trò cơ bản của những người tham gia vào một giao dịch Bitcoin.**

###### Những điểm chính

1. Có bốn loại người tham gia trong mỗi giao dịch bitcoin: người gửi, người nhận, thợ đào và người vận hành nút.
1. Người gửi phải phê duyệt (ký mã hóa) **số lượng bitcoin** cần gửi VÀ **địa chỉ cụ thể** để gửi tới.
1. Người nhận phải cung cấp **địa chỉ hợp lệ** cho người gửi VÀ xác nhận giao dịch đã được xác nhận thành công trên blockchain.
1. Thợ đào đảm bảo tất cả các tiêu chí đều hợp lệ trước khi thêm giao dịch vào các khối tiếp theo.
1. Người vận hành node xác minh các khối đã đào là hợp lệ trước khi cập nhật phiên bản blockchain (sổ cái) của họ.

###### Mẹo cho học viên

Luân phiên qua cả bốn vai trò để trải nghiệm công việc của từng người tham gia.
