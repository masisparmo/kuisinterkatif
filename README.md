Dokumentasi Web App: Kuis Interaktif Seminar
============================================

1\. Deskripsi
-------------

**Kuis Interaktif Seminar** adalah sebuah aplikasi web progresif yang dirancang untuk meningkatkan keterlibatan audiens dalam acara seperti seminar, workshop, pelatihan, atau kegiatan belajar mengajar. Aplikasi ini memungkinkan pembicara (Admin) untuk secara cepat dan otomatis membuat sesi kuis interaktif berdasarkan materi yang disajikan, baik dari file PDF, teks, halaman web, maupun video YouTube.

Peserta dapat dengan mudah bergabung melalui QR Code atau tautan, mengisi data diri, dan mengerjakan kuis secara real-time. Skor akan dihitung berdasarkan kombinasi kecepatan dan ketepatan jawaban, lalu ditampilkan pada Leaderboard yang dapat diperbarui secara langsung untuk menciptakan suasana yang kompetitif dan menyenangkan.

Akses aplikasi ini di [https://kuisinteraktif.isparmo.com/](https://kuisinteraktif.isparmo.com/) 

2\. Fitur-fitur Utama
---------------------

Aplikasi ini memiliki dua peran utama dengan fitur yang berbeda:

### Fitur Admin (Pembicara)

*   **Pembuatan Kuis Otomatis dengan AI:** Membuat soal pilihan ganda secara instan dari berbagai sumber materi:
    
    *   **Unggah File PDF:** Mendukung unggahan satu atau lebih file PDF.
        
    *   **Tempel Teks:** Menyalin dan menempelkan teks materi secara langsung.
        
    *   **URL Web:** Mengambil konten teks dari sebuah artikel atau halaman web.
        
    *   **URL YouTube:** Membuat soal berdasarkan judul dan deskripsi video.
        
*   **Bank Soal:** Menyimpan soal-soal yang telah dibuat ke dalam Google Sheet untuk digunakan kembali di sesi kuis mendatang.
    
*   **Kustomisasi Tampilan (Branding):** Mengubah tampilan kuis agar sesuai dengan tema acara dengan mengunggah logo dan memilih skema warna.
    
*   **Leaderboard Real-time:** Menampilkan peringkat skor peserta secara langsung dengan opsi pembaruan otomatis setiap beberapa detik.
    
*   **Pembahasan & Kunci Jawaban:** Melihat daftar soal beserta kunci jawaban yang benar di dasbor admin untuk keperluan pembahasan.
    
*   **Konfigurasi Fleksibel:** Mengatur jumlah soal dan durasi pengerjaan kuis.
    
*   **Tinjau & Edit Soal:** Admin dapat meninjau dan menyunting soal yang dihasilkan oleh AI sebelum kuis diaktifkan.
    

### Fitur Peserta

*   **Akses Mudah:** Bergabung dengan kuis secara cepat melalui pemindaian QR Code atau klik tautan.
    
*   **Pencegahan Entri Ganda:** Sistem memvalidasi nama dan nomor WhatsApp untuk memastikan setiap peserta hanya bisa mengikuti kuis satu kali.
    
*   **Tampilan Kuis Interaktif:** Antarmuka yang bersih dan mudah digunakan dengan timer hitung mundur.
    
*   **Dukungan Rumus Matematika:** Menampilkan soal dengan rumus matematika (format LaTeX) secara jelas dan mudah dibaca (Rich Text).
    
*   **Halaman Hasil Personal:** Setelah selesai, peserta dapat melihat rincian skor, durasi pengerjaan, dan detail perhitungan skor mereka.
    
*   **Tinjauan Jawaban:** Peserta dapat melihat kembali jawaban yang mereka pilih dan statusnya (Benar/Salah) tanpa melihat kunci jawaban yang benar.
    

3\. Teknologi yang Dipakai
--------------------------

*   **Frontend:** HTML5, Tailwind CSS, JavaScript (Vanilla JS)
    
*   **Backend & Database:** Google Apps Script & Google Sheets
    
*   **AI & Machine Learning:** Google Gemini API (untuk pembuatan soal otomatis)
    
*   **Lain-lain:**
    
    *   **QRious:** Library untuk membuat QR Code.
        
    *   **pdf.js:** Library untuk membaca dan mengekstrak teks dari file PDF.
        
    *   **KaTeX:** Library untuk merender rumus matematika (LaTeX) menjadi format Rich Text.
        

4\. Untuk Siapa Aplikasi Ini?
-----------------------------

Aplikasi ini sangat cocok untuk:

*   **Pembicara Seminar & Webinar:** Untuk menguji pemahaman audiens dan membuat sesi lebih interaktif.
    
*   **Trainer & Pengajar:** Sebagai alat untuk _ice breaking_ atau post-test setelah sesi pelatihan.
    
*   **Event Organizer:** Sebagai nilai tambah untuk acara-acara korporat, _gathering_, atau pameran.
    
*   **Guru & Dosen:** Untuk membuat kuis cepat di dalam kelas tanpa perlu persiapan manual yang lama.
    

5\. Cara Menggunakan
--------------------

### Alur untuk Admin

1.  **Buka Aplikasi & Login:** Pilih peran "Saya Pembicara (Admin)" dan masukkan password.
    
2.  **Konfigurasi Awal:** Masukkan URL Web App dari Google Apps Script dan Kunci API Gemini. Pengaturan ini akan tersimpan otomatis. (Lihat **Panduan Konfigurasi Awal** di bawah untuk detailnya).
    
3.  **Kustomisasi (Opsional):** Unggah logo dan pilih warna tema pada bagian "Kustomisasi Tampilan".
    
4.  **Pilih Sumber Materi:** Pilih salah satu tab sumber materi (PDF, Teks, URL, atau Bank Soal).
    
5.  **Buat Soal:** Masukkan materi Anda, pilih jumlah soal, lalu klik "Buat Soal dengan AI".
    
6.  **Tinjau Soal:** Periksa dan edit soal yang dihasilkan AI jika perlu.
    
7.  **Simpan & Aktifkan:** Klik "Simpan ke Bank Soal" (jika ingin disimpan) dan/atau "Aktifkan Kuis".
    
8.  **Bagikan Kuis:** Tampilkan QR Code atau bagikan tautan kepada peserta.
    
9.  **Pantau Leaderboard:** Buka bagian Leaderboard dan aktifkan "Update Otomatis" untuk melihat skor masuk secara real-time.
    

### Alur untuk Peserta

1.  **Gabung Kuis:** Pindai QR Code atau buka tautan yang dibagikan oleh admin.
    
2.  **Isi Data Diri:** Masukkan Nama Lengkap, Perusahaan/Institusi, dan No. WhatsApp.
    
3.  **Mulai Kuis:** Klik tombol "Mulai Kuis".
    
4.  **Jawab Pertanyaan:** Pilih jawaban yang dianggap benar dalam batas waktu yang ditentukan.
    
5.  **Lihat Hasil:** Setelah selesai, halaman hasil akan menampilkan skor akhir dan rincian jawaban.
    

Panduan Konfigurasi Awal (Langkah demi Langkah)
-----------------------------------------------

Bagian ini menjelaskan secara detail cara mendapatkan tiga kunci utama yang dibutuhkan aplikasi.

### A. Cara Mendapatkan URL Web App Google Sheet

Ini adalah langkah untuk membuat "database" kuis Anda.

1.  **Buat Google Sheet Baru:** Buka browser dan kunjungi https://docs.google.com/spreadsheets/. Beri nama file spreadsheet Anda, misalnya "Database Kuis Seminar".
    
2.  **Buka Editor Apps Script:** Pada menu di atas, klik **Ekstensi** > **Apps Script**. Sebuah tab baru berisi editor kode akan terbuka.
    
3.  **Tempel Kode Skrip:** Hapus semua kode contoh yang ada di dalam file Code.gs. Salin seluruh kode skrip yang tersedia di dalam aplikasi kuis (klik tombol **Bantuan**), lalu tempelkan ke dalam editor Apps Script yang kosong.
    
4.  **Simpan Proyek:** Klik ikon **Simpan proyek** (gambar disket) di bagian atas editor.
    
5.  **Deploy sebagai Aplikasi Web:**
    
    *   Klik tombol biru **Deploy** di pojok kanan atas, lalu pilih **Deployment baru**.
        
    *   Klik ikon gerigi (⚙️) di sebelah "Pilih Jenis", lalu pilih **Aplikasi Web**.
        
    *   Pada bagian **Konfigurasi**, isi sebagai berikut:
        
        *   **Deskripsi:** (Opsional) Isi dengan "Aplikasi Kuis Interaktif".
            
        *   **Jalankan sebagai:** Biarkan Saya (alamat email Anda).
            
        *   **Siapa yang memiliki akses:** **Ubah menjadi Siapa saja**. Ini sangat penting agar semua peserta bisa mengakses kuis.
            
    *   Klik tombol **Deploy**.
        
6.  **Berikan Izin Akses:** Google akan meminta otorisasi agar skrip dapat berjalan.
    
    *   Klik **Otorisasi akses**.
        
    *   Pilih akun Google Anda.
        
    *   Anda mungkin akan melihat peringatan "Google belum memverifikasi aplikasi ini". Ini normal. Klik **Lanjutan**, lalu klik **Buka \[nama proyek Anda\] (tidak aman)**.
        
    *   Tinjau izin yang diminta, lalu klik **Izinkan**.
        
7.  **Salin URL Aplikasi Web:** Setelah deployment berhasil, sebuah jendela akan muncul menampilkan **URL Aplikasi Web**. Salin URL ini. Inilah yang akan Anda tempelkan ke kolom "URL Web App Google Sheet" di aplikasi kuis.
    

### B. Cara Mendapatkan Kunci API Gemini

Ini adalah kunci untuk mengakses mesin AI pembuat soal.

1.  **Buka Google AI Studio:** Kunjungi [aistudio.google.com/app/apikey](https://aistudio.google.com/app/apikey).
    
2.  **Login dengan Akun Google:** Jika diminta, login menggunakan akun Google Anda.
    
3.  **Buat Kunci API:** Klik tombol **"Create API key in new project"**.
    
4.  **Salin Kunci API:** Sebuah kunci rahasia akan langsung dibuat dan ditampilkan. Salin kunci ini dan tempelkan ke kolom "Kunci API Gemini" di aplikasi kuis.
    
    *   **Penting:** Jaga kerahasiaan Kunci API ini dan jangan bagikan kepada siapa pun.
        

### C. Cara Mendapatkan Bitly Access Token (Opsional)

Langkah ini tidak wajib, namun berguna untuk membuat tautan kuis menjadi lebih pendek dan rapi.

1.  **Login ke Bitly:** Buka [bitly.com](https://bitly.com) dan login ke akun Anda. Jika belum punya, silakan mendaftar terlebih dahulu.
    
2.  **Masuk ke Pengaturan API:** Setelah login, klik foto profil Anda di pojok kanan atas, lalu pilih **Settings**. Di menu sebelah kiri, pilih **API**.
    
3.  **Buat Token Baru:** Di bawah bagian "Access tokens", masukkan password akun Bitly Anda untuk verifikasi, lalu klik **"Generate token"**.
    
4.  **Salin Token:** Token akses Anda akan muncul. Salin token tersebut dan tempelkan ke kolom "Bitly Access Token" di aplikasi kuis.
    

6\. Kemungkinan Pengembangan Fitur Baru
---------------------------------------

1.  **Sertifikat Digital:** Fitur untuk men-generate e-sertifikat (PDF) secara otomatis bagi peserta yang telah menyelesaikan kuis.
    
2.  **Mode Tim/Kelompok:** Peserta dapat mendaftar sebagai tim, dan leaderboard akan menampilkan skor tim selain skor individu.
    
3.  **Mode Presentasi (Sinkron):** Admin dapat mengontrol jalannya kuis soal per soal, di mana semua peserta menjawab pertanyaan yang sama secara bersamaan.
    
4.  **Analitik Jawaban:** Dasbor admin menampilkan statistik untuk setiap soal (misalnya, berapa persen peserta yang menjawab benar) untuk memberikan wawasan kepada pembicara.
    
5.  **Ekspor Hasil ke Excel/CSV:** Tombol untuk mengunduh semua data hasil kuis dan leaderboard ke dalam format file spreadsheet.
    
6.  **Tipe Soal Bervariasi:** Menambahkan dukungan untuk tipe soal lain seperti jawaban singkat atau benar/salah yang juga bisa dibuat oleh AI.
    
7.  **Gamifikasi Lanjutan:** Menambahkan elemen seperti avatar, lencana (badges) untuk pencapaian tertentu, dan efek suara untuk meningkatkan keseruan.
    
8.  **Integrasi Platform Streaming:** Menampilkan leaderboard sebagai _overlay_ langsung di platform seperti Zoom atau YouTube Live.
