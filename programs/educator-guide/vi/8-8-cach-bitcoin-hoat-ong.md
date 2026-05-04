# 8 - Cách Bitcoin Hoạt Động

Thời lượng: 90 phút

Ý tưởng cốt lõi: Sự an toàn của Bitcoin dựa vào những ý tưởng kỹ thuật đơn giản nhưng mạnh mẽ như khóa, chữ ký, hàm băm và UTXO, cho phép xác nhận quyền sở hữu và xác minh mà không cần một cơ quan trung tâm.

#### Mục tiêu học tập

Kết thúc bài học này, học viên sẽ có thể:

* Giải thích cách khóa công khai và khóa riêng giúp bảo vệ quyền sở hữu và giao dịch Bitcoin.
* Mô tả chữ ký số là gì và cách nó chứng minh rằng một giao dịch đã được chủ sở hữu hợp pháp cho phép.
* Giải thích một cách đơn giản các khái niệm mật mã, mã hóa và giải mã trong bối cảnh Bitcoin.
* Định nghĩa hàm băm và mô tả lý do tại sao hàm băm lại quan trọng đối với sự an toàn và tính toàn vẹn dữ liệu của Bitcoin.
* Nhận biết các tính chất cơ bản của một hàm băm, như đầu ra có độ dài cố định, tính một chiều và nhạy cảm với thay đổi nhỏ ở đầu vào.
* Giải thích mô hình UTXO và cách bitcoin được chi tiêu, nhận và trả lại tiền thừa thông qua các đầu ra giao dịch.
* Mô tả cách các node giúp ngăn chặn chi tiêu hai lần bằng cách kiểm tra xem một đầu ra đã được sử dụng chưa.

#### Công cụ & Tài nguyên

##### Trợ giúp trực quan

* Chương 8 - Bitcoin hoạt động như thế nào

##### Thư viện hỗ trợ

* Thẻ tham khảo từ vựng — Chương 8 — Thuật ngữ: mật mã, hàm băm, UTXO, chữ ký số, khóa riêng/khóa công khai, cây merkle, blockchain
* Thư viện hiểu lầm — Chương 8 — Giải thích: "có thể khôi phục seed phrase đã mất", "khóa riêng = mật khẩu", "blockchain là ẩn danh"
* Giải thích kỹ thuật & Đào sâu — Hàm băm, khóa công khai/khóa riêng, mô hình UTXO, bảo mật Proof of Work

#### Hoạt động

* Giao dịch thực tế
* Khám phá Mempool

#### Dạy học trực tuyến

* Sử dụng bảng trắng kỹ thuật số và vẽ từng khái niệm trực tiếp thay vì chỉ giải thích bằng lời.
* Dạy từng ý tưởng kỹ thuật một và thường xuyên dừng lại để kiểm tra câu hỏi.
* Sử dụng hình ảnh minh họa cho khóa, chữ ký, hàm băm và UTXO để học viên dễ theo dõi cấu trúc.
* Giữ mục tiêu ở mức khái niệm và tránh đi quá sâu vào toán học hoặc thuật ngữ chuyên ngành.

#### Chuẩn bị

* Chuẩn bị và ép plastic các sơ đồ: cặp khóa công khai/khóa riêng, chữ ký số, mô hình UTXO, hàm băm (hàm một chiều).
* Đánh dấu trang blockchain explorer và máy tính băm SHA-256; chọn 2-3 giao dịch Bitcoin thực tế để hướng dẫn từng bước.
* Chuẩn bị ghi chú bảng trắng để giải thích đầu vào, đầu ra và cách giao dịch được xác nhận trên blockchain.

#### Quy trình

Bài học này giúp học viên có cái nhìn đầu tiên về mặt kỹ thuật của Bitcoin mà không đòi hỏi kiến thức kỹ thuật trước đó. Hướng dẫn này hiện theo cấu trúc rút gọn giống như chương trình Diploma, với phần mật mã được nhóm dưới một tiêu đề và UTXO được nhóm dưới tiêu đề khác.

##### 8.0 Giới thiệu, 8 phút

Bắt đầu bằng cách đặt kỳ vọng:

* Điều gì làm cho Bitcoin an toàn nếu không có ngân hàng trung ương kiểm soát?
* Làm thế nào mạng lưới biết được một người thực sự sở hữu bitcoin mà họ đang cố gửi?
* Thực sự điều gì xảy ra phía sau khi ai đó thực hiện một giao dịch Bitcoin?

Làm rõ rằng chương này tập trung vào các nền tảng kỹ thuật cơ bản của Bitcoin, đặc biệt là khóa, chữ ký, hàm băm và UTXO. Đồng thời trấn an học viên rằng họ không cần trở thành kỹ sư để hiểu logic cốt lõi. Chương này cũng nhấn mạnh điều đó bằng cách so sánh Bitcoin với internet, rất nhiều người sử dụng nó mỗi ngày mà không cần hiểu hết mọi tầng lớp bên dưới.

##### 8.1 Bảo mật thông qua mật mã, 57 phút

**Bitcoin như một sổ cái lưu trữ trên nhiều máy tính**

Bắt đầu với cách diễn giải đơn giản của chương về mạng lưới Bitcoin:

* Bitcoin là một bản ghi các giao dịch
* bản ghi đó được lưu trữ trên nhiều máy tính gọi là node
* sổ cái là công khai và ẩn danh một phần
* nó hiển thị địa chỉ và lịch sử giao dịch, không phải thông tin nhận dạng cá nhân

Phần này giúp học viên liên hệ lại với những gì họ đã biết từ các chương trước. Bitcoin không dựa trên các tài khoản ẩn bên trong ngân hàng. Nó dựa trên một sổ cái chung mà nhiều người tham gia có thể xác minh.  rất hữu ích ở đây vì nó cho thấy người dùng, ví và mạng lưới Bitcoin rộng lớn kết nối với sổ cái công khai.

**Khóa công khai và khóa riêng**

Bây giờ chuyển sang phần mật mã.

Giải thích rằng mỗi người dùng Bitcoin có:

* một khóa riêng, phải được giữ bí mật
* một khóa công khai, có thể chia sẻ

Làm rõ mục đích của chúng bằng cách đơn giản:

* khóa riêng chứng minh quyền kiểm soát và cho phép chi tiêu
* khóa công khai giúp người khác xác minh rằng giao dịch đã được ủy quyền đúng cách

Một điểm dạy học mạnh từ chương này là Bitcoin sử dụng mật mã khóa công khai/khóa riêng, không phải mô hình cũ nơi hai người phải chia sẻ cùng một khóa bí mật trước. Điều này quan trọng vì nó cho phép xác minh an toàn mà không buộc người dùng tiết lộ bí mật bảo vệ tài sản của họ.

Bạn có thể giải thích như sau:

* khóa riêng giống như bằng chứng bí mật rằng bitcoin thuộc về bạn
* khóa công khai là một phần giúp mạng lưới xác minh quyền ủy quyền của bạn
* ai kiểm soát khóa riêng thì kiểm soát khả năng chi tiêu bitcoin

Hãy cẩn thận đừng làm phức tạp ngôn ngữ mã hóa ở đây. Điều quan trọng nhất cho học sinh là quyền sở hữu và quyền ủy quyền.

**Chữ Ký Số và Ủy Quyền Giao Dịch**

Bây giờ hãy giải thích điều gì xảy ra khi ai đó gửi bitcoin.

Sử dụng trình tự của chương:

* người dùng tạo một giao dịch
* người gửi tạo chữ ký số bằng khóa riêng của họ
* giao dịch được phát lên mạng lưới
* các node xác minh rằng chữ ký là hợp lệ
* sau khi được xác minh và xác nhận, quyền sở hữu được chuyển trên sổ cái

Hãy làm rõ rằng chữ ký số không phải là việc gõ tên. Đó là bằng chứng mật mã rằng chủ sở hữu thực sự đã ủy quyền giao dịch. Đây là một trong những cơ chế cốt lõi cho phép Bitcoin hoạt động mà không cần một cơ quan trung ương phê duyệt giao dịch thủ công. Sơ đồ rất hữu ích vì nó cho thấy việc ký và xác minh một cách trực quan, cũng như đường đi của giao dịch từ người gửi đến xác thực mạng.

Một câu hay cho lớp học là:

Các giao dịch Bitcoin không được phê duyệt vì ngân hàng nói vậy. Chúng được chấp nhận vì mạng lưới có thể xác minh bằng chứng mật mã hợp lệ.

**Băm và Hàm Một Chiều**

Tiếp theo, giải thích về băm.

Bắt đầu đơn giản:

* một hàm nhận đầu vào và tạo ra đầu ra
* một hàm một chiều dễ thực hiện theo một hướng, nhưng thực tế không thể đảo ngược
* một hàm băm nhận dữ liệu với bất kỳ kích thước nào và biến nó thành đầu ra có độ dài cố định gọi là hash

Sử dụng một trong các phép so sánh của chương, chọn cái nào rõ ràng nhất cho học sinh của bạn:

* phép so sánh sinh tố cho hàm một chiều
* phép so sánh dấu vân tay cho hash
* phép so sánh bản nhạc cho việc kiểm tra xem có gì thay đổi không

Phép so sánh dấu vân tay có lẽ là rõ ràng nhất cho hầu hết các lớp học:

* hash giống như dấu vân tay số cho dữ liệu
* nếu đầu vào thay đổi dù chỉ một chút, hash sẽ thay đổi hoàn toàn
* điều này giúp máy tính kiểm tra tính toàn vẹn và phát hiện giả mạo

Sau đó giải thích tại sao băm lại quan trọng trong Bitcoin:

* các giao dịch được băm
* mạng lưới sử dụng hash để giúp xác minh tính toàn vẹn
* nếu một giao dịch bị thay đổi, hash cũng thay đổi
* điều này giúp bảo vệ sổ cái khỏi bị thao túng mà không bị phát hiện

Các hình minh họa từ trang 7 đến 10 rất hữu ích ở đây. Chương này cho thấy cả ý tưởng về đầu ra có độ dài cố định và nguyên tắc "thay đổi nhỏ, kết quả hoàn toàn khác biệt", đây là một trong những khái niệm quan trọng nhất mà học sinh cần hiểu.

**Các Tính Chất Cơ Bản của Hàm Băm**

Đi qua ngắn gọn các tính chất được nhấn mạnh trong chương, mà không làm chúng trở nên quá học thuật:

* Tính xác định: cùng một đầu vào sẽ cho cùng một đầu ra mỗi lần
* Một chiều / chống đảo ngược: bạn không thể đảo ngược quá trình một cách thực tế
* Nhạy cảm với thay đổi: chỉ một thay đổi nhỏ ở đầu vào cũng tạo ra đầu ra rất khác
* Chống va chạm: cực kỳ khó để tìm hai đầu vào khác nhau cho cùng một đầu ra
* Dễ xác minh: hàm này chạy và kiểm tra rất hiệu quả

Bạn không cần học sinh phải ghi nhớ từng thuật ngữ, nhưng họ nên hiểu ý chính: băm cung cấp cho Bitcoin một cách đáng tin cậy để nhận diện dữ liệu và phát hiện thay đổi.

##### 8.2 Mô Hình UTXO, 25 phút

**Mô hình UTXO**

Bây giờ chuyển sang phần lớn thứ hai của chương: UTXO, hay Đầu ra Giao dịch Chưa Được Tiêu.

Giải thích nó một cách đơn giản bằng cách sử dụng phép so sánh tiền mặt trong chương:

* bitcoin không được theo dõi giống như số dư tài khoản ngân hàng
* thay vào đó, nó được tạo thành từ các phần có thể chi tiêu gọi là UTXO
* khi bạn chi tiêu bitcoin, bạn sử dụng một hoặc nhiều UTXO hiện có làm đầu vào
* các UTXO mới sau đó được tạo ra làm đầu ra

Sử dụng ví dụ từ chương:

* nếu bạn có một UTXO 10 BTC
* và bạn gửi 6 BTC
* một UTXO mới 6 BTC sẽ chuyển đến người nhận
* một UTXO tiền thừa mới sẽ quay lại cho bạn
* một phần nhỏ được trả làm phí cho thợ đào

Điều này giúp học sinh thấy rằng Bitcoin hoạt động giống như việc tiêu tiền mặt và nhận lại tiền thừa hơn là chỉ trừ số từ một dòng tài khoản đơn giản. Các sơ đồ đặc biệt hiệu quả ở đây vì chúng trực quan cho thấy một UTXO được chia thành đầu ra cho người nhận, đầu ra tiền thừa và phí.

Làm rõ hai điểm chính:

* số dư ví của bạn là tổng các UTXO bạn có
* khi bạn chi tiêu, các UTXO cũ bị tiêu thụ và các UTXO mới được tạo ra

**Ngăn chặn Chi tiêu Hai lần**

Kết thúc nội dung bằng cách giải thích một trong những ý nghĩa quan trọng nhất của mô hình UTXO.

Nếu ai đó cố gắng chi tiêu cùng một đầu ra hai lần, các node sẽ từ chối lần thử thứ hai vì họ duy trì sổ cái và có thể xác minh liệu UTXO đó đã được tiêu hay chưa. Đây là cách Bitcoin ngăn chặn chi tiêu hai lần mà không cần một công ty thanh toán trung tâm để quản lý hồ sơ. Ví dụ này rất hữu ích ở đây vì nó minh họa quá trình Alice kết hợp các UTXO, gửi tiền cho Bob, nhận lại tiền thừa, và giao dịch được xác nhận sẽ cập nhật sổ cái trên toàn bộ các node.

Một cách diễn đạt rõ ràng trong lớp là:

Bitcoin ngăn chặn chi tiêu hai lần vì mạng lưới theo dõi những đầu ra nào còn chưa tiêu và những đầu ra nào đã được sử dụng.

###### Tổng kết và Kiểm tra Hiểu biết

Kết thúc với một vài câu hỏi nhanh:

* Sự khác biệt giữa khóa công khai và khóa riêng là gì?
* Chữ ký số chứng minh điều gì?
* Tại sao hàm băm lại hữu ích trong Bitcoin?
* Điều gì xảy ra nếu một giao dịch bị thay đổi sau khi đã được băm?
* UTXO là gì theo cách đơn giản?
* Mạng lưới ngăn ai đó chi tiêu cùng một bitcoin hai lần như thế nào?

#### Ghi chú cho Giáo viên

Chương này chứa nhiều thuật ngữ kỹ thuật hơn các chương trước, vì vậy hãy ưu tiên sự rõ ràng, ví dụ so sánh và lặp lại.

Mục tiêu không phải là biến học sinh thành lập trình viên. Mục tiêu là giúp họ hiểu tại sao bảo mật của Bitcoin lại hiệu quả.

Những điểm mạnh nhất cần ưu tiên nếu thời gian hạn chế là:

* khóa riêng so với khóa công khai
* chữ ký số
* hàm băm dùng để làm gì
* UTXO là các phần bitcoin có thể chi tiêu
* cách ngăn chặn chi tiêu hai lần

Những hình ảnh minh họa hữu ích nhất trong chương này là:

* sơ đồ người dùng - ví - mạng lưới
* hình minh họa chữ ký số
* các ví dụ về hàm băm và sơ đồ đầu ra cố định ở trang 7 đến 10
* các sơ đồ UTXO ở trang 10 đến 12

##### Tiêu chí Đạt Chuẩn

* Điều quan trọng là xem mật mã học như một nền tảng chứ không phải điều bí ẩn, sử dụng nhiều hình ảnh minh họa, tránh toán học sâu, liên kết lại các chương trước, và kiểm tra hiểu biết bằng các ứng dụng như "Nếu ai đó thay đổi một giao dịch, điều gì sẽ bị phá vỡ?"
* Giáo viên nên kiên nhẫn với học sinh gặp khó khăn, suy nghĩ trực quan và vẽ mọi thứ, thành thật về những gì học sinh không cần hiểu, sẵn sàng nói "Tôi không biết nhưng đây là cách chúng ta sẽ tìm hiểu," và luôn động viên trong suốt quá trình.
* Học sinh hiểu tại sao Bitcoin không thể bị hack vì nó được bảo vệ bởi toán học, tôn trọng thiết kế tinh tế của hệ thống, cảm thấy thoải mái với sự phức tạp dù không cần biết mọi chi tiết, tự tin đặt câu hỏi mà không bị đánh giá, và nhận ra mình đã nâng cao hiểu biết về điều mà phần lớn mọi người không biết.
* Kết quả học tập sẽ đạt được nếu học sinh có thể giải thích các kiến thức cơ bản về mật mã như hàm một chiều và chữ ký số mà không cần toán học sâu, hiểu mô hình UTXO cho thấy bạn sở hữu đồng coin chứ không phải tài khoản, nhận ra hàm băm là nền tảng bảo mật của Bitcoin, hiểu cấu trúc giao dịch bao gồm chữ ký và xác nhận, giải thích tại sao Bitcoin không thể bị thay đổi, và đặt các câu hỏi phản biện về các cuộc tấn công hoặc lỗ hổng tiềm năng.

##### Quản lý Thời gian

Nếu thời gian hạn hẹp, hãy ưu tiên:

* Khóa riêng tư và khóa công khai
* Chữ ký số
* Chức năng của hàm băm
* UTXO là các phần bitcoin có thể chi tiêu
* Cách ngăn chặn chi tiêu hai lần

Nếu còn thời gian, hãy dành thời gian cho:

* Sơ đồ người dùng-ví-mạng lưới và mô hình bảo mật trực quan
* Hình minh họa chữ ký số: quy trình mật mã chi tiết
* Cây Merkle và bảo mật chuỗi
* Các kiểu tấn công nâng cao và lý do chúng thất bại

##### Nếu học viên gặp khó khăn

* Mật mã học có vẻ đe dọa → "Bạn sử dụng nó hàng ngày; My First Bitcoin cũng sử dụng theo cách đó."
* Khái niệm hàm băm → So sánh với dấu vân tay; duy nhất, không thể thay đổi mà không làm thay đổi hàm băm.
* Chữ ký số → "Chứng minh quyền xác thực mà không tiết lộ mật khẩu."
