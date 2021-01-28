# spark-and-mapreduce
<pre><b>Giới thiệu về Spark và mapreduce (BIG-DATA)</b></pre>

Thuật ngữ dữ liệu lớn đã tạo ra rất nhiều sự cường điệu đã có trong thế giới kinh doanh. Hadoop và Spark đều là các khung dữ liệu lớn; họ cung cấp một số công cụ phổ biến nhất được sử dụng để thực hiện các tác vụ lớn liên quan đến dữ liệu lớn. Bài viết này  sẽ đề cập đến sự khác biệt giữa Spark và Hadoop MapReduce.<br>

<pre><b>GIỚI THIỆU</b></pre>
<b>Spark</b> là một khung dữ liệu lớn nguồn mở. Nó cung cấp một công cụ xử lý dữ liệu có mục đích chung nhanh hơn và nhiều hơn. <b>Spark</b> về cơ bản được thiết kế để tính toán nhanh. Nó cũng bao gồm một loạt các khối lượng công việc - ví dụ: <b>lô, tương tác, lặp và phát trực tuyến</b>.<br>

<b>Hadoop MapReduce</b> cũng là một khung nguồn mở để viết các ứng dụng. Nó cũng xử lý dữ liệu có cấu trúc và không cấu trúc được lưu trữ trong <b>HDFS</b>. <b>Hadoop MapReduce</b> được thiết kế theo cách xử lý một khối lượng lớn dữ liệu trên một cụm phần cứng hàng hóa. <b>MapReduce</b> có thể xử lý dữ liệu trong chế độ hàng loạt.<br>

<pre><b>XỬ LÝ DỮ LIỆU</b></pre>
<b>Apache Spark</b> phù hợp cho cả xử lý hàng loạt và xử lý luồng, nghĩa là nó là khung xử lý kết hợp. Spark tăng tốc xử lý hàng loạt thông qua tính toán trong bộ nhớ và tối ưu hóa xử lý. Đó là một lựa chọn tốt để truyền tải <b>khối lượng công việc lớn, truy vấn tương tác và học máy</b>. Spark cũng có thể hoạt động với Hadoop và các mô-đun của nó. Khả năng xử lý dữ liệu thời gian thực của nó khiến Spark trở thành lựa chọn hàng đầu cho các phân tích dữ liệu lớn.<br>
Bộ dữ liệu phân tán linh hoạt (RDD) của nó cho phép Spark lưu trữ dữ liệu trong bộ nhớ một cách trong suốt và chỉ gửi vào đĩa những gì quan trọng hoặc cần thiết. Kết quả là, rất nhiều thời gian dành cho việc đọc và ghi trên đĩa được giảm đi.<br>
<b>Hadoop:</b><br>Apache Hadoop cung cấp xử lý hàng loạt. Hadoop phát triển rất nhiều trong việc tạo ra các thuật toán mới và ngăn xếp thành phần để cải thiện quyền truy cập vào xử lý hàng loạt quy mô lớn.<br>
MapReduce là công cụ xử lý hàng loạt riêng của Hadoop. Một số thành phần hoặc lớp (như YARN, HDFS, v.v.) trong các phiên bản hiện đại của Hadoop cho phép dễ dàng xử lý dữ liệu hàng loạt. Vì MapReduce là về lưu trữ vĩnh viễn, nó lưu trữ dữ liệu trên đĩa, có nghĩa là nó có thể xử lý các bộ dữ liệu lớn. MapReduce có khả năng mở rộng và đã chứng minh hiệu quả của nó để đối phó với hàng chục ngàn nút. Tuy nhiên, quá trình xử lý dữ liệu của Hadoop rất chậm do MapReduce hoạt động theo các bước tuần tự khác nhau.<br>

<pre><b>PHÂN TÍCH THỜI GIAN THỰC</b></pre>
<b>Spark</b> có thể xử lý dữ liệu thời gian thực, tức là dữ liệu đến từ các luồng sự kiện thời gian thực với tốc độ hàng triệu sự kiện mỗi giây, chẳng hạn như dữ liệu Twitter và Facebook. Sức mạnh của Spark nằm ở khả năng xử lý luồng trực tiếp thực sự hiệu quả.<br>
<b>MapReduce</b> không tốt khi xử lý dữ liệu thời gian thực, vì nó được thiết kế để thực hiện xử lý hàng loạt trên lượng dữ liệu khổng lồ.<br>

<pre><b>DỄ SỬ DỤNG</b></pre>
<b>Spark:</b><br> Spark dễ sử dụng hơn Hadoop, vì nó đi kèm với các API thân thiện với người dùng cho Scala (ngôn ngữ gốc của nó), Java, Python và Spark SQL. Vì Spark cung cấp một cách để thực hiện phát trực tuyến, xử lý hàng loạt và học máy trong cùng một cụm, người dùng dễ dàng đơn giản hóa cơ sở hạ tầng của mình để xử lý dữ liệu. REPL tương tác(Read-Eval-Print Loop) cho phép người dùng Spark nhận phản hồi tức thì cho các lệnh.<br>
<b>Hadoop:</b><br> Mặt khác, Hadoop, được viết bằng Java, rất khó lập trình và đòi hỏi sự trừu tượng. Mặc dù không có chế độ tương tác có sẵn với Hadoop MapReduce, các công cụ như Pig và Hive giúp người dùng dễ dàng làm việc với nó hơn.<br>

<b>Sự khác biệt</b> giữa Apache Spark so với Hadoop MapReduce cho thấy Apache Spark là công cụ tính toán cụm tiên tiến hơn nhiều so với MapReduce. Spark có thể xử lý bất kỳ loại yêu cầu nào (ví dụ: tương tác, lặp, phát trực tuyến, đồ thị) trong khi MapReduce giới hạn xử lý hàng loạt.

<pre><b">SPARK PROPERTIES</b></pre>
<b>Thuộc tính Spark</b> kiểm soát hầu hết các cài đặt ứng dụng và được cấu hình riêng cho từng ứng dụng. Các thuộc tính này có thể được đặt trực tiếp trên SparkConf được chuyển tới SparkContext của bạn.<br>
  
<pre><b">APACHE SPARK RDD</b></pre>
<b>Resilient Distributed Datasets</b><br>
  
<b>Resilient Distributed Datasets (RDD)</b> là một cấu trúc dữ liệu cơ bản của Spark. Nó là một tập hợp bất biến phân tán của một đối tượng. Mỗi dataset trong RDD được chia ra thành nhiều phần vùng logical. Có thể được tính toán trên các node khác nhau của một cụm máy chủ (cluster).<br>

<b>RDDs</b> có thể chứa bất kỳ kiểu dữ liệu nào của Python, Java, hoặc đối tượng Scala, bao gồm các kiểu dữ liệu do người dùng định nghĩa. Thông thường, RDD chỉ cho phép đọc, phân mục tập hợp của các bản ghi. RDDs có thể được tạo ra qua điều khiển xác định trên dữ liệu trong bộ nhớ hoặc RDDs, RDD là một tập hợp có khả năng chịu lỗi mỗi thành phần có thể được tính toán song song.<br>

<b>Có hai cách để tạo RDDs:</b><br>
•	Tạo từ một tập hợp dữ liệu có sẵn trong ngôn ngữ sử dụng như <b>Java, Python, Scala</b>.<br>
•	Lấy từ dataset hệ thống lưu trữ bên ngoài như <b>HDFS, Hbase hoặc các cơ sở dữ liệu quan hệ</b>.

<b>Thực thi trên Spark RDD</b><br>
Để khắc phục được vấn đề về <b>MapRedure</b>, các nhà nghiên cứu đã phát triển một <b>framework</b> chuyên biệt gọi là <b>Apache Spark</b>. Ý tưởng chính của <b>Spark</b> là <b>Resilient Distributed Datasets (RDD)</b>; nó hỗ trợ tính toán xử lý trong bộ nhớ. Điều này có nghĩa, nó <b>lưu trữ trạng thái</b> của bộ nhớ dưới dạng một đối tượng trên các công việc và đối tượng có thể chia sẻ giữa các công việc đó. Việc xử lý dữ liệu trong bộ nhớ <b>nhanh hơn 10 đến 100 lần</b> so với <b>network và disk</b>.<br>

<b>Các loại RDD:</b><br>
  •	Các RDD biểu diễn một tập hợp cố định, đã được phân vùng các record để có thể xử lý song song.<br>
  •	Các record trong RDD có thể là đối tượng Java, Scala hay Python tùy lập trình viên chọn. Không giống như DataFrame, mỗi record của DataFrame phải là một dòng có cấu trúc chứa các field đã được định nghĩa sẵn.<br>
  •	RDD đã từng là API chính được sử dụng trong series Spark 1.x và vẫn có thể sử dụng trong version 2.X nhưng không còn được dùng thường xuyên nữa.<br>
  •	RDD API có thể được sử dụng trong Python, Scala hay Java:<br>
    o	Scala và Java: Perfomance tương đương trên hầu hết mọi phần. (Chi phí lớn nhất là khi xử lý các raw object)<br>
    o	Python: Mất một lượng performance, chủ yếu là cho việc serialization giữa tiến trình Python và JVM<br>

<b>Các transformation và action với RDD</b><br>
•	RDD cung cấp các transformation và action hoạt động giống như DataFrame lẫn DataSets. Transformation xử lý các thao tác lazily và Action xử lý thao tác cần xử lý tức thời.<br>
<b>Một số transformation:</b><br>
Nhiều phiên bản <b>transformation</b> của <b>RDD</b> có thể hoạt động trên các <b>Structured API</b>, transformation xử lý lazily, tức là chỉ giúp dựng execution plans, dữ liệu chỉ được truy xuất thực sự khi thực hiện action.<br>
•	<b>distinct</b>: loại bỏ trùng lắp trong RDD<br>
•	<b>filter</b>: tương đương với việc sử dụng <b>where</b> trong <b>SQL</b> – tìm các record trong <b>RDD</b> xem những phần tử nào thỏa điều kiện. Có thể cung cấp một hàm phức tạp sử dụng để <b>filter</b> các <b>record</b> cần thiết – Như trong <b>Python</b>, ta có thể sử dụng hàm <b>lambda</b> để truyền vào <b>filter</b>.<br>
•	<b>map</b>: thực hiện một công việc nào đó trên toàn bộ <b>RDD</b>. Trong Python sử dụng <b>lambda</b> với từng phần tử để truyền vào <b>map</b>.<br>
•	<b>flatMap</b>: cung cấp một hàm đơn giản hơn hàm map. Yêu cầu <b>output</b> của map phải là một <b>structure</b> có thể lặp và mở rộng được.<br>
•	<b>sortBy</b>: mô tả một hàm để trích xuất dữ liệu từ các <b>object</b> của RDD và thực hiện sort được từ đó.<br>
•	<b>randomSplit</b>: nhận một mảng trọng số và tạo một <b>random seed</b>, tách các RDD thành một mảng các RDD có số lượng chia theo trọng số.<br>
<pre><b>SPARK DATAFRAME</b></pre><br>
<b>DataFrame</b> là một <b>API</b> bậc cao hơn RDD được Spark giới thiệu vào năm 2013 (từ <b>Apache Spark 1.3</b>). Tương tự như RDD, dữ liệu trong DataFrame cũng được quản lý theo <b>kiểu phân tán và không thể thay đổi (immutable distributed)</b>. Tuy nhiên dữ liệu này được sắp sếp theo các cột, tương tự như trong <b>Relation Database</b>.<br>


<b>DataFrame</b> được phát triển để giúp người dùng có thể dễ dàng thực hiện các thao tác xử lý dữ liệu cũng như làm tăng đáng kể hiệu quả xử lý của hệ thống.<br>

Khi sử dụng DataFrame API, chúng ta gọi các hàm để trích xuất kết quả mong muốn và Spark sẽ tự động tiến hành <b>các thuật toán xử lý</b>. Tuy nhiên ở bước cuối cùng thì các thuật toán này vẫn được chạy trên RDD mặc dù người dùng chỉ tương tác với DataFrame.<br>

Bên cạnh các ưu điểm, thì <b>nhược điểm</b> lớn nhất của DataFrame là API này không hỗ trợ <b>Compile-time type safety</b>, do đó chúng ta khó có thể tiến hành thao tác trên dữ liệu.<br>
Ví dụ như khi chúng ta dùng <b>DataFrame</b> để truy xuất <b>people(“age”)</b>, kết quả trả về không phải ở dạng Int mà ở dạng <b>Column object</b>. Vì vậy chúng ta không thể thực hiện các thao tác với kết quả này như đối với một <b>Int object</b>.<br>

Việc không hỗ trợ <b>type safefy</b> này làm người dùng không thể phát huy lợi thế của <b>type system</b> mà các ngôn ngữ lập trình như <b>Scala, Java,..</b> hỗ trợ. Ngoài ra, nó còn làm tăng các lỗi <b>runtime</b> mà đáng ra đã được phát hiện tại <b>compile time</b>.<br>


<b><pre>Source:</b></pre><br>
https://laptrinh.vn<br>
http://itechseeker.com<br>




