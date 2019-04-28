---
layout: post
title: Install active directory on window server 2012
categories: sharepoint windowserver
video: https://www.youtube.com/embed/U_sSp8vvvDw
---

Bài viết này sẽ hướng dẫn các bạn cài đặt Active Directory® role trên máy Microsoft® Windows Server® 2012 server, cấu hình domain controller.

# 2. Install Active Directory

Mở **Server Manager** trên thanh task bar, chọn mục số 2 **Add roles and features**

![Add Role and Features Window Server 2012 R2](https://i.ibb.co/6JKCsTC/Server-manager-1.png)
*img-1*

![Before begin Add Role](https://i.ibb.co/GvRgh9v/Server-manager-2.png)
*img-2:* click **Next** để bỏ qua bước Before you begin

![Installation Type Role and Feature Window Server 2012 R2](https://i.ibb.co/dpFjj0C/Server-manager-3.png)
*img-3:* chọn **Role-base or feature-base installation**, click **Next**

![Installation Type](https://i.ibb.co/G0G4L3W/Server-manager-4.png)
*img-4:* click **Next**

![Server Roles Active Directory Domain Services](https://i.ibb.co/ftrqLs6/Server-manager-5.png)
*img-5:* check roles **Active Directory Domain Services**

![Confirm add features Active Directory Domain Services](https://i.ibb.co/dgZgjMd/Server-manager-6.png)
*img-6:* tại dialog, click chọn **Add Features**

![Preview information](https://i.ibb.co/bWPwhsS/Server-manager-7.png)
*img-7:* Xem lại thông tin tại tab **AD DS** và click **Next**

![Confirm Install Roles Active Directory Servics](https://i.ibb.co/KVGHmp3/Server-manager-8.png)
*img-8:* Xem lại thông tin **Confirm installation selections** và click **Install**

# 3. Configure Active Directory

Sau khi cài đặt AD DS role hoàn tất, bước tiếp theo, chúng ta sẽ tiến hành cấu hình domain như sau

![Notify panel](https://i.ibb.co/84bx9bg/Configure-domain-1.png)
*img-9*
*-Bước 1:* Mở **Notify panel**
*-Bước 2:* click **Promote this server to a domain controller** để thực hiện cấu hình

![Register domain name](https://i.ibb.co/FXcL5ks/Configure-domain-2.png)
*-img-10:* Tại tab **Deployment Configuration** thực hiện như sau:
*-Bước 1:* Check **Add a new forest**
*-Bước 2:* click vào textbox **Root domain name** nhập tên domain.
*-Bước 3:* click **Next**.

![input password administrator domain](https://i.ibb.co/5Gvq2Zv/Configure-domain-3.png)
*img-11:* Tại tab **Domain Controller Options** thực hiện như sau:
*-Bước 1:* Nhập **Password**
*-Bước 2:* Nhập lại **Password** Confirm.
*-Bước 3:* click **Next**.

![DNS Options](https://i.ibb.co/sFQvhCb/Configure-domain-4.png)
*img-12:* click **Next**.

![Additional Options](https://i.ibb.co/R2xWsrT/Configure-domain-5.png)
*img-13:* click **Next**.

![Paths location of the AD DS database](https://i.ibb.co/pXFSkwD/Configure-domain-6.png)
*img-14:* click **Next**.

![Review your selection](https://i.ibb.co/bz9ZJwX/Configure-domain-7.png)
*img-15:* Xem lại toàn bộ thông tin đã cấu hình, click **Next**.

![install promotion operation](https://i.ibb.co/6YvVG6C/Configure-domain-8.png)
*img-16:* click **Install** và chờ đợi đến khi hoàn tất.

![Result successfully configured](https://i.ibb.co/tbtDvjT/Configure-domain-9.png)
*img-17:* click **Close** và kết thúc quá trình cấu hình.

Đến đây thì việc cấu hình domain đã hoàn tất, tiến hành khởi động lại server và xem kết quả

![Result successfully configured](https://i.ibb.co/WDrTmdC/Configure-domain-10.png)
*img-18:* Domain controller đã được cài đặt thành công.