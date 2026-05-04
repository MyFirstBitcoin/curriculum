# 9 - Khai thác Bitcoin hoạt động như thế nào

Thời lượng: 90 phút

Ý tưởng cốt lõi: Đào Bitcoin và xác thực nút hoạt động cùng nhau để bảo vệ mạng lưới, xác nhận giao dịch và thực thi các quy tắc của hệ thống thông qua Bằng chứng Công việc (Proof of Work).

#### Mục tiêu học tập

Sau khi hoàn thành bài học này, học viên sẽ có thể:

* Giải thích sự khác biệt giữa vai trò của các nút Bitcoin và vai trò của thợ đào Bitcoin.
* Mô tả cách các nút xác thực giao dịch, chia sẻ thông tin và giúp thực thi các quy tắc của Bitcoin.
* Giải thích công việc của thợ đào, bao gồm chọn giao dịch, xây dựng khối ứng viên và cạnh tranh để tìm ra hàm băm khối hợp lệ.
* Định nghĩa mempool và giải thích tại sao nó hoạt động như một phòng chờ cho các giao dịch chưa được xác nhận.
* Mô tả cách phí giao dịch ảnh hưởng đến việc thợ đào lựa chọn và tốc độ xác nhận.
* Giải thích Bằng chứng Công việc là cơ chế bảo vệ Bitcoin bằng cách khiến các cuộc tấn công trở nên tốn kém.
* Mô tả cách điều chỉnh độ khó giúp duy trì thời gian tạo khối trung bình khoảng 10 phút.
* Trình bày toàn bộ vòng đời của một giao dịch Bitcoin, từ khi tạo và ký đến khi được xác nhận trong một khối.

#### Công cụ & Tài nguyên

##### Trợ giúp trực quan

* Chương 9 - Đào Bitcoin hoạt động như thế nào?

##### Thư viện hỗ trợ

* Thẻ tham khảo từ vựng — Chương 9 — Các thuật ngữ: đào, Bằng chứng Công việc, câu đố hàm băm, điều chỉnh độ khó, phần thưởng khối, mempool, tấn công 51%
* Thư viện hiểu lầm — Chương 9 — Giải thích: "thợ đào tạo ra Bitcoin từ không khí", "thợ đào kiểm soát Bitcoin", "đào nhiều hơn = kém an toàn hơn"
* Bảng so sánh & Tài liệu tham khảo — Kinh tế đào: doanh thu, chi phí, sự đồng thuận về động lực; điều chỉnh độ khó
* Giải thích kỹ thuật & Phân tích chuyên sâu — Bảo mật Bằng chứng Công việc; tại sao tấn công lại tốn kém; ngưỡng 51%

#### Hoạt động

* Khám phá Mempool
* Giao dịch thực tế

#### Dạy học trực tuyến

* Sử dụng một sơ đồ luồng giao dịch rõ ràng từ lúc ví ký đến khi xác nhận.
* Giữ các nút và thợ đào tách biệt rõ ràng trên màn hình trong suốt bài học.
* Sử dụng mempool.space hoặc ảnh chụp màn hình của nó để minh họa các giao dịch chưa xác nhận và áp lực phí.
* Tạm dừng sau mỗi giai đoạn của quá trình đào và đặt một câu hỏi ngắn kiểm tra hiểu biết.

#### Chuẩn bị

* Chuẩn bị sơ đồ quy trình đào (mempool → chọn giao dịch → tạo khối → điều chỉnh độ khó) để trình chiếu.
* Đánh dấu trang mempool.space hoặc trang đào của blockchain.com; chuẩn bị ảnh chụp màn hình thống kê đào và điều chỉnh độ khó hiện tại.
* Tạo giải thích trực quan về Bằng chứng Công việc như một cơ chế bảo mật; trình bày điều chỉnh độ khó trong 3-6 tháng gần đây.

#### Quy trình

Bài học này đi sâu vào cách các giao dịch Bitcoin di chuyển qua mạng lưới và trở thành một phần của blockchain. Hiện tại, bài học tuân theo cấu trúc của chương trình Diploma để các phần chính phù hợp với hướng dẫn học viên, đồng thời vẫn giữ được phần giải thích đầy đủ cho giáo viên trong từng mục.

##### 9.0 Giới thiệu, 8 phút

Bắt đầu bằng cách kết nối chương này với chương trước:

* Nếu một người dùng ký giao dịch bằng khóa riêng, điều gì sẽ xảy ra tiếp theo?
* Ai kiểm tra xem giao dịch đó có hợp lệ không?
* Làm thế nào để giao dịch đó được thêm vào blockchain?
* Tại sao Bitcoin cần cả nút và thợ đào?

Làm rõ rằng chương này giải thích cách mạng lưới xử lý giao dịch trên thực tế và cách đào bảo vệ hệ thống mà không cần một cơ quan trung tâm.

##### 9.1 Các nút và thợ đào Bitcoin, 47 phút

**Nút và thợ đào, vai trò khác nhau**

Bắt đầu bằng cách phân biệt rõ ràng hai vai trò này.

Các nút Bitcoin:

* lưu trữ một bản sao của blockchain
* xác minh xem giao dịch có tuân thủ quy tắc không
* chia sẻ thông tin với các nút khác
* giúp ví và phần mềm khác truy cập dữ liệu blockchain
* có thể từ chối các giao dịch hoặc khối không hợp lệ

Chương này mô tả các node như những người gác cổng xác thực, và mở rộng điều đó với phép so sánh "cảnh sát giao thông kỹ thuật số". Điều này hữu ích vì nó cho thấy các node là những người kiểm tra và điều phối, chứ không phải là người cai trị. Sơ đồ cũng củng cố rằng nhiều node giữ các bản sao của sổ cái trên khắp thế giới.

Thợ đào Bitcoin:

* thu thập các giao dịch hợp lệ
* tập hợp các khối ứng viên
* cạnh tranh để tìm ra hàm băm khối hợp lệ
* phát sóng các khối hợp lệ khi họ chiến thắng
* nhận phần thưởng khối và phí giao dịch

Một điểm giảng dạy quan trọng từ chương này là mục đích của việc đào không chỉ đơn giản là tạo ra bitcoin mới, mà là để phân quyền hóa bảo mật của Bitcoin. Bitcoin mới là động lực, trong khi quá trình đào chính là cơ chế bảo mật.

**Node Thực Sự Làm Gì**

Xây dựng thêm phần node với danh sách chức năng của node trong chương:

* Người gác cổng xác thực: họ kiểm tra các giao dịch và khối có tuân thủ quy tắc không
* Trung tâm giao tiếp: họ kết nối với nhau và chia sẻ dữ liệu giao dịch
* Người kiểm tra chất lượng: họ từ chối thông tin không hợp lệ
* Người cung cấp thông tin blockchain: họ cung cấp dữ liệu cho các phần mềm khác như ví
* Người chào đón node mới: họ giúp các node mới lấy blockchain, trong khi mỗi node mới vẫn tự xác minh dữ liệu độc lập

Đây là thời điểm tốt để nhấn mạnh rằng việc chạy một node giúp người dùng độc lập hơn. Thay vì hoàn toàn phụ thuộc vào các dịch vụ bên ngoài để biết trạng thái mạng lưới, họ có thể tự xác minh. Chương trình này làm rõ điểm đó, bao gồm cả việc đề cập đến Bitcoin Core như một phần mềm mà người dùng có thể chạy.

**Thợ Đào Thực Sự Làm Gì**

Bây giờ hãy giải thích việc đào một cách cẩn thận hơn.

Thợ đào:

* thu thập các giao dịch đã xác minh nhưng chưa được xác nhận
* nhóm chúng thành một khối ứng viên
* liên tục băm dữ liệu khối trong khi tìm kiếm hàm băm khối hợp lệ
* phát sóng khối chiến thắng lên mạng lưới
* nhận phần thưởng nếu khối được chấp nhận

Hãy sử dụng phép so sánh "đống cỏ khổng lồ chứa chìa khóa" trong chương nếu thấy hữu ích. Nó giúp học viên hình dung cụ thể về cuộc đua đào. Ý chính là thợ đào không giải một bài toán toán học hữu ích theo nghĩa thông thường, mà là chứng minh họ đã tiêu tốn năng lượng và tính toán thực tế để bảo vệ hệ thống.

Đây cũng là lúc thích hợp để giải thích về phần thưởng cho thợ đào:

* phần thưởng khối: bitcoin mới phát hành
* phí giao dịch: phí kèm theo các giao dịch mà người dùng muốn xác nhận

Làm rõ rằng thợ đào thường ưu tiên các giao dịch có phí cao hơn, vì điều đó tăng phần thưởng của họ. Chương này cũng giải thích về halving, nên bạn có thể lưu ý ngắn gọn rằng phần thưởng khối giảm sau mỗi 210.000 khối, khoảng bốn năm một lần, theo lịch cung cấp công khai của Bitcoin. Trang 5 và 6 có lịch cung và bảng halving sắp tới, giúp củng cố tính phát hành dự đoán được của Bitcoin.

**Hàm Băm Khối Hợp Lệ, Bằng Chứng Công Việc, và Điều Chỉnh Độ Khó**

Phần này là trọng tâm của chương.

Giải thích rằng thợ đào đang tìm kiếm một hàm băm khối hợp lệ, nghĩa là một hàm băm khối đáp ứng mục tiêu của mạng lưới. Chương này giải thích điều đó như việc tìm một số nhỏ hơn mục tiêu do mạng đặt ra.

Sau đó giải thích rõ về Bằng Chứng Công Việc:

* thợ đào phải thực hiện lặp đi lặp lại các phép tính
* người đầu tiên tìm được hàm băm hợp lệ chứng minh họ đã làm công việc đó
* điều này khiến việc viết lại hoặc tấn công sổ cái trở nên tốn kém
* các node sau đó xác minh khối trước khi chấp nhận

Một câu mạnh để giảng dạy là:

Bằng Chứng Công Việc bảo vệ Bitcoin bằng cách khiến sự gian lận trở nên tốn kém và việc xác minh trở nên dễ dàng.

Cũng giải thích về điều chỉnh độ khó:

* mạng lưới điều chỉnh độ khó đào sau mỗi 2.016 khối
* việc này diễn ra khoảng hai tuần một lần
* mục tiêu là giữ thời gian trung bình giữa các khối gần 10 phút
* nếu có thêm sức mạnh băm tham gia mạng, độ khó sẽ tăng
* nếu sức mạnh băm giảm, độ khó sẽ giảm

Trang 7 và 8 giải thích quá trình này và cho thấy mục tiêu càng khó thì càng cần nhiều công sức hơn. Điều này giúp học viên hiểu rằng thời gian của Bitcoin không bị kiểm soát bởi một cơ quan trung ương mà bởi các quy tắc giao thức tự động phản ứng với điều kiện mạng.

##### 9.2 Mempool Là Gì?, 15 phút

Bây giờ chuyển sang phần mempool.

Giải thích rằng mempool là phòng chờ cho các giao dịch hợp lệ nhưng chưa được xác nhận. Khi người dùng phát sóng một giao dịch, các node sẽ xác minh trước. Nếu hợp lệ, họ thêm vào mempool của mình và chia sẻ với các node khác. Sau đó thợ đào có thể chọn từ các giao dịch đang chờ này khi xây dựng một khối. Trang 10 và 11 giải thích trực tiếp quá trình này.

Những điểm quan trọng cần nhấn mạnh:

* mempool không phải là blockchain
* các giao dịch ở đó vẫn chưa được xác nhận
* mỗi nút đều duy trì mempool riêng của mình
* không có một mempool chung duy nhất
* các giao dịch có phí cao hơn sẽ có khả năng được chọn sớm hơn

Chương này cũng giải thích các lý do phổ biến khiến một giao dịch có thể chưa được xác nhận trong thời gian dài:

* phí thấp
* mạng bị tắc nghẽn
* cố gắng chi tiêu hai lần
* dữ liệu sai hoặc không đầy đủ
* giao dịch bị lỗi định dạng

Nếu phù hợp, hãy nhắc đến hoạt động với mempool.space như một cách thực tế để hình dung các giao dịch chưa xác nhận và mức phí. Cũng cần làm rõ rằng mempool.space chỉ là một trình khám phá, không phải chính mempool.

##### 9.3 Cách Giao Dịch Bitcoin Hoạt Động, 20 phút

Bây giờ hãy tổng hợp mọi thứ lại bằng trình tự từng bước của chương.

Một phiên bản rõ ràng cho lớp học là:



1. Người gửi chọn một UTXO và tạo giao dịch
1. Người gửi thêm địa chỉ người nhận và phí
1. Người gửi ký giao dịch bằng khóa riêng của mình
1. Giao dịch được phát lên mạng lưới
1. Các nút xác minh và thêm vào mempool của họ
1. Thợ đào chọn giao dịch cho một khối ứng viên
1. Thợ đào cạnh tranh thông qua Bằng chứng Công việc
1. Một thợ đào tìm được hàm băm khối hợp lệ và phát khối đó
1. Các nút xác minh khối và thêm vào blockchain
1. Giao dịch nhận được xác nhận khi có thêm các khối mới
1. Hãy làm rõ điểm cuối cùng:
1. khi giao dịch đã được đưa vào một khối hợp lệ, nó được xác nhận
1. các đầu vào đã sử dụng không còn dùng được nữa
1. người nhận giờ kiểm soát các UTXO mới được tạo bởi giao dịch đó

Sơ đồ tóm tắt đặc biệt hữu ích ở đây vì nó kết nối trực quan toàn bộ quá trình từ ký ví đến thợ đào đưa vào khối, đến xác minh của nút và phân phối khối.

###### Tổng Kết và Kiểm Tra Hiểu Biết

Kết thúc bằng một vài câu hỏi nhanh:

* Sự khác biệt giữa nút và thợ đào là gì?
* Mempool là gì?
* Tại sao một số giao dịch được xác nhận nhanh hơn những giao dịch khác?
* Bằng chứng Công việc chứng minh điều gì?
* Tại sao Bitcoin điều chỉnh độ khó khai thác?
* Các bước chính giữa việc gửi giao dịch và nhận xác nhận là gì?

#### Ghi chú cho Giáo viên

Giữ mạch giảng dạy chính rõ ràng: các nút xác minh, thợ đào cạnh tranh, Bằng chứng Công việc bảo mật, và mempool giữ các giao dịch hợp lệ cho đến khi chúng được xác nhận.

Chương này có thể cảm thấy kỹ thuật, vì vậy hãy thường xuyên sử dụng ví dụ so sánh và sơ đồ.

Tránh mô tả khai thác như "tạo bitcoin từ không khí." Hãy nói rõ rằng phần thưởng là động lực, còn quá trình khai thác là để bảo vệ mạng lưới.

Những điểm mạnh nhất cần ưu tiên nếu thời gian hạn chế là:



1. Vai trò của nút và thợ đào
1. Mempool như phòng chờ
1. Bằng chứng Công việc
1. Điều chỉnh độ khó
1. Luồng giao dịch từ ký đến xác nhận

##### Một ví dụ tốt

* Điều quan trọng là phải làm rõ ngay rằng Thợ đào ≠ Nút, cho thấy khai thác là hoạt động kinh tế với chi phí phần cứng và điện thực tế, sử dụng điều chỉnh độ khó và Bằng chứng Công việc để giải thích cơ chế bảo mật, và kiểm tra sự hiểu biết bằng các tình huống về thay đổi mạng lưới.
* Giáo viên nên sử dụng các con số thực tế để làm nền tảng cho các cuộc thảo luận, giải thích thật rõ ràng và lặp đi lặp lại về sự khác biệt giữa Thợ đào (Miners) và Nút mạng (Nodes), thực tế về các mối lo ngại tập trung hóa với các nhóm đào (mining pools), và tôn trọng sự phức tạp thực sự liên quan.
* Học viên hiểu rằng việc đào là những người thông minh làm công việc phức tạp vì họ nhận được Bitcoin, nhận ra rằng động lực thúc đẩy hành vi trung thực vì lợi nhuận của thợ đào phụ thuộc vào sự thành công của Bitcoin, thấy hệ thống tự điều chỉnh thông qua việc điều chỉnh độ khó tự động, hiểu rằng đào là một ngành kinh doanh thực sự chứ không phải từ thiện, và đánh giá rằng bảo mật của Bitcoin tiêu tốn điện và tiền thật.
* Kết quả học tập sẽ đạt được nếu học viên có thể phân biệt thợ đào tạo khối với nút mạng xác thực khối, hiểu Bằng chứng Công việc (Proof of Work) là một cơ chế bảo mật khiến các cuộc tấn công trở nên cực kỳ tốn kém, nhận ra việc điều chỉnh độ khó giữ thời gian tạo khối khoảng 10 phút, hiểu động lực của thợ đào về phần thưởng khối và phí giao dịch, giải thích tại sao tấn công 51% không hiệu quả, và xem việc đào như một hoạt động kinh tế với chi phí và lợi ích thực tế.

##### Quản lý thời gian

Nếu thời gian hạn chế, ưu tiên:

* Vai trò của nút mạng và thợ đào (sự khác biệt then chốt)
* Mempool như phòng chờ
* Cơ chế Bằng chứng Công việc (Proof of Work)
* Điều chỉnh độ khó (hệ thống tự điều tiết)
* Luồng giao dịch từ ký đến xác nhận

Nếu còn thời gian, hãy dành thời gian cho:

* Kinh tế đào và chi tiết phần cứng
* Động lực nhóm đào và các mối lo ngại về tập trung hóa
* Kịch bản tấn công 51% và lý do toán học khiến nó thất bại
* Bảo mật lâu dài thông qua sự đồng thuận về động lực

##### Nếu học viên gặp khó khăn

* Thợ đào vs. nút mạng (nhầm lẫn) → "Nút xác thực, thợ đào đề xuất; trọng tài vs. cầu thủ."
* Bằng chứng Công việc lãng phí → "Bảo mật đắt đỏ ngăn chặn tấn công; khiến chúng trở nên vô nghĩa."
* Điều chỉnh độ khó → "Nhiều thợ đào hơn = khối nhanh hơn = độ khó tăng; hệ thống tự điều tiết."
