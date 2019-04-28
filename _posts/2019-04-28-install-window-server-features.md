---
layout: post
title: How to install window server 2008 r2
categories: sql sharepoint
description: Hướng dẫn cài đặt SQL Server 2008 R2 để cài đặt sharepoint 2010 trên window server 2012R2
video: https://www.youtube.com/embed/PvJ6rtm6zW4
next: install-window-server-features
prev: install-net-framework-3-5-on-window-server-2012-r2
---

# 2. Cài đặt **Server Roles** & **Features**

Mở **Server Manager** trên thanh task bar, chọn mục số 2 **Add roles and features**

![Add Role and Features Window Server 2012 R2](https://i.ibb.co/6JKCsTC/Server-manager-1.png)
*img-1:* Server manager, click next cho đến khi tab **Server Roles** được chọn

![Select role Application Server](https://i.ibb.co/1Q9xR8Y/window-server-features-1.png)
*img-2:* check role **Application Server**, scroll xuống

![Select role Web Server (IIS)](https://i.ibb.co/fFQJKSh/window-server-features-2.png)
*img-2:* check role **Web Server (IIS)**, Nhấn **Next**

![Add roles and features](https://i.ibb.co/C2CTH9L/window-server-features-3.png)
*img-2:* Nhấn **Add Features**

![Select feature Windows Identity Foundation 3.5](https://i.ibb.co/Ry2kVmc/window-server-features-4.png)
*img-2:* check features ** Windows Identity Foundation 3.5**, Nhấn **Next**

# 3. Cài đặt Role Services **Application Server**

![Application Server Role Services](https://i.ibb.co/xhNqLpJ/window-server-features-5.png)
*img-2:* check các role sau
 * .NET Framework 4.5
 * Distributed Transasctions
   * Incoming Network Transactions
   * outgoing Network Transactions
 * TCP Port Sharing
 * Windows Process Activation Service Support
   * HTTP Activation
   * TCP ACtivation

Nhấn **Next**

# 4. Cài đặt Role Services **Web Server Role (IIS)**

![Web Server Role (IIS)](https://i.ibb.co/BTgR8jc/window-server-features-6.png)
*img-2:* **Common HTTP Features** check các role services sau
 * Default Document
 * Directory Browsing
 * HTTP Errors
 * Static Content

![Web Server Role (IIS)](https://i.ibb.co/6bw9xRG/window-server-features-7.png)
*img-2:* **Health and Diagnostics** check các role services sau
 * HTTP Logging
 * Custom Logging
 * Logging Tools
 * Request Monitor
 * Tracing

![Web Server Role (IIS)](https://i.ibb.co/6bw9xRG/window-server-features-7.png)
*img-2:* **Performance** check các role services sau
 * Static Content Compression

![Web Server Role (IIS)](https://i.ibb.co/x8cZqWT/window-server-features-8.png)
*img-2:* **Security** check các role services sau
 * Request Filtering
 * Basic Authentication
 * URL Authorization
 * Window Authentication

![Web Server Role (IIS)](https://i.ibb.co/J58Tr0t/window-server-features-9.png)
*img-2:* **Application Development** check các role services sau
 * .NET Extensibility 3.5
 * .NET Extensibility 4.5
 * ASP
 * ASP.NET 3.5
 * ASP.NET 4.5
 * CGI
 * ISAPI Extentsions
 * ISAPI Filters
 * Server Side Includes

![Web Server Role (IIS)](https://i.ibb.co/CPZzyyL/window-server-features-10.png)
*img-2:* **Management Tools** check các role services sau
 * IIS Management Console
 * IIS 6 Management Compatibility
   * IIS 6 Metabase Compatibility
   * IIS 6 Management Console
   * IIS 6 Scriptiong Tools
   * IIS 6 WMI Compatibility
 * Management Scripts and Tools
 * Management Servcice
Nhấn **Next** cho đến tab Confirmtion thì nhấn **Install** và chờ đến khi cài đặt kết thúc