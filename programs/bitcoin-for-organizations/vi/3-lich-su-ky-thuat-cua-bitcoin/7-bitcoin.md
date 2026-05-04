# 3.7 Bitcoin

Sau nhiều năm và nhiều nỗ lực thất bại, hầu hết các Cypherpunks đã bắt đầu mất dần hứng thú với ý tưởng về một loại tiền kỹ thuật số không cần sự cho phép, thì Adam Back nhận được một email dẫn đến bản nháp white paper có tên ‘electronic cash without a third party’ từ một người ẩn danh tự xưng là Satoshi Nakamoto.

Tóm lại đến thời điểm này, chúng ta đã có ít nhất các ý tưởng sau:

* Chữ ký mật mã có thể cung cấp một mức độ riêng tư và ẩn danh
* Khái niệm về một loại tiền không được bảo chứng (B-Money)
* Các đề xuất (nhưng chưa có cách thực hiện) để giới hạn việc phát hành tiền mới
* Đồng tiền kỹ thuật số mà quyền sở hữu được xác định bằng khóa công khai (B-Money) và có thể được chuyển đi bằng cách ký và gán lại dựa trên địa chỉ người nhận (RPOW và Hashcash)
* Tất cả các node đều duy trì một bản sao của sổ cái phân tán hoàn toàn (B-Money) (vào thời điểm đó bị cho là không khả thi)
* Giao thức đóng dấu thời gian – sử dụng băm cây Merkle để cung cấp một trình tự sự kiện có thể chứng minh bằng toán học và khó bị làm giả nếu tất cả người dùng giữ cùng một bản ghi
* Bằng chứng công việc để gắn nỗ lực thực tế vào hệ thống (nhưng sử dụng chính hàm băm làm tiền tệ)
* Mạng lưới hoàn toàn phi tập trung, nơi tất cả các nút đều bình đẳng và có thể tham gia hoặc rời khỏi mạng bất cứ lúc nào (BitTorrent)
* Khái niệm liên kết các hàm băm mới với các hàm băm trước đó (Bit Gold và đóng dấu thời gian)

Những điều còn thiếu vào thời điểm này bao gồm:

* Một giải pháp khả thi để giải quyết vấn đề ‘các vị tướng Byzantine’
* Một phương pháp để giới hạn lượng tiền lưu thông bất chấp sự cải tiến liên tục của phần cứng
* Cơ chế khuyến khích để mọi người tham gia (vấn đề con gà và quả trứng)

Điểm khác biệt lớn khác giữa các nỗ lực gần đây và Bitcoin là Satoshi đã làm việc trên mã nguồn trong một thời gian dài theo đúng tinh thần ‘Cypherpunks write code’ trước khi công bố trên các danh sách thư, không giống như Bit Gold và B-Money vốn chỉ mang tính ý tưởng.

Đâu là đổi mới đã giúp Bitcoin khác biệt so với các nỗ lực tiền điện tử trước đó?

Bằng chứng công việc sẽ được sử dụng như một cơ chế đồng thuận và là cách để cung cấp tính bảo mật và bất biến: Thay vì sử dụng hàm băm như một dạng tiền, nó sẽ được sử dụng bởi một quy trình khái niệm mới gọi là khai thác, nơi một node sẽ gom một tập hợp các giao dịch, thêm một số ngẫu nhiên và sau đó áp dụng hàm băm cho ‘khối’ dữ liệu đó. Một khối hợp lệ đáp ứng yêu cầu về hàm băm sẽ được quảng bá lên mạng lưới. Các khối này sẽ được liên kết với nhau bằng hàm băm của khối trước đó, và chuỗi khối dài nhất sẽ được sử dụng trong trường hợp có nhiều chuỗi cùng lúc khi các node khác nhau xác thực và quảng bá các khối khác nhau, tạo ra các nhánh chuỗi. Bằng chứng công việc trở thành cơ chế phân tán để giải quyết vấn đề các vị tướng Byzantine.

Những người khai thác này cũng được khuyến khích cung cấp CPU cần thiết để thực hiện bằng chứng công việc bằng cách được phân bổ bitcoin mới cho mỗi khối. Số lượng Bitcoin họ nhận được cũng được lập trình để giảm khoảng mỗi 4 năm cho đến khi toàn bộ Bitcoin được tạo ra, tạo ra giới hạn cứng cho tổng số Bitcoin sẽ lưu thông là 21 triệu.

Ý tưởng độc đáo nhất là cách Satoshi giải quyết vấn đề lượng tiền được tạo ra khi phần cứng ngày càng mạnh và nhiều sức mạnh tính toán hơn có thể được áp dụng vào mạng lưới. Dấu thời gian của một số lượng khối nhất định (2016) sẽ được lấy trung bình, và nếu các khối được tạo ra quá nhanh, độ khó của hàm băm để tạo khối mới sẽ được tăng lên, nếu quá chậm thì sẽ được giảm xuống. Điều này được tích hợp vào giao thức phi tập trung mà tất cả các node đều chạy, nên bất kỳ thợ đào nào bỏ qua nó sẽ tiêu tốn năng lượng để khai thác một khối mà không có lợi ích gì vì nó sẽ bị phần còn lại của mạng từ chối. Sự điều chỉnh này đảm bảo việc tạo ra các khối mới luôn theo đúng lịch trình phát hành dự kiến, và tạo động lực cho thợ đào ‘tuân thủ luật chơi’.

####   
Tóm tắt

Nhiều mảnh ghép của bài toán xây dựng một hệ thống tiền điện tử ngang hàng phi tập trung dựa trên các nguyên tắc tiền tệ vững chắc đã có sẵn trước khi Satoshi phát hành whitepaper và ngay sau khi mã nguồn ban đầu được công bố.

> Bản chất của Bitcoin là một khi phiên bản 0.1 được phát hành thì thiết kế cốt lõi đã được cố định cho suốt vòng đời còn lại của nó  
_Satoshi Nakamoto_

Mặc dù nhiều ý tưởng cải tiến (BIP) đã được đề xuất và áp dụng, Bitcoin vẫn hoạt động ổn định kể từ năm 2009 theo đúng giao thức được thiết kế trong bản phát hành ban đầu và hầu như không bị gián đoạn. Tất cả các cải tiến đều được thực hiện trong khi vẫn đảm bảo khả năng tương thích ngược với tất cả các phiên bản trước.



##### Ghi chú

1. Để giải thích về vấn đề các vị tướng Byzantine – xem [https://vi.wikipedia.org/wiki/L%E1%BB%97i_Byzantine](https://en.wikipedia.org/wiki/Byzantine_fault)
