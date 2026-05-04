# 9.1 Các nút và thợ đào Bitcoin

Các node Bitcoin nghe có vẻ kỹ thuật, nhưng thực chất chỉ là phần mềm lưu trữ một bản sao của blockchain Bitcoin trên máy tính. Blockchain là một bản ghi chung về tất cả các giao dịch Bitcoin.

Khi bạn vận hành node của riêng mình, bạn tự xác minh các giao dịch Bitcoin thay vì phải tin tưởng người khác. Điều này giúp bạn độc lập hơn và góp phần giữ cho mạng lưới Bitcoin phi tập trung.

Bạn có thể hình dung một node Bitcoin như một cảnh sát giao thông kỹ thuật số với một vài nhiệm vụ quan trọng.

1. Node lưu trữ một bản sao của blockchain, tức là lịch sử của tất cả các giao dịch Bitcoin.
1. Các node kết nối với các node khác trên toàn thế giới và chia sẻ thông tin. Một ví dụ là danh sách các giao dịch mới đang chờ xác nhận, được gọi là mempool.
1. Node kiểm tra xem mỗi giao dịch có tuân thủ các quy tắc của Bitcoin hay không. Nếu một giao dịch không hợp lệ, node sẽ từ chối nó.

Node cũng giúp các node mới tham gia mạng lưới bằng cách chia sẻ blockchain với họ. Tuy nhiên, mỗi node mới vẫn tự kiểm tra tất cả các quy tắc một cách độc lập.

Bất kỳ ai cũng có thể vận hành một node bằng cách cài đặt phần mềm như Bitcoin Core và tải về blockchain. Khi đã thiết lập xong, node sẽ tiếp tục nhận các khối mới khoảng mỗi 10 phút và xác minh chúng trước khi thêm vào bản sao blockchain của mình.

Vận hành một node giúp mạng lưới Bitcoin an toàn và phi tập trung hơn, vì càng nhiều người tự xác minh hệ thống.

#### Node Bitcoin là gì?

> Mục đích của việc đào không phải là tạo ra bitcoin mới; đó chỉ là hệ thống khuyến khích. Đào là cơ chế giúp bảo mật của Bitcoin được phi tập trung hóa._Andreas M. Antonopoulos_


> **Callout**
>
> Thợ đào thu thập các giao dịch chưa xác nhận, tạo thành một khối và sử dụng năng lượng để tìm ra một khóa giúp thêm và bảo vệ khối đó.


Các thợ đào cạnh tranh để thêm khối giao dịch tiếp theo vào blockchain. Để làm được điều này, họ phải tìm ra một con số đặc biệt tạo ra một mã băm hợp lệ cho khối. Bạn có thể tưởng tượng như việc tìm đúng chiếc chìa khóa trong hàng tỷ khả năng. Thợ đào đầu tiên tìm ra mã băm đúng sẽ thắng cuộc đua và có quyền thêm khối của mình vào blockchain.

Khi một thợ đào tìm được mã băm hợp lệ, họ sẽ chia sẻ khối của mình với mạng lưới. Các thợ đào khác nhanh chóng xác minh xem giải pháp có đúng không. Nếu đúng, khối sẽ được thêm vào blockchain, giúp bảo vệ sổ cái công khai của Bitcoin.

Thợ đào kiếm bitcoin theo hai cách:

* **Phần thưởng khối:** Bitcoin mới được tạo ra và trao cho thợ đào đã thành công thêm một khối vào blockchain.
* **Phí giao dịch:** Khi mọi người gửi bitcoin, họ kèm theo một khoản phí nhỏ. Thợ đào thêm khối sẽ nhận được các khoản phí từ các giao dịch có trong khối đó.

#### Các lần giảm một nửa Bitcoin


| 2009 | 2012 | 2016 | 2020 | 2024 |
| --- | --- | --- | --- | --- |
| 50 BTC | 25 BTC | 12,5 BTC | 6,25 BTC | 3,125 BTC |



> **Callout**
>
> Phần thưởng cho thợ đào hoàn thành một khối sẽ giảm một nửa sau mỗi 210.000 khối, tức khoảng bốn năm một lần.


Bitcoin có tổng nguồn cung tối đa cố định là 21.000.000 bitcoin, nhưng không phải tất cả đều được tạo ra khi Bitcoin bắt đầu. Thay vào đó, bitcoin mới dần được đưa vào lưu thông thông qua **đào**.

Khi thợ đào thành công thêm một khối giao dịch mới vào mạng lưới Bitcoin, họ nhận được **phần thưởng khối** bằng bitcoin. Những ngày đầu của Bitcoin, phần thưởng này là 50 bitcoin cho mỗi khối. Phần thưởng này khuyến khích mọi người sử dụng sức mạnh tính toán và điện năng để bảo vệ mạng lưới.

Cứ khoảng mỗi 210.000 khối (tức khoảng 4 năm), phần thưởng khối sẽ giảm một nửa. Sự kiện này được gọi là **giảm một nửa**. Việc giảm một nửa làm chậm lại quá trình tạo ra bitcoin mới và giúp đảm bảo tổng nguồn cung sẽ không bao giờ vượt quá 21 triệu. Theo thời gian, điều này khiến bitcoin ngày càng trở nên khan hiếm.


> **Definition – Nguồn cung lưu thông**
>
> **Nguồn cung lưu thông** là tổng số lượng tiền tệ đang có sẵn. Với Bitcoin, tổng nguồn cung lưu thông là số lượng coin đã được đào và đang lưu thông tại bất kỳ thời điểm nào.


![ Bitcoin Supply Schedule](https://cdn.sanity.io/images/vje9ehw2/staging/f82d4058fe667850b29bdbeee8323645a1f3dfb1-292x200.svg)


> **Definition – Lịch trình nguồn cung Bitcoin**
>
> **Lịch trình nguồn cung Bitcoin** là kế hoạch phát hành bitcoin mới vào lưu thông đã được xác định trước và công khai, nhằm duy trì sự khan hiếm của Bitcoin theo thời gian.


Sau mỗi lần giảm một nửa, phần thưởng bitcoin mà thợ đào nhận được khi thêm một khối sẽ giảm một nửa. Điều này làm giảm tốc độ tạo ra bitcoin mới.

Thợ đào vẫn nhận được phí giao dịch từ các giao dịch có trong khối mà họ đào. Theo thời gian, các khoản phí này dự kiến sẽ trở thành phần lớn hơn trong thu nhập của thợ đào.

Các lần Halving được tích hợp sẵn trong giao thức Bitcoin và diễn ra tự động khoảng mỗi bốn năm một lần. Nhờ vậy, lịch trình phát hành Bitcoin có thể dự đoán và minh bạch.

Bảng dưới đây hiển thị các lần Halving sắp tới, bao gồm ngày dự kiến, số khối khi sự kiện diễn ra, phần thưởng khối mới và phần trăm tổng nguồn cung bitcoin đã được khai thác.


| Sự kiện | Ngày | Khối | Phần thưởng | Đã khai thác |
| --- | --- | --- | --- | --- |
| Halving lần thứ 5 | 2028 | 1.050.000 | 1,5625 BTC | 98,44 % |
| Halving lần thứ 6 | 2032 | 1.260.000 | 0,78125 BTC | 99,22 % |
| Halving lần thứ 7 | 2036 | 1.470.000 | 0,390625 BTC | 99,61 % |


Khi ngày càng nhiều bitcoin được khai thác, nguồn cung lưu thông tiếp tục tăng cho đến khi đạt tối đa 21.000.000 bitcoin, dự kiến vào khoảng năm 2140. Vì số lượng bitcoin mới được tạo ra ngày càng ít đi, nếu nhu cầu tăng lên, giá Bitcoin có thể tăng. Điều này cũng khuyến khích các thợ đào tiếp tục bảo vệ mạng lưới bằng cách đóng góp sức mạnh tính toán của họ.

#### Hash khối hợp lệ trong Bitcoin là gì?

Trong Bitcoin, các thợ đào cạnh tranh để tìm một mã đặc biệt gọi là **hash khối**. Mã này xác định một khối giao dịch và cho phép nó được thêm vào blockchain.

Mỗi khối chứa thông tin về các giao dịch gần đây và cũng bao gồm hash của khối trước đó. Điều này liên kết tất cả các khối lại với nhau, tạo thành một chuỗi từ khối đầu tiên (Genesis Block) đến khối mới nhất.

Hash hoạt động giống như một **dấu vân tay số** cho dữ liệu trong khối. Nếu bất kỳ thông tin nào trong khối bị thay đổi, dấu vân tay này cũng sẽ thay đổi. Điều này giúp bất kỳ ai cũng có thể dễ dàng xác minh rằng lịch sử giao dịch của blockchain không bị thay đổi và góp phần bảo vệ an toàn cho mạng lưới.


> **Callout**
>
> Satoshi Nakamoto, người tạo ra Bitcoin, đã khai thác Genesis Block, mở khóa tổng cộng 50 bitcoin.


#### Cuộc đua khai thác một khối

Các thợ đào cạnh tranh để tìm một hash khối hợp lệ. Thợ đào đầu tiên tìm được sẽ được thêm khối mới vào blockchain và nhận phần thưởng bằng bitcoin.

Để hợp lệ, hash của khối phải nhỏ hơn một con số do mạng lưới đặt ra gọi là mục tiêu độ khó. Vì các hash là ngẫu nhiên, các thợ đào phải thử nhiều đầu vào khác nhau cho đến khi tìm được một giá trị phù hợp.

Nếu có quá nhiều thợ đào cạnh tranh, các khối sẽ được tìm thấy quá nhanh. Nếu quá ít thợ đào tham gia, việc tìm khối sẽ mất quá nhiều thời gian. Để hệ thống vận hành trơn tru, Bitcoin tự động điều chỉnh độ khó sau mỗi 2.016 khối (khoảng hai tuần một lần).

Việc điều chỉnh này đảm bảo rằng, trung bình, một khối mới được thêm vào blockchain khoảng mỗi 10 phút.


> **Definition – Định nghĩa về mức độ khó**
>
> **mức độ khó** trong khai thác Bitcoin đo lường mức độ khó để tìm một hash khối hợp lệ. Mạng lưới sẽ điều chỉnh mức độ khó này sau mỗi 2.016 khối (khoảng hai tuần một lần) để các khối mới được thêm vào blockchain khoảng mỗi 10 phút. Độ khó càng cao, thợ đào càng khó tìm được hash hợp lệ.


Bằng cách tìm được một hash khối hợp lệ, thợ đào chứng minh rằng họ đã thực hiện đủ công việc cần thiết để thêm một khối mới vào blockchain. Quá trình này được gọi là **Bằng chứng công việc** (PoW). Đây là cơ chế bảo mật cho phép Bitcoin xác nhận giao dịch và thêm các khối mới vào blockchain. Thợ đào tìm được hash hợp lệ đầu tiên sẽ nhận phần thưởng bằng bitcoin, bao gồm phần thưởng khối và phí giao dịch từ các giao dịch trong khối đó.

Bằng chứng công việc (PoW) giúp bảo vệ Bitcoin bằng cách khiến cho việc gian lận hoặc kiểm soát mạng lưới trở nên cực kỳ tốn kém. Thay vào đó, tuân thủ các quy tắc sẽ có lợi hơn nhiều.

Thợ đào đóng bốn vai trò chính:

1. **Thu thập giao dịch**: Thợ đào chọn các giao dịch đã được gửi lên mạng và đưa chúng vào một khối ứng viên.
1. **Thực hiện Bằng chứng công việc**: Thợ đào cạnh tranh để giải một bài toán toán học khó bằng cách tìm một hash khối hợp lệ.
1. **Phát sóng khối**: Thợ đào đầu tiên tìm ra giải pháp hợp lệ sẽ chia sẻ khối mới với mạng lưới.
1. **Nhận phần thưởng**: Nếu khối hợp lệ, nó sẽ được thêm vào blockchain và thợ đào nhận được bitcoin mới tạo cùng với phí giao dịch.

Nhiều thợ đào trên khắp thế giới cố gắng tạo ra khối tiếp theo cùng lúc. Khi một thợ đào tìm ra giải pháp hợp lệ, mạng lưới sẽ kiểm tra khối đó. Nếu mọi thứ đều đúng, nó sẽ được thêm vào blockchain. Các khối cạnh tranh khác sẽ bị loại bỏ. Quá trình này giúp mạng lưới đồng thuận và ngăn chặn việc chi tiêu hai lần.

* Thợ đào là các máy tính giúp duy trì và cập nhật sổ cái của Bitcoin.
* Họ thu thập các giao dịch và nhóm chúng lại thành một khối. Sau đó, họ chạy dữ liệu của khối qua một thuật toán băm để tạo ra một mã duy nhất gọi là hash.
* Thợ đào lặp lại quá trình này nhiều lần, tìm kiếm một hash đáp ứng các quy tắc của Bitcoin. Thợ đào đầu tiên tìm được hash hợp lệ sẽ nhận được bitcoin mới tạo làm phần thưởng, và khối của họ được thêm vào blockchain.
* Hash của mỗi khối cũng liên kết nó với khối trước đó. Nếu ai đó cố gắng thay đổi một giao dịch trong quá khứ, các hash sẽ không còn khớp nhau nữa và mạng lưới sẽ từ chối chuỗi đã bị thay đổi. Đây là điều giúp sổ cái của Bitcoin luôn an toàn.
