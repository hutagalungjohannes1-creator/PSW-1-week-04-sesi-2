Nama    : Johannes Hutagalung
Prodi   : D4 TRPL
NIM     : 41426034

1. persiapan stylesheet
a. Ringkasan Tugas
Menghubungkan file style.css ke halaman index.html dan memastikan koneksi stylesheet berjalan dengan baik tanpa error 404.
b. Menambahkan warna latar belakang body dengan kode warna f4f6fa di dalam file style.css
c. Membuka browser dan mengecek menu DevTools pada bagian Network untuk memastikan file style.css berhasil dimuat.

Hasil Pengamatan
1. Warna latar belakang web berubah menjadi abu-abu terang, menandakan file css sudah terhubung.
2. Pada menu Network di DevTools, status file style.css menunjukkan angka 200 OK yang artinya file berhasil dipanggil dan tidak error 404.

2. Selector dan Class
a. Ringkasan
Menambahkan class card pada elemen form dan class notice pada paragraf petunjuk untuk menguji penerapan selector CSS.

b. Tindakan yang Dilakukan
1. Menambahkan aturan form.card dan .notice pada file style.css
2. Memastikan tag <form class="card"> dan <p class="notice"> sudah terpasang dengan benar di file index.html.
3. Membuka DevTools di browser (F12) lalu melihat tab Elements untuk mengecek apakah aturan CSS sudah jalan pada form.
4. Coba mengubah nama class secara sementara di DevTools untuk melihat bedanya saat class cocok dan tidak cocok.

Hasil Pengamatan:
1. Tampilan form dan teks petunjuk berubah warnanya sesuai aturan di CSS.
2. Saat nama class diubah jadi nama lain, gaya CSS-nya langsung hilang. Gaya baru muncul lagi kalau nama class-nya dikembalikan seperti semula.

3.  KONFLIK SPECIFICITY
Apa yang Dikerjakan:
Menguji dua aturan CSS yang bentrok warna pada teks petunjuk form untuk melihat mana aturan yang menang.

Langkah-langkah:
1. Menambahkan aturan card p { color: purple; } dan notice { color: orange; } di file style.css.
2. Membuka browser untuk melihat warna teks yang dihasilkan.
3. Memeriksa tab Styles pada DevTools untuk melihat aturan mana yang dicoret.

Langkah-langkah:
1. Menambahkan aturan card p { color: purple; } dan .notice { color: orange; } di file style.css.
2. Membuka browser untuk melihat warna teks yang dihasilkan.
3. Memeriksa tab Styles pada DevTools untuk melihat aturan mana yang dicoret.

4. UKURAN KOTAK
Apa yang Dikerjakan:
Menguji perbedaan perhitungan lebar elemen kartu menggunakan mode Box Model biasa dan mode border-box.

Langkah-langkah:
1. Menambahkan aturan width 240px, padding 16px, border 2px, dan margin 12px pada .card.
2. Memeriksa diagram Box Model di DevTools untuk mengukur total lebar kotak.
3. Menambahkan properti box-sizing: border-box lalu mengukur ulang lebarnya.
4. Mengembalikan ukuran width menjadi fleksibel kembali untuk tampilan final.

Hasil Pengamatan:
1. Tanpa border-box lebar total kartu di layar menjadi 276px (240px + padding 32px + border 4px).
2. Setelah ditambah box-sizing: border-box, lebar kartu berubah dan terkunci pas menjadi 240px.

5. LATIHAN MANDIRI DAN MATRIKS UJI
Hasil Uji Coba:
1. Kasus Normal
   Saat isi semua kolom form dengan benar, form bisa diisi lancar dan tombol daftar bisa diklik tanpa masalah.

2. Kasus Batas
   Saat isi kode peserta pas 6 angka dan jumlah tiket pas 5, inputan diterima karena sesuai batas aturan.

3. Kasus Gagal
   Saat sengaja salah ketik nama file CSS, tampilan web jadi polos/berantakan dan di DevTools muncul pesan error 404.

6. Troubleshooting dan AI Use Statement
1. Cara Mengatasi Error (Troubleshooting)
- Halaman Tidak Berubah: Simpan file dulu, lalu refresh browser.
- Error 404: Cek ulang nama folder dan nama file CSS biar gak ada yang salah ketik.
- Tampilan CSS Tidak Cocok: Cek urutan kode dan nama class di DevTools.
- Kode Error / Elemen Kosong: Cek tanda kurung dan susunan tag HTML di VS Code.

2. Pernyataan Penggunaan AI (AI Use Statement)
- Alat yang Digunakan: AI / Asisten Chat.
- Tujuan: Membantu memahami konsep CSS, merapikan struktur tag HTML yang salah, dan menyusun laporan.
- Verifikasi: Semua saran dan kode dari AI sudah dicoba langsung di browser dan dipastikan berjalan dengan baik.

7. laporan Validator
   - Before: Terdeteksi warning karena terdapat penggunaan tag <h1> ganda pada judul halaman dan judul bagian pendaftaran
   After: Mengubah tag judul bagian menjadi <h2>[cite: 8]. Hasil pengecekan bersih (0 Error, 0 Warning)