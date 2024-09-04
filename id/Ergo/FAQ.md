---
title: PERTANYAAN YANG SERING DIAJUKAN (FAQ)
description: 
published: true
date: 2024-09-04T19:33:46.005Z
tags: 
editor: markdown
dateCreated: 2023-12-19T15:33:30.411Z
---

## Mengapa Proof-of-Work?

Ergo didasarkan pada protokol Proof-of-Work [Autolykos](/en/Glossary/Autolykos). 

Proof-of-Work (PoW) memiliki metode yang telah dicoba dan diuji, dan memberikan beberapa keuntungan dibandingkan dengan Proof-of-Stake (PoS). Anda dapat melihat Charles Hoskinson mendiskusikan beberapa manfaat tersebut dalam [AMA terbaru (timestamped)] (https://youtu.be/Y27Q3wL_Hko?t=207)

Meskipun PoS adalah protokol yang sangat aman, beberapa smart contract mungkin membutuhkan fitur keamanan teori konsensus dari PoW untuk beberapa bagian dari eksekusi mereka. Semakin besar sebuah [dApp](/en/Glossary/dApps), jika ia melakukan DeFi yang dijaminkan, semakin besar pula stake yang dimilikinya, dan karena hal ini belum sepenuhnya diselesaikan dalam konsensus Proof of Stake, maka hal ini menjadi titik lemah. Ergo menghadirkan keamanan PoW yang telah terbukti, dengan keamanan yang memadai untuk semua implementasi DApps yang lebih kompleks di atas model UTxO yang umum.  Model PoW+UTXO dipilih, daripada mencoba menerjemahkan konsep kriptografi yang sangat alami yang melekat pada PoW ke PoS, di mana implikasi teori permainan dari protokol ini sangat berbeda.

* Lihat tulisan kami di [Cardano] (https://ergonaut.space/en/Ergo/Ergo-And-Cardano) untuk informasi lebih lanjut
* [Ergo: Mengapa Proof of Work?] (https://curiaregiscrypto.medium.com/ergo-why-proof-of-work-47c9b25fae70)
* [Memasuki Era Pow Berikutnya bersama Ergo] (https://curiaregiscrypto.medium.com/entering-the-next-era-of-pow-with-ergo-e4d83530410c)

## Mengapa non-outsourceability dimatikan?

Autolykos v1 pada awalnya memiliki non-outsourceability bawaan untuk mencegah mining pool di Ergo. Namun, menjadi jelas bahwa dengan kontrak pintar, pada dasarnya tidak mungkin untuk mencegah pool. Jadi, mereka (para penambang) mematikannya sehingga tidak hanya pemain besar yang dapat memanfaatkan celah tersebut. Ergo sekarang berfokus pada kekerasan memori dalam upaya untuk menjaga penambangan seadil mungkin, yang seharusnya dapat membantu mencegah penambangan ASIC. Ada juga beberapa peningkatan untuk pooling, misalnya protokol Stratum 2. 

> "Melewati Skema Proof-of-Work yang Tidak Dapat Disalurkan Menggunakan Kontrak Cerdas Beragunan" https://ia.cr/2020/044 dipresentasikan oleh Alex Chepurnoy pada lokakarya WTSC yang terkait dengan Kriptografi Keuangan dan Keamanan Data 2020 di Malaysia

{.is-info}

* Hal ini juga dibahas di sini di 'Unblocked with Robert Kornacki' [(14:45)] (https://www.youtube.com/watch?v=2sbTMrQwWOw&feature=youtu.be)

Mining pool memiliki manfaat tertentu yang baru saja diekspos oleh Ergo, seperti distribusi token yang lebih adil untuk dApps/proyek. Hal ini sekarang tersedia untuk para penambang di GETBLOK.io, menggunakan sistem SmartPools/subpooling pertama di dunia.

## Bagaimana dengan serangan 51%?

Mining pools menawarkan sebuah penyangga terhadap serangan jaringan seperti itu karena tingkat hash didistribusikan ke ribuan penambang individu.

Aspek memori yang diperkuat dari ergo juga membuat vektor serangan ini menjadi lebih mahal karena tidak ada dukungan ASIC yang dapat disewa. Dengan rig yang dapat disewa secara kolektif saat ini, hal ini bukanlah jalan yang layak untuk melakukan serangan 51%. Secara teori, seseorang dapat membangun farm GPU besar-besaran untuk mencoba meluncurkan serangan semacam itu. Jika aktor jahat dapat menyewa gudang ASIC dan menambang di rantai kecil dengan serangan 51% adalah pilihan yang layak... jika ada offramp. 

Biasanya, serangan ini dilakukan untuk mendapatkan keuntungan dan ada dumping besar-besaran yang terjadi di bursa saat itu terjadi. Artinya, penyerang akan membuang token di bursa kemudian "membelanjakannya" kembali ke dompet mereka. Situasi bursa saat ini tidak menyediakan likuiditas untuk offramp yang layak. Dukungan ASIC yang dapat disewa bukanlah sebuah pilihan. Jadi, apakah mungkin, secara teori, ya, praktis atau mungkin, saya rasa tidak mungkin sama sekali.

Ethereum classic mungkin merupakan contoh yang buruk, karena memiliki algoritma penambangan yang sama dengan Eth. Seseorang dapat membeli lebih dari 100% hashrate yang ada pada eth classic di NiceHash. Ini bukan kasus yang sama untuk Ergo. Ergo juga percaya pada prinsip 'Penambang yang Baik', Dalam kasus Bitcoin - itu adalah hal yang baik 51% yang ada.

## Dapatkah saya menambang Erg?

Ya! Tetapi pertama-tama Anda memerlukan GPU khusus (AMD/Nvidia), lihat [mining] (https://ergonaut.space/en/Guides/Mining) untuk informasi lebih lanjut.

# Kasus Penggunaan 

**Kutipan berikut ini merupakan jawaban atas pertanyaan tentang **kasus penggunaan** Ergo. Silakan lihat [FMFW x Ergo AMA] (https://sigmanauts.medium.com/fmfw-x-ergo-ama-august-19-ee70af0d3f7e) untuk diskusi AMA lengkap dengan kushti dan Armeanio.** 

**"Ergo adalah L1 (Layer 1) dan kami memiliki banyak aplikasi yang sudah digunakan oleh komunitas atau sedang dalam proses. Stablecoin, kumpulan oracle, lelang terdesentralisasi, kumpulan DEX AMM terdesentralisasi, perdagangan jaringan terdesentralisasi, opsi terdesentralisasi, puluhan proyek NFT, permainan, penyediaan likuiditas untuk biaya yang harus dibayarkan dalam token khusus, jembatan, dll ** ** Stablecoin

 "**Saya bahkan tidak mampu mengikuti semua perkembangan di komunitas!"** -kushti

* Detail [kasus penggunaan] Ergo (https://ergonaut.space/en/Ergo/Use-Cases)

* Jelajahi [Sigmaverse.io](https://sigmaverse.io) untuk melihat seluruh dunia dApp milik Ergo 

## [dApps](/en/dApps/dApps) 

* [ErgoMixer](/en/dApps/ErgoMixer)
* [ErgoAuctions](/en/dApps/ErgoAuctions)
* ErgoUtils
* [ErgoRaffle](/en/dApps/ErgoRaffle)

**Jelajahi daftar lengkap Ergo dApps (aplikasi terdesentralisasi) di [SigmaVerse.io](https://sigmaverse.io/all-projects/?category=All)**

## [SigmaUSD](/en/dApps/SigmaUSD/Overview)

Algorithmic Stablecoin, didukung oleh sebuah cadangan yang dalam bentuknya yang paling sederhana adalah bertaruh taruhan panjang dan pendek satu sama lain. Lihat [SigmaUSD](https://ergonaut.space/en/dApps/SigmaUSD/Overview) untuk informasi lebih lanjut.

## [Spectrum](/en/dApps/ergodex) (sebelumnya ErgoDex)

**[Spectrum. DEX] (https://app.spectrum.fi/ergo/swap) adalah bursa terdesentralisasi tanpa kustodian yang memungkinkan transfer likuiditas yang cepat, mudah, dan aman di dalam dan di antara jaringan Ergo dan Cardano. Model eUTXO memberikan kemungkinan unik untuk berbagi likuiditas di antara jaringan yang berbeda. Spectrum. DEX pada akhirnya akan menampilkan AMM, Order Book, dan banyak lagi.**.

Spectrum. DEX adalah produk DeFi sumber terbuka yang mengambil bagian dalam platform Ergo dan Cardano dan sebagai konsekuensinya ada untuk tujuan kedua komunitas tersebut.

## Oracle Pools

Ada perbandingan yang solid tentang Oracle Pools di Ergo vs Chainlink yang diberikan di [ergoforum] (https://www.ergoforum.org/t/oracle-pools-a-new-oracle-model/263) (oleh Robert Kornacki, Kepala Riset @ Emurgo).

* Lihat artikel rinci kami di [Oracle-Pools](https://ergonaut.space/en/Glossary/Oracle-Pools) untuk lebih lanjut.
* [Apakah Ergo Oracle Sleeper adalah Chainlink Berikutnya?] (https://www.reddit.com/r/AltStreetBets/comments/kfxst7/is_the_ergo_oracle_sleeper_the_next_chainlink/)
* [Sebuah proyek baru berbasis Cardano menangani oracle dengan cara yang jauh berbeda dari Chainlink] (https://cointelegraph.com/news/a-new-cardano-based-project-is-handling-oracles-a-lot-differently-than-chainlink)
# Latar Belakang

## Apa saja dasar-dasarnya?

Bagian kriptografi dari skrip Ergo didasarkan pada protokol sigma dan secara alami mendukung ambang batas tanda tangan m-of-n, tanda tangan cincin, dan banyak lagi. Dengan mengingat semua ini, kami berharap ErgoScript dan desain Ergo membuatnya berguna secara unik sebagai Uang Kontraktual dengan aplikasi yang tak terhitung jumlahnya. Ergo DApps dan protokol offchain dapat diimplementasikan dengan cara yang benar-benar terdesentralisasi karena klien yang ringan.

Untuk perubahan yang lebih mendasar, Ergo mengikuti pendekatan soft-forkability - jika sebagian besar jaringan menerima fitur baru, fitur tersebut akan diaktifkan, namun, node lama yang tidak meng-upgrade akan tetap beroperasi secara normal dan hanya melewatkan validasi fitur ini. Dengan demikian, hard fork yang mengganggu seharusnya tidak diperlukan dalam Ergo.

Penambangan Ergo akan selalu stabil, tidak seperti Bitcoin dan mata uang PoW lainnya, dimana penambangan dapat menjadi tidak stabil setelah periode emisi. Kedua, pertumbuhan ukuran state menjadi terkendali dan dapat diprediksi sehingga mengurangi kebutuhan perangkat keras untuk penambang Ergo. Ketiga, dengan mengumpulkan biaya penyimpanan dari kotak yang sudah tidak terpakai, para penambang mengembalikan koin yang hilang ke dalam sirkulasi untuk mencegah penurunan pasokan yang terus menerus akibat kehilangan kunci. Untuk mencapai kemampuan bertahan, Ergo menyediakan perbaikan ekonomi selain perbaikan teknis, yang paling utama adalah komponen biaya penyimpanan yang memainkan peran penting untuk stabilitas Ergo.

Semua mata uang kripto bergantung pada kontribusi dari komunitas penelitian ilmiah. Dengan senang hati Ergo membawanya ke dalam inti! 

## Apa itu Ergo Foundation? 

Ergo Foundation adalah entitas berbasis komunitas yang berfokus pada:
1. Mempromosikan pengembangan protokol Platform Ergo yang tidak melanggar;
1. Mempromosikan adopsi dan penggunaan Ergo Platform secara luas dan token aslinya (ERG);
1. Mengembangkan ekosistem di sekitar Ergo Platform;
1. Mempromosikan penggunaan Ergo Platform dan teknologi blockchain untuk kebaikan sosial;
1. Mendukung infrastruktur yang benar-benar terdesentralisasi, dan;
1. Mendukung privasi sebagai hak asasi manusia.

Alokasi Erg dari Departemen Keuangan setara dengan 10% dari total hadiah blok selama 2 tahun pertama dan memberikan penambang hadiah blok sebesar 67, 5 Erg per blok. Setelah 2 tahun, Treasury akan terus menerima bagian dari block reward yang melebihi 67, 5 Erg, namun, ini akan menjadi 0 setelah tahun ke-2, 5 ketika block reward menjadi 66 Erg per blok.

* Informasi lebih lanjut tentang [ergoplatform.org] (https://ergoplatform.org/en/foundation/) dan [Jadwal Emisi] (https://ergoplatform.org/en/blog/2019_05_20-curve/)

## Mengapa 'Ergo'? 

"Ergo" berarti "oleh karena itu" dalam bahasa Latin, tetapi "bekerja" dalam bahasa Yunani. Saya lebih suka arti yang kedua, tetapi keduanya sama-sama bagus. Awalnya nama ini dipilih untuk menunjukkan fakta bahwa desain mata uang kripto ini adalah ERGOnomical."

## Apa itu 'EFYT'

Untuk mendanai pengembangan, promosi, acara, menukar Token Tahun Pertama Ergo ("EFYT", dibahas lebih lanjut di bawah) ke dalam Erg dan untuk mendanai kegiatan lain yang dapat memajukan platform, Ergo memiliki Treasury yang akan menerima 4, 43% dari Erg yang dilepaskan selama emisi. Selama 2 tahun pertama pasca peluncuran mainnet, Departemen Keuangan akan menerima 7, 5 Erg per blok. Mengingat bahwa hadiah blok untuk setiap blok adalah total 75 Erg, alokasi Erg Treasury setara dengan 10% dari total hadiah blok selama 2 tahun pertama dan memberikan penambang hadiah blok sebesar 67, 5 Erg per blok. Setelah 2 tahun, Treasury akan terus menerima bagian dari block reward yang melebihi 67.5 Erg, namun, ini akan menjadi 0 setelah tahun ke-2.5 ketika block reward menjadi 66 Erg per blok. Pembaca yang terbiasa dengan beberapa protokol PoW lain dengan Treasury, seperti ZCash, mungkin akan menemukan hal yang serupa, namun perlu dicatat bahwa jumlah Erg yang masuk ke Treasury hanya berjumlah 4.330.791, 5, atau 4, 43% dari total basis moneter, dan selesai hanya dalam waktu 2, 5 tahun. Hal ini dibandingkan dengan Treasury ZCash, yang merupakan 10% dari total basis moneter ZCash dan 20% dari semua koin ZCash yang diterbitkan selama 4 tahun pertama. Dengan Ergo, diharapkan pada 1 tahun setelah peluncuran mainnet, Ergo akan mencapai tingkat desentralisasi yang tinggi dengan pengembang, penambang, dan basis pengguna yang beragam. Untuk tahun pertama, Treasury akan digunakan untuk menukar EFYT pada platform Waves dengan Erg. Selama 1, 5 tahun sisanya, mekanisme pemungutan suara komunitas akan dilakukan untuk menentukan bagaimana dana Treasury dibelanjakan.

> "Distribusi EFYT saat ini dapat ditemukan [di sini] (http://dev.pywaves.org/assets/725Yv9oceWsB4GsYwyy4A52kEwyVrL5avubkeChSnL46). Perlu dicatat bahwa pasokan maksimum EFYT adalah 1.970.945, 0. Ini adalah 10% dari tahun pertama emisi token Ergo dan jumlah Erg yang sama dengan yang akan diterima oleh Departemen Keuangan, yang berarti bahwa Departemen Keuangan akan menerima 1.970.945, 0 Erg selama tahun pertama, cukup untuk menukar pasokan maksimum EFYT dengan Erg."
>
> Untuk info lebih lanjut silakan lihat: **https://ergoplatform.org/en/blog/emission/**

{.is-info}

## Di mana saya bisa membeli Erg?

* ergoplatform.org **#Bursa** 

**https://ergoplatform.org/en/get-erg/#Exchanges**

## Di mana saya bisa menyimpan Erg?

* ergoplatform.org **#Dompet** 

**https://ergoplatform.org/en/get-erg/#Wallets**

## Bagaimana saya bisa mempertaruhkan Erg saya?

Ergo adalah koin PoW (**Proof of Work**), bukan PoS (**Proof of Stake**), yang berarti blok divalidasi oleh penambang, bukan oleh staker, oleh karena itu Anda tidak dapat melakukan staking Erg secara langsung.

Namun, Anda dapat memperoleh hasil dari ERG Anda dengan menggabungkannya dengan Ergo di pool likuiditas, tokenisasi dApps, bot trading, platform peminjaman, dan mekanisme lainnya. 

Anda dapat 'mempertaruhkan' token asli di Ergo dalam beberapa bentuk (di ergopad.io *live*, Night Owl Casino *segera*, ErgoMixer *segera*, dan banyak lagi)  

Untuk info lebih lanjut tentang cara mendapatkan penghasilan dari Erg Anda, lihatlah [Panduan hasil](https://ergonaut.space/en/Guides/yield).

# Pertanyaan Anda Sudah Terjawab

Ada pertanyaan lain? Beri komentar di bawah ini agar kami dapat memperluas halaman ini!
