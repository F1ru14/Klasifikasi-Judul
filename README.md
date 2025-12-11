# Klasifikasi Judul Skripsi Biologi (Text Mining & Rule-Based NLP) 🧬📊

Proyek ini bertujuan untuk mengotomatisasi klasifikasi judul skripsi mahasiswa Biologi ke dalam kelompok studi (KS) atau bidang peminatan tertentu menggunakan pendekatan **Text Mining** dan **Rule-Based NLP** (Natural Language Processing).

Sistem ini memproses teks judul, melakukan pembersihan data, dan mencocokkan kata kunci (keywords) yang telah didefinisikan untuk menentukan penjurusan.

## 🚀 Fitur Utama
* **Preprocessing Bahasa Indonesia:** Menggunakan library **Sastrawi** untuk stemming (mencari kata dasar) dan **NLTK** untuk tokenisasi serta penghapusan *stopwords*.
* **Rule-Based Classification:** Mengklasifikasikan judul berdasarkan kamus kata kunci spesifik untuk setiap bidang biologi.
* **Analisis Distribusi:** Menghitung jumlah skripsi per kelompok studi secara otomatis.

## 📚 Daftar Kelompok Studi (Kategori)
Sistem mengklasifikasikan judul ke dalam kategori berikut berdasarkan kata kunci yang ditemukan:

| Kode / Nama KS | Deskripsi Bidang Studi |
| :--- | :--- |
| **Coral** 🌊 | Fokus pada biota laut, terumbu karang, dan ekosistem laut. |
| **Sokabotanisa** 🌿 | Mempelajari keanekaragaman tumbuhan (Botani), fisiologi, dan ekologi tanaman. |
| **Amoeba** 🍄 | Mempelajari mikrobiologi, jamur (fungi), bakteri, dan organisme mikroskopis. |
| **Formagenbi** 🧬 | Mempelajari genetika, bioteknologi, DNA/RNA, dan molekuler (terutama hewan). |
| **Kutrik** 🦋 | (Entomologi) Mempelajari keanekaragaman serangga, seperti kupu-kupu dan capung. |
| **Stigobites** 🦇 | Mempelajari ekosistem gua, karst, dan biospeleologi. |
| **Varanus** 🦎 | Mempelajari reptil dan amfibi (Herpetologi). |
| **Himantopus** 🐦 | Mempelajari keanekaragaman burung (Ornitologi). |
| **AMS** 🐒 | Mempelajari keanekaragaman mamalia (Mammalogy). |
| **BEC** 🇬🇧 | Pengembangan Bahasa Inggris (English Club) dan bedah jurnal internasional. |

## 🛠️ Teknologi yang Digunakan
* **Python 3.x**
* **Pandas:** Untuk manipulasi data (DataFrame).
* **Sastrawi:** Library Stemming khusus Bahasa Indonesia.
* **NLTK:** Tokenisasi dan Stopwords removal.
* **OpenPyXL:** Membaca file Excel (`.xlsx`).

## 📊 Contoh Hasil Analisis
Berdasarkan sampel data yang dijalankan, berikut adalah contoh distribusi topik skripsi:

```text
Sokabotanisa    96
Coral           90
Amoeba          61
Formagenbi      38
Kutrik          33
Stigobites      16
...
