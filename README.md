# Phần 1 : Cơ bản về cơ sở dữ liệu và ngôn ngữ truy vấn dữ liệu SQL

## Bài 1: Tổng quan về cơ sở dữ liệu và ngôn ngữ truy vấn SQL

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

[Mysql_Community1](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL1.png)

**Bước 2**: Mở file vừa tải về và thực hiện cài đặt

[Mysql_Community2](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL2.png)

[Mysql_Community3](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL3.png)

[Mysql_Community4](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL4.png)

[Mysql_Community5](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL5.png)

[Mysql_Community6](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL6.png)

[Mysql_Community7](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL7.png)

[Mysql_Community8](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL8.png)

[Mysql_Community9](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL9.png)

[Mysql_Community10](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL10.png)

[Mysql_Community11](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL11.png)

**Bước 3**: Sau khi đã việc cài đã hoàn tất, mở Mysql Workbench

[Mysql_Community12](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/InstallMySQL12.png)












