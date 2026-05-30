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

**Nguyen Van Khoi:** Chỗ `maxProfit`, nếu quan sát `price` mà không lớn hơn `lastCheckedPrice (= prices[i-1])` thì có thể bỏ qua tính hiệu và tính `max` lại.
