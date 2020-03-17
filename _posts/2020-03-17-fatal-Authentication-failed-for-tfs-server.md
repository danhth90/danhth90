---
layout: post
title: Fix fatal: Authentication failed for 'http://tfs2017:8080/tfs *
categories: sharepoint
description: 
---

# Lỗi `fatal: Authentication failed for 'http://tfs2017:8080/tfs/MHS/_git/SureHIS-GT/'`


![Error faltal](https://ibb.co/GH0RTVL)

Cách xử lý

* search `Credential Manager` chuyển qua tab `Windows Credentials`
* Tìm khu vực `Generic Credentials` click **Add a generic credential**
* Nhập thông tin:
*  Internet or network address: **git:http://tfs2017:8080**
*  User name: **lvdomain\[username]**
*  Password: **Password login account Lạc Việt**  