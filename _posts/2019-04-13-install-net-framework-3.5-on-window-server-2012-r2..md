---
layout: post
title: Install net framework 3.5 on window server 2012 r2
categories: sharepoint windowserver
---

Tình hình là, khi cài đặt .net framework 3.5 trên window server 2012 thì nó báo lỗi **The feature Installation failed because the source files could not be found!**, hồi trên server 2008 có bao giờ bị đâu chớ, haiza!!!

Để cài đặt được .net framework 3.5 thì chúng ta lần lượt làm theo các bước sau:

# 1. Chuẩn bị

> Đĩa cài đặt window server 2012 R2 hoặc 
> file [**Disk Image ISO**](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2012-r2)

Nếu sử dụng file ISO, các bạn click chuột phải vào file cài đặt và chọn **Mount** để tạo ổ đĩa ảo
![Add Role and Features Window Server 2012 R2](https://i.ibb.co/b7G8WRq/install-dot-net-35-1.png)

# 2. Cài đặt

Mở **Server Manager** trên thanh task bar, chọn mục số 2 **Add roles and features**

![Add Role and Features Window Server 2012 R2](https://i.ibb.co/6JKCsTC/Server-manager-1.png)
*img-1:* Server manager, click next cho đến khi tab **Features** được chọn

![Select features .net framework 3.5 features](https://i.ibb.co/C0zZtXV/install-dot-net-35-3.png)
*img-2:* check features **.Net Framework 3.5 Features**, click **Next** cho đến khi tab **Confirmation** được chọn

![Confirmation installation selections](https://i.ibb.co/KxBNFDj/install-dot-net-35-4.png)
*img-3:* click vào hyperlink **Specify an altermate source path**, xuất hiện dialog **Add Roles and Features Wizard**

![Add Roles and Features Wizard - Specify Altermate Source Path](https://i.ibb.co/jJF1HPB/install-dot-net-35-5.png)
*img-4:* Điền địa chỉ vật lý ổ đĩa đã **Mount** ở bước chuẩn bị vào ô **Path**, click *OK*

![Add Roles and Features Wizard](https://i.ibb.co/KVGHmp3/Server-manager-8.png)
*img-5:* click **Install** chờ đến khi hoàn tất thì click **Close**


# 3. Kết luận
Bài viết đến đây kết thúc rồi. không có kết luận.