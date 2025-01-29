---
title: Strategi Trading Forex
date: 2025-01-29T01:06:05.669Z
tags:
  - Strategi
  - Forex
image: https://www.vecteezy.com/vector-art/7467022-stock-trade-data-on-graph-with-japanese-candles-graph-for-financial-markets-online-analysis-for-investment
draft: true
---
T﻿rading forex merupakan salah satu cara untuk menghasilkan uang yang kemudian dapat dimanfaatkan sebagai salah satu cara memenuhi kebutuhan hidup kita, trading merujuk pada kegiatan jual dan beli. Dalam konteks ini tentunya dibutuhkan sebuah strategi atau cara agar kita tidak hanya melakukan kegiatan tersebut, melainkan dapat menghasilkan sesuatu yakni uang. Berikut merupakan beberapa cara yang mungkin layak untuk dicoba:

### 1﻿. Strategi Memanfaatkan Indikator Supertrend

B﻿erikut informasi pengantar bawaan dari tradingview mengenai supertrend, indikator supertrend yang akan digunakan dalam strategi ini merupakan indikator bawaan dari Tradingview, bukan buatan seseoarang atau entitas tertentu didalamnya, dapat di cek pada link <https://id.tradingview.com/support/solutions/43000634738/>

#### Definisi

Supertrend adalah indikator mengikuti tren berdasarkan Rentang Rata-Rata Sebenarnya/Average True Range (ATR). Perhitungan garis tunggalnya menggabungkan deteksi tren dan volatilitas. Ini dapat digunakan untuk mendeteksi perubahan arah tren dan untuk memposisikan stop.

#### Histori

Indikator Supertrend diciptakan oleh Olivier Seban.

#### Kalkulasi

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

#### Dasar

Supertrend adalah indikator yang mengikuti tren. Indikator ini menimpa chart utama dan plotnya menunjukkan tren saat ini. Supertrend dapat digunakan dengan periode yang bervariasi (harian, mingguan, intrahari, dll.) dan pada berbagai instrumen (saham, kontrak berjangka atau forex).

Supertrend memiliki beberapa input yang dapat anda sesuaikan dengan strategi trading anda. Menyesuaikan pengaturan ini memungkinkan anda membuat indikator tersebut menjadi lebih atau kurang sensitif terhadap perubahan harga.

Untuk input Supertrend, anda dapat menyesuaikan Panjang ATR/atrLength dan pengalinya:

* Pengaturan panjang ATR/atrLength adalah panjang ke belakang untuk kalkulasi ATR;
* pengali adalah jumlah untuk dikalikan kepada ATR untuk melakukan offset pita dari harga.

#### Apa yang dicari

Ketika harga turun di bawah kurva indikator, itu berubah menjadi merah dan menunjukkan tren turun. Sebaliknya, ketika harga naik di atas kurva, indikator berubah menjadi hijau dan menunjukkan tren naik. Setelah setiap penutupan di atas atau di bawah Supertrend, tren baru muncul.

#### Kesimpulan

Supertrend membantu anda membuat keputusan trading yang tepat. Namun, ada kalanya indikator ini menghasilkan sinyal palsu. Oleh karena itu, yang terbaik adalah menggunakan kombinasi yang tepat dari beberapa indikator. Seperti indikator lainnya, Supertrend bekerja paling baik bila digunakan dengan indikator lain seperti MACD, SAR Parabolik / Parabolic SAR (SAR), atau RSI.



> K﻿ita dapat abaikan penjelasan singkat dari tradingview, karena itu hanyalah pelengkap dalam penyusunan strategi ini