# 7.1 Mạng Lightning

Lightning Network là một hệ thống thanh toán cho phép người dùng gửi và nhận bitcoin một cách nhanh chóng và tiết kiệm chi phí. Nó hoạt động bằng cách thiết lập một ví chung, nơi cả hai bên cùng lưu trữ một phần bitcoin của mình. Sau đó, họ có thể thực hiện vô số giao dịch với nhau mà không cần ghi lại từng giao dịch lên blockchain chính. Bằng cách này, họ bỏ qua việc phải xác minh và ghi nhận từng giao dịch vào một khối, giúp quá trình trở nên nhanh chóng và tiết kiệm chi phí. Phí giao dịch thấp hơn đồng nghĩa Lightning Network có thể được sử dụng cho các khoản thanh toán nhỏ mà trên chuỗi chính không phải lúc nào cũng khả thi. Khi hai bên quyết định kết thúc hợp tác, chỉ số dư cuối cùng mới được ghi lại trên blockchain.

Hãy tưởng tượng một ngày làm việc tại quán cà phê. Bạn dự định ngồi lâu nên mở một hóa đơn và trả trước thay vì thanh toán từng lần gọi món. Cuối ngày, bạn và chủ quán cùng kiểm tra hóa đơn để thanh toán. Nếu số tiền bạn đặt cọc lớn hơn số bạn đã tiêu, bạn sẽ nhận lại phần chênh lệch; nếu bạn tiêu nhiều hơn, bạn sẽ trả thêm phần còn thiếu.

Cách làm này có thể mở rộng cho nhiều người tham gia hơn. Ví dụ, trong một lần đến quán cà phê, bạn dẫn theo một người bạn mà nhân viên pha chế không quen và không thể mở hóa đơn cho họ. Bạn đề nghị cho bạn mình sử dụng hóa đơn đã mở của bạn để thanh toán, và hai bạn sẽ tự thỏa thuận trả lại sau. Hãy tưởng tượng hàng ngàn người cùng làm như vậy cùng lúc, cho phép người khác sử dụng hóa đơn có sẵn để kết nối với nhiều người hơn nữa — đó chính là cách Lightning Network hoạt động!

Với Lightning, bạn có thể thanh toán cho bất kỳ ai trên mạng lưới, không chỉ người mà bạn trực tiếp mở hóa đơn chung — miễn là có thể tìm được một tuyến đường giữa hai bên. Thanh toán của bạn có thể đi qua mạng lưới cho đến khi đến được người nhận, ngay cả khi bạn không có kênh mở trực tiếp với họ.

Hãy cùng xem sự khác biệt giữa giao dịch trên chuỗi và ngoài chuỗi.

##### Giao Dịch Trên Chuỗi

Đây là các giao dịch diễn ra trực tiếp trên blockchain của Bitcoin. Chúng mất khoảng 10 phút để xác nhận, và phí giao dịch phụ thuộc vào kích thước giao dịch tính theo byte ảo. Chúng an toàn hơn nhưng chậm hơn, vì cần sự đồng thuận của toàn mạng lưới.

##### Giao Dịch Lightning Network

Các giao dịch này diễn ra trên một mạng lưới riêng biệt được xây dựng trên blockchain của Bitcoin. Chúng được xử lý nhanh hơn và với phí thấp hơn. Thường được sử dụng khi tốc độ và chi phí giao dịch là yếu tố quan trọng. So với giao dịch trên chuỗi, chúng kém an toàn hơn.


|  | Mạng lưới Bitcoin | Lightning Network |
| --- | --- | --- |
| Định nghĩa | Một mạng lưới kỹ thuật số phi tập trung sử dụng mật mã để bảo vệ các giao dịch tài chính. | Một giao thức thanh toán lớp thứ hai hoạt động trên blockchain của Bitcoin, cho phép giao dịch nhanh hơn và rẻ hơn. |
| Ưu điểm | Phi tập trung và an toàn. Không có hoàn trả hoặc gian lận. Có thể sử dụng dưới dạng ẩn danh. Được chấp nhận toàn cầu. | Giao dịch nhanh hơn và rẻ hơn. Tăng khả năng mở rộng. Giao dịch ngoài chuỗi không làm tắc nghẽn blockchain. |
| Nhược điểm | Thời gian giao dịch chậm. Phí cao đối với một số loại giao dịch. Phức tạp đối với người mới bắt đầu. | Có thể cần tin tưởng vào người vận hành kênh. Cần giao dịch trên chuỗi để mở và đóng kênh. |
