
<img width="2048" height="1458" alt="image" src="https://github.com/user-attachments/assets/73435282-dde6-4106-a0a5-7245b6679b2e" />

Cháu Đinh Hải hỏi câu về javascript cũng hay, em post câu trả lời vào đây.

Vấn đề bắt đầu từ topic này:
https://www.facebook.com/chauhonglinh2021/posts/pfbid0cF7Teav3thEmCEENFdv6dV2C3fsXK5hzYsDrZyJ6EJL9fSQ5ZMho5GExi6Pwzutql

⇒ Câu hỏi: "Cháu thắc mắc là theo ý chú thì tại sao js lại quá phò để làm backend tử tế?"

_____

⇒ Trả lời:

Chú nói "backend tử tế" nghĩa là làm các hệ thống enterprise software phức tạp.

Còn làm một vài hệ thống quản lý thông tin không cần scientific accuracy, không cần quá nhiều CPU-bound processing, không có quá nhiều parallel processing, không cần heavy duty security, codebase không quá lớn thì ok.

Lý do là:
- javascript language spec và implementation rất mù mờ trong tính toán số, cụ thể là number và floating point number trong javascript chỉ implement cho nó có, độ chính xác không cao cho các tính toán phức tạp.

- javascript là single-threaded language, vì thế nó phải dùng async để làm I/O và nhiều tác vụ khác, dẫn đến viết code rất khó chịu. Và nó chỉ là giả lập để tạo ra ảo tưởng responsive thôi, chứ bản thân nó không thể so với các ngôn ngữ cho phép chạy multi-thread, multi-process. Do đó đối với những hệ thống đòi hỏi parallel processing nhiều, javascript không đáp ứng được.

- Security kém, vì javascript application phụ thuộc quá nhiều vào các third party package. Hiện nay cộng đồng javascript viết các npm package có kiến thức về security rất kém, nên account của họ dễ bị hack, dễ bị inject javascript malicious code vào. Ngay cách đây một vài tuần, có vụ hơn 1000 npm package dính malware, làm cho mấy chục triệu application bị ảnh hưởng.

Tất nhiên đây không phải là lỗi của ngôn ngữ javascript. Nhưng một ngôn ngữ không chỉ là một ngôn ngữ đơn thuần, mà còn phụ thuộc vào eco-system của nó. Và eco-system của javascript rất không an toàn.

- Third party và Dependency của javascript thường có phụ thuộc rất lớn, nhiều khi tốn hàng GB và hàng đống package chỉ để làm mấy việc vớ vẩn. Đồng thời mấy cái package này được maintain rời rạc, nên nhiều khi chỉ vài ba tuần là có conflict giữa các package lung tung, làm cho các javascript project lớn rất unstable.

Trong khi đó, khi làm software tử tế thì các thư viện phải có base line tử tế, có Long Term Support để bảo đảm compability, thì mới implement, maintain và extend lâu dài được.

Còn một số thứ khác có thể khắc phục được, ví dụ như javascript cho phép lập trình viên viết code dài dòng, vô tổ chức, khó bảo trì ...etc..., nhưng đây chỉ là vấn đề kỹ năng, có thể khắc phục được.

Tuy nhiên, những điểm chú nói ở trên kia thì rất khó - thậm chí không có khả năng - khắc phục.

=====

* Trong ảnh là danh sách các npm package của một javascript application vô cùng nhỏ, chỉ dùng để hiện món ăn trên menu của một nhà hàng Hy Lạp tại một thị trấn nhỏ của Mỹ theo ngày trong tuần, quản lý món ăn, menu ...etc...

App này không hề dùng bất kỳ một frontend framework nào như React, Angular hay Vue ...etc..., mà sau khi chạy "npm install" đã có 826 package. Chưa hề có một dòng code nào của chương trình trong đấy, nhá.

* Còn đây là một số vấn đề về javascript security liên quan đến npm (chỉ là ít ví dụ trong vô số vấn đề về security mà js application mắc phải):

https://www.facebook.com/permalink.php?story_fbid=pfbid02D9ycEFTQnqNKHZCGhYECkXuAeyDfiSQxdL8rev8QoeeZQZHRVPkwAdgjWJ4ZGG8ql&id=100079575759287

https://www.facebook.com/chauhonglinh2021/posts/pfbid0bPrk1BXhCMbVEYjkWdWNez2Bj9vyoZVFLEMYiyAg36WDAxB1Zg3e6X4Arm9kiMVxl

https://www.facebook.com/chauhonglinh2021/posts/pfbid036LXTdAfKjUJcMLM9ERPei86r7Zdmy2MrjunL6tpS58seU1sNwh76roD41HjLEdnfl 


**Nguyen Van Khoi:** Tầm 7-8 năm trước, có lần em dùng cái lib gì đó bên JS, nhưng không fix cứng version (cái số cuối cùng á), và sau đó nó làm chết ứng dụng, kiểu nó thay đổi hoàn toàn luôn. Đúng là cái gì dễ viết quá dẫn tới contributor không tốt.

> Bài học: luôn fix cứng tới chữ số cuối cùng của version.

Lần làm React Native 0.54(?) của Facebook (khoảng 8 năm trước), có cái kiểu như localStorage, `get("x")` lần đầu chạy, lần sau không bao giờ resolve. Lúc này mới học React Native, debug nguyên ngày.

> Bài học lúc đó: code JS thì lên mạng xem có thằng nào lỗi tương tự không thay vì tự đọc code debug lại :))

Mà chuyện version, em dính cả với MariaDB, dùng chỉ cập nhật bản fix security 🙁

> Bài học: gấp tới đâu, cũng test trước :3

---

**Châu Hồng Lĩnh:** Mà bây giờ có cơn điên DevOps bịp bợm, có version conflict lại càng nhục.

Vì sau khi fix làm cho application chạy trở lại rồi thì lại phải fix cả Dockerfile, fix Terraform file hoặc Ansible hoặc whatever, rồi phải fix cả CI/CD cho nó build và chạy test cho đúng...

Làm mẹ nó bằng tay, làm đi làm lại hàng nghìn lần còn nhanh hơn automation kiểu bọn nhà quê.

Tất nhiên là biết automation tử tế lại là câu chuyện khác.

---

**Nguyen Van Khoi:** Em cũng không biết. Mỗi lần nói chuyện với bọn DevOps là lại thấy mệt :3, toàn chơi những cách complex nhất thì phải :))

Ở VN giờ còn đỡ, chứ có giai đoạn không làm dev được mới đi làm ops, nên làm việc cùng rất chi là mệt.

---

**Châu Hồng Lĩnh:** Bọn DevOps vốn là bọn trước đây chỉ biết đào tường, khoét vách, cắm dây mạng, cài hệ điều hành dạo.

Đến lúc có cơn lên đồng DevOps thì bọn đào tường khoét vách cắm dây cài OS dạo đấy quay ra viết YAML và JSON dạo.

Thế thì khá thế đéo nào được.

---

**Nguyen Van Khoi:** Lâu lâu xem lại lại thấy vui. Đoạn cuối là JS.

[https://www.destroyallsoftware.com/talks/wat](https://www.destroyallsoftware.com/talks/wat)

Wat

---

**Châu Hồng Lĩnh:** Phải công nhận bọn viết JS language spec không biết gì về ngôn ngữ lập trình. 😃
