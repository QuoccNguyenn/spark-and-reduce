# spark-and-reduce
Giới thiệu về Spark và mapreduce (BIG-DATA)<br>

Thuật ngữ dữ liệu lớn đã tạo ra rất nhiều sự cường điệu đã có trong thế giới kinh doanh. Hadoop và Spark đều là các khung dữ liệu lớn; họ cung cấp một số công cụ phổ biến nhất được sử dụng để thực hiện các tác vụ lớn liên quan đến dữ liệu lớn. Bài viết này  sẽ đề cập đến sự khác biệt giữa Spark và Hadoop MapReduce.<br>

GIỚI THIỆU<br>
<pre>Spark</pre> là một khung dữ liệu lớn nguồn mở. Nó cung cấp một công cụ xử lý dữ liệu có mục đích chung nhanh hơn và nhiều hơn. Spark về cơ bản được thiết kế để tính toán nhanh. Nó cũng bao gồm một loạt các khối lượng công việc - ví dụ, lô, tương tác, lặp và phát trực tuyến.<br>

Hadoop MapReduce cũng là một khung nguồn mở để viết các ứng dụng. Nó cũng xử lý dữ liệu có cấu trúc và không cấu trúc được lưu trữ trong HDFS. Hadoop MapReduce được thiết kế theo cách xử lý một khối lượng lớn dữ liệu trên một cụm phần cứng hàng hóa. MapReduce có thể xử lý dữ liệu trong chế độ hàng loạt.<br>

XỬ LÝ DỮ LIỆU<br>
Spark:<br>
Apache Spark phù hợp cho cả xử lý hàng loạt và xử lý luồng, nghĩa là nó là khung xử lý kết hợp. Spark tăng tốc xử lý hàng loạt thông qua tính toán trong bộ nhớ và tối ưu hóa xử lý. Đó là một lựa chọn tốt để truyền tải khối lượng công việc lớn, truy vấn tương tác và học máy. Spark cũng có thể hoạt động với Hadoop và các mô-đun của nó. Khả năng xử lý dữ liệu thời gian thực của nó khiến Spark trở thành lựa chọn hàng đầu cho các phân tích dữ liệu lớn.<br>
Bộ dữ liệu phân tán linh hoạt (RDD) của nó cho phép Spark lưu trữ dữ liệu trong bộ nhớ một cách trong suốt và chỉ gửi vào đĩa những gì quan trọng hoặc cần thiết. Kết quả là, rất nhiều thời gian dành cho việc đọc và ghi trên đĩa được giảm đi.<br>
Hadoop:<br>Apache Hadoop cung cấp xử lý hàng loạt. Hadoop phát triển rất nhiều trong việc tạo ra các thuật toán mới và ngăn xếp thành phần để cải thiện quyền truy cập vào xử lý hàng loạt quy mô lớn.<br>
MapReduce là công cụ xử lý hàng loạt riêng của Hadoop. Một số thành phần hoặc lớp (như YARN, HDFS, v.v.) trong các phiên bản hiện đại của Hadoop cho phép dễ dàng xử lý dữ liệu hàng loạt. Vì MapReduce là về lưu trữ vĩnh viễn, nó lưu trữ dữ liệu trên đĩa, có nghĩa là nó có thể xử lý các bộ dữ liệu lớn. MapReduce có khả năng mở rộng và đã chứng minh hiệu quả của nó để đối phó với hàng chục ngàn nút. Tuy nhiên, quá trình xử lý dữ liệu của Hadoop rất chậm do MapReduce hoạt động theo các bước tuần tự khác nhau.<br>

<b>PHÂN TÍCH THỜI GIAN THỰC</b><br>
<b><pre></pre>Spark</b> có thể xử lý dữ liệu thời gian thực, tức là dữ liệu đến từ các luồng sự kiện thời gian thực với tốc độ hàng triệu sự kiện mỗi giây, chẳng hạn như dữ liệu Twitter và Facebook. Sức mạnh của Spark nằm ở khả năng xử lý luồng trực tiếp thực sự hiệu quả.<br>
<b>MapReduce</b> không tốt khi xử lý dữ liệu thời gian thực, vì nó được thiết kế để thực hiện xử lý hàng loạt trên lượng dữ liệu khổng lồ.<br>

<b>DỄ SỬ DỤNG</b><br>
<b>Spark:</b><br> Spark dễ sử dụng hơn Hadoop, vì nó đi kèm với các API thân thiện với người dùng cho Scala (ngôn ngữ gốc của nó), Java, Python và Spark SQL. Vì Spark cung cấp một cách để thực hiện phát trực tuyến, xử lý hàng loạt và học máy trong cùng một cụm, người dùng dễ dàng đơn giản hóa cơ sở hạ tầng của mình để xử lý dữ liệu. REPL tương tác(Read-Eval-Print Loop) cho phép người dùng Spark nhận phản hồi tức thì cho các lệnh.<br>
<b>Hadoop:</b><br> Mặt khác, Hadoop, được viết bằng Java, rất khó lập trình và đòi hỏi sự trừu tượng. Mặc dù không có chế độ tương tác có sẵn với Hadoop MapReduce, các công cụ như Pig và Hive giúp người dùng dễ dàng làm việc với nó hơn.<br>
