# 6 - Cách sử dụng Bitcoin

Thời lượng: 90 phút

Ý tưởng cốt lõi: Sử dụng Bitcoin trên chuỗi giúp học sinh hiểu cách hoạt động của quyền sở hữu, tự lưu ký và xác minh trong thực tế, biến lý thuyết thành hành động tài chính trực tiếp.

#### Mục tiêu học tập

Sau khi hoàn thành bài học này, học sinh sẽ có thể:

* Nhận biết các cách phổ biến để mua và trao đổi bitcoin, bao gồm phương thức ngang hàng và sàn giao dịch tập trung.
* Giải thích sự khác biệt giữa ví tự lưu ký và ví lưu ký, và lý do tại sao tự lưu ký lại quan trọng trong Bitcoin.
* Mô tả mục đích của khóa riêng tư, địa chỉ công khai, cụm từ khôi phục và giao diện ví.
* So sánh các loại ví khác nhau và đánh giá ưu nhược điểm dựa trên bảo mật, tiện lợi, quyền riêng tư và quyền kiểm soát.
* Cài đặt một ví Bitcoin trên điện thoại và giải thích quy trình khôi phục cơ bản.
* Thực hành nhận và gửi một giao dịch bitcoin trên chuỗi.

Áp dụng nguyên tắc "Đừng tin, hãy xác minh" vào việc chọn ví, giao dịch và sử dụng Bitcoin nói chung.

#### Công cụ & Tài nguyên

##### Trợ giúp trực quan

* Chương 6 - Cách sử dụng Bitcoin

##### Thư viện hỗ trợ

* Thẻ tham khảo từ vựng — Chương 6 — Thuật ngữ: ví, khóa riêng tư, địa chỉ công khai, cụm từ khôi phục, lưu ký, tự lưu ký, UTXO, phí giao dịch
* Bảng so sánh & Tài liệu tham khảo — So sánh các loại ví (lưu ký, di động, phần cứng, giấy)
* Giải thích kỹ thuật & Phân tích chuyên sâu — Khóa công khai/riêng tư, mô hình UTXO, xác nhận giao dịch
* Phân tích chuyên sâu về bảo mật khóa riêng tư — Cụm từ khôi phục, dẫn xuất khóa, phương pháp sao lưu, các kiểu tấn công
* Hướng dẫn cấu trúc giao dịch — Ví dụ từng bước về cách một giao dịch Bitcoin hoạt động
* Danh sách kiểm tra các thực hành bảo mật tốt nhất — Trước khi bắt đầu, tạo ví, nhận, gửi, phòng tránh lừa đảo

#### Hoạt động

* Giao dịch thực tế
* Cuộc đua tiếp sức Lightning
* Khám phá Mempool

#### Dạy học trực tuyến

* Làm rõ ngay từ đầu rằng học sinh đang xem trình diễn hay tự mình cài đặt ví.
* Sử dụng ảnh chụp màn hình lớn, dễ đọc cho từng bước cài đặt ví.
* Tạm dừng sau mỗi bước và yêu cầu học sinh xác nhận đã hiểu trong phần trò chuyện trước khi tiếp tục.
* Cảnh báo trực tiếp trước phần cụm từ khôi phục và nhắc học sinh không bao giờ chia sẻ thông tin nhạy cảm lên mạng.

#### Chuẩn bị

* Tải về và thử nghiệm một ứng dụng ví di động (Blue Wallet hoặc Muun); chuẩn bị ảnh chụp màn hình các bước cài đặt chính.
* Chuẩn bị hướng dẫn cài đặt ví (tải về → tạo → sao lưu cụm từ khôi phục → nhận) để tham khảo.
* Đảm bảo mạng/WiFi hoạt động; chuẩn bị sẵn địa chỉ demo và mã QR để trình chiếu.

#### Quy trình

Bài học này chuyển từ lý thuyết sang thực hành trực tiếp. Hiện tại, nó phù hợp trực tiếp với cấu trúc của Chứng chỉ, để các phần mua, ví, cài đặt, giao dịch và xác minh xuất hiện dưới cùng các tiêu đề chính như trong hướng dẫn học sinh. Các hỗ trợ giảng dạy bổ sung vẫn được lồng ghép trong các phần đó.

##### 6.0 Giới thiệu, 8 phút

Bắt đầu bằng cách kết nối chương này với chương trước:

* Nếu Bitcoin là tiền, vậy mọi người thực sự lấy và sử dụng nó như thế nào?
* Thực sự kiểm soát bitcoin của bạn nghĩa là gì?
* Tại sao sử dụng Bitcoin lại khác với dùng ứng dụng ngân hàng?

Làm rõ rằng chương này tập trung vào việc sử dụng thực tế. Học sinh không chỉ học Bitcoin là gì, mà còn học cách tương tác trực tiếp với nó.

##### 6.1 Mua và trao đổi Bitcoin, 12 phút

Giải thích rằng mọi người có thể mua bitcoin theo nhiều cách khác nhau, bao gồm:

* nhận lương bằng bitcoin
* đào bitcoin
* đổi tiền mặt lấy bitcoin trực tiếp
* đổi tiền mặt lấy bitcoin trực tuyến

Sau đó tập trung vào hai cách mua chính được đề cập trong chương:

* giao dịch ngang hàng, trực tiếp
* ngang hàng (peer-to-peer), trực tuyến
* sàn giao dịch tập trung

Làm rõ những điểm đánh đổi.

Với P2P trực tiếp, nhấn mạnh việc trao đổi trực tiếp không qua ngân hàng hay bên trung gian, nhưng cũng cần đề cập đến những rủi ro thực tế khi gặp mặt để giao dịch tiền mặt.

Với P2P trực tuyến, giải thích về dịch vụ ký quỹ (escrow) một cách đơn giản, như một cách để giảm rủi ro đối tác mà vẫn cho phép trao đổi trực tiếp giữa các cá nhân.

Với sàn giao dịch tập trung, cần làm rõ rằng chúng tiện lợi, nhưng người dùng phải tin tưởng vào một công ty, thường phải cung cấp thông tin cá nhân, và tiền sẽ do bên thứ ba kiểm soát cho đến khi rút ra. Đây là dịp tốt để nhấn mạnh rằng sự tiện lợi thường đi kèm với đánh đổi về quyền riêng tư và quyền tự chủ.

##### 6.2 Giới thiệu về Ví Bitcoin, 35 phút

**Ví Bitcoin Thực Sự Là Gì**

Làm rõ một hiểu lầm phổ biến ngay từ đầu: bitcoin không được lưu trữ bên trong ứng dụng ví như tiền mặt trong túi.  
Bitcoin tồn tại trên sổ cái do mạng lưới duy trì. Điều người dùng kiểm soát là khả năng chi tiêu thông qua các khóa riêng.

Sau đó giải thích hai ý nghĩa mà mọi người thường nói khi nhắc đến "ví":

* hệ thống khóa riêng, từ đó tạo ra các địa chỉ
* ứng dụng hoặc giao diện dùng để tương tác với mạng lưới

Sử dụng phép so sánh với email trong chương nếu cần thiết:

* địa chỉ công khai = giống như địa chỉ email bạn có thể chia sẻ
* khóa riêng = giống như mật khẩu bạn phải bảo vệ

Cần nhấn mạnh rõ ràng: ai kiểm soát khóa riêng thì kiểm soát bitcoin. Đây là khái niệm cốt lõi mà học viên cần hiểu.

**Ví Tự Quản Lý và Ví Lưu Ký**

Đây là một trong những phần quan trọng nhất của chương.

Giải thích sự khác biệt một cách rõ ràng:

* Ví tự quản lý: người dùng kiểm soát khóa riêng
* Ví lưu ký: một bên thứ ba kiểm soát khóa riêng thay cho người dùng

Sau đó trình bày các điểm đánh đổi:

Tự quản lý

* toàn quyền kiểm soát tài sản
* không cần quy trình phê duyệt
* bảo vệ khỏi việc tịch thu tùy tiện
* trách nhiệm lớn hơn
* không dễ khôi phục nếu mất cụm từ khôi phục (seed phrase)

Lưu ký

* dễ dàng khôi phục và được hỗ trợ
* đơn giản hơn cho người mới bắt đầu
* dễ bị đóng băng tài khoản, bị hack, và kiểm soát bởi bên thứ ba
* người dùng thực sự không nắm giữ bitcoin

Đây là thời điểm thích hợp để nhấn mạnh câu:

"Không phải khóa của bạn, không phải tiền của bạn."

Học viên nên rời khỏi phần này không chỉ hiểu khẩu hiệu, mà còn hiểu ý nghĩa thực tế của nó.

**Các Loại Ví Khác Nhau và Cách Chọn**

Giới thiệu các loại ví được đề cập trong chương:

* ví trực tuyến
* ví di động
* ví máy tính để bàn
* ví phần cứng
* ví giấy

Không nên coi loại nào là hoàn hảo. Thay vào đó, hãy giải thích rằng mỗi loại đều có sự đánh đổi giữa:

* bảo mật
* quyền riêng tư
* tiện lợi
* tương thích
* phí
* kiểm soát
* uy tín

Cũng cần làm rõ rằng chúng tôi khuyến nghị chú ý xem phần mềm ví có mã nguồn mở hay không, vì các công cụ mã nguồn mở có thể được cộng đồng kiểm tra, đánh giá và tiếp tục phát triển. Điều này liên quan trực tiếp đến nguyên tắc xác minh trong Bitcoin.

##### 6.3 Cài Đặt Ví Bitcoin Trên Điện Thoại, 10 phút

Hướng dẫn học viên qua các bước cơ bản được trình bày trong chương:

* tải ví về
* tạo ví mới
* tạo và ghi lại cụm từ khôi phục
* xác nhận cụm từ khôi phục
* thêm bảo mật bổ sung nếu có
* mở ví và tìm chức năng nhận

Hãy nhấn mạnh cảnh báo về cụm từ khôi phục:

* nếu mất cụm từ khôi phục, có thể mất quyền truy cập vào tiền
* nếu người khác có được cụm từ khôi phục, họ có thể lấy tiền

Nếu học viên thực hành trực tiếp, giáo viên nên dừng lại ở mỗi bước và kiểm tra xem mọi người đã hiểu mình đang làm gì chưa. Nếu lớp học mang tính lý thuyết hơn, phần này có thể được giải thích như một hướng dẫn thay vì thực hiện trực tiếp. Tùy chọn khôi phục được trình bày trong chương cũng rất hữu ích để giải thích rằng ví có thể được khôi phục nếu cụm từ khôi phục đã được sao lưu đúng cách.

##### 6.4 Nhận và Gửi Giao Dịch, 17 phút

**Nhận và Gửi Giao Dịch Trên Chuỗi**

Bây giờ hãy giải thích cách các giao dịch trên chuỗi hoạt động.

Để nhận bitcoin:

* mở ví
* chọn nhận hoặc nạp
* sao chép địa chỉ, chia sẻ liên kết hoặc hiển thị mã QR

Để gửi bitcoin:

* mở ví
* dán hoặc quét địa chỉ người nhận
* nhập số tiền
* kiểm tra lại tất cả thông tin
* gửi giao dịch lên mạng
* chờ xác nhận

Hãy làm rõ các điểm chính sau:

* giao dịch chuyển quyền sở hữu, không phải chuyển đồng tiền vật lý
* giao dịch không thể đảo ngược
* các node xác minh tính hợp lệ
* thợ đào đưa giao dịch vào các khối
* phí ảnh hưởng đến mức độ ưu tiên xác nhận
* giao dịch trên chuỗi thường an toàn, nhưng chậm hơn và thường tốn phí cao hơn giao dịch Lightning

Sơ đồ luồng giao dịch trong chương này đặc biệt hữu ích, vì nó giúp học viên hình dung được quá trình từ yêu cầu ví đến xác nhận trên mạng.

**Giao Dịch Thực Tế và Thực Hành Theo Vai Trò**

Sử dụng cấu trúc bài tập hợp tác từ chương để củng cố kiến thức. Giải thích bốn vai trò liên quan:

* người gửi
* người nhận
* thợ đào
* người vận hành node

Một cách đơn giản trong lớp học là phân vai và cùng nhau thực hiện một giao dịch từng bước. Điều này giúp học viên thấy rằng giao dịch Bitcoin không phải là phép màu, mà là một quá trình phối hợp gồm phê duyệt, xác minh, đưa vào khối và cập nhật sổ cái.

Mục tiêu ở đây không phải là đi sâu kỹ thuật. Mà là giúp học viên hiểu ai làm gì trong một giao dịch và tại sao xác minh lại quan trọng.

##### 6.5 Đừng Tin, Hãy Xác Minh, 8 phút

Giải thích rằng điều này áp dụng cho:

* ví
* sàn giao dịch
* ứng dụng
* chi tiết giao dịch
* những tuyên bố về "lợi nhuận dễ dàng"
* các dự án giả vờ giống như Bitcoin

Làm rõ rằng Bitcoin yêu cầu người dùng phải suy nghĩ phản biện, tự xác minh những gì mình đang sử dụng và tránh tin tưởng một cách mù quáng. Cũng giải thích tại sao các công cụ mã nguồn mở lại quan trọng trong bối cảnh này: chúng cho phép việc xác minh độc lập.

###### Tổng kết và Kiểm tra Hiểu biết

Kết thúc bằng một vài câu hỏi nhanh:

* Sự khác biệt giữa ví lưu ký và ví tự lưu ký là gì?
* Tại sao cụm từ khôi phục (seed phrase) lại quan trọng đến vậy?
* Điều gì xảy ra khi bạn gửi một giao dịch trên chuỗi (on-chain)?
* Tại sao các giao dịch trên chuỗi lại chậm hơn một số hình thức thanh toán Bitcoin khác?
* "Đừng tin, hãy xác minh" có ý nghĩa gì trong thực tế?

#### Ghi chú cho Giáo viên

Chương này mang tính thực hành cao, vì vậy hãy ưu tiên sự rõ ràng, an toàn và lặp lại.

Học viên không cần phải thành thạo mọi loại ví chỉ trong một buổi học. Mục tiêu chính là:

* hiểu những kiến thức cơ bản về ví
* hiểu về tự lưu ký
* học quy trình giao dịch cơ bản
* hình thành tư duy xác minh có trách nhiệm

Hãy đặc biệt cẩn trọng khi nói về cụm từ khôi phục và việc thiết lập ví. Học viên cần hiểu rằng đây không phải là chi tiết nhỏ, mà là nền tảng của quyền sở hữu Bitcoin.

Những hình ảnh minh họa và hoạt động hữu ích nhất trong chương này là:

* so sánh giữa ví tự lưu ký và ví lưu ký
* bảng so sánh ưu nhược điểm các loại ví
* bài tập thiết lập ví từng bước
* sơ đồ quy trình giao dịch
* hoạt động giao dịch theo vai trò

##### Biểu hiện Tốt là như thế nào

* Điều quan trọng là học viên thực sự thiết lập một ví hoặc xem một hướng dẫn cẩn thận, lấy cụm từ khôi phục làm trung tâm với câu "12 từ này CHÍNH LÀ Bitcoin của bạn", kiểm tra các tình huống như "Điều gì xảy ra nếu bạn mất điện thoại?", và luyện tập nhận diện lừa đảo phishing.
* Giáo viên nên là người hướng dẫn thực hành, đã từng làm việc này trước đó, có ý thức bảo mật nhưng không hoang tưởng, và trung thực về độ khó cũng như quá trình học hỏi cần thiết.
* Học viên cảm thấy mình đã học được một kỹ năng thực tế có thể sử dụng, hiểu rằng cụm từ khôi phục là thật và quan trọng chứ không phải khái niệm trừu tượng, cảm thấy tự tin giữ Bitcoin của chính mình, và hiểu rằng sự phi tập trung đòi hỏi trách nhiệm cá nhân.
* Kết quả học tập sẽ đạt được nếu học viên có thể thiết lập ví và hiểu sự khác biệt giữa khóa công khai và khóa riêng tư, hiểu các lựa chọn giữa ví lưu ký và tự lưu ký, giải thích được cách hoạt động của một giao dịch bao gồm đầu vào, đầu ra và phí, thể hiện nhận thức về bảo mật như bảo vệ cụm từ khôi phục, và biết đặt câu hỏi phản biện về quyền sở hữu và kiểm soát.

##### Quản lý Thời gian

Nếu thời gian hạn chế, hãy ưu tiên:

* Hiểu những kiến thức cơ bản về ví
* Hiểu về tự lưu ký
* Học quy trình giao dịch cơ bản
* Hình thành tư duy xác minh có trách nhiệm

Nếu còn thời gian, hãy dành thêm cho:

* Bảng so sánh ví tự lưu ký và ví lưu ký
* Bảng so sánh ưu nhược điểm các loại ví
* Bài tập thiết lập ví từng bước với hướng dẫn trực tiếp
* Sơ đồ quy trình giao dịch kèm tính toán phí
* Thực hành bảo mật nâng cao và cân nhắc về ví phần cứng

##### Nếu Học viên Gặp Khó khăn

* Cụm từ khôi phục là "thật" → "Cụm từ này CHÍNH LÀ bitcoin của bạn; không có dịch vụ khách hàng."
* Khóa công khai vs. khóa riêng tư → So sánh với email (địa chỉ vs. mật khẩu).
* Tại sao lại khó → "Bạn kiểm soát nó; bạn chịu trách nhiệm." Hãy thừa nhận sự đánh đổi.
