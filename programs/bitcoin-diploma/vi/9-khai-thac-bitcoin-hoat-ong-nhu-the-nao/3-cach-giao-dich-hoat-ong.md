# 9.3 Cách Giao Dịch Hoạt Động

Bây giờ bạn đã hiểu về khóa công khai và khóa riêng, cũng như vai trò của các node và thợ đào, sau đây là cách một giao dịch Bitcoin diễn ra từ đầu đến cuối.

1. An muốn gửi bitcoin cho Hùng. Anh ấy tạo một giao dịch với địa chỉ của Hùng, số lượng muốn gửi và một khoản phí.
1. An ký giao dịch bằng khóa riêng của mình để chứng minh quyền sở hữu.
1. Anh ấy phát giao dịch lên mạng lưới Bitcoin.
1. Các node nhận được giao dịch và kiểm tra xem nó có tuân thủ các quy tắc không, bao gồm xác minh chữ ký và kiểm tra xem An có đủ bitcoin không.
1. Nếu hợp lệ, giao dịch sẽ được chia sẻ trên toàn mạng và thêm vào mempool, nơi các giao dịch chờ xử lý.
1. Các thợ đào chọn giao dịch từ mempool và đưa vào một khối mà họ cố gắng đào.
1. Khi một thợ đào đào thành công một khối, khối đó sẽ được chia sẻ với mạng lưới và các node khác kiểm tra.
1. Nếu hợp lệ, khối sẽ được thêm vào blockchain. Hùng nhận được bitcoin.
1. Khi có thêm nhiều khối được thêm vào, giao dịch sẽ có thêm xác nhận, làm cho nó an toàn hơn.

Khi đã được đưa vào một khối, giao dịch được xác nhận. An không thể tiêu số bitcoin đó nữa, và Hùng có thể sử dụng số bitcoin nhận được trong một giao dịch mới.


> **Light**
>
> Chọn giao dịch & phí → Ví ký và gửi → Các node phân phối → Thợ đào thêm giao dịch vào mẫu khối → Thợ đào thắng cuộc thi Bằng chứng Công việc → Khối mới được xác thực → Khối mới được các node phân phối


###### Tài nguyên


[▶ Xem video này về các Node Bitcoin](https://www.youtube.com/watch?v=xc_TxlByxeY)
