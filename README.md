# Phần 1 : Cơ bản về cơ sở dữ liệu và ngôn ngữ truy vấn dữ liệu SQL

## Bài 1: Tổng quan về cơ sở dữ liệu và ngôn ngữ truy vấn SQL

Đây là bài học đầu tiên của môn học Các hệ cơ sở dữ liệu. Ở bài học này các bạn sẽ được làm quen với các khái niệm như cơ sở dữ liệu, hệ quản trị cơ sở dữ liệu và ngôn ngữ truy vấn dữ liệu.

**Cơ sở dữ liệu (Database)** là một tập hợp dữ liệu hoặc thông tin có tổ chức để có dễ dàng truy cập, cập nhật hoặc thao tác. Ví dụ như chúng ta có các cơ sở dữ liệu trường học, ngân hàng,...

**Hệ quản trị cơ sở dữ liệu (Database management system - DBMS)** như một phần mềm để giúp quản lý cơ sở dữ liệu. DBMS sẽ bao gồm các chức năng để xác định, thao tác cũng như truy xuất và quản lý dữ liệu. Ví dụ như: định dạng dữ liệu, tên của file, cấu trúc của bản record. DBMS cũng sẽ giúp xác định những quy tắc nhằm xác thực cũng như thao tác với những dữ liệu được lưu trữ trong DBMS.

Có hai DBMS rất phổ biến là **MySQL** và **SQL Server**. MySQL được phát hành từ giữa thập niên 90s (sau đó bị thâu tóm bởi Oracle), MySQL ban đầu là một DBMS mã nguồn mở và cũng vẫn mở cho tới tận bây giờ. Vì là mã nguồn mở, MySQL được phát hành từ giữa thập niên 90s (sau đó bị thâu tóm bởi Oracle), MySQL ban đầu là một DBMS mã nguồn mở và cũng vẫn mở cho tới tận bây giờ. Vì là mã nguồn mở, MySQL có rất nhiều phiên bản khác dựa trên nó, sự khác biệt giữa các biến thể này là không lớn; cấu trúc và chức năng cơ bản tương đương nhau. SQL Server xuất hiện trước MySQL. Microsoft phát triển SQL Server từ giữa thập niên 80s, với mục tiêu hướng đến là SQL Server sẽ cung cấp giải pháp đáng tin cậy và có thể mở rộng. Việc này trở thành đặc tính đáng giá của SQL Server cho tới tận bây giờ, vì nó là một nền tảng được chọn cho những phần mềm doanh nghiệp cần mở rộng lớn theo thời gian. SQL Server sẽ hoạt động tốt trong hệ sinh thái của Microsoft nhưng chưa được hỗ trợ tốt trong Linux, trong khi đó MySQL hoạt động tốt ở cả Windows và Linux. Chính vì MySQL là một phần mềm miễn phí và hoạt động tốt trong các hệ điều hành khác nhau nên trong bài này và xuyên suốt môn học, các bạn sẽ được làm quen và thực hành với hệ quản trị cơ sở dữ liệu **MySQL**.

Ngoài hai khái niệm về cơ sở dữ liệu và hệ quản trị cơ sở dữ liệu. Chúng ta còn có một khái niệm nữa là **ngôn ngữ truy vấn dữ liệu (Structured Query Language - SQL)**. Trong mỗi một hệ quản trị cơ sở dữ liệu sẽ có một ngôn ngữ truy vấn dữ liệu khác nhau để phục vụ cho việc lấy và truy vấn dữ liệu. Ví dụ như khi bạn sử dụng MySQL để truy vấn dữ liệu sẽ có một số cú pháp khác so với khi các bạn sử dụng SQL Server. MySQL là một hệ quản trị cơ sở dữ liệu được sử dụng để lưu trữ, quản lý dữ liệu có cấu trúc trong khi đó SQL là một ngôn ngữ truy vấn dữ liệu được sử dụng bên trong MySQL.

Ví dụ: Ở trong 1 quyển danh bạ điện thoại , ta cần tìm số của Ned Flanders's phone number thay vì phải tìm không biết bao nhiều lần, kiểm tra hàng nghìn lần tìm tất cả người có tên Ned, hoặc tìm tất cả các phone numbers với mã khu vực là 415, tìm tất cả các người có 3 chữ cái trong first name thì dùng SQL.

Sự khác nhau giữa SQL và My SQL:

Giống nhau:
```sql
MySQL
SELECT * FROM Users WHERE Age>= 18;
PostgreSQL
SELECT * FROM Users WHERE Age>= 18;
```

Lab 1.1 Cài đặt MySQL Community

Ở phần đầu tiên của môn học, các bạn đã được thực hiện viết truy vấn trong MySQL. Vì vậy, điều đầu tiên cần bạn cài đặt được MySQL Community.

**Bước 1**: Tải  MySQL Community

Truy cập [Tại đây](https://dev.mysql.com/downloads/mysql/). Và tải xuống phiên bản Mysql Community.

![Mysql_Community1](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL1.png)

**Bước 2**: Mở file vừa tải về và thực hiện cài đặt

![Mysql_Community2](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL2.png)

![Mysql_Community3](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL3.png)

![Mysql_Community4](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL4.png)

![Mysql_Community5](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL5.png)

![Mysql_Community6](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL6.png)

![Mysql_Community7](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL7.png)

![Mysql_Community8](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL8.png)

![Mysql_Community9](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL9.png)

![Mysql_Community10](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL10.png)

![Mysql_Community11](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL11.png)

**Bước 3**: Sau khi đã việc cài đã hoàn tất, mở Mysql Workbench

![Mysql_Community12](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/Install/InstallMySQL12.png)

Quiz 1:

Câu 1: Điều nào sau đây là đúng khi nói về cơ sở dữ liệu?

A. Là nơi quản lý dữ liệu  B. Là một tập hợp dữ liệu hoặc thông tin có tổ chức để có thể dễ dàng truy cập, cập nhật hoặc thao tác. <br>
C. Có thể gọi là Database.  D. Được gọi là DBMS.

Đáp án: B, C

Câu 2: Tính năng nào sau đây không phải là tính năng của SQL Server?

A. Hỗ trợ lưu trữ dữ liệu lớn.  B. Hỗ trợ các giao dịch (transactions) và tính toàn vẹn dữ liệu.<br>
C. Chỉ chạy trên hệ điều hành Linux.  D.Hỗ trợ sao lưu và khôi phục dữ liệu.

Đáp án: C

Câu 3: Hệ quản trị cơ sở dữ liệu DBMS là gì?

A. Là một cơ sở dữ liệu.  B. Là một phần mềm để giúp quản lý cơ sở dữ liệu. DBMS sẽ bao gồm các chức năng để xác định, thao tác cũng như truy xuất và quản lý dữ liệu.<br>
C. Là một môi trường Cloud để phát triển ứng dụng.  D. Là một ngôn ngữ lập trình.

Đáp án: B

Câu 4: DBMS là viết tắt của từ gì?

A. Database  B. Database management system  C. Data management system D. Database storage system

Đáp án: B

Câu 5: MySQL là gì?

A. Là một ngôn ngữ dữ liệu  B. Là một ngôn ngữ truy vấn  C. Là một DBMS D. Là tên một cơ sở dữ liệu

Đáp án: C

Câu 6: SQL là gì?

A. Là một ngôn ngữ truy vấn dữ liệu  B. Có tên đầy đủ là Structured Query Language  C. Là một DBMS  D. Là một cơ sở dữ liệu

Đáp án: A, B

Câu 7: Trong các đáp án dưới đây, đâu là một DBMS?

A. SQL  B. MySQL  C. SQL SERVER  D. T-SQL

Đáp án: B,C

Câu 8: Để có thể sử dụng được MySQL trong chế độ dòng lệnh của GoormIDE, chúng ta cần chạy đoạn mã nào dưới đây?

A. mysql-ctl  B. mysql -u root -p  C. mysql cli  D. mysql-ctl cli

Đáp án: D

Câu 9: Chúng ta có thể sử dụng SQL trong MySQL.

A. Đúng  B. Sai

Đáp án: A

Câu 10: Điểm khác biệt giữa SQL và MySQL gì?

A. SQL là một ngôn ngữ truy vấn dữ liệu có cấu trúc còn MySQL là một hệ thống quản lý cơ sở dữ liệu.<br>
B. Có thể sử dụng MySQL trong SQL.<br>
C. Có thể sử dụng SQL trong MySQL.<br>
D. Không có đáp án nào đúng.

Đáp án: A,C

## Bài 2: Tạo một cơ sở dữ liệu và thao tác với bảng

Trong bài học này các bạn sẽ được làm quen với ngôn ngữ định nghĩa dữ liệu (Data Definition Language - DDL). Đây là các lệnh để **định nghĩa cấu trúc** lưu trữ dữ liệu. Chúng ta sẽ sử dụng các câu lệnh này để thao tác trên Database (cơ sở dữ liệu), Table (bảng), các trường (cột). Một số lệnh thuộc nhóm DDL như CREATE, DROP, TRUNCATE, ALTER, ...

### 1. Tạo và xóa cơ sở dữ liệu

Để có thể lưu trữ dữ liệu trong MySQL, chúng ta phải thực hiện chỉ định một database trong trường hợp database đã tồn tại. Trong trường hợp chưa tồn tại, chúng ta phải thực hiện tạo một database mới bằng lệnh CREATE. Lưu ý là MySQL không phân biệt chữ hoa và chữ thường khi thực hiện câu lệnh, ví dụ lệnh CREATE sẽ tương đương Create. 

> Syntax: Lệnh tạo một database: CREATE DATABASE ten_database;

Lab 2.1 - Creating Database

1.1 Yêu cầu:

Chạy lần lượt và làm quen với câu truy vấn dưới đây:<br>
**CREATE DATABASE donation; (tạo mới database tên là donation);**

1.2 Hướng dẫn:

Để chạy các lệnh trên các bạn thực hiện như sau:<br>
Bước đầu khi mở MySQL Workbench lên sẽ là một giao diện trắng, bạn cần phải tạo file .sql để thực hiện viết câu lệnh.

![Database](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE.png)

Lựa chọn vào icon sql đầu tiên ở góc trên bên tay trái để thực hiện tạo 1 file .sql mới trong mysql workbench

![Database1](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE1.png)

![Database2](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE2.png)

Thực hiện viết câu lệnh “**CREATE DATABASE donation;**” với mục đích là tạo cơ sở dữ liệu có tên là donation.

![Database3](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE3.png)

Để thực hiện câu lệnh, bạn hãy lựa chọn icon ‘sấm sét’ ở phía bên tay trái.

![Database4](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE4.png)

Ngay lập tức, thực hiện thành công việc khởi tạo database, sẽ được thông báo ở “Action Output”

![Database5](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE5.png)

Muốn hiển thị tên database “donation” trong MySQL, thì cần thực hiện chuột phải vào tab bên trái của MySQL. Lựa chọn “Refresh All” để load lại hệ quản trị cơ sở dữ liệu MySQL Workbench

![Database6](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE6.png)

![Database7](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateDatabase/CREATEDATABASE7.png)










