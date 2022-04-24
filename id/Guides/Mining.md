---
title: Pertambangan
description: Menjaga panduan original para penambang saat ini
published: true
date: 2022-04-24T00:49:45.392Z
tags: mining, penambang, miner, gpu
editor: markdown
dateCreated: 2022-04-24T00:49:45.392Z
---

# **Buku Panduan Lengkap Menambang Ergo v2.0**

![5e8765a7-6344-4a81-b283-87c695056ef6.jpeg](/5e8765a7-6344-4a81-b283-87c695056ef6.jpeg =x350)

> Anda bisa bergabung pada komunitas penambang aktif Ergo di [Discord](https://discord.gg/Q86PNMwRsu) dan [Telegram](https://t.me/ergo_mining). Untuk dukungan secara langsung bisa ke channel #mining-support di Discord - Aktifkan peran penambangan pada #get-roles. 
{.is-info}

- [Menambang Ergo Menggunakan HiveOS](https://ergoplatform.org/en/blog/2022-03-22-mining-ergo-on-hiveos/)
- [Menambang Ergo di Windows](https://ergoplatform.org/en/blog/2022-03-17-mining-ergo-on-windows/)

## Koin: Apa itu Ergo?

Ergo memiliki pasokan yang sangat terbatas, jadwal emisi 8 tahun dan tingkat penurunan emisi selama 8 tahun ini. Semua token ditambang melalui algoritma Proof-of-Work (“PoW”) asli yang disebut Autolykos v2, dirancang agar tahan ASIC, menggunakan [smoothed difficulty algorithm](https://ergoplatform.org/docs/ErgoPow.pdf).

Penambang harus melakukan komputasi memori-keras~(setidaknya memori 2,5 GB diperlukan, tetapi implementasi paling efisien saat ini menggunakan sekitar 4 GB vRAM) yang membuat Ergo ramah untuk penambangan GPU.

Ada 0 ERG saat peluncuran mainnet karena tidak ada ICO atau pra-penambangan. Pada akhir 8 tahun, pasokan Erg akhir akan menjadi 97.739.925 Ergs. Interval blok Ergo adalah 2 menit dan untuk 2 tahun pertama, setiap blok akan melepaskan total 75 Erg untuk dibagikan antara penambang dan treasury (treasury dibahas di bawah). Tetapi mulai tahun ke-2, tingkat emisi akan turun sebesar 3,0 Ergs dan selanjutnya turun lagi setiap 3 bulan dengan tambahan 3,0 Ergs, yang akan menghasilkan penghentian emisi 8 tahun setelah peluncuran.

- [Ergo Emission: detail, penargetan ulang melalui soft-fork](https://www.ergoforum.org/t/ergo-emission-details-retargeting-via-a-soft-fork/2778)

Tidak akan ada inflasi tambahan dan basis moneter Erg akan tetap. [Bagan jadwal emisi](https://ergoplatform.org/en/blog/2019_05_20-curve/) menggambarkan hal ini yang juga dapat ditemukan di [ergo.watch](https://ergo.watch/emission).

- Bagian [explorer](https://explorer.ergoplatform.com) dapat memberikan berbagai informasi dan statistik pada pertambangan dan jaringan. 
- Gambaran [Tingkat kesulitan selama ini](https://explorer.ergoplatform.com/en/charts/difficulty) bisa dilihat di sini.
- [Monitor Tingkat kesulitasn dan Epoch.](http://cds.oette.info/ergo_diff.htm)

Untuk informasi tentang Ergo bisa ikuti tautan berikut ini :

-   [Platform Ergo](https://ergoplatform.org/en/)
-   [Dasar Ergo](https://ergoplatform.org/en/basics/)
-   [Manifesto Ergo](https://ergoplatform.org/en/blog/2021-04-26-the-ergo-manifesto/)
-   [Ergo Whitepapers](https://ergoplatform.org/en/documents/)

## Dompet:

Sebuah dompet diperlukan bagi Anda untuk mengumpulkan hasil dari penambangan Anda. Dompet digital ini dapat membantu menjaga mata uang digital Anda tetap aman, rahasia, dan dalam kendali Anda. Kami sangat merekomendasikan penggunaan dompet untuk menyimpan aset Ergo (secara teknis, dompet menyimpan kunci ke alamat Ergo Anda). Namun perlu diingat, dompet Anda tidak seperti rekening bank Anda, jadi berhati-hatilah dengan kata sandi Anda dan pastikan untuk melakukan pencadangan rutin untuk melindungi uang Anda.

### Tipe-tipe Dompet:

[Dompet Pihak Ketiga](https://docs.ergoplatform.com/dev/wallet/)

[Dompet Ergo Node](https://github.com/ergoplatform/ergo/wiki/Set-up-a-full-node)

-   [Bagaimana membuat dompet dan mengkonfigurasi node lengkap ergo di Windows (Youtube)](https://www.youtube.com/watch?v=fpEDJ1CM6ns)

> Perhatikan bahwa sebagian besar dompet didukung oleh pihak ketiga, kami hanya memberikan informasi sebagai rasa hormat, untuk menyederhanakan keseluruhan pengalaman mata uang digital untuk Anda.
{.is-warning}


> Tolong jangan menambang langsung ke bursa penukaran koin karena ini memungkinkan mereka untuk mengontrol pergerakan harga. Mari mendukung desentralisasi.
{.is-danger}


## Perangkat Keras:

Anda akan memerlukan perangkat keras komputer untuk menambang Ergo juga disebut sebagai rig penambangan. Penambangan ergo tahan terhadap ASIC dan membutuhkan GPU (Kartu Grafik) untuk menambang. Rig penambangan bisa sesederhana komputer gaming GPU tunggal, hingga rig penambangan multi GPU.

Meskipun memungkinkan untuk menambang Ergo dengan GPU 4gb. GPU 6GB adalah minimum yang disarankan karena Ergo sangat bergantung pada penggunaan memori sementara prosesor inti tidak digunakan. *Catatan: pernyataan terakhir ini tampaknya sudah ketinggalan zaman. Seperti yang disebutkan sebelumnya di Buku Pegangan, 3gb adalah VRAM yang cukup untuk menambang Erg. Dan prosesor inti kartu TIDAK diam saat menambang Ergo.

### Komponen yang dibutuhkan untuk membangun sebuah rig :

-   [Kartu Grafis (GPU)](https://ergonaut.space/en/Guides/Mining/Graphics_Cards)


-   [Motherboards (MOBO)](/en/Guides/Mining/Motherboards)

-   Power Supply (PSU)
-   Processor (CPU)
-   Memory (RAM)
-   Storage (USB, SSD, HDD)
-   Other Hardware
    -   GPU Risers
    -   CPU Cooler
    -   Mining Rack
    -   Fans

Cari kartu grafis Anda di sini [Autolykos v2 hashrates](https://docs.google.com/spreadsheets/d/1NsuoDB27EwCo_BlSjCP3GMLfTSJRPIWIBsL-wPTllUg) untuk melihat besar hashrate.

## Kolam-kolam Penambangan / Pools:

![photo_2021-10-15_23-03-13.jpg](/photo_2021-10-15_23-03-13.jpg =x300)  
- Desain oleh: Autolykos Megistos
---

### [GetBlok.io Smart Pool](https://ergo.getblok.io)
- [Bagaimana koneksi ke GetBlok](https://www.getblok.io/how-to-connect/)
- [GetBlok Telegram Chat](https://t.me/getblok)
- [GetBlok Discord](https://discord.gg/h9uF3cNXdY)

### [LeafPool](https://ergo.leafpool.com/)
- [Memulai dengan LeafPool](https://ergo.leafpool.com/getting-started)

### [Enigma Pool](https://enigmapool.com/)
- [Mulai pada Enigma Pool](https://enigmapool.com/getstarted) 

### [Miningcore](https://miningcore.pro/pool/ergo/)
- [Tanya Jawab Miningcore](https://miningcore.pro/faq)

### [WoolyPooly](https://woolypooly.com/en/coin/erg)
- [Bagaimana mulai menambang Ergo pada windows dengan kartu grafik AMD RX 4GB](https://www.youtube.com/watch?v=47eBVIjWYqY)
- [WoolyPooly Discord](https://woolypooly.com/discord)
- [WoolyPooly Telegram Chat](https://woolypooly.com/telegram)

### [K1pool](https://k1pool.com/pool/erg)
- [Bagaimana mulai menambang di K1pool](https://k1pool.com/pool/erg/how-to-start)

### [2Miners](https://2miners.com/erg-mining-pool)
- [Bagaimana mulai menambang Ergo](https://erg.2miners.com/help)


 ### [F2pool](https://www.f2pool.com/?_ga=2.253802568.1957310317.1634436769-1506845288.1634436769)
- [Bagaimana mulai menambang ergo di f2pool](https://f2pool.io/mining/guides/how-to-mine-ergo/)

### [FlyPool](https://ergo.flypool.org/)
- [Bagaimana menghubungkan ke FlyPool](https://ergo.flypool.org/start)

### [HeroMiners](https://ergo.herominers.com/)

-   [Hero Miners: Bagaimana menambang Ergo (ERG)? Panduan Lengkap Untuk Pemulai](https://herominers.medium.com/how-to-mine-ergo-erg-complete-beginners-guide-608a87e89ed6)
-   [HeroMiners: Bagaimana menambang Ergo](https://ergo.herominers.com/#how-to-mine-ergo-erg)
-   [Bagaimana menambang Ergo? Langkah demi langkah (Youtube)](https://www.youtube.com/watch?v=4SnpCF67kyc)

---

Periksa statistik kumpulan untuk melihat peringkat kumpulan. Lihat catatan tentang 51% serangan di bawah ini
-   [Mining Pool Stats](https://miningpoolstats.stream/ergo)

> Tolong jangan menambang ke kolam penambangan yang telah memiliki hashrate besar. Kolam penambangan yang mendekati 51% dari total jaringan berisiko terkena serangan.
{.is-warning}


-   [Apa itu 51% attacks](https://www.reddit.com/r/ergonauts/comments/mgpnb7/51_attack_possibilities/) ?

## Para Penambang: (Perangkat Lunak Pertambangan)
Ada beberapa penambang yang dapat digunakan untuk menambang Ergo (Autolykos2). Di bawah ini Anda akan menemukan daftar perangkat lunak penambangan yang dapat digunakan untuk menambang ERG. Ada berbagai pendapat tentang perangkat lunak penambangan mana yang terbaik dan ada juga yang jelas pemenangnya. Saran terbaik adalah mencoba semuanya jika Anda bisa dan melihat apa yang paling cocok untuk pengaturan rig Anda secara khusus. Apa yang berhasil untuk satu mungkin atau mungkin tidak bekerja untuk yang lain.

Selain perangkat lunak penambangan khusus, ada juga OS Penambangan atau sistem operasi seperti HiveOS, yang merupakan salah satu opsi yang lebih populer. Ini memungkinkan Anda untuk mengontrol rig Anda melalui perangkat lunak khusus yang akan membantu menghubungkan ke kumpulan, pengaturan OC, dan penambang atau perangkat lunak penambangan. Ini akan dianggap sebagai paket lengkap di mana menggunakan penambang tertentu mungkin memerlukan sumber daya atau plugin lain.

![capture.jpg](/capture.jpg)
  [Gambar dari r/Erg_Miners](https://www.reddit.com/r/erg_miners/comments/njmlfq/list_of_currently_used_miners_for_ergo_with/)

### Perangkat Lunak Pertambangan:
####	[Lolminer](https://github.com/Lolliedieb/lolMiner-releases)
#### [Nanominer](https://github.com/nanopool/nanominer/releases)
####	[NB Miner](https://github.com/NebuTech/NBMiner)
#### [SRB Miner](https://github.com/doktor83/SRBMiner-Multi/releases)
-   [SRBMiner-MULTI - How to mine Ergo coin (autolykos2)](https://www.youtube.com/watch?v=thBPstQJVWo)
#### [Team Red Miner](https://github.com/todxx/teamredminer/releases)
#### [Trex Miner](https://github.com/trexminer/T-Rex/releases)

### Mining OS:
#### [Hive OS](https://hiveos.farm/)
#### [Minerstat](https://minerstat.com/)

#### [Nice Hash](https://www.nicehash.com/) 
- [NiceTalk live with Ergo](https://www.nicehash.com/blog/post/join-us-live-with-ergo-on-nice-talk-on-the-29th)
#### [Rave OS](https://raveos.com/)
####	[Simple Mining OS](https://simplemining.net/)




## Kode Sumber Miners

For the [AMD miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner), sistem operasi yang cocok:

-   RedHat Enterprise Linux 7.2 (64-bit version)
-   RedHat Enterprise Linux 6.8 (64-bit version)
-   Ubuntu 16.04 (64-bit version)

Ergo bisa ditambangan dengan [Nvidia miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)

Penambang bisa menyimpan hasil dengan menukar [SigUSD](https://sigmausd.io/#/)

[Mulai menambang](https://git.io/fjqwp)


# Menambang Sendiri

Anda dapat menambang sendiri di salah satu kolam yang menawarkan port "solo". Jika tidak, Anda perlu membangun node dan server stratum (pool) juga dapat mencoba [ergoNomp](https://github.com/btclinux/ergo-nomp)

Silakan periksa [formulir ini](https://docs.google.com/forms/d/e/1FAIpQLScBFv3mxpu5Erv55zvfFuIo2NnaWht3cc70xZoRo-3c58Cv0A/viewform) untuk melihat apakah penambangan tunggal bermanfaat.


- [Autolykos2_NV_Miner](https://github.com/mhssamadani/Autolykos2_NV_Miner)
- [Autolykos2_AMD_Miner](https://github.com/mhssamadani/Autolykos2_AMD_Miner)

Untuk mengoperasikannya, Anda mungkin perlu atau tidak perlu menggunakan Stratum Server dan Stratum Proxy. Kedua proyek ini ada di sini:

- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer)
- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy)

# Kesulitan

Ergo menggunakan metode kuadrat terkecil linier yang menghaluskan lebih dari 8 epoch (8 x 1024 blok). Ini dirancang untuk mencegah serangan time warp dan coin-hopping yang berbahaya.

[Kesulitan dari waktu ke waktu](https://explorer.ergoplatform.com/en/charts/difficulty) terlihat di sini. Jika Anda menginginkan perkiraan tentang apa yang mungkin terjadi selanjutnya, Anda dapat mengamati [Monitor Kesulitan dan zaman.](http://cds.oette.info/ergo_diff.htm)

# Menjadi Host Sebuah Pool / Kolam

Saat ini [#host-a-pool](https://discord.gg/kxbrHVwnm5) di Discord adalah tempat terbaik untuk mendapatkan dukungan dalam mengonfigurasi pool.

- [ErgoStratumProxy](https://github.com/mhssamadani/ErgoStratumProxy) | Koneksi Penambang + Manajemen Kerja
- [ErgoStratumServer](https://github.com/mhssamadani/ErgoStratumServer) | Server kolam renang
- [ergo-nomp](https://github.com/btclinux/ergo-nomp) | Portal penambangan terbuka simpul dikonfigurasi untuk ergo

**Langkah-langkah**

1. Siapkan Node
2. Atur ErgoStratumServer
3. Arahkan [ergo-nomp](https://github.com/btclinux/ergo-nomp) ke (1) dan (2)


## Sumber daya

**Kalkulator**

- [ErgoPlatform - Kalkulator Penambangan](https://ergoplatform.org/en/mining/)
- [Kalkulator Plutomonkey](https://pool.plutomonkey.com/)
- [Statistik Penambang](https://minerstat.com/coin/erg)

**Penambang Lainnya**
- [Penambang GPU berbasis CUDA untuk Ergo](https://github.com/ergoplatform/Autolykos-GPU-miner) untuk kartu NVidia
- [Penambang OpenCL untuk ERGO](https://github.com/mhssamadani/ergoAMDminer) untuk kartu AMD
- [#smartpools](https://discord.gg/qdEpkRQZ4P)

<!-- Memberikan pesan 503 Service Unavailable Error pada 31 Desember 2021, berkomentar. Pergi karena saya tidak tahu apakah ini masalah sementara. @cafebedouin
- [ErgoPool - kolam penambangan untuk penambang Ergo yang berdiri sendiri!](https://ergopool.io/) -->



## Panduan

- [Menambang $ERG: Panduan Lengkap](https://thecryptodrip.com/how-to-mine-erg-guide/)
- [ErgoForum: Menambang Ergo untuk Kesenangan dan Keuntungan](https://www.ergoforum.org/t/mining-ergo-for-fun-and-profit/154)
- [ErgoPlatform: Menambang Ergo untuk Kesenangan dan Keuntungan](https://ergoplatform.org/en/blog/2019_12_22_mining_for_fun/)
- [ErgoForum: Tanya Jawab tentang penambangan (untuk operator kumpulan dan penambang solo)](https://www.ergoforum.org/t/q-a-on-mining-for-pool-operators-and-solo-miners/587)

Kredit [@ÅrÖhBê](https://t.me/arohbe) [@Glasgowm](https://t.me/glasgowm)