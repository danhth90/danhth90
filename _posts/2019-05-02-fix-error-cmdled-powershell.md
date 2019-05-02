---
layout: post
title: Fix lỗi 'cmdlets with featuredependencyid are not registered'
categories: sharepoint
description: Hướng dẫn fix lỗi powershell 'the local farm is not accessible. cmdlets with featuredependencyid are not registered' khi cài sharepoint 2010 trên window server 2012R2
video: https://www.youtube.com/embed/PvJ6rtm6zW4
next: install-sharepoint-2010-on-window-server-2012-r2
prev: install-net-framework-3-5-on-window-server-2012-r2
---

# 2. Chuẩn bị

Copy đoạn lệnh sau vào file txt
>C:\Windows\System32\WindowsPowerShell\v1.0\PowerShell.exe -Version 2 -NoExit  " & ' C:\Program Files\Common Files\Microsoft Shared\Web Server Extensions\14\CONFIG\POWERSHELL\Registration\\sharepoint.ps1 ' "

# 3. Vấn đề

Khi chạy **Sharepoint 2010 Management Shell**, bạn nhận được một trong hai thông báo lỗi sau:
  * "Microsoft SharePoint is not supported with version 4.0.30319 of the Microsoft .Net runtime"
  * "The local farm is not accessible. cmdlets with feature dependency are not registered."

# 4. Giải quyết
