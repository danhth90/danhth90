---
layout: post
title: Install active directory on window server 2012,
categories: sharepoint windowserver
---

Bài viết này sẽ hướng dẫn các bạn cài đặt Active Directory® role trên máy Microsoft® Windows Server® 2012 server, cấu hình domain controller.

# Install Active Directory

Mở **Server Manager** trên thanh task bar, chọn mục số 2 **Add roles and features**

![Add Role and Features Window Server 2012 R2](https://i.ibb.co/6JKCsTC/Server-manager-1.png)
*img-1*

![Before begin Add Role](https://i.ibb.co/GvRgh9v/Server-manager-2.png)
*img-2* click **Next** để bỏ qua bước Before you begin

![Installation Type Role and Feature Window Server 2012 R2](https://i.ibb.co/dpFjj0C/Server-manager-3.png)
*img-3* chọn **Role-base or feature-base installation**, click **Next**

![Server Selection](https://i.ibb.co/G0G4L3W/Server-manager-4.png)
*img-4* click **Next**

![Server Selection](https://i.ibb.co/ftrqLs6/Server-manager-5.png)
*img-5* check roles **Active Directory Domain Services**

![Server Selection](https://i.ibb.co/dgZgjMd/Server-manager-6.png)
*img-6* tại dialog, click chọn **Add Features**

![Server Selection](https://i.ibb.co/bWPwhsS/Server-manager-7.png)
*img-7* Xem lại thông tin tại tab **AD DS** và click **Next**

![Server Selection](https://i.ibb.co/KVGHmp3/Server-manager-8.png)
*img-8* Xem lại thông tin **Confirm installation selections** và click **Install**