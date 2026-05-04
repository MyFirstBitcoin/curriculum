# 3.4 Hashcash

Hashcash được tạo ra bởi Adam Back, một trong những nhà đổi mới tiên phong trong lĩnh vực này. Adam rất quan tâm đến thị trường tự do và quyền riêng tư trên internet, và đã tình cờ biết đến danh sách thư Cypherpunks, nơi anh tham gia và trở thành một thành viên tích cực.

Anh rất quan tâm đến tiền kỹ thuật số, và đã đưa ra một số đề xuất về cách nhóm có thể hợp tác chặt chẽ hơn với Chaum về DigiCash, nhưng những ý tưởng này không đi đến đâu. Sau đó, anh chuyển sự chú ý sang một vấn đề mới nổi khác – thư rác email. Anh và các thành viên Cypherpunks khác muốn tìm ra giải pháp cho vấn đề thư rác, nơi mà những kẻ gửi thư rác có thể dễ dàng tạo và gửi hàng ngàn email làm tắc nghẽn mạng lưới. Giải pháp sáng tạo của anh dựa trên hashing – khả năng của mật mã học để biến bất kỳ dữ liệu nào thành một chuỗi ký tự ngẫu nhiên và duy nhất với độ dài xác định, nhằm tạo ra một loại 'tem' kỹ thuật số cần được thêm vào email để nó được coi là hợp lệ và truyền qua mạng lưới. Một chi phí nhỏ đối với email thật, nhưng lại là rào cản lớn đối với kẻ gửi thư rác.

Điểm đổi mới quan trọng mà Hashcash mang lại là gắn tài nguyên thực – sức mạnh tính toán – vào một mạng lưới kỹ thuật số. Trong khi các tài nguyên kỹ thuật số trước đó có thể được sao chép không giới hạn, số lượng 'hashcash' được tạo ra bị giới hạn bởi mức năng lượng mà mọi người sẵn sàng đầu tư vào nó.

Mặc dù giải pháp này đáp ứng một số tiêu chí mà Adam tin rằng cần có trong một hệ thống tiền kỹ thuật số; nó ẩn danh, bền vững và không cần tin tưởng, mỗi hashcash lại không thể tái sử dụng và không thực sự khan hiếm. Anh đã đề xuất những cách khác để giải quyết các vấn đề này bằng cách sử dụng các bên thứ ba bên ngoài.

##### BitGold

Nick Szabo đã phát triển dựa trên ý tưởng của Hashcash và bằng chứng công việc để đề xuất một giải pháp thay thế, mà anh mô tả trên một danh sách thư một năm sau khi Hashcash được công bố, vào năm 1998.

Mặc dù đã tiến gần hơn đến một giải pháp, đề xuất này vẫn còn một số thách thức.

* Ai sẽ vận hành Sổ đăng ký quyền sở hữu hash và làm sao có thể tin tưởng họ?
* Việc hashing nhìn chung sẽ ngày càng rẻ hơn theo thời gian, đây cũng là một thách thức đối với HashCash.

Vì các hash được liên kết sẽ được đóng dấu thời gian, anh đề xuất một hình thức theo dõi lịch sử độ khó của hashing tại thời điểm đó; một hash được tạo sớm sẽ đòi hỏi chi phí xử lý cao hơn so với hash được tạo sau này khi chi phí đã giảm xuống. Đáng tiếc, điều này có nghĩa là các hash sẽ không 'có thể thay thế lẫn nhau', tức là không có giá trị ngang nhau, trong khi đây lại là một thuộc tính quan trọng của tiền kỹ thuật số. Để giải quyết vấn đề này, Nick đề xuất một hình thức 'ngân hàng tự do' hoạt động trên nền tảng BitGold, có thể tổng hợp các nhóm hash khác nhau để chúng được định giá như nhau.

##### B-Money

Ngay sau đề xuất Bit Gold, Wei Dai đã đề xuất một giải pháp tương tự. Anh đã phát triển một số công cụ khác cho nhóm Cypherpunks, và có những ý tưởng riêng về tiền kỹ thuật số.

Đề xuất của anh giống với Bit Gold ở chỗ sử dụng chữ ký số để chuyển tiền, và các bản ghi giao dịch sẽ được lưu trữ trên một sổ cái, chứa các khóa công khai và số lượng đơn vị tiền tệ được gán cho mỗi khóa. Cũng như Bit-Gold, các bên thứ ba đáng tin cậy được coi là lỗ hổng bảo mật, và quan điểm là một hệ thống tiền điện tử không nên dựa vào một thực thể duy nhất để theo dõi số dư, giao dịch hoặc ngăn chặn chi tiêu hai lần.

Wei Dai đã đề xuất một số giải pháp cho những vấn đề này, trong đó có một ý tưởng là thay vì một thực thể trung tâm duy trì sổ cái, TẤT CẢ các nút sẽ duy trì một bản sao. Nếu tất cả người dùng kiểm tra sổ cái của mình và tính hợp lệ của từng giao dịch, miễn là tất cả các nút đều được cập nhật thì các sổ cái sẽ được đồng bộ hóa trên toàn mạng. Hệ thống phân tán cao này sẽ rất khó bị làm sai lệch.

Wei Dai nhận ra rằng điều này không giải quyết được vấn đề các vị tướng Byzantine (1), vì các nút có thể dễ dàng mất đồng bộ hoặc đơn giản là nói dối. Anh đề xuất các phương pháp thay thế như có một tập hợp các máy chủ 'đáng tin cậy' duy trì sổ cái, và tạo ra các động lực tài chính để giữ cho các máy chủ này trung thực.

Về chính sách tiền tệ, anh đề xuất gắn sức mua của B-Money với một dạng chỉ số giá tiêu dùng bên ngoài. Anh muốn cùng một lượng B-Money có thể mua được một phần tương đương của chỉ số này theo thời gian, nhằm mang lại sự ổn định giá cả. Như vậy, bất kỳ ai cũng có thể tạo ra đơn vị tiền tệ mới bằng cách cung cấp một hash hợp lệ, nhưng độ khó của việc tạo hash có thể thay đổi theo thời gian dựa trên chi phí CPU và chỉ số giá, để mỗi đơn vị là 'bất biến'.
