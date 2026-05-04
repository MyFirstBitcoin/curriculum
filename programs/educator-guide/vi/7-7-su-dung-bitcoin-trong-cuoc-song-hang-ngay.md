# 7 - Sử dụng Bitcoin trong cuộc sống hàng ngày

Thời lượng: 90 phút

Ý tưởng cốt lõi: Lightning Network giúp Bitcoin trở nên thực tế hơn cho các khoản thanh toán hàng ngày bằng cách cho phép giao dịch nhanh hơn, rẻ hơn trong khi vẫn giữ Bitcoin làm nền tảng.

#### Mục tiêu học tập

Sau khi hoàn thành bài học này, học viên sẽ có thể:

* Giải thích Lightning Network là gì và lý do nó được xây dựng trên nền tảng của Bitcoin.
* So sánh giao dịch on-chain và Lightning về tốc độ, chi phí và các đánh đổi về bảo mật.
* Phân biệt ví Lightning lưu ký và tự lưu ký, và giải thích tại sao tự lưu ký lại quan trọng.
* Thiết lập một ví Lightning và mô tả vai trò của cụm từ khôi phục (seed phrase) trong việc phục hồi ví.
* Trình bày cách các khoản thanh toán Lightning di chuyển qua mạng lưới, ngay cả khi hai người dùng không có kênh trực tiếp với nhau.
* Nhận biết các cách sử dụng Bitcoin trong đời sống hàng ngày thông qua Lightning, bao gồm mua cà phê, đi chợ, thanh toán cho cửa hàng và chi tiêu tại địa phương.
* Giải thích cách các công cụ như BTCPay Server, BTCMap và thẻ quà tặng giúp mở rộng việc sử dụng Bitcoin trong thực tế.
* Mô tả kinh tế tuần hoàn Bitcoin là gì và tại sao Lightning giúp nó khả thi hơn.

#### Công cụ & Tài nguyên

##### Trợ giúp trực quan

* Chương 7 - Sử dụng Bitcoin trong đời sống hàng ngày

##### Thư viện hỗ trợ

* Thẻ tham khảo từ vựng — Thuật ngữ: Lightning Network, kênh thanh toán, định tuyến, Layer 2, kinh tế tuần hoàn, kiều hối
* Thư viện ví dụ thực tế & nghiên cứu tình huống — El Salvador, kinh tế tuần hoàn tại Austin, câu chuyện các cửa hàng chấp nhận Lightning
* Bảng so sánh & Phiếu tham khảo — So sánh On-Chain và Lightning; So sánh phí & tốc độ giữa các phương thức thanh toán
* Giải thích đơn giản về Lightning Network — Cách hoạt động của kênh thanh toán không dùng thuật ngữ chuyên môn; định tuyến; bảo mật; các trường hợp sử dụng
* Hướng dẫn các tình huống thanh toán — Từng bước: gửi cho bạn bè, nhận thanh toán, kiều hối, nhận thanh toán với tư cách freelancer
* Công cụ so sánh phí & tốc độ — Khi nào nên dùng Lightning, on-chain hay ngân hàng (kèm ví dụ về chi phí)

#### Hoạt động

* Cuộc đua tiếp sức Lightning

#### Dạy học trực tuyến

* Sử dụng slide so sánh song song giữa thanh toán on-chain và Lightning.
* Bắt đầu bằng một tình huống thực tế như mua cà phê hoặc gửi kiều hối để học viên hiểu lý do Lightning ra đời.
* Sử dụng sơ đồ định tuyến ba người đơn giản để giải thích mạng lưới một cách rõ ràng.
* Giữ phần cơ chế kênh ở mức đơn giản trừ khi lớp học đã có nền tảng vững chắc.

#### Chuẩn bị

* Tải ví Lightning và chuẩn bị ảnh chụp màn hình thể hiện tốc độ giao dịch on-chain (chậm) và Lightning (nhanh) cạnh nhau.
* Tìm hiểu 2-3 cửa hàng hoặc cộng đồng thực tế đang sử dụng Lightning; lưu lại BTCMap.org để tham khảo.
* Chuẩn bị bảng so sánh on-chain và Lightning (tốc độ, phí, bảo mật, trường hợp sử dụng) để phát cho học viên.

#### Quy trình

Bài học này giúp học viên thấy cách Bitcoin trở nên thực tế cho các khoản thanh toán hàng ngày thông qua Lightning Network. Hướng dẫn này hiện tuân theo cấu trúc của chương trình Diploma nên các phần chính về Lightning sẽ tương ứng với hướng dẫn cho học viên, trong khi các phần so sánh, công cụ cho cửa hàng và kinh tế tuần hoàn sẽ được lồng ghép vào đúng vị trí.

##### 7.0 Giới thiệu, 8 phút

Bắt đầu bằng cách kết nối chương này với chương trước:

* Nếu Bitcoin đã hoạt động on-chain, tại sao lại cần thêm một lớp nữa?
* Điều gì xảy ra khi mọi người muốn thực hiện nhiều khoản thanh toán nhỏ một cách nhanh chóng?
* Hệ thống thanh toán nào sẽ phù hợp hơn cho việc mua cà phê, đi chợ hoặc trả tiền cho bạn bè?

Làm rõ rằng chương này tập trung vào việc sử dụng Bitcoin trong đời sống hàng ngày, đặc biệt khi tốc độ và phí thấp là quan trọng. Nhấn mạnh rằng Lightning được xây dựng trên nền tảng của Bitcoin, không phải là một hệ thống tách biệt.

##### 7.1 Lightning Network, 25 phút

**Lightning Network là gì**

Giải thích rằng Lightning Network là một hệ thống thanh toán được xây dựng trên nền tảng của Bitcoin, cho phép người dùng gửi và nhận bitcoin một cách nhanh chóng và tiết kiệm. Nó hoạt động bằng cách chuyển nhiều khoản thanh toán nhỏ ra khỏi blockchain chính và chỉ ghi nhận kết quả cuối cùng lên on-chain sau này.

Một cách giải thích dễ hiểu là ví dụ về sổ ghi nợ ở quán cà phê trong chương:

* thay vì thanh toán từng món một trên on-chain
* hai bên mở một kênh thanh toán
* họ cập nhật số dư khi giao dịch với nhau
* chỉ số dư cuối cùng mới được ghi lại trên blockchain khi họ đóng kênh

Điều đó giúp Lightning nhanh hơn và rẻ hơn cho các khoản thanh toán nhỏ thường xuyên. Cũng cần làm rõ rằng các khoản thanh toán Lightning có thể được định tuyến qua mạng lưới, nên người dùng không cần có kênh trực tiếp với tất cả những người họ muốn thanh toán.

**Giao dịch On-chain và Lightning**

Bây giờ hãy làm cho sự khác biệt trở nên thật rõ ràng.

Giao dịch On-chain

* diễn ra trực tiếp trên blockchain của Bitcoin
* thường chậm hơn
* phụ thuộc vào việc được đưa vào block và xác nhận
* có xu hướng an toàn hơn
* có thể tốn kém hơn tùy vào phí giao dịch

Giao dịch Lightning

* diễn ra trên một lớp thứ hai được xây dựng trên nền tảng của Bitcoin
* được xử lý nhanh hơn nhiều
* thường có chi phí thấp hơn nhiều
* phù hợp cho các khoản thanh toán nhỏ và thường xuyên
* có những đánh đổi so với việc thanh toán trực tiếp trên chuỗi

Giữ cho ý chính đơn giản: on-chain mạnh hơn cho việc thanh toán cuối cùng, Lightning mạnh hơn về tốc độ và chi phí thấp cho sử dụng hàng ngày. Sự so sánh này đặc biệt hữu ích ở đây.

##### 7.2 Các loại ví Lightning khác nhau, 10 phút

Giải thích rằng ví Lightning thực hiện chức năng cơ bản giống như ví Bitcoin, nhận và gửi bitcoin, nhưng nó được thiết kế để sử dụng trên Mạng Lightning. Sau đó, trình bày các điểm khác biệt chính về ví trong chương này:

* tự quản lý: người dùng kiểm soát khóa riêng
* ủy thác: người khác kiểm soát khóa riêng

Làm rõ sự đánh đổi cốt lõi:

* ví ủy thác có thể cảm thấy dễ sử dụng và tiện lợi hơn
* nhưng người dùng phải phụ thuộc vào sự cho phép và kiểm soát của người khác
* ví tự quản lý mang lại quyền sở hữu và chủ quyền cao hơn

Cũng nhấn mạnh khuyến nghị của chương là nên ưu tiên sử dụng ví mã nguồn mở, vì các công cụ mã nguồn mở có thể được cộng đồng kiểm tra, cải tiến và xác minh.

##### 7.3 Thiết lập ví Bitcoin Lightning, 10 phút

Hướng dẫn học viên qua các bước thiết lập cơ bản:

* tải về một ví Lightning
* tạo một ví mới
* ghi lại cụm từ khôi phục
* xác nhận các từ theo đúng thứ tự
* thêm bảo mật bổ sung nếu ví cho phép
* bắt đầu sử dụng ví

Hãy đặc biệt nhấn mạnh về cụm từ khôi phục:

* đây là thứ cho phép người dùng khôi phục quyền truy cập
* nếu bị mất, có thể mất quyền truy cập vào tiền
* nếu người khác có được, họ có thể kiểm soát số tiền

Phần này cần nhấn mạnh mạnh mẽ về trách nhiệm và cách xử lý an toàn, giống như trong chương về on-chain.

##### 7.4 Gửi và nhận giao dịch Lightning, 17 phút

**Cách giao dịch Lightning hoạt động trong thực tế**

Sử dụng ví dụ về Minh, Nam và Lan để giải thích về định tuyến. Minh không cần có kênh trực tiếp với Lan. Thanh toán của Minh có thể đi qua Nam, người đã kết nối với mạng, và vẫn đến được Lan một cách an toàn.

Làm rõ các điểm sau:

* Thanh toán Lightning có thể đi qua các bên trung gian
* các bên trung gian này giúp định tuyến thanh toán
* quá trình định tuyến không có nghĩa là người dùng phải tin tưởng vào ngân hàng hoặc nhà cung cấp thanh toán tập trung
* mạng lưới sử dụng mật mã để đảm bảo thanh toán đến đúng người nhận

Điều này giúp học viên hiểu rằng Lightning vẫn là ngang hàng, ngay cả khi thanh toán đi qua một cấu trúc mạng rộng lớn hơn. Nếu cần, hãy chỉ ra rằng chương này cũng đề cập đến việc các nhà vận hành node có thể kiếm phí và giúp củng cố mạng lưới bằng cách định tuyến thanh toán.

**Nạp kênh và sử dụng Lightning nhiều lần**

Giải thích thêm về ví dụ của Mai:

* Mai chuyển bitcoin từ ví on-chain sang ví Lightning của mình
* điều này sẽ nạp tiền cho một kênh thanh toán
* cô ấy sau đó có thể thực hiện các khoản thanh toán lặp lại mà không cần mở lại quy trình mỗi lần
* khi kênh đóng lại, số dư cuối cùng sẽ được quyết toán lại trên chuỗi khối

Làm rõ một giới hạn quan trọng: số tiền bị khóa trong một kênh đang hoạt động là đang được sử dụng cho Lightning và không thể sử dụng tự do cho các giao dịch trên chuỗi cùng lúc. Điều này giúp học viên hiểu rằng Lightning rất mạnh mẽ, nhưng nó liên quan đến một cấu trúc thanh toán khác biệt.

##### 7.5 Mua cà phê và thực phẩm bằng Bitcoin, 20 phút

**Các trường hợp sử dụng hàng ngày**

Chuyển từ cơ chế sang thực tế đời sống.

Giải thích rằng Lightning đặc biệt hữu ích cho:

* mua cà phê
* mua thực phẩm
* mua sắm
* trả tiền cho bạn bè
* giao dịch nhỏ hàng ngày

Ví dụ về Mina trong chương này giúp minh họa tại sao Lightning phù hợp hơn các hệ thống thanh toán truyền thống trong nhiều tình huống: nó nhanh, phí thấp, không biên giới và tiếp cận được cả những người không có tài khoản ngân hàng. Bảng so sánh và sơ đồ xử lý thanh toán là những công cụ giảng dạy mạnh mẽ ở đây, đặc biệt để cho thấy có bao nhiêu bên trung gian trong thanh toán thẻ truyền thống.

**Công cụ cho thương nhân và chi tiêu Bitcoin trong đời thực**

Bây giờ hãy giải thích cách doanh nghiệp và người dùng có thể áp dụng Lightning vào cuộc sống hàng ngày.

Trình bày ba công cụ hoặc con đường chính trong chương:

BTCPay Server

* bộ xử lý thanh toán mã nguồn mở
* giúp thương nhân nhận bitcoin trực tiếp
* không có bên trung gian kiểm soát tiền
* hữu ích cho thanh toán doanh nghiệp trực tuyến và trực tiếp

BTCMap

* giúp người dùng tìm thương nhân và cộng đồng chấp nhận bitcoin
* cho phép mọi người tìm kiếm tại địa phương
* có thể được cộng đồng cập nhật

Thẻ quà tặng và phiếu mua hàng

* công cụ chuyển tiếp để chi tiêu bitcoin ở nơi chưa chấp nhận trực tiếp
* giúp thu hẹp khoảng cách trong khi việc chấp nhận đang phát triển

Phần này quan trọng vì nó cho học viên thấy rằng việc sử dụng Bitcoin không chỉ là lý thuyết. Đã có những công cụ thực tế mà mọi người có thể sử dụng ngay hôm nay.

**Nền kinh tế tuần hoàn và Bitcoin như một phương tiện trao đổi**

Kết thúc nội dung chính bằng cách giải thích rằng nền kinh tế tuần hoàn là một cộng đồng nơi các thành viên cố gắng mua bán với nhau càng nhiều càng tốt. Áp dụng với Bitcoin, điều này có nghĩa là thương nhân, người lao động và người dùng chọn giao dịch bằng bitcoin và hỗ trợ lẫn nhau về kinh tế.

Làm rõ tại sao Lightning quan trọng ở đây:

* thanh toán gần như tức thì
* phí thấp
* thanh toán nhỏ trở nên thực tế
* giao thương địa phương trở nên dễ duy trì hơn

Bạn có thể đề cập rằng chương này nhắc đến các ví dụ như Arnhem và Bitcoin Beach, cho thấy nền kinh tế tuần hoàn không phải là giả định. Chúng đã tồn tại và tiếp tục phát triển. Dòng thời gian trực quan đặc biệt hữu ích ở đây

###### Tổng kết và kiểm tra sự hiểu biết

Kết thúc với một vài câu hỏi nhanh:

* Tại sao Lightning Network được xây dựng?
* Một điểm khác biệt lớn giữa thanh toán trên chuỗi và Lightning là gì?
* Tại sao tự quản lý ví lại quan trọng trong ví Lightning?
* Làm thế nào một người có thể nhận thanh toán Lightning mà không cần kênh trực tiếp với mọi người?
* Nền kinh tế tuần hoàn Bitcoin là gì?

#### Ghi chú cho giáo viên

Giữ mạch giảng dạy chính rõ ràng: Bitcoin là lớp nền tảng, Lightning giúp thanh toán hàng ngày nhanh hơn và rẻ hơn.

Chương này nên mang tính thực tiễn và cụ thể, không quá kỹ thuật.

Ưu tiên sự hiểu biết hơn là đi sâu vào cơ chế kênh.

Những điểm mạnh nhất cần ưu tiên nếu thời gian hạn chế là:

* Lightning là gì
* so sánh giữa on-chain và Lightning: những đánh đổi
* quản lý và thiết lập ví
* thanh toán thực tế ngoài đời
* nền kinh tế tuần hoàn

Những hình ảnh minh họa hữu ích nhất trong chương này là:

* so sánh giữa on-chain và Lightning
* phân biệt các loại ví
* ví dụ về định tuyến với Minh, Hùng và Lan
* bảng so sánh và biểu đồ dung lượng
* sơ đồ xử lý thanh toán truyền thống
* dòng thời gian của nền kinh tế tuần hoàn

##### Hình Mẫu Tốt

* Điều quan trọng là bắt đầu với vấn đề "Bitcoin mất 10 phút và tốn 50.000₫", giải thích Lightning như làn đường nhanh trên nền tảng Bitcoin, sử dụng ví dụ thực tế từ các thương nhân và hành lang kiều hối, đồng thời tạo sơ đồ quyết định khi nào nên dùng on-chain và khi nào nên dùng Lightning.
* Giáo viên nên thực tế về những gì Lightning thực sự giải quyết, chia sẻ các câu chuyện thực tế nơi Bitcoin đang được sử dụng, làm rõ những đánh đổi cụ thể, và giữ thái độ thực tế về mức độ phổ biến trong khi vẫn hào hứng với các khả năng mới.
* Học viên được trải nghiệm việc Bitcoin thực sự hoạt động cho các khoản thanh toán ngoài đời, hiểu rằng tốc độ và chi phí là quan trọng, hình dung một nền kinh tế tuần hoàn nơi Bitcoin lưu thông tại địa phương, nhận ra rằng Lightning ≠ Bitcoin (công cụ khác nhau cho mục đích khác nhau), và trở nên tò mò về các hệ thống kinh tế xây dựng trên thanh toán Bitcoin.
* Kết quả học tập sẽ đạt được nếu học viên có thể giải thích Lightning Network là một lớp trên nền tảng Bitcoin, hiểu cơ bản về kênh thanh toán và định tuyến, thấy các trường hợp sử dụng thực tế của thanh toán Lightning, so sánh on-chain và Lightning trong các tình huống khác nhau, hiểu khái niệm kinh tế tuần hoàn, và nhận biết những đánh đổi cụ thể của từng phương pháp.

##### Quản Lý Thời Gian

Nếu thời gian hạn chế, hãy ưu tiên:

* Lightning là gì
* So sánh giữa on-chain và Lightning: những đánh đổi
* Thanh toán thực tế ngoài đời
* Nền kinh tế tuần hoàn

Nếu còn dư thời gian, hãy dành thời gian cho:

* Cơ chế kênh thanh toán và định tuyến
* Công cụ so sánh phí và tốc độ
* Nghiên cứu điển hình về nền kinh tế tuần hoàn tại El Salvador và Austin
* Hướng dẫn thực hành các tình huống thanh toán Lightning

##### Nếu Học Viên Gặp Khó Khăn

* Tại sao Lightning tồn tại → So sánh: 10 phút/50.000₫ với vài giây/một phần nhỏ của đồng.
* Kênh thanh toán → ví dụ ghi nợ tại quán cà phê; thanh toán nội bộ rồi mới lên Bitcoin.
* Tại sao điều này quan trọng trên toàn cầu → "Nếu không có ngân hàng nhưng có Bitcoin thì sao?"
