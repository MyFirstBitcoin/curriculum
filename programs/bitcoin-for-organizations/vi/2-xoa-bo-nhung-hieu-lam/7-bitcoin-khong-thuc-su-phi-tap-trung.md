# 2.7 Bitcoin không thực sự phi tập trung

> Sự phức tạp của tiền mã hóa xuất phát từ nỗ lực phi tập trung hóa—bằng cách phân phối quyền lực và quản trị trong hệ thống, về mặt lý thuyết sẽ không cần đến các trung gian đáng tin cậy như các tổ chức tài chính. Đó là tiền đề của bản cáo bạch ban đầu của Bitcoin, trong đó đưa ra một giải pháp mật mã nhằm cho phép thanh toán được gửi đi mà không cần sự tham gia của bất kỳ tổ chức tài chính hay trung gian đáng tin cậy nào khác. Tuy nhiên, Bitcoin đã trở nên tập trung hóa rất nhanh và hiện nay phụ thuộc vào một nhóm nhỏ các nhà phát triển phần mềm và các nhóm đào để vận hành  
_Quỹ Tiền tệ Quốc tế_

Như trích dẫn ở trên từ một bài đăng khá gần đây của Quỹ Tiền tệ Quốc tế cho thấy, ngành tài chính truyền thống vẫn tiếp tục khẳng định rằng Bitcoin không phải là phi tập trung, đồng thời nhầm lẫn giữa Bitcoin với các tài sản mã hóa khác.

##### Giới thiệu

![Trilemma](https://cdn.sanity.io/images/vje9ehw2/staging/fbf9dc03884c24152bd34813c12c0731c2d327cd-161x167.svg)

Phi tập trung hóa là một khía cạnh quan trọng của Bitcoin. Khả năng duy trì các quy tắc của giao thức như sự khan hiếm và phân phối mà không cần một cơ quan trung ương đảm bảo rằng nó có thể hoạt động như một loại tiền không cần xin phép cho xã hội toàn cầu.

Như Satoshi đã đề cập trong các trao đổi trực tuyến của mình, các dịch vụ phi tập trung như BitTorrent đã 'tự đứng vững' trước các cuộc đàn áp của chính phủ, so với các dịch vụ có chủ sở hữu xác định và máy chủ tập trung. Ông rõ ràng lo ngại về nguy cơ tiềm ẩn khi các chính phủ hoặc các thế lực khác có thể đóng cửa hoặc gây ảnh hưởng tiêu cực đến Bitcoin.

Trong bối cảnh này, chúng ta quan tâm đến sự phi tập trung của:

* Việc phát triển và quản lý mã nguồn vận hành giao thức; ai được phép thay đổi các quy tắc?
* Chức năng đào tạo ra các khối mới theo đúng quy tắc và xác thực chống chi tiêu hai lần
* Các node xác thực giao dịch về tính hợp lệ và lưu trữ một bản sao của blockchain

##### Nhà phát triển

Bitcoin là một giao thức mã nguồn mở mà bất kỳ ai cũng có thể xem, tải về, sao chép hoặc đề xuất thay đổi. Nó có sẵn trong thư viện GitHub, mã nguồn ban đầu được Satoshi Nakamoto phát hành vào năm 2009. Bất kỳ ai cũng có thể tải mã về và vận hành một node, phần lớn trong số đó chạy phần mềm Bitcoin Core gốc, đã được cập nhật qua thời gian.

![How Does an idea Make Its Way Into Bitcoin Core?](https://cdn.sanity.io/images/vje9ehw2/staging/49f70d059c9dbe19a6e4500e9abd8db66ca97bff-1300x1439.png)

_Nguồn: https://river.com/learn/what-is-bitcoin-core/_

Việc phát triển Bitcoin Core tuân theo các thực tiễn tốt nhất của phát triển mã nguồn mở. Bất cứ lúc nào, có thể có nhiều nhà phát triển viết hoặc xem xét các thay đổi mã. Họ cần lắng nghe ý kiến của các nhà vận hành node và thợ đào, cũng như cộng đồng người dùng trước khi thực hiện bất kỳ thay đổi quan trọng nào đối với mã, những thay đổi này sẽ được xem xét và đồng thuận như thể hiện trong sơ đồ luồng ở trên trước khi được đưa vào mã nguồn.

Các quy tắc của Bitcoin sau đó được mã hóa trong phần mềm Bitcoin Core này, chạy trên mỗi node. Bất kỳ ai cũng có thể đề xuất thay đổi quy tắc – các quy tắc là mã, nhưng chúng không phải là_chỉ là_ mã, chúng là_mã đã được đồng thuận_. Nếu thay đổi một cách đơn phương, mã mới sẽ không còn là một phần của sự đồng thuận và không còn là một phần của Bitcoin. Thay đổi điều gì đó với Bitcoin mà vẫn giữ được sự đồng thuận là điều không đơn giản. Các đề xuất thay đổi mã được chia thành ba loại:

* Trong phạm vi các quy tắc hiện có: Các nâng cấp nhỏ như sửa lỗi chính tả, giao diện người dùng đẹp hơn hoặc quản lý dữ liệu tốt hơn có thể thuộc loại này và khá dễ dàng để được phê duyệt.
* Thêm một quy tắc mới làm tăng sự hạn chế cho các quy tắc hiện tại – ví dụ như giảm kích thước khối. Điều này được gọi là 'soft fork'. Các node không áp dụng thay đổi mã và vẫn ở phiên bản cũ vẫn có thể tham gia mạng lưới.
* Thêm một quy tắc mới phá vỡ các quy tắc hiện tại, ví dụ như tăng kích thước khối. Các node không nâng cấp lên mã mới sẽ coi một khối được tạo với kích thước lớn hơn là không hợp lệ. Điều này được gọi là 'hard fork' và sẽ tạo ra sự chia tách chuỗi giữa các node chạy mã gốc và mã mới, đồng thời tạo ra một đồng tiền mới. Điều này đã từng xảy ra trước đây nhưng chưa từng mang lại thành công lâu dài cho đồng tiền mới vì phần lớn các node quyết định giữ nguyên mã gốc.

Do đó, một cá nhân hoặc nhóm người không thể đơn phương thay đổi mã Bitcoin mà không đạt được sự đồng thuận, nếu không sẽ có nguy cơ chia tách chuỗi và tạo ra một đồng tiền mới với bộ quy tắc khác.

##### Đào

Chức năng đào xác thực các giao dịch giống như bất kỳ node nào khác trên mạng, nhưng sau đó sẽ tiêu tốn năng lượng cần thiết để tạo ra một khối mới đáp ứng các quy tắc đồng thuận trong mã. Nếu thành công, thợ đào sẽ nhận được phần thưởng dưới dạng phí giao dịch và phần thưởng Bitcoin (tại thời điểm viết là 3,125 đồng mỗi khối).

Việc đào thường được thực hiện bởi các 'Pool đào', nơi mọi người hợp nhất sức mạnh đào hoặc tỷ lệ băm để tăng cơ hội đào thành công một khối và chia sẻ phần thưởng. Có nguy cơ một hoặc nhiều pool đào có thể kết hợp lại để đạt được 51% sức mạnh đào và về cơ bản có thể vượt qua giao thức xác thực mạng lưới theo ý mình để chi tiêu hai lần đồng coin. Điều này sẽ đòi hỏi một lượng tài nguyên khổng lồ với chi phí rất lớn, và các thợ đào cá nhân có thể dễ dàng chuyển sang pool đào khác bất cứ lúc nào. Một cuộc tấn công như vậy cũng có khả năng làm sụp đổ giá trị của bitcoin, vì sẽ rõ ràng rằng tính toàn vẹn của mạng đã bị xâm phạm. Do đó, kẻ tấn công sẽ phải nhanh chóng chuyển đổi bất kỳ bitcoin nào kiếm được sang tiền pháp định trước khi giá trị bị giảm. Điều này càng khiến việc duy trì một cuộc tấn công trong thời gian dài trở nên khó khăn hơn, và do đó khiến việc tuân thủ các quy tắc và cố gắng đào các khối hợp lệ trở nên có lợi hơn cho thợ đào hoặc người điều hành pool.

Phân bố địa lý của chức năng đào cũng rất quan trọng để tránh trường hợp chính phủ, ví dụ, tiếp quản hoặc đóng cửa năng lực đào. Ví dụ, lệnh cấm đào gần đây của Trung Quốc đã cho thấy khả năng thích nghi và tồn tại của Bitcoin trước sự can thiệp của chính phủ, khi mạng lưới đã thích nghi và phục hồi nhanh chóng sau sự sụt giảm sức mạnh băm.

##### Node

Khác với đào, vốn đòi hỏi đầu tư tài chính đáng kể để cạnh tranh hiệu quả trong cuộc đua đào khối mới, hoặc phát triển mã nguồn đòi hỏi chuyên môn lập trình, việc vận hành một node là điều mà bất kỳ ai quan tâm đến việc duy trì sự phi tập trung của Bitcoin đều có thể làm.

Các node chạy phần mềm Bitcoin Core và thực thi các quy tắc mà mã nguồn bao gồm để đảm bảo thợ đào không gian lận, ví dụ như tự cấp cho mình phần thưởng khối lớn hơn mức cho phép. Chúng cũng thực thi giới hạn nguồn cung 21 triệu, điều rất quan trọng để duy trì sự khan hiếm của Bitcoin. Để bất kỳ chính phủ hoặc kẻ xấu nào ngăn chặn Bitcoin, họ sẽ phải phá hủy mọi bản sao của blockchain, hiện đang chạy trên hàng nghìn node phân bố toàn cầu, một nhiệm vụ gần như bất khả thi.

##### Con người

Một khía cạnh khác của nguy cơ tập trung hóa là con người. Mỗi đồng 'alt-coin' khác đều có một người đứng đầu—ai đó có thể bị ép buộc để ủng hộ những thay đổi không có lợi cho Bitcoin. Satoshi Nakamoto đã ở lại đủ lâu để đảm bảo Bitcoin đi đúng hướng thành công trước khi biến mất hoàn toàn, để lại nó trong tay những người khác để phát triển và thích nghi phần mềm.

Vậy còn những người nắm giữ lượng lớn Bitcoin thì sao? Những nhà đầu tư sớm, đã giữ coin của mình và không làm mất chúng, đến thời điểm này sẽ cực kỳ giàu có. Điều quan trọng cần lưu ý là điều này có thể đúng, nhưng điều đó không mang lại cho họ ảnh hưởng lớn hơn đối với hệ thống so với bất kỳ ai khác, không giống như các đồng 'proof of stake' nơi những người tham gia sớm đã giàu có với đồng coin đó sẽ có lợi thế trong việc ra quyết định và phân phối các đồng coin tương lai. Điều này đã hoặc chắc chắn sẽ dẫn đến sự tập trung hóa theo thời gian.

##### Kết luận

Những mối đe dọa tiềm ẩn nào mà sự phi tập trung có thể cố gắng giảm thiểu?

* Chính phủ đóng cửa hoặc cấm Bitcoin
* Những thay đổi không mong muốn đối với mã nguồn có lợi cho một nhóm lợi ích trong Bitcoin, ví dụ như tăng phần thưởng khối
* Sự ép buộc giao thức bởi chính phủ hoặc các tác nhân xấu nhằm ảnh hưởng đến hướng đi của giao thức
* Khả năng một nhóm thợ đào kiểm soát mạng lưới và 'chi tiêu hai lần' Bitcoin – một cuộc tấn công 51%

Như chúng ta có thể thấy, sự kết hợp giữa các node, nhà phát triển mã nguồn và thợ đào, cũng như việc sử dụng cơ chế 'bằng chứng công việc', đã phi tập trung hóa Bitcoin ở mức đủ để những mối đe dọa tiềm ẩn này không còn là mối lo ngại lớn. Cộng đồng sẽ cần tiếp tục theo dõi tình hình để đảm bảo điều này vẫn đúng.
