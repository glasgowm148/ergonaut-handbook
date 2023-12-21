---
title: Penjelajah
description: 
published: true
date: 2023-12-21T12:31:31.652Z
tags: 
editor: markdown
dateCreated: 2023-12-21T12:31:31.652Z
---

> https://explorer.ergoplatform.com/en/
{.is-info}

Kita akan melihat lebih dekat ke dalam format alamat Ergo. Selain itu, kita akan menjelaskan bagaimana cara kerjanya secara spesifik serta apa yang membuatnya lebih disukai daripada jenis alamat blockchain lainnya.

Mari kita mulai dari yang paling awal.

Pada saat Anda memasang dompet mata uang kripto, Anda secara otomatis membuat alamat dengannya. Secara sangat longgar, Anda dapat membandingkan dompet dengan rekening bank tradisional dan alamat dengan nomor rekening yang sesuai. Alamat alfanumerik inilah yang dibutuhkan untuk mengirim uang dari orang A ke orang B, menerima uang, atau menarik reward penambangan Anda. Jika Anda ingin mulai menggunakan dompet Ergo dan mempelajari fungsinya lebih dalam, lihat tautan berikut.

Sekarang, apa sebenarnya alamat itu?

Alamat adalah sebuah string pendek yang berhubungan dengan skrip tertentu dan digunakan untuk melindungi sebuah kotak (postingan yang dipublikasikan oleh pengembang inti kushti di forum kami menjelaskan dengan baik apa itu "kotak"). Tidak seperti representasi biner (yang dikodekan dengan heksa) dari sebuah skrip, sebuah alamat Ergo menggunakan pengkodean Base58 dan oleh karena itu memiliki beberapa karakteristik yang sangat berguna yang tidak dimiliki oleh representasi biner:


    Integritas sebuah alamat dapat dengan mudah diperiksa melalui checksum terintegrasi (yang merupakan "datum berukuran kecil yang berasal dari sebuah blok data digital dengan tujuan untuk mendeteksi kesalahan yang mungkin terjadi selama transmisi atau penyimpanan", menurut Wikipedia).
    Awalan alamat menunjukkan kepada Anda jaringan dan jenis alamat. Secara khusus, awalan jaringan mencegah Anda salah mengirim token mainnet ke alamat testnet.
    Alamat tersebut menggunakan pengkodean (yaitu, Base58 seperti yang telah disebutkan) yang menghindari karakter yang terlihat mirip dan ramah terhadap klik dua kali dan juga pemenggalan baris pada email.
    Sebuah alamat mengkodekan tipe jaringan, tipe alamat, checksum, dan informasi yang cukup untuk berhubungan dengan skrip tertentu.

Mari kita lihat byte awalan yang berisi informasi tentang jenis jaringan dan alamat:

Jenis jaringan yang mungkin adalah:

    Mainnet - 0x00
    Testnet - 0x10

Jenis alamat adalah (semantik yang dijelaskan di bawah):

    0x01 - Pay-to-PublicKey(P2PK) address
    0x02 - Pay-to-Script-Hash(P2SH)
    0x03 - Pay-to-Script(P2S)

Untuk jenis alamat, kami membentuk byte konten sebagai berikut:

    P2PK - serialized (compressed) public key
    P2SH - first 192 bits of the Blake2b256 hash of serialized script bytes
    P2S - serialized script (this is where mining rewards go!)

Sebagai contoh, mengirimkan 10 Erg ke alamat P2PK biasanya berarti bahwa transaksi yang sesuai akan berisi sebuah kotak yang di dalamnya terdapat 10 Erg yang dikunci oleh kunci publik yang dikodekan dalam alamat P2PK. Sama halnya dengan alamat P2S, kotak tersebut akan dikunci oleh sebuah skrip yang dikodekan dalam alamat tersebut. Dalam kasus yang paling rumit dari skrip P2SH, kotak akan dilindungi oleh skrip khusus yang telah ditentukan sebelumnya yang mengambil 192 bit pertama dari nilai hash Blake2b256 untuk skrip yang akan ditampilkan oleh input yang menggunakan kotak tersebut.

Berikut ini adalah contoh bagaimana alamat tertentu akan terlihat pada testnet:

    3 - P2PK (3WvsT2Gm4EpsM9Pg18PdY6XyhNNMqXDsvJTbbf6ihLvAmSb7u5RN)
    ? - P2SH (rbcrmKEYduUvADj9Ts3dSVSG27h54pgrq5fPuwB)
    ? - P2S (Ms7smJwLGbUAjuWQ)

Dan inilah tampilannya di mainnet kami:

    9 - P2PK (9fRAWhdxEsTcdb8PhGNrZfwqa65zfkuYHAMmkQLcic1gdLSV5vA)
    ? - P2SH (8UApt8czfFVuTgQmMwtsRBZ4nfWquNiSwCWUjMg)
    ? - P2S (4MQyML64GnzMxZgm, BxKBaHkvrTvLZrDcZjcsxsF7aSsrN73ijeFZXtbj4CXZHHcvBtqSxQ)

Rangkuman singkatnya:

    Prefix byte = network type + address type (for example, P2S script on the testnet starts with 0x13 before Base58)
    checksum = leftmost_4_bytes (blake2b256 (prefix byte || content bytes))
    address = prefix byte || content bytes || checksum

Jika semua hal ini menarik minat Anda, Anda dapat bergabung dengan komunitas kami dan mengajukan pertanyaan lebih lanjut di saluran telegram dan/atau forum kami. Sampai jumpa di sana!