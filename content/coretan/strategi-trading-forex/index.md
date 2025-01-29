---
title: Strategi Trading Menggunakan Indikator Supertrend Pendekatan MTF
date: 2025-01-29T09:36:39.164Z
tags:
  - Strategi
  - Forex
image: vecteezy_businessman-worried-about-stock-market-volatility-he-was_5084691.jpg
draft: false
---
T﻿rading forex merupakan salah satu cara untuk menghasilkan uang yang kemudian dapat dimanfaatkan sebagai salah satu cara memenuhi kebutuhan hidup kita, trading merujuk pada kegiatan jual dan beli. Dalam konteks ini tentunya dibutuhkan sebuah strategi atau cara agar kita tidak hanya melakukan kegiatan tersebut, melainkan dapat menghasilkan sesuatu yakni uang. Berikut merupakan beberapa cara yang mungkin layak untuk dicoba:

# P﻿engenalan Supertrend

B﻿erikut informasi pengantar bawaan dari tradingview mengenai supertrend, indikator supertrend yang akan digunakan dalam strategi ini merupakan indikator bawaan dari Tradingview, bukan buatan seseoarang atau entitas tertentu didalamnya, dapat di cek pada link <https://id.tradingview.com/support/solutions/43000634738/>

## Definisi

Supertrend adalah indikator mengikuti tren berdasarkan Rentang Rata-Rata Sebenarnya/Average True Range (ATR). Perhitungan garis tunggalnya menggabungkan deteksi tren dan volatilitas. Ini dapat digunakan untuk mendeteksi perubahan arah tren dan untuk memposisikan stop.

## Histori

Indikator Supertrend diciptakan oleh Olivier Seban.

## Kalkulasi

Untuk mengkalkulasi ikatan dari Supertrend, gunakan formula berikut ini:

```
hl2 = (high + low) / 2
basicUpperBand = hl2 + (multiplier × ATR)
basicLowerBand = hl2 - (multiplier × ATR)

upperBand = basicUpperBand < prev upperBand or
			prev close > prev upperBand ? basicUpperBand : prev upperBand
lowerBand = basicLowerBand > prev lowerBand or
			prev close < prev lowerBand ? basicLowerBand : prev lowerBand

superTrend = trendDirection == isUpTrend ? lowerBand : upperBand
```

trendDirection ditentukan berdasarkan pemenuhan dari kondisi berikut ini:

```
Until the ATR value is calculated trendDirection = isDownTrend
else if prev superTrend == prev upperBand
    trendDirection := close > upperBand ? isUpTrend : isDownTrend
else
    trendDirection := close < lowerBand ? isDownTrend : isUpTrend
```

## Dasar

Supertrend adalah indikator yang mengikuti tren. Indikator ini menimpa chart utama dan plotnya menunjukkan tren saat ini. Supertrend dapat digunakan dengan periode yang bervariasi (harian, mingguan, intrahari, dll.) dan pada berbagai instrumen (saham, kontrak berjangka atau forex).

Supertrend memiliki beberapa input yang dapat anda sesuaikan dengan strategi trading anda. Menyesuaikan pengaturan ini memungkinkan anda membuat indikator tersebut menjadi lebih atau kurang sensitif terhadap perubahan harga.

Untuk input Supertrend, anda dapat menyesuaikan Panjang ATR/atrLength dan pengalinya:

* Pengaturan panjang ATR/atrLength adalah panjang ke belakang untuk kalkulasi ATR;
* pengali adalah jumlah untuk dikalikan kepada ATR untuk melakukan offset pita dari harga.

## Apa yang dicari

Ketika harga turun di bawah kurva indikator, itu berubah menjadi merah dan menunjukkan tren turun. Sebaliknya, ketika harga naik di atas kurva, indikator berubah menjadi hijau dan menunjukkan tren naik. Setelah setiap penutupan di atas atau di bawah Supertrend, tren baru muncul.

## Kesimpulan

Supertrend membantu anda membuat keputusan trading yang tepat. Namun, ada kalanya indikator ini menghasilkan sinyal palsu. Oleh karena itu, yang terbaik adalah menggunakan kombinasi yang tepat dari beberapa indikator. Seperti indikator lainnya, Supertrend bekerja paling baik bila digunakan dengan indikator lain seperti MACD, SAR Parabolik / Parabolic SAR (SAR), atau RSI.

> K﻿ita dapat abaikan penjelasan singkat dari tradingview, karena itu hanyalah pelengkap dalam penyusunan strategi ini

### B﻿agaimana Cara Memanfaatkannya?

M﻿enarik, setelah kita mengetahui cara kerjanya, tentu pertanyaan berikutnya adalah cara memanfaatkannya untuk keuntungan kita tentunya. Berikut merupakan SOP yang disusun, yang kemudian harus dilakukan backtest untuk mengujinya berdasarkan data sebelum pengujian secara real.

P﻿emanfaatan indikator Supertrend dapat kita lakukan dengan cara entry ataupun exit berdasarkan multi time frame, dasar dari pemanfaatan ini adalah ketika kita menggunakan indikator ini, kita dapat melihat arah harga atau trend dari setiap timeframe yang ada, kita dapat melihat dan mengetahui bahwasannya dari trend besar pasti ada trend yang lebih kecil yang masih sesuai dengan jalur dari timeframe yang lebih besar, dan hal tersebut yang akan kita manfaatkan. Berikut beberapa staregi yang disusun.

#### M﻿ulti time frame sederhana

1. P﻿ilih timeframe lebih besar yang akan kita gunakan untuk melihat arah trend.
2. P﻿ada timeframe yang lebih kecil, kita dapat melihat koreksi trend besar yang sudah kita pilih ditandai dengan arah trend yang berlawanan.
3. E﻿ntry dilakukan ketika trend yang berlawanan berakhir atau kita anggap sebagai akhir dari koreksi yang telah dikonfirmasi oleh indikator supertrend.

C﻿ontoh penggunaan langkah diatas sebagai berikut:

1. 4﻿ H sebagai timeframe besar, entry pada 1 H sebagai timframe kecil
2. 1﻿ H sebagai timeframe besar, entry pada 15 M sebagai timeframe kecil

P﻿emilihan timeframe dipilih berdasarkan gaya trading yang akan kita gunakan, misalnya scalping disarankan menggunakan timeframe dibawah 4 H, atau dapat dimulai dari 1 H hingga seterusnya. Perhitungan pemilihan timeframe yang lebih kecil diambil setidaknya 1/4 dari timeframe besar yang kita pilih.

#### M﻿ulti time frame sedikit lebih kompleks

1. C﻿ari arah trend di timeframe yang lebih besar, dalam kasus ini kita akan memilih menggunakan 4 Hour
2. C﻿ari kesempatan entry sesuai dengan arah trend di timeframe lebih kecil dengan filter berikut
3. F﻿Ilter entry yang dimanfaatkan adalah timeframe 1 Hour
4. E﻿ntry sebenarnya dapat dilakukan di timeframe 15 Minutes
5. P﻿ada timeframe 15 Minutes letak entry seharusnya pada awal perubahan trend yang berlawanan, atau setelah koreksi selesai, walaupun mungkin ini akan diangap sedikit lebih telat. Namun, tidak menjadi persoalan selama sesuai dengan timeframe besar.

P﻿ada strategi ini, digunakan filter yakni 1/4 dari arah trend besar yang kita pilih berguna untuk melakukan filterisasi terhadap entrian yang kita pilih, dalam kata lain kita tidak langsung entry sesuai dengan timeframe 1/4 dari timeframe pilihan kita, melainkan dapat melakukan entry pada entry yang lebih sharp. Strategi ini dirasa lebih cocok untuk jangka panjang dan memilih entry yang lebih cepat dibanding menunggu akhir koreksi dari trend 1/4 timeframe.

### Akhir Kata

D﻿emikian susunan strategi ini disusun sesuai pemikiran yang belum matang ini, segera lakukan backtest baik secara manual atau menggunakan tools tertentu. Hasil dari backtest haruslah diungah atau dilaporkan kembali di website ini.

A﻿pabila ada saran, silahkan sampaikan pada kontak sesuai media yang anda pilih dibagian footer website ini. Saya akan sangat senang mendengar saran dari anda.