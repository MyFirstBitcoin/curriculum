# 8.2 Các chỉ số để phân tích sổ cái

Vì tính minh bạch của Bitcoin khác biệt so với các hệ thống tài chính truyền thống — nơi phần lớn dòng tiền diễn ra sau cánh cửa đóng kín của các tổ chức — nên nó tạo ra một lĩnh vực phân tích on-chain phong phú, nơi dữ liệu ở cấp độ mạng lưới trở thành lăng kính để hiểu hành vi người dùng, dòng tiền và các xu hướng dài hạn. Những chỉ số này có thể giúp trả lời các câu hỏi cụ thể, như mức độ hoạt động của mạng lưới, liệu các đồng Bitcoin đang được tích lũy hay bán ra, và liệu mạng lưới có trở nên an toàn hơn hay không.

Việc hiểu các chỉ số này không chỉ hữu ích cho người dùng Bitcoin, mà còn cho các nhà nghiên cứu hoặc nhà hoạch định chính sách muốn tìm hiểu về hệ thống tài chính minh bạch độc đáo này.

Phần này trình bày một số chỉ số thường dùng để phân tích hoạt động của Bitcoin, được nhóm thành các danh mục phụ. Đây không phải là danh sách đầy đủ. Truy cập [www.bitcoinmagazinepro.com/charts](https://www.bitcoinmagazinepro.com/charts) để xem danh sách và mô tả đầy đủ hơn.



#### 8.2.1 Chỉ số Địa chỉ

Các chỉ số về địa chỉ hữu ích để theo dõi theo thời gian vì chúng phản ánh mức độ hoạt động trên mạng lưới Bitcoin. Ví dụ, khi Bitcoin được chấp nhận rộng rãi hơn, số lượng địa chỉ hoạt động sẽ tăng lên. Chúng ta có thể phân tích sâu hơn bằng cách lọc ra số lượng địa chỉ nắm giữ tối thiểu một lượng Bitcoin nhất định, chẳng hạn 0,1 BTC, trong một khoảng thời gian nhất định, ví dụ một năm. Dù điều này cho thấy mức độ chấp nhận Bitcoin theo thời gian, nhưng nó không hoàn hảo vì một cá nhân có thể sở hữu nhiều địa chỉ Bitcoin. Ngược lại, các sàn giao dịch hoặc quỹ ETF có thể xuất hiện như một thực thể duy nhất khi nắm giữ tiền cho nhiều người dùng.

![Bitcoin: Addresses Hodling > X BTC by Year](https://cdn.sanity.io/images/vje9ehw2/staging/b88a9239820e45ed50ce00812170e2bb4d02b5d2-1407x766.png)

_Địa chỉ Hodling Bitcoin > X BTC theo năm. Nguồn: Bitcoin Magazine Pro._

Bằng cách so sánh các địa chỉ với giá thị trường hiện tại của BTC, chúng ta có thể xem tỷ lệ phần trăm tổng số địa chỉ Bitcoin đang có lãi. Điều này cho phép chúng ta theo dõi tâm lý thị trường khi có thể thấy tỷ lệ phần trăm thị trường đang giữ BTC ở trạng thái lãi hoặc lỗ.

Ví dụ, biểu đồ **Tỷ lệ Lợi nhuận Chưa Thực hiện** dưới đây cho thấy tỷ lệ phần trăm tất cả các địa chỉ trên sổ cái có lợi nhuận chưa thực hiện tính theo đô la Mỹ. Lưu ý rằng, vì biểu đồ dưới đây được lấy gần mức đỉnh lịch sử của Bitcoin, nên tỷ lệ địa chỉ có lợi nhuận chưa thực hiện gần như đạt 100%. Chúng ta cũng có thể thấy rằng các giai đoạn kéo dài mà Tỷ lệ Lợi nhuận Chưa Thực hiện thấp hơn một độ lệch chuẩn so với trung bình là hiếm gặp. Do đó, việc giảm xuống dưới đường này có thể gợi ý một điểm vào lệnh tốt cho người mua.

![Percent Unrealised Profit](https://cdn.sanity.io/images/vje9ehw2/staging/f306f03f31ce4faada8bf34137dd76f9d550697a-1041x491.png)

_Tỷ lệ Lợi nhuận Chưa Thực hiện. Nguồn: checkonchain.com_



#### 8.2.2 Chỉ số On-Chain

Các chỉ số on-chain hữu ích vì chúng cung cấp cái nhìn sâu sắc về hành vi mạng lưới, vượt ra ngoài những gì mà chỉ số giá và địa chỉ có thể cho thấy. Chúng giúp các nhà phân tích hiểu được hành động và tâm lý của các nhóm tham gia khác nhau, như những người nắm giữ dài hạn so với nhà giao dịch ngắn hạn, bằng cách theo dõi cách các đồng Bitcoin được giữ, di chuyển hoặc định giá theo thời gian. Những chỉ số này tận dụng tính minh bạch của sổ cái để tiết lộ các động lực thị trường ẩn như tích lũy, phân phối hoặc thậm chí là niềm tin của nhà đầu tư. Điều này khiến chúng đặc biệt hữu ích để nhận diện các xu hướng cấu trúc, đánh giá thị trường đang quá nóng hay bị định giá thấp, và dự đoán các điểm đảo chiều trong chu kỳ thị trường.

Ví dụ, bằng cách xem xét giá trị nắm giữ BTC kể từ lần giao dịch cuối cùng, chúng ta có thể suy ra liệu thị trường có đang gặp khó khăn hay không (như trong giai đoạn đáy của một chu kỳ lớn). Chỉ số này được gọi là **Giá Đã Thực hiện** và cho chúng ta biết 'giá vốn trung bình' của tất cả BTC đang lưu thông. Nếu giá thị trường giảm xuống dưới Giá Đã Thực hiện, điều này cho thấy phần lớn các địa chỉ đang chịu lỗ trên giấy tờ.

Bằng cách nhóm thêm dữ liệu sổ cái thành các dải tuổi, chúng ta có thể thấy lượng BTC di chuyển giữa các địa chỉ theo thời gian, tạo thành các mô hình dạng sóng trên biểu đồ được gọi là **sóng HODL**.

![Bitcoin HODL Waves](https://cdn.sanity.io/images/vje9ehw2/staging/ce108e45a1a7217e081101e4a276ee2d9e95a22e-1129x577.png)

_Sóng HODL của Bitcoin. Nguồn: Bitcoin Magazine Pro._

Sóng HODL cho thấy những người nắm giữ BTC dài hạn, trung hạn và ngắn hạn đang làm gì với số BTC của họ. Ví dụ, trên biểu đồ trên, những người nắm giữ ngắn hạn được thể hiện bằng màu đỏ và cam, và chúng ta có thể thấy các đợt tăng đột biến hoạt động khi nhóm này đổ xô mua gần đỉnh thị trường. Ở phía ngược lại, chúng ta thấy những người nắm giữ rất dài hạn (màu tím và xanh dương) đang tăng dần tỷ trọng trên mạng lưới, cho thấy niềm tin mạnh mẽ của các nhóm này. Biểu đồ này không hoàn hảo vì một số đồng có thể di chuyển từ địa chỉ cũ sang địa chỉ mới nhưng vẫn do cùng một người kiểm soát. Tuy nhiên, nó vẫn cung cấp một góc nhìn thú vị về niềm tin của những người nắm giữ dài hạn.

Một cách khác để xem xét 'dòng tiền thông minh' của những người nắm giữ dài hạn là phân tích **Coin Days Destroyed** (CDD). Khái niệm 'Coin Days' là tích số giữa số lượng BTC và số ngày kể từ lần di chuyển cuối cùng của các đồng đó. Ví dụ, 5 BTC không di chuyển trong 100 ngày sẽ tích lũy được 500 coin days và 10 BTC không di chuyển trong 10 ngày sẽ tích lũy được 100 coin days. Bằng cách này, chúng ta ưu tiên cho các đồng được giữ lâu hơn. Khi các đồng đó được di chuyển, số coin days đó bị 'tiêu hủy'. Chỉ số này cho thấy sự gia tăng CDD vào những thời điểm có biến động giá lớn, giúp các nhà phân tích phân biệt hoạt động thị trường thường nhật với những thay đổi có ý nghĩa trong tâm lý của người nắm giữ dài hạn.

Một chỉ số khác có thể giúp xác định liệu thị trường đang định giá thấp hay cao BTC là tỷ lệ Giá trị Thị trường trên Giá trị Đã Thực hiện, hay còn gọi là **MVRV**. Nó được tính đơn giản bằng tỷ số giữa Giá trị Thị trường (số lượng BTC phát hành nhân với giá thị trường) chia cho Giá trị Đã Thực hiện (tổng giá trị của tất cả BTC kể từ lần di chuyển cuối cùng). MVRV cao cho thấy nhiều đồng đang có lãi (thường thấy gần đỉnh thị trường) và MVRV thấp cho thấy nhiều đồng đang bị lỗ (thường thấy gần đáy thị trường).



#### 8.2.3 Chỉ số Khai thác

Các chỉ số khai thác hữu ích để hiểu về mức độ an toàn, động lực kinh tế và sức khỏe tổng thể của mạng lưới Bitcoin. Các chỉ số như hashrate, doanh thu thợ đào, độ khó và tỷ lệ phí cho thấy lượng sức mạnh tính toán đang bảo vệ blockchain và mức độ thợ đào được trả công cho hoạt động của họ.

**Hashrate** của mạng lưới Bitcoin có lẽ là chỉ số thường được nhắc đến nhất về sức khỏe mạng lưới và mức độ an toàn. Vì quá trình khai thác bảo vệ mạng lưới và xác nhận các giao dịch trên sổ cái là hợp lệ, nên càng có nhiều sức mạnh tính toán (hoặc hashing), thì càng khó để một tác nhân xấu áp đảo và tấn công mạng lưới.

![Bitcoin Hashrate](https://cdn.sanity.io/images/vje9ehw2/staging/fcb4a24c431a37580d3d6c4ec62b664e7e41c362-1134x584.png)

_Hashrate của Bitcoin. Nguồn: Bitcoin Magazine Pro._

Biểu đồ trên cho thấy, vào tháng 5 năm 2025, tổng sức mạnh tính toán của mạng lưới đạt khoảng 900 TeraHash/s (900 nghìn tỷ phép tính 'hash' mật mã mỗi giây). Nếu hashrate tăng, điều đó cho thấy mạng lưới đang trở nên an toàn hơn, điều này mang lại sự yên tâm cho người dùng.

Chỉ số Puell Multiple (do David Puell phát triển) xem xét chu kỳ thị trường từ góc nhìn của thợ đào và doanh thu của họ. Chỉ số này được tính bằng cách lấy lượng BTC phát hành hàng ngày (tính theo USD) chia cho giá trị phát hành trung bình 365 ngày. Chỉ số này giúp xác định các giai đoạn thợ đào gặp áp lực hoặc được giải tỏa. Lịch sử cho thấy, khi chỉ số này trên 3 thì thường báo hiệu giá trị thị trường của BTC sẽ giảm, vì điều đó cho thấy thợ đào đang rất có lãi. Giá trị dưới 0,5 cho thấy áp lực và thường báo hiệu đáy thị trường cho giá trị của BTC.
