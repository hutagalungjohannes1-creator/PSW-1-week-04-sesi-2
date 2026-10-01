Nama    : Johannes Hutagalung
Prodi   : D4 TRPL
NIM     : 41426034

1. MENYIAPKAN FORM DAN ATURAN WAJIB
Catatan Hasil Pengujian Input Jumlah Tiket:
- Nilai Kosong: Ditolak oleh browser dengan pesan peringatan wajib diisi (required).
Nilai 0: Ditolak karena kurang dari batas minimal (min="1")
Nilai 1: Diterima karena memenuhi syarat batas min="1" dan max="5"
Nilai 5: Diterima karena memenuhi syarat batas min="1" dan max="5".
Nilai 6: Ditolak karena melebihi batas maksimal (max="5").
Nilai 1.5: Ditolak karena bukan bilangan bulat sesuai aturan

2. FORMAT DAN PETUNJUK YANG TERHUBUNG
Catatan Hasil Pengujian Kode Peserta:
A. 001234: Diterima. Tepat 6 digit angka dan nol di awal tetap  tersimpan karena tipe input berupa text.
B. 12345: Ditolak. Jumlah angka kurang dari 6 digit
C. abc123: Ditolak. Mengandung huruf (tidak sesuai pola hanya angka).
D. Kosong: Ditolak karena terdapat atribut required.
E. Uji Fokus Label: Ketika teks label diklik, kursor/fokus langsung berpindah ke kolom input kode.
F. Pemeriksaan Accessibility DevTools:
Accessible Name: Kode peserta (6 angka, wajib) (diambil dari elemen <label>).
G. Accessible Description: Contoh: 001234. Gunakan tepat enam angka. (dihubungkan via aria-describedby="kode-help").
H. Penjelasan inputmode vs Validasi: Atribut inputmode="numeric" hanya berfungsi memunculkan papan ketik angka pada perangkat seluler/HP dan TIDAK melakukan validasi. Validasi sebenarnya dilakukan oleh atribut pattern="[0-9]{6}" dan required.

3. KEYBOARD DAN FOKUS
Indikator Fokus: Terlihat sangat jelas berupa garis outline warna biru saat berpindah elemen menggunakan tombol Tab.
Urutan Navigasi: Berjalan secara logis dari atas ke bawah mengikuti alur dokumen tanpa perlu menggunakan tabindex positif.
Pengoperasian Tanpa Mouse: 100% berhasil. Seluruh kontrol seperti input teks, pilihan prodi, radio button, checkbox, dan tombol daftar dapat dijangkau serta diisi penuh menggunakan keyboard (Tab, Shift+Tab, Panah, Space, Enter).

4. MATRIKS UJI DAN EKSPERIMEN KEGAGALAN
 Catatan Pengujian Kasus Form:
 Email Kosong: Form ditolak browser dengan peringatan wajib diisi.
 Email abc: Form ditolak browser karena format email tidak valid (tanpa @).
 Email Contoh Valid: Form menerima input dengan baik.
 Jumlah 0 / 6: Form ditolak karena berada di luar jangkauan minimal 1 dan maksimal 5.
 Jumlah 1 / 5: Form menerima input.
 Jumlah 1.5: Form ditolak karena step="1" mengharuskan angka bulat.
 Kode 12345: Form ditolak karena kurang dari 6 digit.
 Kode 001234:  Form menerima input 6 digit angka.
 Keyboard: Semua kontrol formulir dapat dicapai dan dioperasikan lancar.
 a. Mengapa Server Tetap Perlu Memvalidasi Data:
 Server wajib memvalidasi data karena validasi di browser hanya bertujuan membantu kenyamanan pengguna bukan untuk keamanan. Pengguna dapat dengan mudah mengubah HTML via DevTools atau langsung mengirimkan data ke server menggunakan aplikasi lain. Validasi server adalah benteng utama untuk menjamin integritas data dan keamanan dari ancaman bahaya.

 5. Pernyataan Penggunaan AI (AI Use Statement):
 Alat AI yang Digunakan: Gemini AI.
 Tujuan Penggunaan: Membantu penjelasan konsep HTML/CSS, membaca dan memperbaiki pesan error syntax, serta membantu penyusunan laporan hasil pengujian dan audit aksesibilitas.
 Bagian Kode yang Dibantu:

Perbaikan tag HTML pada gambar (<figure>, <img>, dan <figcaption>).
Konfigurasi indikator fokus CSS (input:focus-visible)
Atribut aksesibilitas (aria-describedby, pattern, inputmode, required).
Verifikasi Mandiri: Seluruh kode hasil bantuan AI telah saya uji langsung secara manual di browser 
 

