# 7.4 Gửi và Nhận Giao Dịch Lightning

Với ví Lightning, việc sử dụng Bitcoin trở nên nhanh chóng, rẻ và riêng tư, giúp giao dịch giữa hai người trở nên dễ dàng. Bạn có thể gửi và nhận bitcoin một cách nhanh chóng cho các hoạt động hàng ngày như mua cà phê.

Hãy cùng xem một vài ví dụ về Lightning Network trong thực tế.

###### Ví dụ 1

Cả Minh và Lan đều có 5 đơn vị tiền. Minh muốn gửi 2 đơn vị cho Lan. Khoản thanh toán này đi qua Nam, người giúp chuyển tiếp khoản thanh toán trên Lightning Network. Sau khi thanh toán hoàn tất, Lan có 7 đơn vị và Minh còn 3.

Nam giúp định tuyến khoản thanh toán, nhưng anh ấy không thể lấy cắp tiền. Lightning Network sử dụng mật mã để đảm bảo chỉ người nhận dự định mới có thể nhận được khoản thanh toán. Nam chỉ đơn giản là giúp khoản thanh toán di chuyển qua mạng lưới.

Điều này cho thấy một lợi thế quan trọng của Lightning Network: mọi người có thể gửi tiền nhanh chóng mà không cần phải tin tưởng vào các bên trung gian như ngân hàng.

Những người vận hành node như Nam cũng có thể kiếm được một khoản phí nhỏ khi giúp định tuyến các khoản thanh toán. Bằng cách này, họ giúp mạng lưới duy trì tính phi tập trung và hiệu quả.

So với các giao dịch Bitcoin thông thường:

* **Giao dịch trên chuỗi** diễn ra trực tiếp trên blockchain của Bitcoin. Chúng rất an toàn nhưng có thể chậm hơn và tốn kém hơn.
* **Giao dịch Lightning** diễn ra ngoài chuỗi và cho phép các khoản thanh toán di chuyển nhanh hơn nhiều với chi phí thấp hơn nhiều.

Vì lý do này, Lightning rất hữu ích cho các khoản thanh toán nhỏ, hàng ngày, trong khi các giao dịch trên chuỗi thường được sử dụng cho các khoản chuyển lớn hoặc lưu trữ dài hạn.

###### Ví dụ 2

Mai thích ăn ngoài và thường ghé quán cà phê yêu thích gần nhà. Với rất nhiều lựa chọn thanh toán khác nhau, cô ấy không chắc đâu là lựa chọn tốt nhất. May mắn thay, Mai đã biết một chút về Bitcoin và Lightning Network. Sau khi xem xét các lựa chọn, Mai nhận ra rằng sử dụng phương thức thanh toán Lightning là lựa chọn tốt nhất.

Mai muốn mua một ly cà phê, nhưng thanh toán bằng giao dịch Bitcoin thông thường đôi khi có thể mất thời gian và phí cao hơn. Thay vào đó, cô quyết định sử dụng Lightning Network.

Lightning Network cho phép mọi người gửi bitcoin ngay lập tức với phí rất thấp. Điều này khiến nó trở nên lý tưởng cho các khoản mua sắm nhỏ, hàng ngày như cà phê.

Để bắt đầu sử dụng Lightning, Mai tải một ví Lightning về điện thoại. Sau đó, cô ấy chuyển một ít bitcoin từ ví Bitcoin thông thường sang ví Lightning của mình. Bước này sử dụng một giao dịch Bitcoin bình thường trên blockchain. Khi tiền đã ở trong ví Lightning, chúng có thể được sử dụng trên Lightning Network.

Bây giờ Mai có thể thanh toán cho quán cà phê ngay lập tức bằng Lightning. Khoản thanh toán diễn ra ngoài blockchain chính của Bitcoin, đó là lý do tại sao nó nhanh hơn và rẻ hơn nhiều so với giao dịch trên chuỗi thông thường.


| Lợi ích | Lightning Network | Hệ thống ngân hàng truyền thống |
| --- | --- | --- |
| Tốc độ | Nhanh | Chậm |
| Minh bạch | Minh bạch | Không minh bạch |
| Bảo mật | An toàn | Dễ bị tấn công |
| Phí giao dịch | Thấp | Cao |
| Tiếp cận tài chính | Cao | Hạn chế |
| Khả năng mở rộng | Cao | Thấp |
| Riêng tư | Cao | Trung bình |
| Khả năng tương tác | Cao | Thấp |
| Tuân thủ pháp lý | Trung bình | Cao |
| Hiệu quả chi phí | Cao | Trung bình |


Giao dịch on-chain diễn ra trực tiếp trên blockchain của Bitcoin và có thể mất nhiều thời gian cũng như phí hơn. Giao dịch Lightning diễn ra ngoài chuỗi, cho phép thanh toán nhanh và chi phí thấp trong khi vẫn sử dụng bitcoin.


| Visa, Inc. | Bitcoin On-chain | Lightning Network |
| --- | --- | --- |
| Công suất 65.000 giao dịch mỗi giây. | Công suất 7 giao dịch mỗi giây. | Công suất hàng triệu giao dịch mỗi giây. |


![Lightning Network Map](https://cdn.sanity.io/images/vje9ehw2/staging/5a760247cf4c32074c62f40aea8dc21095882740-504x245.svg)


https://mempool.space/graphs/lightning/nodes-channels-map

_Mempool.space Nodes Channels Map_


Đây là bản đồ của toàn bộ Lightning Network. Nhờ hàng ngàn người vận hành node Lightning, bạn có thể gửi sats cho bất kỳ ai có ví Bitcoin Lightning, dù họ ở đâu trên thế giới. Thanh toán sẽ đến trong vài giây và chỉ tốn vài nghìn đồng.**Tự mình kiểm tra nhé!**

#### Hoạt động: Cuộc đua tiếp sức Lightning


https://qr.myfirstbitcoin.org/lightning.pdf

_Activity: Lightning_


**Đây là một bài tập thực hành, nơi học viên gửi và nhận sats thật bằng Lightning Network.**

###### Điểm chính

1. Việc sử dụng ví Lightning sẽ giúp bạn tự tin hơn khi nhận và gửi sats thật.
1. Chú ý đến đơn vị. Một số ví cho phép người dùng gửi bitcoin HOẶC sats (1/100.000.000 của một bitcoin).
1. Thanh toán Lightning đôi khi có thể bị kẹt trong quá trình định tuyến, đặc biệt với các khoản thanh toán lớn. Tuy vẫn có thể xảy ra, nhưng trải nghiệm này ngày càng ít gặp hơn khi mạng lưới phát triển.

###### Mẹo cho học viên

Hãy xác nhận với giảng viên của bạn xem phí giao dịch Bitcoin on-chain hiện tại sẽ ảnh hưởng như thế nào đến ví Lightning mà bạn sử dụng.
