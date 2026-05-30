<img width="1481" height="2048" alt="image" src="https://github.com/user-attachments/assets/6cc467c5-1839-42aa-b55c-a7b56cfff6a1" />


Chú Trần Quang Khải hỏi mấy câu khá hay, em trả lời thành một tút luôn, ai đọc được cái gì thì đọc.
Câu hỏi:
"Tương lai tới (5-20 năm) a đánh giá các tình hình các ngôn ngữ sẽ thế nào ạ, ý em là về độ phổ biến, tính ứng dụng... của các ngôn ngữ nhất là trong enterprise software và distributed system, golang hay rust/kotlin/scala có thay thế java/c# ko?
Mất bao năm học và luyện OOP với java e thấy nó cho mình ko chỉ là ngôn ngữ mà cả tư duy phân tích thiết kế và cách viết clean code và xây dựng hệ thống, từ design pattern, solid, đến các loại tdd/ddd... mà giờ thấy nó ko thịnh hành và có ưu thế như xưa cũng thấy tiếc quá. Cảm giác cả đời luyện võ rồi đi đánh nhau lại gặp thằng vác Ak47 ra 🥲 Thời a ngày xưa chắc cũng làm java thời đầu, sau đấy thì a chuyển dịch thế nào để adapt thời thế mà ko bỏ phí cái cũ ? em cảm ơn ạ."
=====
Trả lời:
Trước hết phải có hai cái disclaimer đã:
1) Anh cũng chỉ là một người bình thường, dự đoán tương lai cũng chỉ là dựa theo tư duy chủ quan của anh. Nhưng lịch sử cho thấy là bọn deep định hướng phát triển theo hướng có lợi cho chúng nó, chứ không phải theo logic, nên không đoán trước hoàn toàn được.
2) Ai mà muốn sống một cuộc đời bình yên, không sóng gió, sống ổn định, sung sướng, không lên voi xuống chó thì không nên nghe lời anh khuyên. Lời anh khuyên là dành cho những người thích mạo hiểm, sống không cần đời và không cần gì.
*
Bây giờ vào nội dung chính. 
➪ Theo như anh quan sát thấy trong tình hình industry ở Mỹ, trong vòng 5 năm tới, thì Java và C# vẫn là ngôn ngữ phổ biến để làm enterprise software. 
Bên cạnh đó, Python cũng là ngôn ngữ phổ biến vì có mấy cơn sốt DevOps/Cloud, Data Science và AI. Python là một ngôn ngữ tốt, nhưng mà boring. Hơn nữa bây giờ bọn dùng Python cũng không phải là bọn làm enterprise software, nên Python cũng không thay thế Java và C# trong việc làm enterprise software được. 
Dù cho Python + Django và Ruby + Rails tốt hơn hàng tỷ lần Java và C#, nhưng cả Python lẫn Ruby rất khó trở thành ngôn ngữ phổ biến trong enterprise software. Tuy nhiên có nhiều hãng lớn cũng dùng Ruby làm enterprise software. 
Thậm chí nguyên cái infrastructure của AWS lẫn phần các Brazil package cho software development của Amazon là viết hoàn toàn bằng Ruby, nhưng bọn kỹ sư em chã ở các department khác của Amazon mỗi lần nói đến Ruby thì lại ra cái vẻ chê bai, dè bỉu. Chẳng qua là kỹ năng dùng dynamic typed language của chúng nó kém quá, lại không đủ trình làm meta programming, nên mỗi lần viết Ruby code thì lại sai lung tung, không biết đâu mà sửa.
Có nhiều bọn dùng javascript để viết backend code, nhưng cũng không phổ biến bằng Java và C#. Hơn nữa, chỉ có bọn dân chơi nhà quê, viết code chưa sạch if-else mới tính đến chuyện dùng javascript viết backend code.
Kotlin hay Scala rất khó vào mainstream của các project lớn, vì đặc trưng ngôn ngữ của nó cũng chả khác gì Java, với một số idiot-proof feature,  không có incentive gì cho các lập trình viên switch từ Java hay C# sang Kotlin hay Scala.
Về Go và Rust thì cũng khó vào mainstream của enterprise software trong 5 năm tới được, vì hiện giờ các lập trình viên dùng Go và Rust chủ yếu là làm system programming. Các lập trình viên làm enterprise software cũng không thấy incentive gì nhiều khi chuyển từ Java hay C# sang Go hoặc Rust.
Trừ rất ít trường hợp cần tốc độ nhanh, ví dụ như hồi anh viết cái Cryptography Server cho bọn Cisco, để generate certificate, public/private keys cho hàng trăm triệu communication devices, thì phải cần tốc độ xử lý cực nhanh - Hồi đó anh viết con server này bằng Go.
Những thứ liên quan đến docker đa số viết bằng Go, nên Go sẽ phổ biến trong system programming là chủ yếu.
Rust cũng tương tự như Go. Sắp tới, Linux kernel có thêm các component viết bằng Rust, thì Rust cũng chỉ phổ biến trong system programming.
Bây giờ, embedded software dùng cả C, Go và Rust.
Có một vài ngôn ngữ mà chú không nhắc tới, mà lại tương đối phổ biến trong một số niche, là Erlang, và ngôn ngữ khác chạy trên Erlang BEAM VM là Elixir. Erlang và Elixir là hai ngôn ngữ xử lý huge number of concurrent request, massive parallel processing cực tốt.
Do đó, trong industry hiện nay, có nhiều hệ thống cần có parallel processing cực nhiều, rất nhiều concurrent request, nhất là trong Telecom, media ...etc... đều sử dụng Erlang hoặc Elixir.
Hồi anh làm cái startup về dược phục vụ cho tất cả các bệnh viện, bác sĩ, hãng dược của Mỹ cũng dùng Elixir + Phoenix.
Tuy nhiên, trong lĩnh vực enterprise software, trong vòng 5 - 10 năm tới, anh không nghĩ là có ngôn ngữ nào trở nên phổ biến hơn  Java hay C#.
Trong những sản phẩm nhố nhăng kiểu chat chiệc, share siệc, làm những thứ vớ vẩn lừa tiền nhà đầu tư như bọn nó đang làm phổ biến bây giờ thì không tính.
Nói về 10 năm hoặc 20 năm nữa thì cũng khó nói. Nhưng trong vòng 10 năm, chắc là không có ngôn ngữ nào phổ biến hơn Java và C# trong việc viết code cho backend của các phần mềm tử tế.
Còn nói về độ phổ biến nói chung, thì từ chục năm nay cho đến có lẽ là chục năm sau, javascript và các quái thai của nó như TypeScript, ES, các library và framework đáng ghê tởm như React, Angular, Vue, Ember, Stimulus ...etc... vẫn là phổ biến nhất.
Nhưng phổ biến nhất không có nghĩa là tốt nhất. Cũng như Java và C# là phổ biến nhất trong lĩnh vực enterprise software, nhưng cũng không phải là công cụ tốt nhất, có productivity cao nhất.
Đến hai mươi năm nữa thì anh không biết thế nào. Biết đâu vài năm nữa lại ra ngôn ngữ lập trình nào tốt, rồi hai mươi năm sau nó thành phổ biến.
➪ Còn chuyện anh adapt thế nào để khỏi lãng phí những ngôn ngữ, công cụ cũ thì nói chung cũng không có ích lợi gì cho người bình thường muốn có cuộc sống ổn định.
Anh bắt đầu làm việc một cách chuyên nghiệp là dùng C/C++ để viết các ứng dụng chạy trên AT&T Unix System V, Linux và Windows. Sau đó vào khoảng 1995 Java ra đời, 1996 bắt đầu truyền khắp thế giới thì anh viết cái hệ thống AI dùng Multi-Agent System ở Đức là dùng Java. 
Về sau, khi sang Mỹ, thì dự án làm enterprise software đầu tiên của anh ở Mỹ là viết phần mềm về Healthcare / Medical Insurance cho bọn 3M Healthcare, là viết hoàn toàn bằng C++.
Sau đó anh mới chính thức chuyển sang viết enterprise software bằng Java, làm phần mềm cho manufacturing, từ sản xuất máy bay chiến đấu, tàu chiến, ô tô cho đến quần lót phụ nữ, đều dùng Windchill Core do anh làm trong R&D. Đến hệ thống cyber warfare đầu tiên của Bộ quốc phòng Mỹ dùng tại Iraq năm 2003 là Future Combat System (FCS) cũng dùng Windchill Core.
Sau đó, khi anh đã có hơn chục năm kinh nghiệm làm Java trong enterprise software, thì một ngày đẹp trời, anh vào hiệu sách, thấy có cuốn sách nói đến Ruby. Năm đó cả thế giới chỉ có bốn quyển sách viết về Ruby. Anh mua cả bốn cuốn về nhà đọc, sau khi đọc xong thì anh bỏ job, bỏ Java, chuyển hẳn sang Ruby.
Lúc đó ở Mỹ hầu như không ai biết Ruby là cái gì, và không có công ty nào làm Ruby. Anh cùng mấy chú tốt nghiệp MIT mở một cái startup, làm enterprise software bằng Ruby on Rails, về sau bán được một vài triệu $ cho bọn Washington Post. Tiếp theo, anh với mấy chú tốt nghiệp UC Berkeley mở một startup khác, dùng Ruby On Rails làm enterprise software cho lĩnh vực Footwear and Apparel, đại khái là cho công nghiệp thời trang. 
Nhưng lúc này, khủng hoảng kinh tế 2008, 2009 xảy ra, công ty anh bị phá sản. Thế là anh phải đi làm thuê, chuyên tư vấn cho các công ty ở Mỹ từ lớn đến vừa, đến nhỏ, đến startup viết enterprise software bằng Ruby. Sau đó anh cũng mở một startup khác về buôn bán sỉ xe ô tô, cũng dùng Ruby.
Cho đến một ngày kia, anh tình cờ đọc về bọn Ericson của Thụy Điển dùng Erlang trong Telecom, bọn Whatsapp dùng một server chạy Erlang mà handle được một triệu concurrent request, thế là anh quay ra nghiên cứu Erlang và tiếp đó là một ngôn ngữ vừa mới ra đời, không ai biết, là Elixir.
Sau đó vài năm, thì anh làm một cái startup làm về dược phẩm, sử dụng Elixir và Phoenix.
Những thứ khác như Go, Rust, Python, Objective C ...etc... này nọ anh cũng tìm hiểu do thích, và dùng vào công việc khi có requirement thích hợp, chứ không phải là do nó phổ biến. Kể lan man về các ngôn ngữ lập trình anh đã làm, về cuộc đời và sự nghiệp của anh nữa thì quá dài.
♣︎ Đại khái là con đường đi của anh là do thích tìm hiểu công nghệ, ngôn ngữ, công cụ, chứ không phải làm những thứ phổ biến. Do đó anh làm toàn những thứ từ khi nó mới ra đời, hầu như không có ai biết, hầu như không có ai dùng, cũng có nghĩa là hầu như không có job, cũng hầu như không có tiền đầu tư. Một người khác kém may mắn hơn anh mà làm thế thì chết đói từ hai mươi đời rồi.
* Nói về làm thế nào để khỏi lãng phí những cái cũ thì những thứ như Data Structures, Algorithms, phong cách lập trình, phong cách thiết kế sẽ không thay đổi mấy khi mình thay đổi công cụ. 
Tuy nhiên, lập trình cũng như kiến trúc phần mềm, nếu chỉ làm một thứ, thì sẽ giống như ếch ngồi đáy giếng. Ví dụ như một người cả đời chỉ biết có OOP, chỉ lập trình với compiler language hoặc hybrid languge, chỉ biết có static-typed language, mà không biết Functional, không biết dynamic-typed language, không biết interpreter language, chỉ biết imperative language mà không biết descriptive language, thì cũng như thằng thầy bói mù, sờ được bộ phận nào của con voi thì biết bộ phận đó.
Thậm chí, nếu chỉ giới hạn trong OOP, imperative language, thì chỉ cần OO Design cho static-typed language và OO Design cho dynamic-typed language là đã khác nhau rất nhiều rồi, có rất nhiều Design Pattern không cần dùng, có rất nhiều phong cách thiết kế có thể rút gọn, tăng productivity cao hơn, làm chương trình ngắn hơn, Object hierarchy ít phức tạp hơn.
Do đó, muốn có một cái nhìn từ nhiều góc, có kiến thức tổng hợp về Computer Science, Software Engineering và Architecture Design, thì phải biết nhiều phong cách lập trình, nhiều loại ngôn ngữ, nhiều phương pháp thiết kế. Vì thế, không có cái gì là lãng phí cả.
Đấy là đang nói về việc nghiên cứu công nghệ, làm vì kiến thức, tri thức, không cần tiền, không cần job, không cần ổn định.
Chứ còn cứ đi trước thời đại, làm những thứ mới vào lúc mà chưa có ai biết, chưa có job, chưa có nhà đầu tư, chưa có tiền thì mau chết lắm. Cuộc đời không phải như bọn em chã mơ mộng vẫn bị bọn tài phiệt nó lừa là "phải sáng tạo, phải đi tiên phong mới tốt" đâu.
Đến như Paul Graham, sư tổ của các loại startup, trùm Y! Combinator chuyên đầu tư tiền cho startup ở Silicon Valley còn phải phát biểu: "Làm startup, làm công nghệ mà ra cái mới, chưa ai làm thì quên mẹ nó đi, không ai ngu mà đầu tư tiền cho chúng mày đâu. Phải làm cái gì có nhiều người làm rồi, mà đưa ra giải pháp tốt hơn".
Lão ấy chắc là deep, nên không nói nốt đoạn cần nói: Phải làm bung xung cho deep, rửa tiền cho deep thì làm cái gì cũng ra tiền được, kể cả là làm những thứ rất ngu như chat chiệc, share siệc, share vợ đợ con và bán quảng cáo online.
➪ Tóm lại là đường ai nấy đi thôi, chứ các chú đừng đi theo con đường của anh, nếu không muốn chết già, chết đói trong một khu rừng hẻo lánh nào đó của thế giới.

**Trần Quang Khải:** "...Thậm chí, nếu chỉ giới hạn trong OOP, imperative language, thì chỉ cần OO Design cho static-typed language và OO Design cho dynamic-typed language là đã khác nhau rất nhiều rồi, có rất nhiều Design Pattern không cần dùng, có rất nhiều phong cách thiết kế có thể rút gọn, tăng productivity cao hơn, làm chương trình ngắn hơn, Object hierarchy ít phức tạp hơn.

Do đó, muốn có một cái nhìn từ nhiều góc, có kiến thức tổng hợp về Computer Science, Software Engineering và Architecture Design, thì phải biết nhiều phong cách lập trình, nhiều loại ngôn ngữ, nhiều phương pháp thiết kế. Vì thế, không có cái gì là lãng phí cả...."

Đoạn này hay quá, em chưa thấy ai nói được/làm được thế này. Phần lớn đều bám chấp, giáo điều, luẩn quẩn trong cái vòng/thế giới quan của họ, hoặc có nói thì cũng chỉ nói theo sách vở cóp nhặt trên mạng chứ không có trải nghiệm thực tế thì cũng vô nghĩa.

**Châu Hồng Lĩnh:** He...he... bây giờ thì chú thấy một người rồi, phỏng?

Thực ra là ai cũng có khả năng làm thế, vấn đề là người ta có bỏ được chấp niệm ở trong lòng không.

---

**Đào Duy Thanh:** Anh đúng là kiểu Explorer rồi, ông nào yếu thì ở đồng bằng ăn lúa gạo thôi.

**Châu Hồng Lĩnh:** Vấn đề là người ta có dám đi và có dám trả giá để đi không thôi, chứ không liên quan gì đến yếu, mạnh.

Nếu không sợ bị chết giữa đường, mà thích đi thì cứ đi thôi chứ. 😃

---

**Nguyen Hoang Chung:** 20 năm trước anh say mê nói về vẻ đẹp của Ruby, nay vẫn vậy, thật bái phục.

Thực ra thì nhiều khi nghĩ con người là cái con mẹ gì mà suốt ngày phải nghĩ đến chuyện đi kiếm ăn... 🙁

**Châu Hồng Lĩnh:** He...he... chuyện con người phải vất vả kiếm ăn là do bọn deep tạo ra để con người ta vướng vào cơm áo gạo tiền, không nghĩ tới chuyện phản kháng deep.

Chứ thời buổi bây giờ, khoa học kỹ thuật phát triển, năng suất lao động, sản xuất cao. Tại sao con người ta phải sống vất vả, tốn nhiều thời gian để lao động, kiếm ăn thế?

Nhưng có một số người nào đó không sợ đói, không sợ khổ, không cần nhiều tiền, thì vẫn có thể có một số giá trị tinh thần nhất định.

---

**Long Tran:** Em đọc dài quá, kéo xuống tìm ra tấm hình, đúng là khuyên dùng lập trình hướng hình ảnh là lời khuyên, nhưng không làm theo nổi.

**Châu Hồng Lĩnh:** Chú nhìn thấy cái ảnh là hay rồi. 😃

---

**Đinh Hải:** Cháu thắc mắc là theo ý chú thì tại sao JS lại quá phò để làm backend tử tế?

**Châu Hồng Lĩnh:** Chú nói "backend tử tế" nghĩa là làm các hệ thống enterprise software phức tạp.

Còn làm một vài hệ thống quản lý thông tin không cần scientific accuracy, không cần quá nhiều CPU-bound processing, không có quá nhiều parallel processing, không cần heavy-duty security, codebase không quá lớn thì OK.

Lý do là:

* JavaScript language spec và implementation rất mù mờ trong tính toán số. Cụ thể là `number` và `floating point number` trong JavaScript chỉ implement cho nó có, độ chính xác không cao cho các tính toán phức tạp.

* JavaScript là single-threaded language, vì thế nó phải dùng async để làm I/O và nhiều tác vụ khác, dẫn đến viết code rất khó chịu. Và nó chỉ là giả lập để tạo ra ảo tưởng responsive thôi, chứ bản thân nó không thể so với các ngôn ngữ cho phép chạy multi-thread, multi-process. Do đó đối với những hệ thống đòi hỏi parallel processing nhiều, JavaScript không đáp ứng được.

* Security kém, vì JavaScript application phụ thuộc quá nhiều vào các third-party package. Hiện nay cộng đồng JavaScript viết các npm package có kiến thức về security rất kém, nên account của họ dễ bị hack, dễ bị inject malicious code vào. Ngay cách đây một vài tuần, có vụ hơn 1000 npm package dính malware, làm cho mấy chục triệu application bị ảnh hưởng.

Tất nhiên đây không phải là lỗi của ngôn ngữ JavaScript. Nhưng một ngôn ngữ không chỉ là một ngôn ngữ đơn thuần, mà còn phụ thuộc vào ecosystem của nó. Và ecosystem của JavaScript rất không an toàn.

* Third-party dependency của JavaScript thường có phụ thuộc rất lớn, nhiều khi tốn hàng GB và hàng đống package chỉ để làm mấy việc vớ vẩn. Đồng thời mấy cái package này được maintain rời rạc, nên nhiều khi chỉ vài ba tuần là có conflict giữa các package lung tung, làm cho các JavaScript project lớn rất unstable.

Trong khi đó, khi làm software tử tế thì các thư viện phải có baseline tử tế, có Long Term Support để bảo đảm compatibility, thì mới implement, maintain và extend lâu dài được.

Còn một số thứ khác có thể khắc phục được, ví dụ như JavaScript cho phép lập trình viên viết code dài dòng, vô tổ chức, khó bảo trì... nhưng đây chỉ là vấn đề kỹ năng, có thể khắc phục được.

Tuy nhiên, những điểm chú nói ở trên kia thì rất khó, thậm chí không có khả năng khắc phục.

---

**Loc Ho:** Điểm mạnh Java là ecosystem và community vô cùng mạnh. Nó cũng là ngôn ngữ khá secure hơn các ngôn ngữ khác với các practice như static typing, null pointer exception hay tính năng như JVM, memory access.

Điểm yếu là Java nặng memory footprint, cồng kềnh, chi phí deploy khá cao hơn các ngôn ngữ khác.

Các software enterprise của Java chỉ giỏi thu tiền khách hàng là chủ yếu.

Ví dụ là khi cài Oracle bạn không thể uninstall bình thường mà phải xóa các mục trong registry hay services. Hay với IBM WebSphere gần như là không ai cài app trên platform mà không có lỗi cả 🙂))

Anh có tin em từng làm việc tới team mà chưa bao giờ dựng môi trường local thành công với IBM WebSphere không?

Productivity khi viết code dĩ nhiên cũng sẽ chậm hơn các dynamic language như Ruby.

Còn về mấy khái niệm design pattern, clean code thì áp dụng cho các ngôn ngữ khác, không cứ gì Java.

Java hợp với enterprise vì có các ông lớn support, charge triệu đô không vấn đề gì miễn là chạy được ổn định là được.

Nói gì thì nói các phiên bản Java sau này cũng cải thiện hơn trước nhiều về performance và garbage collection.

Nếu ai muốn việc ổn định thì học Java cơ hội việc làm hơn các ngôn ngữ khác tuy không nhiều.

---

**Châu Hồng Lĩnh:** Java với ý nghĩa là một ngôn ngữ OOP static-typed language thì nó được design khá tốt. Ngay cả Java VM cũng tốt.

Sở dĩ các Java app chạy chậm, footprint nhiều, tốn resource đa số là do các lập trình viên Java viết code kém hiệu quả.

Không nói đâu xa, chỉ cần chọn collection để chứa data cần xử lý trong bộ nhớ mà chọn sai kiểu, hoặc chọn duyệt collection lớn bằng iterator là tốn thời gian và resource hơn rất nhiều so với chọn đúng.

Nó là sự khác nhau giữa hàng minute và hàng millisecond.

Nhưng khi dùng Java làm enterprise software, bọn lập trình viên Java có một cái tởm là thích tạo ra những object hierarchy rất loằng ngoằng, phức tạp.

Đấy là indirection, nhưng mà chúng nó lại tưởng nhầm là abstraction, bảo là làm thế thì mới làm hệ thống flexible, dễ bảo trì, dễ mở rộng.

Nhưng mà chúng nó dùng sai thiết kế, dùng sai design pattern. Indirection không phải abstraction.

Nên khi cần thay đổi method signature hay thêm method vào component, thì phải sửa không chỉ một class, mà phải sửa interface, abstract class và tất cả các concrete class implementation.

Thay vì sửa một hai file thì phải sửa cả chục file, chưa kể test case.

Tất nhiên đấy là lỗi con người chứ không phải lỗi ngôn ngữ, nhưng con người cũng là một phần của ecosystem của ngôn ngữ.

Và khi lũ người ngu đủ đông, viết ra đủ nhiều thư viện, đủ nhiều component thì chết lây sang cả những người khôn.

Vì thế người khôn tham gia vào cộng đồng Java enterprise cũng chả làm được cái đếch gì mấy, vì hệ thống nó thế, thư viện nó thế, cuối cùng là low productivity cả lũ.

Còn nói về application server thì cả bọn IBM lẫn Oracle đều tởm như nhau.

Bọn IBM có cái WebSphere siêu hủi, siêu tởm, thì bọn Oracle có cái WebLogic cũng tởm gần bằng thế.

Hồi bọn Oracle chưa mua WebLogic, thì nó là một J2EE App Server rất tốt. Oracle mua về phá một thời gian làm nó phò hẳn đi.

Tuy nhiên, bọn open-source J2EE App Server như Tomcat hay JBoss thì cũng không tệ, dùng tốt.

Đáng tiếc là bọn doanh nghiệp lớn vì sợ trách nhiệm và thích ăn tiền lại quả của bọn bán, nên hay chọn WebSphere hoặc WebLogic.

Nhưng mà ai ngu thì cho chúng nó chết.

---

**Loc Ho:** Một thực tế là đa phần web app phần lớn là I/O data nên dù code rất phò nhưng nếu at the end of the day mọi thứ chạy "bình thường", đem lại doanh thu về cho doanh nghiệp thì họ không có nhu cầu sửa đổi.

Thậm chí rất ngại bỏ ra vài sprint chỉ để bảo team refactor code lại toàn bộ hay redesign app sao cho chuẩn chỉ.

Miễn là tốc độ và bảo mật được đảm bảo, không có leak data, lượng traffic đều đặn là OK.

Em từng làm dự án code có function 2000 dòng kết hợp jQuery, JSTL suốt 5 năm mà không có ai sửa gì cả!

**Châu Hồng Lĩnh:** Bọn doanh nghiệp lớn đều ù lì, trì trệ lắm, nên bọn nó cứ miễn là có cái gì chạy được là được.

Chỉ có khi nào không dùng được nữa, hoặc muốn tỏ ra cho cổ đông thấy là công ty có cố gắng đổi mới công nghệ nhằm thu hút tiền đầu tư và tăng giá cổ phiếu, hoặc là bọn management có cơ hội ăn tiền lại quả khi làm project thì chúng nó mới làm project mới.

Chả thế mà đầy công ty tài chính, chứng khoán, healthcare và các tổ chức chính phủ Mỹ còn chạy COBOL từ những năm 1960 đến giờ.

Nhiều bọn thì cố gắng làm project mới nhưng không xong.

Đến lúc có công nghệ mới, lại cố gắng làm cái mới, nhưng cũng không xong.

Cứ thế, có ba bốn thế hệ software và hardware khác nhau chạy cùng lúc trong công ty:

* Máy tính to bằng cả căn nhà.
* Máy tính to bằng cái tủ.
* Máy tính to bằng cái bể cá.
* Và máy tính nhỏ như bây giờ.
