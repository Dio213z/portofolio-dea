# Dea Nuraini — Album Kecilku
HTML, CSS, JavaScript statis. Tema coquette coklat: sampul album tengah, potret oval, kartu surat, renda cream, pita caramel, hiasan hati dan animasi halus.

## Jalankan
Ekstrak ZIP dan buka index.html. Font dan aset disertakan lokal. Tidak membutuhkan npm install.

## Data diri
Dea Nuraini, X RPL 3, absen 1. SDN Wirobiting 1, SMPN 1 Prambon, SMK Krian 1 Sidoarjo.
HTML & CSS, JavaScript, Python, Java ditampilkan 100% sebagai penilaian diri sesuai formulir, bukan bukti sertifikasi.
WhatsApp 087755277520 sudah ditautkan ke format internasional 6287755277520. Tautan membuka percakapan, bukan mengirim otomatis.

## Foto profil
Edit config.js, bagian PORTFOLIO_PROFILE.imageUrl. Isi URL HTTPS publik langsung menuju gambar, bukan halaman album/login. Bisa juga path lokal assets/fotoprofil.jpg.
objectPosition mengatur posisi pemotongan visual, misalnya center top.
Jika URL kosong/gagal, website mencoba assets/fotoprofil.png, .jpg, .jpeg; terakhir menampilkan inisial dn.
Foto asli belum diberikan. Email dan Instagram juga belum diberikan dan dapat diisi di config.js.

## Prestasi
Folder asset disediakan untuk sertifikat/foto prestasi asli: prestasi1.png, prestasi2.jpg, prestasi3.jpeg, dan seterusnya.
Tanpa build: harus berurutan mulai nomor 1; pencarian berhenti pada nomor pertama yang kosong.
Dengan build: semua file dengan pola tersebut ditemukan, termasuk nomor yang tidak berurutan.
Jalankan: node scripts/build-prestasi.mjs
Output: dist, sudah berisi daftar galeri otomatis. Foto bisa diperbesar dengan klik.

## GitHub / Vercel
Unggah isi ZIP yang sudah diekstrak ke root repository GitHub. Pastikan index.html dan vercel.json berada di root.
Import repo di Vercel; vercel.json mengatur build node scripts/build-prestasi.mjs, output dist, tanpa framework.
Deploy ulang setelah menambah foto prestasi. Untuk hosting statis lain, unggah isi dist. GitHub Pages tanpa build juga bisa memakai nomor prestasi berurutan.

## Tiga proyek baru
- Surat Mini: kartu ucapan dengan pilihan kertas dan unduhan pesan .txt; isi tidak dikirim ke server. Kertas hanya untuk pratinjau, file unduhan berupa teks biasa.
- Ritme Belajar: timer 1/5/15 menit, mulai/jeda/reset, memakai waktu target agar tidak melambat karena tab latar. Saat kembali ke tab, tampilan diperbarui pada tick berikutnya. Menutup dialog menghentikan sesi, tanpa suara.
- Susun Kata: lima teka-teki istilah pemrograman, validasi jawaban, progres dan ulang dari awal.
Demo dibuat untuk portofolio ini, bukan klaim proyek terdahulu.

## Tampilan & animasi
Pita bergoyang, potret dan surat melayang, hati di tepi layar, jam berputar, amplop melayang, dan efek scroll. Tombol jeda menghentikan animasi dekoratif; timer memiliki tombol jeda sendiri. Reduced motion perangkat dihormati. Menu mobile, tema terang/gelap dan navigasi keyboard tersedia.
Lisensi font lokal disertakan di assets/fonts.
