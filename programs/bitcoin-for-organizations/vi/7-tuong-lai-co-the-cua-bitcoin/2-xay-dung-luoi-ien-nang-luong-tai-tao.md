# 7.2 Xây dựng lưới điện năng lượng tái tạo

#### 7.2.0: Giới thiệu

Bitcoin dựa vào năng lượng cho cơ chế đồng thuận ‘bằng chứng công việc’, giúp đảm bảo nó luôn là một loại tiền tệ phi tập trung, không cần sự cho phép. Lưới điện hiện đang đối mặt với những thách thức khi tích hợp các nguồn năng lượng tái tạo mới, gây áp lực lên hạ tầng hiện tại. Chương này cung cấp phần giới thiệu ngắn gọn về những thách thức này và tổng quan về các khía cạnh liên quan của Bitcoin trước khi trình bày cách nó đang hỗ trợ quá trình chuyển đổi sang lưới điện năng lượng tái tạo.


> **Info – Bitcoin như một loại tiền tệ năng lượng**
>
> Vào ngày 4 tháng 12 năm 1921, tờ New York Tribune đã đăng một bài báo trình bày tầm nhìn của Ford về việc thay thế vàng bằng một loại tiền tệ năng lượng mà ông tin rằng có thể phá vỡ sự kiểm soát của giới tinh hoa ngân hàng đối với tài sản toàn cầu và chấm dứt chiến tranh. Ông dự định thực hiện điều này bằng cách xây dựng “nhà máy điện lớn nhất thế giới” và tạo ra một hệ thống tiền tệ mới dựa trên “đơn vị năng lượng”.


Như Henry Ford đã hình dung, Bitcoin sử dụng năng lượng để tạo ra và bảo vệ tiền tệ một cách độc lập với bất kỳ lợi ích nào từ chính phủ hay doanh nghiệp. Điều này khiến nó trở thành loại tiền tệ toàn cầu thực sự phi tập trung đầu tiên mà thế giới từng chứng kiến. Quá trình khai thác Bitcoin – thuật ngữ chỉ quá trình tạo và thêm các khối mới vào mạng lưới – diễn ra rất cạnh tranh và thúc đẩy cộng đồng khai thác Bitcoin tìm kiếm các nguồn năng lượng giá rẻ. Nó cũng rất linh hoạt khi có thể tăng giảm nhanh chóng lượng năng lượng sử dụng trong các môi trường cụ thể. Đặc điểm này có thể mang lại lợi ích lớn cho lưới điện sử dụng các nguồn năng lượng tái tạo.

##### Tầm quan trọng của phát triển Lưới điện Năng lượng Tái tạo

Việc chuyển sang các nguồn năng lượng tái tạo tạo ra một loạt thách thức mới cho các nhà vận hành lưới điện, như tính gián đoạn và phân tán của các nguồn năng lượng, tắc nghẽn truyền tải và hạn chế hiện tại về lưu trữ năng lượng. Điều này làm tăng mức độ phức tạp cho vận hành lưới điện mà trước đây không có khi chỉ sử dụng các nguồn năng lượng tập trung và ổn định. Để đối phó, các nhà vận hành lưới điện sẽ cần nghiên cứu các công nghệ lưới điện thông minh và công nghệ dự báo dựa trên AI để nâng cao hiệu quả. Một lựa chọn đang được sử dụng hiện nay là các chương trình đáp ứng nhu cầu, yêu cầu một nguồn năng lượng có thể thích ứng linh hoạt gần như theo thời gian thực để giúp cân bằng cung cầu năng lượng. Đây chính là nơi khai thác Bitcoin có thể hỗ trợ.



#### 7.2.1 Những thách thức của việc tích hợp năng lượng tái tạo

Các nhà vận hành lưới điện phải liên tục cân bằng cung và cầu điện năng. Nếu nhu cầu điện quá cao, lưới điện có thể bị quá tải, dẫn đến mất điện luân phiên hoặc thậm chí mất điện diện rộng.

Nếu quá nhiều năng lượng được đưa vào lưới cũng có thể gây ra các vấn đề như tăng nhiệt và làm hỏng hạ tầng. Trong những trường hợp nghiêm trọng, điều này có thể kích hoạt hệ thống tự động ngắt an toàn, gây ra phản ứng dây chuyền trên toàn lưới và dẫn đến mất điện cục bộ hoặc diện rộng. Mất điện là sự kiện thảm khốc khiến các doanh nghiệp thiệt hại hàng tỷ euro. Nó cũng gây thiệt hại về người.

##### Tình trạng hạ tầng hiện tại

Hạ tầng lưới điện ngày nay được tối ưu hóa cho các nguồn năng lượng truyền thống như nhiên liệu hóa thạch, ví dụ như than đá, khí đốt hoặc hạt nhân, có thể cung cấp dòng năng lượng ổn định, tập trung và kiểm soát để đáp ứng nhu cầu. Điều này khiến việc cân bằng cung cầu trở nên khá đơn giản. Khi năng lượng tái tạo được đưa vào, lưới điện phải quản lý nhiều loại năng lượng phân tán khác nhau, tất cả đều có hành vi rất khác so với các nguồn năng lượng mà lưới điện được thiết kế ban đầu. Các nguồn tái tạo như gió và mặt trời tạo ra điện không liên tục. Ví dụ, trong thời gian không có gió, một trang trại gió có thể không sản xuất được điện, trong khi khi gió mạnh, các tuabin có thể đưa lượng điện dư thừa vào lưới. Hệ thống lưới điện hiện tại chưa được trang bị để xử lý hiệu quả những biến động này.

##### Đáp ứng nhu cầu

Có một vài cách tiếp cận tiềm năng mà nhà vận hành lưới điện có thể áp dụng để đối phó với biến động cung cầu:

* Xây dựng thêm các nhà máy điện truyền thống (dựa trên nhiên liệu hóa thạch) có thể duy trì ở chế độ chờ với chi phí nhất định. Khi nhu cầu tăng đột biến, các nhà máy này có thể được đưa vào hoạt động để cung cấp thêm năng lượng cần thiết.
* Xây dựng dư thừa các nguồn năng lượng tái tạo và sau đó áp dụng các kế hoạch cắt giảm để ngăn các nguồn này làm quá tải lưới điện vào những thời điểm sản xuất điện cao mà không có nhu cầu tương ứng.

Phương án khác là cố gắng giảm nhu cầu vào các thời điểm sử dụng cao điểm**.** Tuy nhiên, trước khi có khai thác Bitcoin, các nhà vận hành lưới điện chưa từng tìm ra cách giảm nhu cầu một cách đáng tin cậy, nhanh chóng và có thể mở rộng, buộc họ phải đầu tư vào các nhà máy dự phòng hoặc trả tiền cho các nguồn tái tạo để ngừng hoạt động – cả hai đều rất tốn kém.

##### Năng lượng bị mắc kẹt

Các thách thức khi kết nối các trang trại gió vào lưới điện thường bao gồm nhiều bước: nghiên cứu khả năng tiếp cận, phân tích tác động chi tiết, lập kế hoạch triển khai và ký thỏa thuận kết nối. Quá trình này có thể kéo dài nhiều năm. Ví dụ, sơ đồ dưới đây cho thấy tổng công suất trang trại gió đang chờ đánh giá kết nối lưới điện vào giữa năm 2024.

![Total wind energy on the waiting list for grid connection assessment](https://cdn.sanity.io/images/vje9ehw2/staging/47c8e509b367a51a036409fe4fd0b7c845ae550a-1694x1410.png)

_Tổng công suất năng lượng gió đang chờ đánh giá kết nối lưới điện (Nguồn: windeurope.org)_

##### Kết nối lưới điện

Sau khi các nguồn năng lượng tái tạo được xây dựng, thường có sự chậm trễ trong việc kết nối do thiếu công suất trên lưới. Điều này dẫn đến công suất bị bỏ không cho đến khi kết nối được thực hiện, trong thời gian đó năng lượng tiềm năng tạo ra có thể được sử dụng để vận hành các máy đào bitcoin và tạo ra thu nhập.

##### Sản xuất dư thừa và cắt giảm

Khi công suất này đã được bổ sung vào lưới, vấn đề chuyển sang cắt giảm. Khi gió tạo ra nhiều công suất hơn mức cần thiết tại một thời điểm, hiện chưa có công nghệ nào lưu trữ được lượng điện này, nên công suất đó bị lãng phí. Để giảm rủi ro cho việc xây dựng các trang trại gió, các nhà vận hành được đảm bảo giá cho bất kỳ lượng điện nào tạo ra, và để tránh quá tải lưới, họ được trả tiền để tắt các tuabin gió. Ví dụ, người tiêu dùng tại Anh đã phải trả 1 tỷ euro vào năm 2024 để ‘cắt giảm’ 6,6 GWh công suất.

Một cách tiếp cận khác đối với việc cắt giảm là sử dụng các nhà máy điện khí đỉnh. Đây là các nhà máy sử dụng khí tự nhiên để phát điện vào các thời điểm nhu cầu cao. Chúng cũng được dùng để cân bằng lưới điện bằng cách phát điện khi nhu cầu cao hoặc nguồn cung thấp. Đúng như tên gọi, chúng thường chỉ được sử dụng vào thời điểm nhu cầu đỉnh, nhưng phải được lắp đặt và bảo trì liên tục, nên phần lớn thời gian chúng ở chế độ chờ, tức là cũng bị ‘cắt giảm’. Khi nhu cầu tăng cao, nhà vận hành lưới điện có thể sử dụng chúng để tăng nguồn cung. Ví dụ, việc triển khai khai thác Bitcoin thay vì mua và vận hành các nhà máy điện khí đỉnh được ước tính đã giúp Texas tiết kiệm 18 tỷ euro.

##### Hiện đại hóa lưới điện

Các lưới điện thông minh đang được xây dựng để quản lý sự pha trộn ngày càng đa dạng của các nguồn năng lượng, tích hợp liền mạch cả nhiên liệu hóa thạch truyền thống và các phương pháp tái tạo hiện đại vào một mạng lưới duy nhất, hiệu quả. Bằng cách tận dụng các công nghệ tiên tiến như lưu trữ pin, lưới điện thông minh có thể lưu trữ năng lượng dư thừa và giải phóng khi cần thiết, cho phép xử lý các biến động và tính gián đoạn của năng lượng tái tạo như các đợt sản xuất cao và thiếu hụt trong các giai đoạn sản xuất thấp. Tại thời điểm viết, công nghệ này vẫn đang ở giai đoạn phát triển ban đầu.

##### Tiến bộ công nghệ

Giám sát và phân tích là chìa khóa để triển khai lưới điện thông minh trên quy mô lớn. Điều này bắt đầu bằng việc lắp đặt các cảm biến và công nghệ giám sát tại chỗ ở nhà máy nơi năng lượng được tạo ra. Phần mềm phân tích sau đó sẽ phân tích và dự đoán xu hướng dựa trên dữ liệu thu thập được, đưa ra cảnh báo về các vấn đề sức khỏe của nhà máy như nguy cơ ngừng hoạt động hoặc hỏng hóc để chuẩn bị cho lưới điện thông minh đối phó với các tình huống này. Đồng hồ thông minh là điểm cuối để thu thập dữ liệu, giám sát việc sử dụng năng lượng của người tiêu dùng tại nguồn. Việc ứng dụng AI được kỳ vọng sẽ giúp quản lý sự phức tạp này, do đó các nhà vận hành lưới điện sẽ cần nâng cao kỹ năng trong lĩnh vực này.

##### Tóm tắt

Việc các chính phủ đẩy mạnh triển khai năng lượng tái tạo quy mô lớn vào lưới điện đang gây áp lực lên thiết kế lưới hiện tại và đòi hỏi đầu tư lớn để thích ứng với tính phân tán và động của các nguồn năng lượng tái tạo. Thiết kế hiện tại gây lãng phí năng lượng lớn, làm tăng chi phí cho doanh nghiệp và người tiêu dùng. Nhiều công nghệ cần thiết để thành công vẫn đang được phát triển tại thời điểm này. Một giải pháp tốt hơn là cần thiết.



#### 7.2.2 Giới thiệu về khai thác Bitcoin

##### Khai thác Bitcoin là gì?

Khai thác Bitcoin là quá trình tạo ra các đơn vị bitcoin mới và xác minh các giao dịch mới. Quá trình này bao gồm một mạng lưới các máy tính trên toàn thế giới xác minh và bảo mật blockchain – một sổ cái ảo ghi lại tất cả các giao dịch và giải quyết vấn đề ‘chi tiêu kép’ khi cùng một số tiền có thể bị chi tiêu hai lần.

Các máy đào Bitcoin là những máy tính sử dụng ASIC chuyên dụng (mạch tích hợp dành riêng cho ứng dụng) để tạo ra các khối tiềm năng mới và có cơ hội thêm một khối mới vào sổ cái bằng cách tạo ra một giải pháp mật mã đáp ứng tiêu chí nhất định. Càng nhiều máy đào hoạt động trong mạng lưới, việc tìm ra giải pháp này càng khó, và độ khó này được điều chỉnh động bởi một phần của giao thức gọi là điều chỉnh độ khó. Phần thưởng cho việc thêm một khối mới là nhận được các đồng coin mới cũng như phí giao dịch trong khối cho máy đào thành công.

Cuộc đua tạo ra khối tiếp theo và giành phần thưởng đã tạo nên một mạng lưới máy đào phi tập trung rộng lớn, luôn tìm kiếm nguồn năng lượng giá rẻ để cạnh tranh, và tạo ra một động lực thú vị trong cuộc đua bổ sung năng lượng tái tạo vào lưới điện.

##### Tranh cãi về tiêu thụ năng lượng

Như đã đề cập ở phần giới thiệu, khai thác Bitcoin gắn liền với việc sử dụng năng lượng thực tế. Việc sử dụng năng lượng này đã được nhắc đến trên các phương tiện truyền thông trong nhiều năm. Nó thường bị chỉ trích là tiêu tốn quá nhiều năng lượng, không sử dụng năng lượng hiệu quả, hoặc trong một số trường hợp cực đoan, bị coi là thảm họa về khí hậu/năng lượng. Tuy nhiên, mạng lưới Bitcoin về cơ bản chỉ chiếm một phần rất nhỏ trong tổng tiêu thụ năng lượng toàn cầu, dù thành công hay không, và mức tiêu thụ năng lượng của nó sẽ không vượt quá giá trị sử dụng lâu dài của nó (dù giá trị đó cao hay thấp). Như chúng ta sẽ thấy, các đặc điểm cụ thể của việc sử dụng năng lượng này có thể hỗ trợ việc áp dụng năng lượng tái tạo.

##### Tính linh hoạt về địa lý của hoạt động khai thác

> Một tác động ngoại lai thú vị của các đồng tiền PoW – chúng luôn sẵn sàng mua năng lượng ở mức 3-5 cent/kWh. Và một số tài sản năng lượng tốt nhất lại nằm ngoài lưới điện. Mạng lưới năng lượng toàn cầu này giải phóng các tài sản bị mắc kẹt và làm cho các tài sản mới trở nên khả thi. Hãy tưởng tượng một bản đồ địa hình 3D của thế giới với các điểm năng lượng rẻ là vùng trũng và năng lượng đắt là vùng cao. Tôi hình dung việc khai thác Bitcoin giống như một ly nước đổ lên bề mặt, nước sẽ chảy vào các ngóc ngách, làm phẳng bề mặt đó.  
_Nic Carter_

Tại bất kỳ thời điểm nào, các máy đào Bitcoin trên khắp thế giới đều đang tìm cách tạo ra khối tiếp theo, và vì chi phí lớn nhất đối với thợ đào là tiền điện, điều này tạo ra một cuộc cạnh tranh để các thợ đào tìm kiếm và tận dụng nguồn năng lượng rẻ nhất ở bất cứ đâu. Mọi người thường tưởng tượng rằng các thợ đào Bitcoin cạnh tranh với các ngành công nghiệp khác để lấy điện, như thể việc đào Bitcoin phải đẩy lùi các mục đích sử dụng điện khác để hoạt động. Tuy nhiên, vì các thợ đào Bitcoin vốn dĩ chỉ có thể sử dụng nguồn điện cực kỳ rẻ, họ _không thể_ cạnh tranh bình thường với người dùng điện thông thường. Do đó, các thợ đào Bitcoin tìm kiếm những nơi trên thế giới có sự lãng phí hoặc sử dụng điện chưa hiệu quả. Điều này đã được Nic Carter mô tả rất rõ vào năm 2018.

##### Tính linh hoạt về nhu cầu của các hoạt động đào

> Các thợ đào Bitcoin là những người mua năng lượng độc đáo vì họ có thể điều chỉnh nhu cầu linh hoạt và dễ dàng ngắt tải, thanh toán bằng tiền mã hóa có tính thanh khoản toàn cầu, và hoàn toàn không phụ thuộc vào vị trí địa lý, chỉ cần có kết nối Internet. Những đặc điểm kết hợp này tạo nên một tài sản phi thường: một người mua năng lượng cuối cùng có thể bật hoặc tắt ngay lập tức ở bất cứ đâu trên thế giới.  
_Jack Dorsey_

Bên cạnh sự linh hoạt về địa lý, các thợ đào Bitcoin còn có thể cung cấp sự linh hoạt về nhu cầu. Đào Bitcoin giúp việc xây dựng dư thừa các nguồn năng lượng tái tạo trở nên có lợi nhuận, vì nó cho phép nguồn cung dư thừa đó được tận dụng để kiếm tiền. Mọi cộng đồng muốn có nguồn điện ổn định đều cần xây dựng công suất điện dư thừa, và đối với gió, mặt trời, thủy điện thì điều này càng quan trọng hơn vì chúng biến động. Tuy nhiên, việc xây dựng dư thừa thường không hiệu quả về chi phí, trừ khi bạn có thể sử dụng nó cho một mục đích có lợi nhuận và hữu ích khi không cần thiết cho nhu cầu khác. Các thợ đào Bitcoin là giải pháp độc đáo cho vấn đề này, có thể biến việc xây dựng dư thừa thành lợi nhuận, và do đó đóng vai trò gián tiếp như một giải pháp lưu trữ năng lượng.

Trong phần lớn thời gian khi nguồn cung vượt quá nhu cầu, các thợ đào Bitcoin là một trong những người tiêu thụ điện trong cộng đồng, có thể vận hành máy móc, kiếm doanh thu và trả chi phí điện. Nếu có sự tăng đột biến về nhu cầu điện hoặc giảm nguồn cung có thể gây ra mất điện cục bộ, các thợ đào này có thể tạm thời tắt máy.

Một hợp đồng thương mại với mức giá điện được cấu trúc tốt có thể giúp quá trình này diễn ra suôn sẻ. Công ty điện lực có thể cung cấp cho thợ đào mức giá thấp nhất trong khu vực, đổi lại họ phải chấp nhận sự biến động và các điều khoản linh hoạt khác trong hợp đồng.

Tóm lại, các thợ đào Bitcoin là duy nhất ở chỗ:

* Hầu như toàn bộ chi phí vận hành của họ là tiền điện
* Họ có thể chấp nhận việc tiêu thụ điện không liên tục
* Họ linh hoạt về vị trí, nên có thể tránh được chi phí truyền tải đắt đỏ bằng cách đặt máy ngay cạnh nguồn điện.

Do đó, họ có thể hy sinh những yếu tố mà hầu hết các công ty khác không thể, để đổi lấy giá điện cực thấp khi điện dư thừa. Điều này có nghĩa là với việc đào Bitcoin, chúng ta giờ đây có người mua cho mọi watt điện được sản xuất, ở bất cứ đâu trên thế giới, 24/7.



#### 7.2.3 Các nghiên cứu tình huống

Về mặt lý thuyết, chúng ta có thể thấy rằng việc đào Bitcoin có thể đóng vai trò lớn trong việc thúc đẩy áp dụng năng lượng tái tạo. Hãy cùng xem một số ví dụ triển khai thực tế hiện nay.

##### Thủy điện bị bỏ phí

Các nhà máy thủy điện sản xuất điện liên tục, có thể dao động theo mùa và vị trí địa lý. Điều này thường dẫn đến việc lãng phí điện vào ban đêm khi mọi người ngủ, hoặc khi sản lượng tăng cao vào mùa mưa, như ở Trung Quốc. Vì các thợ đào Bitcoin có thể di chuyển đến nơi có nguồn điện, họ từng đổ về Tứ Xuyên vào mùa mưa để tận dụng nguồn năng lượng bị lãng phí này. Họ làm vậy không phải vì là những nhà môi trường vị tha, mà đơn giản vì điện rẻ và không ai khác sử dụng. Khi Trung Quốc cấm đào Bitcoin, họ chỉ đơn giản là thu dọn và rời đi.

Các thị trấn hoặc làng mạc xa xôi gần nguồn thủy điện tiềm năng thường không đủ khả năng đầu tư xây dựng hạ tầng truyền tải điện. Trong trường hợp này, các thợ đào Bitcoin có thể huy động vốn để xây dựng nhà máy, cung cấp điện giá rẻ cho người dân địa phương và sử dụng phần điện dư để vận hành máy đào. Một lần nữa, điều này không phải vì lòng vị tha, mà vì lợi nhuận; một giải pháp đôi bên cùng có lợi cho thợ đào và cộng đồng địa phương.

##### Đào Bitcoin để ổn định lưới điện

Lưới điện phải bù đắp cho hai yếu tố: sự thay đổi nguồn cung và sự thay đổi nhu cầu. Một số nguồn điện rất ổn định, như điện hạt nhân nền, có thể hoạt động 24/7. Các nguồn khác như gió, mặt trời và phần nào đó là thủy điện, lại biến động tùy vào thời tiết. Do sự biến động này, nguồn cung điện cần được xây dựng dư thừa để ngay cả vào những ngày sản xuất thấp vẫn đủ cung cấp cho cộng đồng. Ở Texas, kế hoạch mặc định là xây dựng các nhà máy điện hóa thạch dự phòng để sẵn sàng đáp ứng khi nhu cầu tăng. Phương án thay thế được áp dụng là tăng tính linh hoạt về nhu cầu bằng cách tích hợp các thợ đào Bitcoin vào mạng lưới. Cách tiếp cận này đã giúp người dân Texas tiết kiệm hàng triệu euro đầu tư và mang lại giải pháp thân thiện với môi trường hơn.

##### Các lợi ích liên quan khác

Mặc dù không liên quan trực tiếp đến hạ tầng lưới điện tái tạo, nhưng còn có các giải pháp liên quan đến năng lượng mà đào Bitcoin có thể mang lại:

* Khí đốt bị đốt bỏ: tránh việc khí đốt bị xả hoặc đốt bỏ ra môi trường bằng cách sử dụng nó cho đào Bitcoin tại chỗ.
* Khí bãi rác: thu giữ khí mê-tan tại các bãi rác và sử dụng để phát điện, giảm phát thải khí nhà kính độc hại
* Thúc đẩy công nghệ mới: Chuyển hóa năng lượng nhiệt đại dương (OTEC) là một phương pháp nổi tiếng để khai thác sự chênh lệch nhiệt độ giữa mặt nước và tầng sâu để phát điện. Trước đây điều này chưa từng khả thi về mặt thương mại cho đến khi có Bitcoin.
* Khởi động phát triển điện tại các quốc gia mới nổi: Như đã đề cập trước đó, các thợ đào Bitcoin có thể là 'khách thuê mỏ neo' luôn sử dụng điện được tạo ra, giúp hợp lý hóa đầu tư ban đầu và sau đó rút đi khi cộng đồng địa phương phát triển và tìm được mục đích sử dụng điện tốt hơn.

##### Tóm tắt

Đào Bitcoin có thể hỗ trợ đầu tư và sự bền vững của hạ tầng năng lượng tái tạo:

* Hấp thụ năng lượng dư thừa trong các giai đoạn nhu cầu thấp
* Ổn định lưới điện bằng cách cân bằng cung và cầu
* Tạo nguồn thu cho các nhà phát triển năng lượng tái tạo
* Tài trợ cho các dự án năng lượng ở vùng sâu vùng xa hoặc chưa được phục vụ
* Thúc đẩy giới hạn hiệu quả năng lượng
* Đóng vai trò là người mua cuối cùng cho nguồn năng lượng bị lãng phí ở bất cứ đâu, bất cứ lúc nào trên thế giới



#### 7.2.4 Giải quyết các mối quan ngại

Chúng ta đã thấy việc đào Bitcoin có thể giúp phát triển năng lượng tái tạo như thế nào, nhưng những rào cản nào đang tồn tại?

##### Tác động môi trường và những hiểu lầm

Để Bitcoin có thể được tích hợp thành công vào một lĩnh vực quan trọng như lưới điện, mọi lo ngại về tác động môi trường và những hiểu lầm như việc sử dụng năng lượng cần được giải quyết. Các tổ chức như Bitcoinpolicy.uk đang nỗ lực giải quyết những lo ngại này với các ngành công nghiệp và cơ quan chức năng liên quan, nhưng đây thường là một cuộc chiến khó khăn. Việc giúp thị trường hiểu rõ các lợi ích tiềm năng trong việc kiếm tiền từ năng lượng bị bỏ phí hoặc tận dụng năng lượng dư thừa là rất quan trọng để áp dụng thành công.

##### Quy định và ưu đãi cho đào thân thiện với môi trường

Các quốc gia có thể có cách tiếp cận rất khác nhau đối với việc áp dụng đào Bitcoin, từ các quốc gia như Bhutan đào Bitcoin trực tiếp, đến các bang của Mỹ như Texas cho phép đào mà không ngăn cản, đến Trung Quốc đã ban hành lệnh cấm hoàn toàn việc đào.

Các quốc gia khác như Vương quốc Anh có thể đang trả số tiền lớn cho các nhà vận hành điện gió để tắt máy khi gió mạnh. Do đó, động lực tích hợp đào Bitcoin trong trường hợp này là rất hạn chế, dù nó có thể thay đổi mô hình kinh doanh từ việc gây tốn kém cho người tiêu dùng sang tạo ra lợi nhuận giúp giảm hóa đơn.

##### Rào cản pháp lý gián tiếp

Có thể tồn tại các rào cản pháp lý gián tiếp không đề cập trực tiếp đến Bitcoin nhưng vẫn có tác động. Ví dụ, hạ tầng cần xây dựng cho các trang trại điện gió ngoài khơi để kết nối với lưới điện có thể bị hạn chế không được chia sẻ với hạ tầng trung tâm dữ liệu cần thiết cho đào Bitcoin.



#### 7.2.5 Kết luận và kêu gọi hành động

* Bitcoin cung cấp một dịch vụ mà mọi người có thể sử dụng để lưu trữ và chuyển giá trị. Cho đến nay, thị trường với hàng triệu người tham gia đã quyết định rằng mạng lưới này có giá trị, và như bất cứ thứ gì có giá trị, nó tiêu thụ năng lượng.
* Đào Bitcoin sử dụng chưa đến 0,1% tổng năng lượng toàn cầu, và những lo ngại về việc sử dụng năng lượng lãng phí đã được giải quyết đầy đủ trên thị trường.
* Một phần lớn năng lượng được sử dụng cho đào Bitcoin thực chất là năng lượng bị bỏ phí và không thể sử dụng vào mục đích khác. Điều này là do các thợ đào Bitcoin có khả năng độc đáo là di chuyển đến những nơi xa xôi và xử lý nguồn điện không ổn định mà người tiêu dùng khác không thể tận dụng.
* Bitcoin có thể giúp ổn định lưới điện, đóng vai trò là khách thuê mỏ neo bằng cách là người đầu tiên sử dụng và trả tiền cho điện cho đến khi có thể kết nối với lưới điện và sử dụng cho mục đích khác, đồng thời cung cấp phản ứng nhu cầu bằng cách tắt máy nhanh chóng trong các giai đoạn nhu cầu cao.

Thị trường Bitcoin và năng lượng đang hội tụ, và quyền sở hữu tài sản cũng có khả năng hội tụ. Cũng có sự giao thoa tiềm năng với AI, vốn đòi hỏi kỹ năng và hạ tầng tương tự như Bitcoin và sẽ được sử dụng để quản lý lưới điện thông minh. Các công ty định hướng phát triển sản phẩm phù hợp với các xu hướng này sẽ có vị thế tốt nhất để hưởng lợi từ những phát triển này.



###### Phụ lục - Tài liệu tham khảo

1. [https://www.btcpolicy.org](https://www.btcpolicy.org/)
1. [https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion](https://www.da-ri.org/articles/how-bitcoin-mining-saved-texans-18-billion)
1. [https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/](https://gript.ie/uks-hidden-1billion-cost-of-wind-energy/)
1. [https://www.lynalden.com/bitcoin-energy/#electricity](https://www.lynalden.com/bitcoin-energy/#electricity)
1. [https://squareup.com/gb/en/press/bcei-white-paper](https://squareup.com/gb/en/press/bcei-white-paper)
1. [https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities](https://www.mara.com/posts/bitcoin-mining-the-environment-the-positive-externalities)
