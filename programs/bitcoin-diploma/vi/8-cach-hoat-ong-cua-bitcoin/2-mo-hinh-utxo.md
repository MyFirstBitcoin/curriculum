# 8.2 Mô hình UTXO

##### UTXO là gì?

Đừng để bị choáng ngợp bởi cái tên lạ lẫm này. Bạn có thể hình dung UTXO như những mảnh bitcoin, tương tự như các tờ tiền và đồng xu trong ví của bạn. Ví dụ, nếu bạn trả cho một món hàng trị giá 150.000₫ bằng một tờ 250.000₫, bạn sẽ nhận lại 100.000₫ tiền thừa. Bitcoin hoạt động theo cách tương tự.

Tất cả số bitcoin bạn sở hữu đều được tạo thành từ các UTXO khác nhau. Khi bạn gửi bitcoin, ví của bạn sẽ sử dụng một hoặc nhiều mảnh này để thực hiện thanh toán.

Nếu mảnh bạn sử dụng lớn hơn số tiền bạn gửi, giá trị còn lại sẽ được trả lại cho bạn dưới dạng tiền thừa, tạo thành một UTXO mới. Đồng thời, người nhận sẽ nhận được một UTXO mới đại diện cho số bitcoin bạn đã gửi.

Số dư ví của bạn đơn giản là tổng giá trị của tất cả các UTXO bạn kiểm soát.


> **Callout – Quyền riêng tư**
>
> Bạn không nên để người khác biết về các UTXO của mình vì khi ai đó biết, họ có thể theo dõi các giao dịch của bạn và cuối cùng sẽ biết bạn sở hữu bao nhiêu tiền.


###### Ví dụ

1. Lan muốn gửi cho Bình 5 BTC.
1. Ví của cô ấy sử dụng hai UTXO mà tổng cộng trị giá 6 BTC.
1. Giao dịch gửi **5 BTC cho Bình**, tạo ra một UTXO mới trong ví của Bình.
1. Số còn lại **0,99 BTC trả lại cho Lan như tiền thừa**, sau khi trả **phí giao dịch 0,01 BTC**.
1. Khi giao dịch được xác nhận, nó sẽ được thêm vào sổ cái của Bitcoin và các UTXO mà Lan đã sử dụng sẽ được đánh dấu là đã chi tiêu, nên không thể sử dụng lại.

###### Tài nguyên tham khảo


[▶ YouTube](https://www.youtube.com/watch?v=Lx9zgZCMqXE)
