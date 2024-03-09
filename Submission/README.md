# Panduan Menjalankan Aplikasi Analisis Data dengan Streamlit

Aplikasi ini memungkinkan pengguna untuk menganalisis data sepeda menggunakan Python dan berbagai library seperti Pandas, Matplotlib, Seaborn, dan Streamlit.

## Langkah-langkah untuk Menjalankan Aplikasi:

1. **Persiapan:**
   - Pastikan Python telah terinstal di komputer.

2. **Instalasi Library yang Diperlukan:**
   - Pastikan semua library yang diperlukan telah diinstal. Gunakan pip dengan perintah berikut:
     ```bash
     pip install numpy pandas matplotlib seaborn streamlit babel
     ```

3. **Jalankan Aplikasi dengan Streamlit:**
   - Buka terminal atau command prompt.
   - Pastikan sudah terarahkan ke direktori tempat menyimpan file Python.
   - Jalankan aplikasi dengan perintah:
     ```bash
     streamlit run dashboard.py
     ```
     atau
     ```bash
     streamlit run (insert path ke folder project).py
     ```

4. **Navigasi Halaman:**
   - Setelah menjalankan perintah tersebut, aplikasi akan berjalan dan tampil di browser. Navigasi di samping kiri memungkinkan pengguna memilih antara "Pertanyaan 1" dan "Pertanyaan 2".

5. **Pilih Pertanyaan:**
   - Klik pada salah satu opsi pertanyaan untuk melihat visualisasi dan kesimpulan terkait pertanyaan tersebut.

6. **Buka dari VSCode:**
   - Buka VSCode dan pastikan Anda telah membuka folder proyek yang sesuai.
   - Buka terminal di VSCode.
   - Pastikan terminal terarahkan ke folder proyek yang berisi file Python.
   - Jalankan aplikasi dengan perintah seperti yang disebutkan di langkah 3.

7. **Memperbaiki Kesalahan: (OPSIONAL)**
   - Jika mengalami kesalahan terkait dengan file `dashboard.py`, saran dari mentor dosen saya adalah coba periksa dan perbaiki jalur file pada bagian berikut:
     ```python
     # Load data 
     day_df = pd.read_csv("Submission\dashboard\day_clean.csv")
     hour_df = pd.read_csv("Submission\dashboard\hour_clean.csv")
     ```
     Ganti menjadi:
     ```python
     # Load data 
     day_df = pd.read_csv("dashboard/day_clean.csv")
     hour_df = pd.read_csv("dashboard/hour_clean.csv")
     ```

Dengan mengikuti langkah-langkah di atas, pengguna akan dapat menjalankan aplikasi analisis data menggunakan Streamlit dan menjelajahi hasil analisisnya.
