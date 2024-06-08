+++
author = "zhaviran"
title = "Konfigurasi VLAN"
date = "2024-04-01"
description = "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
tags = [
    "markdown",
    "css",
    "html",
]
categories = [
    "themes",
    "syntax",
]
series = ["Themes Guide"]
aliases = ["migrate-from-jekyl"]
+++

This article offers a sample of basic configuration of VLAN

<!--more-->
## Topologi

![images](https://citraweb.com/images/artikel/vlan_management/01.png)

## Configuration

Konfigurasi pada router, IP Address untuk management terpasang pada interface yang mengarah ke switch.

![images](https://citraweb.com/images/artikel/vlan_management/02.png)

## Dan konfigurasi pada switch adalah sebagai berikut:

Pada kasus ini ether1 adalah trunk, ether2, dan ether3 adalah port access yang akan digunakan untuk client

![images](https://citraweb.com/images/artikel/vlan_management/03.png)

Pertama, buat bridge untuk ether1 (trunk), ether2 (access), dan ether3 (access). Jangan lupa tentukan pvid untuk port access, detail cek pada gambar berikut:
![images](https://citraweb.com/images/artikel/vlan_management/04.png)
![images](https://citraweb.com/images/artikel/vlan_management/05.png)
![images](https://citraweb.com/images/artikel/vlan_management/06.png)
![images](https://citraweb.com/images/artikel/vlan_management/07.png)

## Kemudian konfigurasikan pada tab VLANs

![images](https://citraweb.com/images/artikel/vlan_management/08.png)
![images](https://citraweb.com/images/artikel/vlan_management/09.png)

Jangan lupa aktifkan vlan filtering pada bridge yang kita buat tadi

![images](https://citraweb.com/images/artikel/vlan_management/10.png)

Selanjutnya konfigurasikan IP address untuk vlan management pada interface bridge yang sudah dibuat tadi.
![images](https://citraweb.com/images/artikel/vlan_management/11.png)

