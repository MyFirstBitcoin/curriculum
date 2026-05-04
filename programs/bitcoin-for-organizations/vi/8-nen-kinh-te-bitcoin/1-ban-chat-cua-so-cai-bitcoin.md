# 8.1 Bản chất của sổ cái Bitcoin

Sổ cái giao dịch của Bitcoin (còn gọi là timechain hoặc blockchain) là một bản ghi công khai, có dấu thời gian của mọi giao dịch hợp lệ từng diễn ra trên mạng lưới. Trong hệ thống tài chính truyền thống, các giao dịch nội bộ chỉ hiển thị cho những người tham gia được ủy quyền, như ngân hàng, cơ quan quản lý, hoặc các nhà vận hành dữ liệu như SWIFT, BACS hoặc SEPA. Việc truy cập dữ liệu thanh toán trên các hệ thống truyền thống thường bị hạn chế nghiêm ngặt và tốn kém.

Ngược lại, trong mạng lưới Bitcoin, bất kỳ ai có kết nối internet đều có thể xem mọi giao dịch, từ giá trị lớn nhất cho đến từng Satoshi riêng lẻ. Người tham gia có thể theo dõi tổng cung bitcoin theo thời gian thực, giám sát hoạt động của địa chỉ và ví, cũng như xem phần thưởng và phí của thợ đào. Mặc dù các hoạt động trên sổ cái được liên kết với địa chỉ khóa công khai chứ không phải danh tính cá nhân, nhưng vẫn có thể tổng hợp các bộ dữ liệu lớn về hành vi chi tiêu, cho phép mọi người thu thập và nghiên cứu hoạt động kinh tế theo thời gian thực. Khi mạng lưới phát triển và ngày càng được chấp nhận như một nguồn sự thật kinh tế, chúng ta có thể sẽ ít phụ thuộc hơn vào các cơ quan chính phủ và nhà cung cấp bên thứ ba trong việc sản xuất các phân tích thống kê và báo cáo về hành vi chi tiêu.



#### 8.1.1 Node và Block Explorer

Bất kỳ ai muốn tự mình xác minh sổ cái Bitcoin và truy cập dữ liệu của nó nên chạy một node đầy đủ. Node đầy đủ thường được mô tả là cách cơ bản nhất để tham gia và xác minh nền kinh tế Bitcoin. Nó có sẵn trên toàn cầu dưới dạng phần mềm mã nguồn mở, khi chạy sẽ tải xuống và xác thực toàn bộ sổ cái Bitcoin từ 'Khối Genesis', được công bố vào tháng 1 năm 2009, cho đến hiện tại. Nó cũng hỗ trợ bảo mật cho mạng lưới Bitcoin bằng cách giúp xác minh các giao dịch mới được thêm vào sổ cái. Khi truy cập sổ cái Bitcoin theo cách này, node đầy đủ đóng vai trò là nguồn sự thật cho các nhà nghiên cứu và kiểm toán viên của mạng lưới. Và, đối với người dùng Bitcoin, node đầy đủ hoạt động như một cổng thông tin 'tự chủ' đến thông tin giao dịch của nền kinh tế Bitcoin vì nó tăng cường quyền riêng tư và bảo mật bằng cách loại bỏ sự phụ thuộc vào các dịch vụ bên thứ ba.

Trong khi node đầy đủ tải xuống dữ liệu thô, các block explorer như mempool.space hoặc blockstream.info cung cấp giao diện trực quan để tìm kiếm và diễn giải hoạt động trên sổ cái. Block explorer cho phép theo dõi từng giao dịch, xem số dư và lịch sử ví. Nó cũng hiển thị các chỉ số hoạt động của thợ đào như phần thưởng khối và dữ liệu phí giao dịch.

Kết hợp lại, node đầy đủ và block explorer là những công cụ giúp tính minh bạch của mạng lưới Bitcoin trở nên hữu ích.



#### 8.1.2 Hoạt động: Khám phá Sổ cái Bitcoin

1. Mở [mempool.space](https://mempool.space) và khám phá trang chủ.
  * Khối mới nhất có chiều cao là bao nhiêu?
  * Phí giao dịch hiện tại là bao nhiêu (Ưu tiên Thấp, Trung bình và Cao)?
  * Có bao nhiêu giao dịch đang chờ trong mempool cho khối tiếp theo?
1. Truy cập khối mới nhất trên sổ cái.
  * Có bao nhiêu giao dịch đã được đưa vào?
  * Tên thợ đào của khối này là gì?
  * Phần thưởng khối là bao nhiêu?
1. Truy cập một giao dịch trong khối.
  * Giao dịch này có bao nhiêu đầu vào và đầu ra?
  * Giá trị giao dịch là bao nhiêu BTC và VND?

Thảo luận về sự khác biệt giữa cách tiền di chuyển trong hệ thống truyền thống và cách một doanh nghiệp hoặc chính phủ sử dụng loại minh bạch này.
