# 📊 Analisis Penjualan PT MariBelajar (ETL & Power BI Dashboard)

Repository ini berisi laporan akhir dan proyek *Project-Based Learning* untuk mata kuliah **Data Mining II**[cite: 2]. Proyek ini bertujuan untuk membangun alur kerja **ETL (Extract, Transform, Load)** dan merancang dashboard interaktif menggunakan **Microsoft Power BI** guna menganalisis performa penjualan PT MariBelajar[cite: 6, 13].

---

## 👥 Tim Penyusun (Kelompok VI - Kelas B)
* **Armalia Kusuma Putri** (22083010004)[cite: 2]
* **Tsabita Rosyidah Putri** (22083010012)[cite: 2]
* **Winna Dhestyan Putri** (22083010015)[cite: 2]
* **Hanif Ziva Zavira** (22083010078)[cite: 2]
* **Dosen Pengampu:** Kartika Maulida Hindrayani, S.Kom., M.Kom.[cite: 2]

---

## 🏗️ Alur Proses Penerapan (Workflow)
Proyek ini mengikuti tahapan Data Mining dan arsitektur ETL yang sistematis:
1. **Menyiapkan Data Sumber:** Menggunakan dataset operasional PT MariBelajar dalam format Excel yang terdiri dari tabel *Product*, *Sales*, dan *Supervisor*[cite: 8, 11].
2. **Extract:** Mengekstraksi data mentah dari file Excel ke dalam lingkungan **Power BI Desktop** melalui *Power Query Editor*[cite: 8, 13].
3. **Transform:** Melakukan pembersihan data (*data cleaning*), yang meliputi:
   * Menghapus kolom dan baris kosong (*null*) yang tidak relevan[cite: 14, 15].
   * Memperbaiki kesalahan penulisan (*typo*) menggunakan fitur *Replace Values* (misalnya menyeragamkan format nama produk dan supervisor)[cite: 16, 17, 18].
   * Menyesuaikan tipe data kolom (*Text*, *Number*, *Fixed Decimal Number* / *Currency*)[cite: 16, 17].
   * Menambahkan kolom kalkulasi baru yaitu **Revenue** pada tabel *Sales* menggunakan ekspresi **DAX** (`Unit Sold * Price per unit`)[cite: 11, 12].
4. **Load:** Memuat tabel yang telah bersih ke dalam model data Power BI[cite: 13].
5. **Pemodelan & Relasi Antar Tabel:** Menghubungkan relasi antar tabel (*Star Schema* / relasi *Foreign Key* ke *Primary Key*) antara tabel *Sales*, *Product*, dan *Supervisor*[cite: 6, 11, 12].
6. **Visualisasi Dashboard:** Membangun dashboard interaktif 2 halaman yang dilengkapi dengan *Card*, *Slicer*, *Line Chart*, *Bar Chart*, dan *Matrix Table*[cite: 13, 14].
7. **Analisis & Interpretasi Hasil:** Mengevaluasi tren penjualan berdasarkan waktu, produk unggulan (*Top 10 Products*), serta performa supervisor dan karyawan[cite: 14, 16, 17].

---

## 📈 Ringkasan Hasil Analisis
* **Periode Pengamatan:** 1 Januari 2019 – 20 April 2019[cite: 15, 20]
* **Total Pendapatan (Revenue):** Rp96.621.081[cite: 15, 20]
* **Total Unit Terjual:** 1.122.881 unit[cite: 15, 20]
* **Total Produk:** 30 produk[cite: 15, 20]
* **Total Transaksi:** 6.490 transaksi[cite: 15, 20]
* **Temuan Utama:** Penjualan harian menunjukkan pola fluktuatif yang dipengaruhi oleh waktu[cite: 16, 20], dan terdapat kontribusi pendapatan yang didominasi oleh beberapa produk unggulan tertentu (*Top Products*)[cite: 16, 20]. Performa tim penjualan juga bervariasi berdasarkan struktur supervisor dan karyawan[cite: 16, 17, 20].

---

## 📁 Struktur Repository
```text
├── Product.xlsx,Sales Data.xlsx,Supervisor.xlsx/               # Berisi file sumber data Excel (Product, Sales, Supervisor)
├── sales PT MARI BELAJAR.pbix/                                 # File laporan Power BI (.pbix)
├── Poster.png/                                                # Tangkapan layar dashboard dan diagram alir
├── Laporan.pdf                                                 # Laporan Hasil
└── README.md                                                    # Dokumentasi proyek
