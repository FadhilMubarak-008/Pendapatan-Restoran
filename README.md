## Analisis Pendapatan Restoran

## Gambaran Umum

Proyek ini bertujuan untuk menganalisis data penjualan restoran guna memahami faktor utama yang memengaruhi pendapatan.

Analisis ini fokus pada :

* Produk
* Kota
* Metode pembayaran

Dengan pendekatan berbasis data, proyek ini mencoba menjawab "apakah ada hubungan volume transaksi dan nilai transaksi berkontribusi terhadap performa bisnis ?".

Disclimer : 

* Saya masih dalam tahap belajar data analis

-  Dataset yang digunakan berasal dari kaggle dan hanya memiliki sedikit data (hanya ada 270 baris data)  
- Saya menggunakan bantuan AI untuk membantu saya berpikir dalam menganalisis data

---

## 📊 Dataset

Dataset berisi data transaksi dengan kolom:

* Order ID
* Date
* Product
* Price
* Quantity
* Purchase Type
* Payment Method
* Manager
* City

### 🔧 Feature Engineering

Kolom baru yang dibuat:

> **Revenue = Price × Quantity**

---

## Rumusan Masalah

> Faktor apa yang paling memengaruhi pendapatan restoran, dan bagaimana produk, kota, serta metode pembayaran berperan dalam hal tersebut?

---

## Alur Analisis

Tahapan analisis sebgai berikut :

1. Membuat fitur Revenue
2. Menganalisis distribusi Revenue
3. Analisis berdasarkan Product
4. Analisis berdasarkan City
5. Analisis berdasarkan Payment Method
6. Cross analis untuk memahami hubungan antar variabel

Metode yang dipakai :

* **Sum** → kontribusi total
* **Mean** → nilai rata-rata transaksi
* **Median** → nilai tipikal transaksi
* **Count** → jumlah transaksi

---

## Distribusi Revenue

* Distribusi bersifat **right-skewed**
* Mayoritas transaksi bernilai rendah–menengah
* Terdapat transaksi bernilai tinggi yang signifikan

👉 Hasil:

> Sebagian kecil transaksi memiliki kontribusi besar terhadap total revenue

---

## Analisis Produk

* **Burgers** memiliki:

  * Revenue total tertinggi
  * Rata-rata dan median tertinggi
* Jumlah transaksi relatif merata antar produk

👉 Hasil:

> Perbedaan revenue dipengaruhi oleh **nilai transaksi**, bukan frekuensi pembelian

---

## Analisis Kota

* **Lisbon**

  * Jumlah transaksi tertinggi
* **Berlin**

  * Rata-rata revenue tertinggi
* Median antar kota relatif mirip

👉 Hasil:

> Lisbon unggul dalam **volume transaksi**,
> Berlin unggul dalam **nilai transaksi**

---

## Analisis Metode Pembayaran

* Cash memiliki total revenue tinggi
* Namun:

  * **Credit Card memiliki rata-rata transaksi lebih tinggi**

👉 Insight:

> Metode pembayaran mencerminkan perilaku pengeluaran yang berbeda

👉 Implikasi:

* Dorong penggunaan Credit Card untuk meningkatkan nilai transaksi

---

## Cross Analysis

Analisis lanjutan menunjukkan:

* Produk tertentu memiliki performa lebih tinggi di kota tertentu
* Payment method berkaitan dengan nilai transaksi

👉 Hasil:

> Revenue dipengaruhi oleh kombinasi:

* Produk
* Lokasi
* Perilaku pembayaran

---

## Insight Utama

* Revenue tidak hanya soal jumlah transaksi
* Ada dua faktor utama:

  * **Volume (Lisbon)**
  * **Value (Berlin, Burgers, Credit Card)**

👉 Hasil ini membuat saya belajar bahwa pentingnya membedakan antara transaksi banyak dan transaksi bernilai tinggi  

---

## 💡 Rekomendasi Bisnis

* Fokus pada produk bernilai tinggi (Burgers)
* Tingkatkan average order di kota dengan volume tinggi (Lisbon)
* Pertahankan strategi premium di Berlin
* Dorong penggunaan metode pembayaran dengan nilai tinggi (Credit Card)

---
---

## Tools yang digunakan

* Python
* Pandas
* Matplotlib

---

## 📌 Kesimpulan

Analisis ini menunjukkan bahwa:

> **Performa bisnis tidak hanya ditentukan oleh seberapa banyak transaksi, tetapi juga seberapa besar nilai tiap transaksi.**

Memahami perbedaan ini memungkinkan pengambilan keputusan yang lebih strategis dan tepat sasaran.

---

## Penutup 

Proyek ini dibuat untuk belajar mengenai data analis untuk memahami lebih dalam tentang dunia bisnis, dalam proyek ini saya belajar : bagaimana cara membuat alur analisis, memahami hubungan antar kolom, membersihkan data dan mengetahui kolom mana yg relevan untuk menyelesaikan kasus bisnis.

---
