## bioinfo-pilot

### Topik: Genomik

#### Tujuan

1. **Identifikasi Data (EDA):**

   - Memahami sifat dan struktur data genomik.
   - Melakukan Exploratory Data Analysis (EDA) untuk mendapatkan wawasan awal.

2. **Penilaian Kualitas Data FASTQ:**

   - Fokus pada memastikan kualitas data (ambang Q30).
   - Menstabilkan skor kualitas antar sampel (variabilitas diperbolehkan tetapi dengan wawasan yang jelas).
   - Menggunakan contoh dari berbagai dataset FASTQ untuk mendemonstrasikan metrik kualitas.

3. **Jenis Data yang Difokuskan:**

   - Analisis data dari file **FASTQ**, **Global Screening Array (Genotyping)**, dan **Microarray**.

4. **Analisis Pasca-FASTQ:**

   - Melakukan analisis lanjutan setelah penilaian kualitas.

---

### Kasus 1: Quality Control dan EDA

#### Tujuan: Pengolahan Data dan Exploratory Data Analysis (EDA)

##### Quality Control File FASTQ

1. **Konsep FASTQ:**

   - Pengenalan struktur dan komponen file FASTQ.
   - Memahami pembacaan sekuens dan skor kualitas terkait.

2. **Phred Score:**

   - Penjelasan skor kualitas Phred dan pentingnya.
   - Interpretasi skor Q30 dan implikasinya untuk analisis lanjutan.

3. **Jenis File FASTQ:**

   - Gambaran umum berbagai format data FASTQ dan penggunaannya.

4. **EDA Batch dan Visualisasi:**

   - Melakukan EDA pada beberapa file FASTQ.
   - Membuat visualisasi untuk mengidentifikasi pola dan anomali.

5. **Contoh Langkah-langkah di Google Colab:**

   - **Langkah 1:** Upload file FASTQ ke Google Colab menggunakan Google Drive atau file uploader.
   - **Langkah 2:** Instal dan gunakan alat seperti `FastQC` dengan perintah Linux di Colab.
   - **Langkah 3:** Lakukan pemeriksaan kualitas menggunakan `FastQC` dan simpan laporan hasil.
   - **Langkah 4:** Analisis laporan kualitas (Phred score, distribusi skor kualitas, dll.) dengan visualisasi menggunakan Python (misalnya, `matplotlib` atau `seaborn`).
   - **Langkah 5:** Identifikasi pola atau outlier dalam data dengan teknik EDA.
   - **Langkah 6:** Interpretasi hasil untuk menentukan langkah selanjutnya dalam analisis.

6. **Batch Analysis:**

   - **Langkah 1:** Automasi analisis untuk beberapa file FASTQ dalam satu batch.
   - **Langkah 2:** Gunakan Python untuk iterasi file dan integrasikan dengan `FastQC`.
   - **Langkah 3:** Buat laporan gabungan dari semua file untuk membandingkan metrik kualitas antar sampel.
   - **Langkah 4:** Visualisasi perbandingan batch menggunakan pustaka statistik seperti `pandas` dan `seaborn`.

7. **Tools:**

   - Menggunakan **FastQC** untuk pemeriksaan kualitas.
   - Memanfaatkan alat baris perintah **Unix/Linux** untuk preprocessing data dan visualisasi.
   - Gunakan **Python** untuk membuat visualisasi dan analisis lebih lanjut.
   - Tambahkan aplikasi statistik seperti **R** untuk analisis mendalam dan visualisasi tambahan jika diperlukan.