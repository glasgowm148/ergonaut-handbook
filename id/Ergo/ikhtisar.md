---
title: Ikhtisar
description: Komunitas mengumpulkan sumber daya untuk Blockchain Ergo
published: true
date: 2024-09-08T18:17:24.035Z
tags: 
editor: markdown
dateCreated: 2024-09-08T18:17:24.034Z
---

> ergonaut.space adalah sebuah ruang yang digerakkan oleh komunitas di mana setiap orang dapat berkontribusi. Hubungi @glasgowm/unomie/sigmanaut\_ di telegram/Discord/reddit untuk menambahkan bagian bahasa daerah baru.
{.is-success}


## Generasi Berikutnya dari Blockchain

Ergo adalah blockchain Proof-of-Work (PoW) Layer 1 yang menyediakan platform bagi para pengembang untuk membangun kontrak keuangan yang tidak dapat dipercaya dan memungkinkan keuangan akar rumput yang terdesentralisasi dan peer-to-peer.

Ergo memprioritaskan fitur-fitur yang berguna tanpa mengorbankan keamanan dengan model pengembangan yang digerakkan oleh penelitian namun tetap praktis. 

*Ergo*, **platform yang tangguh untuk uang kontrak**



- Lihat [Ergo Wiki](https://github.com/ergoplatform/ergo/wiki) di GitHub

> *"Ini adalah salah satu mata uang kripto paling revolusioner yang pernah dibuat. Memiliki begitu banyak ide gila seperti protokol sigma dan pemangkasan blockchain dan roller chain. Semua hal gila ini. Bahkan memiliki bukti tidak ada premine. Jadi benar-benar keajaiban teknologi dalam banyak hal, dan ini mencerminkan sekitar 8 tahun pengetahuan yang telah dikumpulkan Alex sebagai peneliti dan pengembang. Kode yang sangat ringkas dan membuat saya heran dengan kapitalisasi pasarnya. Seharusnya ini menjadi 10 koin teratas atau 15 koin teratas “* - Charles Hoskinson



## Dipimpin oleh penelitian tetapi berfokus pada dunia nyata

Token asli Ergo Platform, ERG, digunakan untuk membayar semua biaya transaksi untuk transfer dan eksekusi kontrak pintar. [Biaya penyimpanan](/en/Glossary/Sewa-Penyimpanan) juga dibebankan pada akun yang tidak aktif, memberikan insentif yang berkelanjutan bagi para penambang bahkan setelah hadiah blok berakhir. Model ekonomi baru ini memastikan jaringan yang berkelanjutan. ERG berfungsi sebagai token inti dan akan digunakan untuk jaminan dApps yang berbeda seperti stablecoin dan banyak aplikasi lainnya. Penggunaan tanda tangan ring dan ambang batas di luar pasak mendukung dApps non-kustodian dan non-interaktif seperti ErgoMixer untuk ERG dan token khusus.

Token khusus adalah token warga negara kelas satu di Ergo; ada juga pertukaran atom yang dibangun untuk mereka di dalam inti. Token khusus dapat didistribusikan kepada penambang dan pemangku kepentingan ekosistem lainnya, menggunakan kontrak pintar yang ditentukan secara logis, termasuk jadwal emisi gaya PoW bawaan.

Ergo dirancang dari awal (termasuk algoritme POW-nya [Autolykos v2] (/en/Glossary/Autolykos) dan tahan terhadap memori, ramah terhadap GPU, dan berdasarkan keadilan. Tim Ergo percaya bahwa jaringan harus beradaptasi dengan perubahan lingkungan tanpa campur tangan pihak-pihak yang dipercaya, sehingga memiliki protokol pemungutan suara penambang on-chain yang memungkinkan perubahan bertahap dalam sejumlah besar parameter, termasuk ukuran blok maksimum, faktor biaya penyimpanan, dan banyak lagi. Untuk perubahan yang lebih mendasar, Ergo mencoba mengikuti pendekatan kemampuan soft-fork. Jika sebagian besar jaringan menerima fitur baru, maka fitur tersebut akan diaktifkan, namun, node lama yang tidak meng-upgrade akan terus beroperasi secara normal dan melewatkan validasi fitur ini.

Ergo dirancang untuk menjadi protokol yang dapat diubah sendiri yang memungkinkannya untuk menyerap ide-ide baru dan meningkatkan dirinya sendiri dengan cara yang terdesentralisasi.

## Kuat tetapi aman

Dalam berbagai pengalaman kami dalam bekerja dengan platform blockchain, kami telah mempelajari bahwa smart contract konvensional yang lengkap dengan Turing mungkin sangat kuat, tetapi bisa berisiko. Menerapkan tugas komputasi yang kompleks pada blockchain dapat menimbulkan konsekuensi yang tidak diinginkan. Kondisi jaringan, bug, dan eksploitasi kode dapat membuat kita tidak dapat mengetahui seberapa mahal biaya yang dibutuhkan untuk mengeksekusi perangkat lunak - atau apakah kode tersebut akan berjalan sebagaimana mestinya. Hal ini dapat menyebabkan kerentanan keamanan dan dApps yang salah.

Kontrak pintar Ergo memungkinkan kita untuk mengeksekusi tugas yang luas, tetapi kita selalu tahu sebelumnya berapa biaya kode dan apakah kode tersebut akan berjalan dengan sukses. Sementara itu, kita masih dapat menulis skrip lengkap Turing dengan mengulangi proses di beberapa blok. Ini berarti Ergo dapat mendukung dApps serbaguna yang dapat diprediksi, dengan biaya yang diketahui, dan tidak memiliki bahaya dari fungsionalitas yang tidak dibatasi.

## Cerdas namun lugas

Protokol Sigma adalah fondasi kontrak pintar Ergo. Protokol ini memungkinkan kelas protokol tanpa pengetahuan yang efisien yang memungkinkan kita untuk mengimplementasikan tugas-tugas yang sebelumnya tidak mungkin dilakukan atau berisiko dan mahal.

Sebagai contoh, protokol Sigma memungkinkan kita untuk mengimplementasikan tanda tangan cincin dan ambang batas di luar kotak. Katakanlah Anda ingin membuat sebuah 'kontrak pembelanjaan cincin', di mana salah satu dari kita bisa melakukan transaksi dari alamat yang sama, tetapi kita tidak ingin orang lain mengetahui siapa di antara kita yang membelanjakan dana tersebut. Hal itu tidak mungkin dilakukan dengan Bitcoin. Meskipun Ethereum dapat melakukannya dengan Ethereum, namun akan menjadi mahal dan rumit - terutama dengan ukuran lingkaran 10 atau 20 anggota, yang diperlukan untuk privasi yang kuat.

Dengan Ergo, aplikasi semacam ini dapat dibuat dengan cepat, berkat integrasi protokol Sigma di dalam intinya. Hal ini memungkinkan privasi tingkat aplikasi yang berdaulat: skrip tanpa kepercayaan yang dapat digunakan untuk mengakses mixer atau fungsionalitas lain tanpa memerlukan pihak ketiga.

## Aman tetapi dapat diakses

Setiap skrip diterapkan pada output yang tidak terpakai. Kami telah mengambil fitur ini dari protokol Bitcoin, yang menggunakan UTXO atau model 'koin' daripada model 'akun' seperti Ethereum. Kami menganggap ini sebagai pendekatan yang lebih aman karena kotak tidak dapat diubah, dan juga lebih fleksibel.

***Autolykos v2*** 

Blockchain Ergo menggunakan algoritma Autolykos2 untuk konsensus, yang merupakan versi yang sangat dioptimalkan dari Autolykos asli, **dengan pool-resistance dimatikan**. 

Autolykos yang asli adalah varian dari Equihash dan menawarkan ketahanan ASIC yang lebih baik dan tingkat resistensi pool. Hal ini memungkinkan desentralisasi yang lebih baik, menghindari kumpulan besar yang dapat berkolusi atau dipaksa untuk menyerang jaringan. Pada saat yang sama, kami menyadari bahwa pengguna biasa yang tidak menjalankan node penuh harus menikmati manfaat keamanan yang sama dengan penambang. Proof-of-proof-of-work (NiPoPoW) non-interaktif dari Ergo memungkinkan siapa saja untuk membuat dan memverifikasi transaksi dengan penuh keyakinan, tanpa memerlukan penyimpanan, bandwidth, dan waktu yang dibutuhkan untuk mengunduh blockchain secara penuh. Hanya dibutuhkan data sebesar 1 MB - yang berarti perangkat apa pun dapat digunakan.

> Dalam hal keamanan, kami selalu mencoba untuk menggunakan pendekatan yang paling mudah dan telah dipelajari dengan baik; jika tidak, untuk membahas arah baru dengan makalah yang diterbitkan dan banyak pengujian. Kami mempertimbangkan beberapa hal secara serius yang hanya diperbaiki oleh proyek lain setelah terjadi serangan, misalnya kontrak spam (yang menyebabkan “dilema verifikator”).

## Deflasi tetapi berkelanjutan secara ekonomi

Seperti banyak fitur lain di Ergo, model ekonomi jaringan didasarkan pada pendekatan Bitcoin. Kami percaya bahwa kelangkaan digital sangat penting untuk menopang nilai dan membatasi pasokan koin di bawah 100 juta ERG. ~~Tidak seperti Bitcoin, imbalan blok akan terus menurun setelah dua tahun pertama, tanpa adanya emisi yang panjang. Imbalan blok mulai dari 75 ERG, dan setelah delapan tahun akan turun menjadi nol, setelah itu total pasokan akan ditetapkan.~~

<div class=“panel panel-info”>

  ** PEMBARUAN: EMISI yang ditargetkan kembali dengan EIP-27**{: .panel-heading}


> Lihatlah [Ergos Reemission Vote EIP27: A Path to Sustained Growth?] (https://ergoplatform.org/en/blog/Ergos-Reemission-Vote-EIP27-A-Path-to-Sustained-Growth/) untuk mengetahui informasi rinci mengenai jadwal emisi 8 tahun Ergo yang semula. EIP-27 menampilkan kemampuan rantai untuk mengubah dirinya sendiri/berkembang, dengan cara yang terdesentralisasi. Mirip dengan EIP-27, sebagian besar perubahan protokol Ergo akan terjadi tanpa rasa sakit, melalui garpu yang lembut dan halus. 
{.is-info}

Selain biaya transaksi, para penambang juga akan mendapatkan keuntungan dari [Biaya Sewa Penyimpanan] (https://ergonaut.space/en/Glossary/Storage-Rent) yang dibebankan pada kotak (UTXO) yang tidak bergerak (tetap “tidak terpakai”) selama empat tahun atau lebih. Setidaknya ada dua keuntungan dari pendekatan ini. Pertama, pendekatan ini memberikan penambang sebuah sumber pendapatan tambahan setelah reward blok berakhir. Karena keamanan jaringan bergantung pada tingkat hash dan partisipasi penambang, ini merupakan insentif yang signifikan untuk diberikan. Kedua, ini memiliki efek mendaur ulang koin yang hilang (dan debu) kembali ke dalam ekonomi Ergo. Penelitian menunjukkan bahwa hingga 4 juta BTC telah dihapus secara permanen dari peredaran karena private key yang hilang. Biaya penyimpanan Ergo perlahan-lahan akan mendapatkan kembali koin-koin tersebut untuk tujuan produktif, sementara pengguna yang ingin menyimpan koin dalam jangka panjang dapat menghindari biaya penyimpanan dengan memindahkan dana mereka.

## PoW ditambang tetapi didanai oleh protokol

Ada keseimbangan yang sulit antara memastikan proyek didanai secara memadai dan berpotensi merugikan pengguna selanjutnya jika sebagian besar token ditambang atau dicadangkan dalam ICO. Kami telah memilih strategi yang telah terbukti berhasil untuk mata uang kripto lainnya, di mana persentase token dari setiap hadiah blok dialokasikan untuk pengembangan dan pemasaran.

Dalam kasus Ergo, token Foundation ini dikelola oleh kontrak pintar yang dibangun ke dalam protokol. 10% dari setiap hadiah blok untuk dua tahun pertama, atau 7,5 ERG per blok, dialokasikan ke Departemen Keuangan, dengan 67,5 ERG sisanya diberikan kepada para penambang. Ketika hadiah blok mulai berkurang setelah dua tahun, Yayasan akan terus menerima hadiah lebih dari 67,5 ERG, dengan alokasi Treasury turun menjadi nol setelah 2,5 tahun.

## Dipimpin oleh konsensus tetapi mudah beradaptasi

Ergo dirancang dan diimplementasikan oleh tim pengembang dan peneliti berpengalaman yang memiliki publikasi dan gelar PhD dalam bidang kriptografi, teori kompiler, teknologi blockchain, dan e-cash kriptografi. Tim ini juga memiliki latar belakang yang kuat dalam pengembangan inti dengan kerangka kerja mata uang kripto dan blockchain seperti Nxt, Scorex, dan Waves.

Kami juga didukung oleh para pengembang komunitas, yang dapat bekerja secara sukarela atau menerima hibah dari Yayasan untuk mengimplementasikan fitur dan dApps yang bermanfaat. Sebagai contoh, ErgoMix, layanan pencampuran terdesentralisasi berdasarkan protokol Sigma, dibangun oleh pengembang pihak ketiga dari komunitas Ergo, dan bursa terdesentralisasi Ergo juga sedang dikembangkan atas dasar ini.

## Digerakkan oleh komunitas tetapi Gesit

Ergo dirancang dan diimplementasikan oleh sebuah tim yang terdiri dari para pengembang dan peneliti berpengalaman yang memiliki publikasi dan gelar PhD di bidang kriptografi, teori kompiler, teknologi blockchain, dan e-cash kriptografi. Tim ini juga memiliki latar belakang yang kuat dalam pengembangan inti dengan mata uang kripto dan kerangka kerja blockchain seperti Nxt, Scorex, dan Waves.

Kemampuan bertahan jangka panjang dan kemampuan untuk mengubah diri sendiri adalah apa yang memberi Ergo ketahanannya. Pertumbuhan yang digerakkan oleh komunitas yang konstan dan stabil: tidak ada dukungan ICO / VC dan **tidak ada pra-tambang**. 
