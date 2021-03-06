---
layout: post
title: How to install sharepoint 2010 on window server 2012 r2
categories: sharepoint
description: Vào một ngày đẹp trời như mọi ngày, đang nhâm nhi ly cafe tại quán [Ghiền cà phê Biên Hòa](https://www.facebook.com/ghiencafebienhoa) thì được thằng đồng nghiệp giới thiệu cho một job freelance (đội ơn thằng em) trong lúc túng thiếu. Mà ngặc nỗi, công nghệ từ thời cổ đại... ứng dụng trên nền tảng sharepoint 2010.
---

# 1. Bối cảnh lịch sử
Công việc đầu tiên mình làm là tiến hành cài đặt môi trường server. Giàng ơi, sharepoint 2010 thì yêu cầu chạy trên window server 2008, mà resource của mình thì toàn window server 2012 r2. Cài đặt lên môi trường này là cả một vấn đề đau đầu :v, lang man vậy thôi, vô vấn đề chính, mình sẽ log lại quá trình mình cài đặt cho bạn nào gặp hoàn cảnh giống mình. Let go.

# 2. Danh mục các bài lab hướng dẫn

* [Lab sharepoint 2010 (P1): Cài đặt Active Directory](https://danhpoint.info/install-active-directory-on-window-server-2012)
* [Lab sharepoint 2010 (P2): Cài đặt .NET Framework 3.5 Features (Offline)](https://danhpoint.info/install-net-framework-3-5-on-window-server-2012-r2).
* [Lab sharepoint 2010 (P3): Cài đặt SQL Server 2008 R2](https://danhpoint.info/install-sql-server-2008-r2).
* [Lab sharepoint 2010 (P4): Cài đặt Window Server Features và Role Services](https://danhpoint.info/install-window-server-features).
* [Lab sharepoint 2010 (P5): Cài đặt Sharepoint Server 2010](https://danhpoint.info/install-sharepoint-2010-on-window-server-2012-r2).
* [Lab sharepoint 2010 (P6): Tạo mới web application và site collection](https://danhpoint.info/create-web-application-and-site-collection)
* [Lab sharepoint 2010 (P7): Sử lỗi **'SharePoint 2010 Management Shell – .Net 4.0 runtime version error'**](https://danhpoint.info/fix-error-cmdled-powershell)
* [Lab sharepoint 2010 (P7): Restore site collection từ máy khách](https://danhpoint.info/move-sharepoint-site-from-another-machine)