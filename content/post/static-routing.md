+++
author = "zhaviran"
title = "Static Routing"
date = "2024-04-01"
description = "Lorem Ipsum Dolor Si Amet"
tags = [
    "markdown",
    "text",
]
weight = 10
+++

## Topologi 1

![images](https://citraweb.com/images/artikel/Simple-Static-Route/Routing1.png)

Topologi yang paling sederhana. Router A dan Router B direct connect / terhubung langsung via ethernet. Maka pengaturan routing yang perlu ditambahkan sebagai berikut

### Router A

![images](https://citraweb.com/images/artikel/Simple-Static-Route/routing1-A.png)

### Router B

![images](https://citraweb.com/images/artikel/Simple-Static-Route/routing1-b.png)

Cukup mudah bukan??

Sekarang bagaimana kalau router A dan router B tidak bisa direct connect, mungkin harus melewati perangkat lain, misalnya link wireless, atau mungkin tunnel / VPN?.
Contoh berikutnya yaitu topologi 2.

## Topologi 2

![images](https://citraweb.com/images/artikel/Simple-Static-Route/Routing2.png)

Disini Router A dan Router B supaya bisa berkomunikasi harus melewati perangkat lain yang melakukan BRIDGING. Pada umumnya, perangkat-perangkat router / wireless bisa melakukan fungsi bridging. Ciri paling mudah mengenali perangkat yang dilewati (dalam contoh ini perangkat wireless) apakah melakukan bridging atau tidak adalah IP Router A, IP wireless router/perangkat lain dan IP Router B memiliki IP segment yang sama (10.10.10.x/24)
Karena Router A dan Router B memiliki IP segment yang sama, maka metode routingnya sama dengan contoh topologi 1. Tinggal disesuaikan IPnya

### Router A

![images](https://citraweb.com/images/artikel/Simple-Static-Route/routing2-A.png)

### Router B

![images](https://citraweb.com/images/artikel/Simple-Static-Route/routing2-B.png)

Dari kedua contoh topologi diatas, mungkin masih terlalu sederhana. Mari kita ulas untuk topologi yang sedikit lebih kompleks.

[Simple Static Route](https://citraweb.com/artikel/44/)

<svg class="canon" xmlns="http://www.w3.org/2000/svg" overflow="visible" viewBox="0 0 496 373" height="373" width="496"><g fill="none"><path stroke="#000" stroke-width=".75" d="M.599 372.348L495.263 1.206M.312.633l494.95 370.853M.312 372.633L247.643.92M248.502.92l246.76 370.566M330.828 123.869V1.134M330.396 1.134L165.104 124.515"></path><path stroke="#ED1C24" stroke-width=".75" d="M275.73 41.616h166.224v249.05H275.73zM54.478 41.616h166.225v249.052H54.478z"></path><path stroke="#000" stroke-width=".75" d="M.479.375h495v372h-495zM247.979.875v372"></path><ellipse cx="498.729" cy="177.625" rx=".75" ry="1.25"></ellipse><ellipse cx="247.229" cy="377.375" rx=".75" ry="1.25"></ellipse></g></svg>

{{< css.inline >}}

<style>
.canon { background: white; width: 100%; height: auto; }
</style>

{{< /css.inline >}}
