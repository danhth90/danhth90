---
layout: post
title: How to install SQL Server 2008 R2 on Window Server 2012 R2
categories: sql sharepoint
description: Hướng dẫn cài đặt SQL Server 2008 R2 để cài đặt sharepoint 2010 trên window server 2012R2
---

Trong bài trước, chúng ta đã cài đặt thành công "[.net framework 3.5](/install-net-framework-3.5-on-window-server-2012-r2)". Đây là bước tiền đề, để có thể cài đặt thành công **SQL Server 2008 R2** trên Window Server 2012 R2.

# Chuẩn bị

* Bộ Source cài đặt [**MS SQL Server 2008 R2**](https://www.microsoft.com/en-us/download/details.aspx?id=1279)
* Tài khoản **Administrator** hoặc quyền admin trên server.

# Cài đặt

Chạy file **setup.exe** từ bộ cài đặt, xuất hiện dialog **Program Compatibility Asistant**
![Program Compatibility Asistant](https://i.ibb.co/z66wJT1/Setup-sql-2008-r2-1.png)
*img-1:* Chọn **Run the program without getting Help**

![SQL Server Installation Center](https://i.ibb.co/ZMfNmZg/Setup-sql-2008-r2-2.png)
*img-2:* Chuyển qua tab **Installation** chọn **New installation or add features to an existing installation.**

![Input product key SQL Server 2008 R2](https://i.ibb.co/JqZTg9X/Setup-sql-2008-r2-4.png)
*img-3:* Nhập **Product Key**, nhấn **Next**

![Accept Liense Terms](https://i.ibb.co/1Q9VH33/Setup-sql-2008-r2-5.png)
*img-4:* Check **I accept the lcense terms**, nhấn **Next**

![Setup Support Rules](https://i.ibb.co/nwRmcQk/Setup-sql-2008-r2-6.png)
*img-5:* Nếu xảy ra lỗi **Windows Firewall** trong quá trình kiểm tra, thì tiến hành vào **Server Manager** turn off **Windows Firewall**, nhấn **Next**

![Setup role](https://i.ibb.co/SxtKnTj/Setup-sql-2008-r2-8.png)
*img-6:* Check **SQL Server Fearture Installation**, nhấn **Next**

![Feature Selection](https://i.ibb.co/qr4WqyF/Setup-sql-2008-r2-9.png)
*img-7:* Check chọn các features sau:
* Database Engine Services
*  Full-Text Search
* Analysis Services
* Reporting Services
* Management Tools - Basic
*  Management Tools - Complete
* Microsoft Sync Framework
nhấn **Next**

![Server Configuration - Service Accounts](https://i.ibb.co/gJ9jH6t/Setup-sql-2008-r2-10.png)
*img-8:* Click **Use the same account for all SQL Server services**, nhấn **Next**

![Set account run services](https://i.ibb.co/4f0sGHt/Setup-sql-2008-r2-11.png)
*img-9:* Nhập user name/password admin hoặc tài khoản có quyền admin để chạy services, nhấn **OK**

![Server Configuration - Service Accounts](https://i.ibb.co/N3KmdgT/Setup-sql-2008-r2-12.png)
*img-10:* Nhập user name/password admin hoặc tài khoản có quyền admin để chạy services, nhấn **Next**

![Database Engine Configuration](https://i.ibb.co/Hrp3XJB/Setup-sql-2008-r2-13.png)
*img-11:* Thực hiện các thao tác sau:
* Check **Mixed Mode (SQL Server authentication and Windows authentication)**
*  Nhập **password** cho tài khoản ***sa***
*  Nhập lại mật khẩu giống với mật khẩu vừa nhập
* Click button **Add Current User**
nhấn **Next**

![Analysis Services Configuration](https://i.ibb.co/vV7Bfyr/Setup-sql-2008-r2-14.png)
*img-12:* Click button **Add Current User**, nhấn **Next**

![Reporting Services Configuration](https://i.ibb.co/8M7qHws/Setup-sql-2008-r2-15.png)
*img-13:* Check **Install the native mode default configuration**, nhấn **Next**

![Eror Reporting](https://i.ibb.co/cCXVt63/Setup-sql-2008-r2-16.png)
*img-14:* nhấn **Next**

![installation Configuration Rules](https://i.ibb.co/BsTmrRr/Setup-sql-2008-r2-17.png)
*img-15:* nhấn **Next**

![Ready to install](https://i.ibb.co/FDsmpBs/Setup-sql-2008-r2-18.png)
*img-16:* nhấn **Install** và chờ đợi cho đến khi hoàn tất

![Complete](https://i.ibb.co/qdRDWdN/Setup-sql-2008-r2-19.png)
*img-16:* nhấn **Close**

## Hết