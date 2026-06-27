1.
<img width="2048" height="1221" alt="image" src="https://github.com/user-attachments/assets/ca7ddc4b-e41b-4269-9b03-4a9d3ef371f2" />

**Trần Quang Khải:** Liên tục update giá mua nếu thấp hơn. Còn gặp giá cao hơn thì tính thử profit rồi lấy max.

Có O(n) time và O(1) memory.

---

**Châu Hồng Lĩnh:** He...he... chú viết thế này với tư cách là một bài giải LeetCode của sinh viên thì OK.

Tuy nhiên, với tư cách là bài viết của một software engineer, thì có một vài điểm chưa được.

Đầu tiên là tên biến.

`c` là cái đếch gì?

Nếu chú thay `c` bằng `minBuyPrice` hoặc `minPrice` thì tốt hơn.

Tương tự, `ret` là viết tắt cho `return`, có lẽ ai cũng hiểu. Nhưng trường hợp này, thay nó bằng `maxProfit` thì tốt hơn.

Đặt tên như thế, chương trình dễ hiểu và dễ bảo trì hơn, nhất là đối với những chương trình lớn.

Tất nhiên là một cái hàm nhỏ thế này không thành vấn đề, nhưng nên tập thành thói quen ngay từ những cái nhỏ.

Tiếp theo, cũng là chương trình như của chú, chú thử xem có cách nào làm nó ngắn hơn, ít số dòng code hơn không?

---

**Trần Quang Khải:** Vâng em viết ẩu để cho nhanh ấy mà. Anh review có tâm vãi.

Em thử sửa lại như sau.

<img width="833" height="350" alt="image" src="https://github.com/user-attachments/assets/d97d668a-9165-41c2-8e2a-7065003e3960" />


---

**Châu Hồng Lĩnh:** Đấy, code như thế mới là code của software engineer.

Nói chung chơi mấy cái trò này, giải được bài toán là dễ, nhưng rèn luyện cách viết code mới là quan trọng.

Nhất là khi mình phỏng vấn người khác, nhìn người ta viết code, dù chỉ rất đơn giản, nhưng có thể đánh giá xem người ta cẩn thận đến đâu, phong cách lập trình có tốt hay không, có kinh nghiệm không...

---

**Trần Quang Khải:** Em thấy giờ phần lớn các developer làm ăn ẩu chán lắm, kiểu miễn code chạy được là được, viết test/mock còn kiểu đối phó cho có.

À bình thường anh phỏng vấn (nhất là với senior) thì anh hay hỏi gì hoặc ra đề gì thế nào để chọn, đánh giá đúng?

---

**Châu Hồng Lĩnh:** Nói chung, anh phỏng vấn sẽ có mấy phần:

* Coding đơn giản, nhưng không chỉ là làm kiểu LeetCode. Cũng có ít thuật toán, cơ sở dữ liệu, nhưng quan trọng nhất là nó đòi hỏi phải thiết kế một số object (nếu làm OOP) hoặc module (nếu làm Functional Programming).

  Để đạt được yêu cầu thì phải chia object hoặc module clean theo functionality, app layer. Đồng thời khi có yêu cầu về thay đổi chức năng, mở rộng chức năng thì phải ít viết lại code nhất, sử dụng lại được nhiều nhất, thêm component vào dễ nhất.

* Database Design:

  Cho một số yêu cầu đơn giản về đối tượng cần quản lý, ví dụ như:

  * Trường đại học, các khoa, các khóa học, sinh viên...
  * Nhà xuất bản sách, bao gồm sách, tác giả, các loại format sách khác nhau, các lần tái bản...

  Rồi cho design table, column, relationship, các thể loại key, index.

  Sau đó discuss về performance, khả năng thêm, sửa, mở rộng của design.

* Software Architecture:

  Hỏi về một số Design Pattern và cách vận dụng nói chung.

  Đưa ra một số thiết kế để cho người ta nhận xét xem:

  * Trường hợp nào có thể cải tiến.
  * Trường hợp nào dùng Design Pattern là không cần thiết.
  * Trường hợp nào dùng sai...

* Đưa ra một số bài toán có data cực lớn để xem họ xử lý thế nào, ví dụ:

  * MapReduce.
  * Parallel processing.
  * Distributed processing...

* Hỏi về Cyber Security, Defensive Coding, kỷ luật về giữ an toàn hệ thống và máy tính cá nhân...

Đại khái là cũng không có gì khó và đánh đố, toàn những thứ cơ bản.

Nhưng nhìn những chi tiết nhỏ mà người ta thể hiện khi giải quyết vấn đề là mình có thể thấy rất nhiều thứ về:

* Trình độ.
* Kinh nghiệm.
* Phong cách làm việc.
* Tính sáng tạo.
* Kỷ luật...

---

**Trần Quang Khải:** Tức là anh hỏi cả 5 phần trên cho 1 người hay tùy job/profile mà chỉ hỏi vài cái trong số đó ạ?

Em thấy thế cũng nhiều đấy chứ, không dễ, không cơ bản tí nào.

Để ngon được cái đống đấy là đòi hỏi rất nhiều kinh nghiệm với kỹ năng.

Tức là ngon được 2-3 cái thì không khó, nhưng ngon được cả 5-6 cái đấy thì trình cũng kinh đấy.

Như architecture với big data kia cũng là nâng cao rồi.

---

**Châu Hồng Lĩnh:** He...he... cả 5 chứ, nhưng tùy theo job mà hàm lượng cái nào ít hay nhiều, đòi hỏi cái nào cao hơn thôi.

Một software engineer có trình độ thì phải có cả 5 thứ đó.

Vấn đề là có nhiều hay có ít, hiểu đến tầm nào, vận dụng đến tầm nào.

Thiếu một trong mấy cái đấy là dễ làm ra software lung tung lắm.

---
2.
𝐋𝐨̣̂ 𝐭𝐫𝐢̀𝐧𝐡 𝐦𝐨̣̂𝐭 𝐜𝐨𝐝𝐞𝐫 𝐧𝐞̂𝐧 𝐩𝐡𝐚́𝐭 𝐭𝐫𝐢𝐞̂̉𝐧
Hôm nay đi chém dạo trên Phê tê bốc, tình cờ thấy một cháu coder hỏi đại khái là giờ cháu nó biết làm backend bằng Python và Django rồi, nhưng cứ mài chuột, mài bàn phím if-else-do-while-for mãi cũng vô nghĩa, giờ nên phát triển theo lộ trình nào.
Em có cái tham luận như sau đây, chả biết rồi có bổ ích gì cho cháu nó không, nhưng em cũng chỉ chém cho nó sướng cái bàn phím là chính.
Ai đọc được cái gì thì tốt, mà không được cái gì thì càng tốt, nhá.

Một anh coder muốn thành một cái gì khá hơn coder, nghĩa là không chỉ ngồi suốt ngày mài if-else-do-while-for, viết yaml, dockerfile, javascript import bullshit, thì phải biết một thứ rất cơ bản, rất người (chứ không phải đinh ốc, bàn phím) là: "Viết code để làm cái gì?"

Một thằng thợ code chỉ biết có ngôn ngữ, công cụ, library, framework, cũng không khác gì một anh thợ mộc chỉ có kỹ năng dùng cưa, bào, đục. 
Dù anh thợ này có kỹ thuật dùng công cụ vô cùng hoàn hảo, có thể bào ngang, cưa dọc, đục chéo tạo thành bất kỳ một hình gì, chính xác đến từng micrometer, thì vẫn là thằng sử dụng công cụ, nếu không có nhận thức là mình đang chế tạo cái gì, cái giường, cái tủ hay cái quan tài, và mỗi thứ có những yêu cầu về mỹ thuật, sử dụng, business logic như thế nào. Thế thì chỉ suốt đời làm một tay mù quáng, ai bảo cưa chỗ này 3 cm, đục chỗ kia 5 cm là hì hục làm, rồi ghép với những mảnh cưa 7 cm, đục 9cm của người khác, mà chả biết là mình đang làm cái chó gì. Mà làm một cách mù quáng thế thì trước sau gì cũng bị robot thay thế.

Có nhiều công ty Việt nam kêu bọn em muốn làm phần mềm bán sang Mỹ, bọn em biết ngôn ngữ nọ, framework kia, database ấy, lại biết những docker. Mịa kíp, who cares bọn em biết cái đếch gì. Vấn đề là giả sử viết phần mềm quản lý công ty bán cám lợn ở Mỹ đi, thì có ai biết ở Mỹ người ta bán cám lợn thế nào không, mà đòi viết software quản lý nó?
Cái thiếu nhất của các lập trình viên thời hiện đại là một cái nhìn tổng quát: "Người ta dùng software để làm cái gì?".

Thời bây giờ, từ lúc bọn nó bơm vá thị trường chứng khoán và giá trị công ty giả tạo trên thế giới, nhiều người không nghĩ đến "Viết software để làm việc gì? Có lợi cho ngành nào? Có lợi cho ai?", mà chỉ nghĩ "Viết software ra bao nhiêu tiền?"

Kể ra thì ý nghĩ "Viết software ra bao nhiêu tiền?" cũng không sai. Nhưng nhìn một đám viết software bán quảng cáo, bán hàng đồng nát, bán phim khiêu dâm, share vợ đợ con và phao tin đồn nhảm trên mạng xã hội, nhờ thế mà thành các công ty nghìn tỷ đô, Big 4`, FAANG này nọ, rồi muốn bắt chước chúng nó thì chỉ có đi ăn mày sớm.

Đấy không phải là các câu chuyện về những thanh niên thiên tài, sáng tạo, bỏ học đại học, đi làm ra cái sản phẩm vớ va vớ vẩn, chả đem lại lợi ích kinh tế, dịch vụ, khoa học kỹ thuật chó nào thực sự ngoài việc phao tin đồn nhảm và làm công cụ dò la, mật thám cho chính quyền và tài phiệt, kiêm công cụ rửa tiền và tuyên truyền propaganda tẩy não, rồi tự nhiên có nghìn tỷ. Chỉ có bọn con bệnh tâm thần, muốn tiền đến phát điên rồi mới tin những câu chuyện cổ tích dành cho lũ hoang tưởng điên rồ.

Bọn đấy đều là những mặt tiền bung xung của bọn tài phiệt, được chúng nó dựng lên để chơi trò phù thủy ảo thuật cổ phiếu, bơm vá stock lừa tiền, đồng thời làm công cụ cho chính quyền. Những đồ ngon của bọn nó toàn là bọn khác ẩn danh, giấu mặt không ai biết, làm ra rồi quăng cho chúng nó thành lập công ty. Chứ công ty big tech, lập trình viên của chúng nó từ trên xuống dưới ngu bỏ mẹ, chỉ giỏi sắp xếp mảng, cân bằng cây nhị phân, deep search bằng stack, breadth search bằng queue chứ biết cái chó gì. Suốt ngày làm đinh ốc, bánh răng trong cỗ máy khổng lồ, nói năng như những con vẹt, đầu óc thì như cái máy làm mì tôm tự động, nạp nguyên liệu nào vào thì ra mì tôm loại đấy, chứ có tự nghĩ ra được cái chó gì mà đòi làm sản phẩm.

Còn người làm software lương thiện, không ở trong băng nhóm của chúng nó, không có tài phiệt, venture capital nào bơm vá, chống lưng, rửa tiền, nếu muốn làm software tử tế chứ không phải suốt đời mài giũa if-else-do-while-for thì phải biết mình viết software làm cái chó gì, software của mình làm ra có giúp cho công ty nào làm ăn có hiệu quả hơn không, tiết kiệm được thời gian, chi phí và công sức hơn không? Có giúp cho các giai xinh, gái đẹp của các ngành nghề khác khỏi phải làm overtime, khỏi stress, làm việc ít hơn để có thời gian bổ củi nhau nhiều hơn không?

Nếu software của mình làm lợi cho người ta một đô, thì người ta mới trả mình năm mươi cent, chứ làm software có phải làm ăn cướp đéo đâu mà làm ra cái software phò không có lợi gì cho ai, chỉ có share siệc, chat chiệc, mail miệc, quảng cáo quảng kiệc, bán thông tin người dùng cho chính quyền và tội phạm, lại muốn người ta trả nghìn tỷ cho mình. Bọn có nghìn tỷ kia là bọn bung xung, mặt tiền cho bọn ăn cướp, chứ không phải là làm software, nhá.

Tóm lại, làm software trong ngành nào, thì ngoài việc cắm cúi viết code phò do architect, senior và sếp ra lệnh, thì cũng nên nghiên cứu xem mình đang viết software cho ngành gì, business logic của ngành này gồm những cái gì, có đoạn nào trong quy trình của ngành này mình có thể viết software tự động hóa cho nó tối ưu lên, giúp người ta làm việc tốt hơn, ít phải mài đũng quần và bàn phím hơn, có thời gian sờ tí nhau nhiều hơn. Thế mới là người làm software có lương tâm. 

Và nói dại, nói gở, phỉ phui cái bàn phím thối, lỡ sau này, đến năm 3030, nghĩa là hơn nghìn năm nữa, lỡ chẳng may AI nó viết code ngon hơn lập trình viên thật, thì những thằng gọi là lập trình viên biết business logic vẫn còn sống, vì logic trong đời thật, kiểu đưa hối lộ, tiền lại quả bán hàng, trốn thuế các thứ thì AI khó mà hiểu được. Những thằng lập trình viên như thế sẽ không thất nghiệp.
Còn bọn chỉ biết if-else-do-while-for, đục đẽo yaml, json, cầm chuột, cầm bàn phím như một lũ khỉ, đi mài AWS, GCP, Azure, docker, tool tiệc, copilot copiliệc, anthropic anthropiệc, viết prompt, gọi API như những con khỉ sẽ chết hết.

À, tuy nhiên, ở mức cơ bản thì vẫn phải biết hết if-else-do-while-for những thứ ất ơ ất iệc kể trên, phải giỏi nữa, để khi bọn khác hoặc AI làm thì mình còn biết nó làm cái gì mà review, sửa chữa, enforce nó. Chứ không thì chả khác gì mấy thằng manager, architect, tech lead, director chả biết cái chó gì, chỉ giỏi ăn tục nói phét và ra những lệnh phi thực tế không ai làm được, bị coder biết làm nó khinh cho không bằng con lợn. 

=====
**Li Mu Bai:** Chàu 23t đang bắt đầu học cyber security, chú có thể cho cháu lời khuyên về việc học và hướng đi như nào được không ạ?

---

**Châu Hồng Lĩnh:** Trong Cyber Security, lên chuyên biệt sẽ có nhiều hướng khác nhau, ví dụ như:

* Pen Test
* Binary Analysis
* Network, System and Application Defense
* Cryptography

Tuy nhiên, ở mức cơ bản thì nó đòi hỏi những kiến thức nền tảng tương đối giống nhau.

Hôm trước, chú mới khuyên một bạn khác muốn làm Cyber Security về kiến thức nền tảng như dưới đây, cháu có thể tham khảo:

---

Muốn làm tốt Cyber Security thì kiến thức cơ bản về máy tính, kiến trúc máy tính, kiến trúc hệ điều hành, networking (network protocol, network topology), lập trình, kiến trúc phần mềm phải tốt. Ngoài ra thì kiến thức về toán và cryptography cũng phải tốt.

### ➔ Hệ điều hành

Không chỉ có Linux mà cả MacOS, Windows và các hệ điều hành khác như:

* BSD Unix
* AT&T System V
* Minix
* ...

Quan trọng nhất không phải là học như con vẹt, mà phải phân biệt được:

* Monolithic kernel và microkernel
* Preemptive sharing và time sharing
* Process và thread
* Các loại lightweight process
* Inter-process communication (IPC)
* Lock, mutex, semaphore
* ...

Cũng cần hiểu:

* Quản lý bộ nhớ
* Quản lý đĩa
* I/O management
* ...

### ➔ Network

Phải biết:

* Mô hình OSI
* TCP/IP
* UDP

Và các protocol liên quan:

* HTTP(S)
* FTP / SFTP
* SSH
* ...

Ngoài ra còn:

* Network topology
* LAN, WAN
* Star, Mesh, Bus, Ring
* VPN
* Network I/O
* Tunneling
* ...

### ➔ Lập trình

Muốn làm Cyber Security thì phải biết lập trình ở mức system level, ví dụ:

* Kernel development
* Driver development
* Memory management
* Heap memory
* Stack memory
* I/O management
* Bitwise manipulation
* CPU register
* Hardware interrupt
* Hardware port

Để còn hiểu cách tấn công vào điểm yếu của hệ thống và cách phòng thủ.

Ngoài ra cũng phải biết application development, bao gồm:

* Stand-alone application
* Enterprise application

Để hiểu:

* Authentication
* Authorization
* DOS / DDOS
* Encryption at rest
* End-to-end encryption
* Script injection
* SQL injection
* Cookie hijacking
* Session hijacking
* Cross-site scripting (XSS)
* ...

### ➔ Toán và Cryptography

Để hiểu:

* Điểm mạnh, điểm yếu của các thuật toán mã hóa
* PKI (Public Key Infrastructure)
* Các chuẩn mã hóa của chính phủ
* Các cơ chế quản lý public/private key
* Các vấn đề bảo mật liên quan đến hạ tầng khóa công khai

...

Về cơ bản còn nhiều thứ khác nữa, nhưng chú lười viết.

Đấy mới là cơ bản thôi. Nhưng phải có cơ bản tốt thì mới học sâu, học vững và lên cao được.

Còn những thứ mà dân làm cyber security hay học trên ngọn và hay làm bây giờ thì có cơ bản rồi, học lên cũng nhanh, cũng dễ, mà mình mới có con đường đi bằng kiến thức của mình chứ không phải chỉ bắt chước chiêu trò trên mạng.

---

**Trần Bình An:** Cháu cảm ơn chú ạ.

---

**Trần Bình An:** Chú cho cháu hỏi thêm, muốn học những thứ trên thì mình nên học, tìm kiếm tài liệu ở đâu như nào ạ?

---

**Châu Hồng Lĩnh:** Theo chú thì đọc sách vẫn là tốt nhất.

Những thứ đấy bây giờ có rất nhiều ebook. Cứ kiếm những thứ cũ cũ một tí để đọc, ngày xưa người ta viết bài bản hơn bây giờ, rồi đọc dần lên những thứ hiện đại.

Đọc đến đâu nên thử đến đấy.

Vì thế cháu nên làm mấy con VM chạy các hệ thống khác nhau để thử nghiệm.

Cái nào headless thì dùng Docker cũng được.

Tuy nhiên, cũng có những thứ cần thử thẳng trên máy thật, vì VM với Docker chỉ là giả lập.
