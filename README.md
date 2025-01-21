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

Nếu các bạn muốn xoá một database, các bạn có thể sử dụng lệnh **DROP**.

>Syntax: Xoá một database: **DROP DATABASE ten_database;**

Lab 2.2 Drop database

Thực hiện lần lượt các câu truy vấn dưới đây trong giao diện MySQL Workbench:

**DROP DATABASE data_name;** (Xoá một database hiện có)

**CREATE DATABASE company;**<br>
**USE company;**<br>
**DROP DATABASE company;**

### 2. Sử dụng cơ sở dữ liệu vào thao tác với bảng

Để sử dụng một database đã tồn tại trong MySQL, các bạn phải chỉ định database đó cho MySQL bằng câu lệnh **USE**. 

> Syntax: Lệnh chỉ định một database: USE ten_database;

Sau khi đã chỉ định cơ sở dữ liệu, giờ các bạn có thể tạo bảng được trong MySQL.

Lệnh tạo bảng: 

```sql
CREATE TABLE ten_bang(

       ten_cot      kieu_du_lieu     cac_dieu_kien_khac,

);
```

**ten_cot** : Đây là tên của cột mà các bạn muốn tạo
**kieu_du_lieu** : Đây là kiểu dữ liệu của cột mà các bạn muốn tạo
**cac_dieu_kien_khac** : Đây là một số điều kiện khác của cột như not null, primary key ...

Ví dụ lệnh tạo bảng Persons:

```sql
CREATE TABLE Persons (

    PersonID int,

    LastName varchar(255),

    FirstName varchar(255),

    Address varchar(255),

    City varchar(255)

);
```

Để xoá hoàn toàn một bảng, các bạn có thể sử dụng lệnh **DROP**. 

> Syntax: Cú pháp DROP: DROP TABLE ten_bang;

**Có một số kiểu dữ liệu trong MySQL như sau:**

- int: Kiểu số nguyên
- float: Kiểu số thực
- char: Kiểu chuỗi nhưng sẽ có độ dài cố định
- varchar: Kiểu chuỗi nhưng sẽ có độ dài động
- date: Đây là kiểu dữ liệu ngày tháng có dạng  YYYY-MM-DD
- datetime: Đây là kiểu dữ liệu thời gian có dạng YYYY-MM-DD HH:MM:SS
- timestamp: Đây là kiểu dữ liệu thời gian có dạng hiển thị HH:MM:SS. Sự khác biệt chính của DATETIME và TIMESTAMP là giá trị của TIMESTAMP được chuyển đổi từ múi giờ hiện tại sang UTC trong khi lưu trữ, và chuyển ngược trở lại từ UTC sang múi giờ hiện tại trong lúc lấy ra. Còn kiểu dữ liệu DATETIME thì không có gì thay đổi.

Lab 2.3 Create Table – Drop Table

Yêu cầu

1. Yêu cầu 1: Tạo database tên cat_app.
2. Yêu cầu 2: Trong database cat_app, tạo bảng pastries có hai trường (cột) như sau:

- Trường name có kiểu dữ liệu VARCHAR(50)
- Trường quantity có kiểu dữ liệu int

3. Yêu cầu 3: Sau khi tạo xong bảng pastries, hãy hiển thị các bảng hiện có trong cơ sở dữ liệu cat_app ( thông qua giao diện )

Ví dụ:

![Create_Table](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateTable/CreateTable.png)

4. Yêu cầu 4: Xoá table pastries
5. Yêu cầu 5: Kiểm tra lại các table hiện có trong database cat_app.

![Create_Table1](https://github.com/Fakerrrrrrrrrrr/Database_system/blob/main/Images/CreateTable/CreateTable1.png)

Quiz 2

Câu 1: Trong hệ quản trị csdl MYSQL để có thể viết truy vấn trong một DBMS, chúng ta sẽ sử dụng công cụ gì?

A. Database       B. DBMS       C. SQL       MySQL

Đáp án: A

Câu 2: Trong các đáp án dưới đây, đâu là cú pháp tạo một cơ sở dữ liệu trong MySQL?

A. CREATE DATABASE ten_database;       B. CREATE ten_database;       C. DATABASE ten_database;       D. NEW DATABASE ten_database;

Đáp án: A

Câu 3: Trong các đáp án dưới đây, đâu là cú pháp tạo một bảng trong MySQL?

A. CREATE DATABASE ten_database TABLE ten_bang;       B. DATABASE ten_database TABLE ten_bang(cac_cau_lenh_tao_cot);       C. CREATE ten_bang;       D. CREATE TABLE ten_bang(cac_cau_lenh_tao_cot);

Đáp án: D

Câu 4: Trong hệ quản trị csdl MYSQL để sử dụng một database đã tồn tại, chúng ta sẽ sử dụng câu lệnh nào dưới đây?

A. USE ten_database;       B. USE DATABASE ten_database;       C. DATABASE ten_database;       D. ten_database;

Đáp án: A

Câu 5: Điều nào sau đây là đúng?

A. Để có thể tạo bảng, trước hết chúng ta cần chỉ định cho DBMS biết chúng ta đang sử dụng DATABASE nào bằng cách sử dụng USE.<br>
B. DBMS sẽ tự chỉ định DATABASE khi tạo bảng mà không cần can thiệp của người dùng.
C. Có thể tạo một Table trống mà không cần tạo Columns.
D. Không đáp án nào đúng.

Đáp án: A

Câu 6: Cú pháp để tạo một cột name có kiểu varchar(50) với điều kiện là NOT NULL trong một bảng là đáp án nào dưới đây?

A. CREATE COLUMN name VARCHAR(50) NOT NULL       B. name VARCHAR(50)       C. name VARCHAR(50) NOT NULL       D. name NOT NULL VARCHAR(50)

Đáp án C

Câu 7: Lệnh DROP có tác dụng gì?

A. Chỉ xoá dữ liệu của bảng, cấu trúc bảng sẽ không bị xoá.       B. Xoá một bản ghi cụ thể.       C. Xoá toàn bộ bảng, bao gồm cả cấu trúc bảng.       D. Xoá dữ liệu của bảng nhưng không xoá trong bộ nhớ.

Đáp án: C

Câu 8: Kiểu dữ liệu INT để lưu trữ dữ liệu kiểu gì?

A. Kiểu số thực       B. Kiểu chuỗi       C. Kiểu ngày tháng       D. Kiểu số nguyên

Đáp án: D

Câu 9: Kiểu dữ liệu FLOAT để lưu trữ dữ liệu kiểu gì?

A. Kiểu chuỗi       B. Kiểu số thực       C. Kiểu ngày tháng       D. Kiểu số nguyên

Đáp án: B

Câu 10: Điều nào sau đây là đúng khi nói về kiểu dữ liệu CHAR và VARCHAR?

A. CHAR không bị giới hạn độ dài chuỗi, VARCHAR bị giới hạn độ dài chuỗi.<br>
B. VARCHAR là một kiểu dữ liệu chuỗi động, sẽ cấp bộ nhớ bằng với kích thước chuỗi truyền vào nhưng không được vượt quá độ dài đã quy định. CHAR là kiểu dữ liệu chuỗi cố định, tức chương trình sẽ luôn cấp bộ nhớ bằng kích thước đã cài đặt trước.<br>
C. CHAR và VARCHAR đều được sử dụng để lưu trữ dữ liệu chuỗi hay văn bản.<br>
D. CHAR và VARCHAR được sử đụng để lưu trữ dữ liệu thời gian.

Đáp án: B,C

## Bài 3: CRUD

Trong bài học này các bạn sẽ được làm quen với ngôn ngữ thao tác dữ liệu (Data Manipulation Language - DML). Đây là các lệnh để thao tác với dữ liệu trên một bảng. Một số lệnh thuộc về nhóm DML như DELETE, INSERT, UPDATE, SELECT, ...

### 1. Thêm dữ liệu vào bảng với lệnh INSERT

Để lấy dữ liệu hay hiển thị dữ liệu từ một bảng, các bạn sẽ sử dụng lệnh SELECT.

Cú pháp lệnh SELECT:  **SELECT** ten_cot_1, ten_cot_2, ... ten_cot_n FROM ten_bang;<br>
Nếu muốn lấy tất cả các cột, các bạn sẽ sử dụng *: **SELECT * FROM** ten_bang;

Để thêm hay chèn dữ liệu vào một bảng, các bạn sẽ sử dụng lệnh INSERT.

Cú pháp lệnh INSERT: **INSERT INTO** ten_bang VALUES(gia_tri_cot_1, gia_tri_cot_2, ...,gia_tri_cot_n);

Ví dụ: INSERT INTO cats(name,age)<br>
       VALUES ("Jetson",7);

Lab 3.1 INSERT

Yêu cầu<br>
Từ database cat_app hãy thực hiện các yêu cầu dưới đây:

1. Yêu cầu 1: Tạo bảng people với các trường như sau
- first_name: Giới hạn 20 ký tự
- last_name: Giới hạn 20 ký tự
- age: Kiểu dữ liệu số nguyên

2. Yêu cầu 2: Thực hiện INSERT dữ liệu vào bảng people<br>
Cú pháp INSERT:<br>
INSERT INTO table_name(field1, field2 …)  VALUES (values1, values 2…);<br>
Dữ liệu INSERT  lần lượt theo các cột first_name, last_name, age như sau:<br>
('Tina', 'Belcher', 13)<br>
('Bob', 'Belcher', 42)<br>
('Linda', 'Belcher', 45)<br>
('Phillip', 'Frond', 38)<br>
('Calvin', 'Fischoeder', 70)<br>

3. Yêu cầu 3: Thực hiện truy vấn tất cả dữ liệu trong bảng people<br>
Cú pháp truy vấn:<br>
SELECT * FROM people;<br>
Kết quả:<br>

4. Yêu cầu 4: Thực hiện xóa bảng people<br>
5. Yêu cầu 5: Kiểm tra bảng people chắc chắn đã được xoá bằng câu lệnh “show tables;“<br>

### 2. Tạo ràng buộc cơ bản của bảng

Ở bài này, các bạn sẽ được giới thiệu một số ràng buộc cơ bản khi tạo bảng như NULL, NOT NULL, cài đặt các giá trị mặc định cho cột. Ngoài ra các bạn cũng sẽ được làm quen về cột khoá chính (primary key) khi tạo bảng. Một cột có thể được gọi là primary key của bảng nếu nó xác định duy nhất từng bộ (hàng) trong bảng đó. Nó thực thi các ràng buộc toàn vẹn đối với bảng. Chỉ có một primary key trong một bảng. Primary key không chấp nhận các giá trị trùng lặp và NULL.

Nếu các bạn muốn giữ nguyên dấu ngoặc kép khi truy vấn thì thay vì chỉ sử dụng " các bạn hãy sử dụng \".

Để hiểu rõ hơn về một số ràng buộc cơ bản khi tạo cột, mời các bạn theo dõi các bài học bên dưới:

**Lưu ý về việc sử dụng dấu ngoặc kép bên trong các giá trị được chèn**

Nếu bạn đang băn khoăn về cách chèn một giá trị xâu ký tự (VARCHAR) chứa dấu ngoặc kép thì hãy xem ở đây nè.

Bạn có thể làm theo các cách sau:<br>
- Thoát dấu nháy với dấu gạch chéo ngược: "This text has \"quotes\" in it" or 'This text has \'quotes\' in it'
- Thay dấu nháy đơn bằng dấu nháy kép và ngược lại, thay dấu nháy kép bằng dấu nháy đơn: "This text has 'quotes' in it" or 'This text has "quotes" in it'

Từ khóa NULL và NOT NULL được đặt phía sau kiểu dữ liệu của mỗi column được khai báo với mỗi lần tạo bảng
```sql
CREATE TABLE cats (
       name VARCHAR(100) NOT NULL,
       age INT NOT NULL
);
```
Từ khóa DEFAULT (Adding DEFAULT Values) là giá trị mặc định nếu không gán giá trị chèn hàng ở cột không dùng tới
```sql
CREATE TABLE cats3 (
       name VARCHAR(100) DEFAULT 'unnamed',
       age INT DEFAULT 99
);
CREATE TABLE cats4 (
       name VARCHAR(100) NOT NULL DEFAULT 'unnamed',
       age INT NOT NULL DEFAULT 99
);
```
Từ khóa Primary Key là một cột nào đó được sử dụng làm mã định danh duy nhất cho mỗi hàng riêng lẻ (A Unique Identifier)
```sql
CREATE TABLE unique_cats (
       cat_id INT NOT NULL PRIMARY KEY,
       name VARCHAR(100),
       age INT
);
```

**Lab 3.2 PRIMARY KEY - NULL – NOT NULL - DEFAULT**

**Yêu cầu**<br>
Sử dụng database cat_app hãy thực hiện các yêu cầu sau:<br>
1. **Yêu cầu 1**: Tạo  bảng unique_cats có các trường như sau:<br>
- cat_id: Có kiểu int và NOT NULL, cat_id là một primary_key<br>
- name: Có kiểu varchar(100)<br>
- age: Có kiểu int<br>
2. **Yêu cầu 2**: insert các dữ liệu sau lần lượt theo các cột cat_id, name, age cho bảng **unique_cats** và đưa ra nhận xét:<br>
(1, 'Fred', 23)<br>
(2, 'Louise', 3)<br>
(3, 'James', 3)<br>
3. **Yêu cầu 3**: Tạo bảng unique_cats2 có các trường như sau:<br>
- cat_id: Có kiểu int và NOT NULL, là một primary_key và có thể tự động tăng (auto_increment)<br>
- name: Có kiểu varchar(100)<br>
- age: Có kiểu int<br>
4. **Yêu cầu 4**:  insert các dữ liệu sau lần lượt theo các cột name, age cho bảng unique_cats2:<br>
('Skippy', 4)<br>
('Jiff', 3)<br>
('Jiff', 3)<br>
('Jiff', 3)<br>
('Skippy', 4)<br>
5. **Yêu cầu 5**: Hiển thị tất cả dữ liệu của bảng unique_cats2 và đưa ra nhận xét về trường cat_id<br>
6. **Yêu cầu 6**: Tạo bảng employees với các trường như sau:<br>
- id: Là một primary key, có kiểu int, tự động tăng và not null<br>
- first_name: Có kiểu varchar(255) và not null<br>
- last_name: Có kiểu varchar(255) và not null<br>
- middle_name: Có kiểu varchar(255)<br>
- age: Có kiểu int và not null<br>
- current_status: Có kiểu varchar(255) và not null, giá trị mặc định sẽ là “employed”<br>
7. **Yêu cầu 7**: Insert dữ liệu lần lượt theo các cột first_name, last_name, age cho bảng employees như sau:<br>
('Dora', 'Smith', 58);<br>
8. **Yêu cầu 8**: Hiển thị tất cả dữ liệu trong bảng employees và đưa ra nhận xét về các cột id, middle_name, current_status.<br>



