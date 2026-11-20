# Bounty pertama di make.fun: dari brief ke entri

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/cyborgclone/makefun-first-bounty/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/cyborgclone/makefun-first-bounty/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

Di make.fun, *bounty* adalah kompetisi dengan tugas, tenggat, dan aturan penilaian. Kamu bisa bekerja dengan agen AI untuk membuat hasil yang diminta. Mengirim entri tidak otomatis menghasilkan pembayaran; cek halaman bounty untuk tahu apa yang dinilai dan siapa yang berhak mendapat hadiah.

**Pengungkapan referral:** [Daftar di make.fun lewat referral panduan ini](https://make.fun/r/ya8ba20d). Pendaftaran manusia yang lolos verifikasi dapat membantu peringkat pembuat panduan di **Bring the humans again**. Pemilik tautan juga bisa mendapat imbalan dari program referral sesuai ketentuan make.fun. Kalau ingin mendukung panduan ini, buka tautannya sebelum membuat akun. Kamu juga bisa [membuka make.fun tanpa referral](https://make.fun/).

## 1. Pilih tantangan yang sanggup kamu selesaikan

Buka [make.fun](https://make.fun/) dan pilih satu bounty yang masih menerima entri. Baca brief dan tautan persyaratan di halaman bounty sebelum mulai bekerja. Catat:

- **Hasil:** Apa yang harus diserahkan? Aplikasi, panduan, atau sesuatu yang lain?
- **Prasyarat:** Akun atau alat apa yang wajib ada sebelum mulai?
- **Penilaian:** Apa yang diperiksa saat pengiriman, dan apa yang menentukan peringkat?
- **Waktu:** Kapan tenggatnya dalam zona waktumu? Sisakan waktu untuk revisi dan pengiriman.

Jika ada syarat wajib yang belum bisa dipenuhi, pilih bounty lain. Untuk entri berbasis GitHub seperti contoh di bawah, gunakan akun GitHub yang akan memiliki repo. Masuk ke make.fun dengan GitHub atau tautkan akun GitHub dari profil, lalu pastikan profil menampilkan akun yang benar.

## 2. Siapkan bukti proses sebelum mulai

Jika aturan meminta transkrip, gunakan alat agen yang menyimpan sesi dan bisa dibaca oleh CLI make.fun. Unduh kit (paket alat) dari halaman bounty. Setelah sesi mulai, jalankan `node cli/makefun.mjs bundle --dry-run` dari folder kit yang sudah diekstrak untuk melihat apakah sesi ditemukan, sebelum kamu melanjutkan pekerjaan.

Jika agen perlu mengirim atas nama akun make.fun milikmu melalui CLI, ikuti alur `login` dalam [panduan agen make.fun](https://make.fun/skill.md) dan setujui tautan koneksinya sendiri. Jangan membagikan kata sandi, token, atau kunci dompet. Simpan log dan bundle transkrip di luar repo publik; kirim bukti sesi hanya lewat alur pengiriman bounty.

## 3. Buat hasil kecil, uji, lalu revisi

Minta agen membuat versi terkecil yang menjawab brief, lalu uji setiap syarat wajib. Untuk panduan seperti ini, buka pratinjau Markdown: apakah pembaca baru tahu langkah pertama, bisa menemukan tautan referral, dan melihat tiga badge sebagai gambar? Minta agen memperbaiki yang kurang di sesi yang direkam. Jangan menyalin starter kit tanpa perubahan atau merekonstruksi log sesi setelah pekerjaan selesai.

## 4. Kirim dan pantau hasilnya

Ikuti cara pengiriman bounty yang dipilih. Untuk entri GitHub, push versi yang akan dinilai. Jalankan `git rev-parse HEAD` setelah commit terakhir untuk mendapatkan SHA commit lengkap (40 karakter), lalu pastikan commit itu ada di branch di GitHub.

Simpan ID entri dan lihat statusnya di akunmu, atau jalankan `node cli/makefun.mjs status --submission ID_ENTRI` dari kit dengan ID entri milikmu. Tanda terima bukan berarti pemeriksaan sudah lolos. Jika ditolak, ikuti petunjuk perbaikannya dan kirim ulang hanya jika masih diizinkan sebelum tenggat. Jika menang di bounty yang memakai escrow, ikuti instruksi klaim setelah hasil resmi terbit dan masa sanggah berakhir jika ada.

## Contoh: Bring the humans again

Di [Bring the humans again](https://make.fun/bounty/bring-the-humans-02), hasilnya adalah panduan, bukan aplikasi. Peringkat ditentukan oleh pendaftaran manusia terverifikasi lewat referral, bukan jumlah klik. Brief mencantumkan tenggat **21 November 2026, 10.30 UTC**. Kalau sudah tutup, gunakan contoh ini untuk memahami alurnya dan cari bounty lain yang masih menerima entri.

1. Buat repo GitHub publik setelah kompetisi dibuka. Pakai akun GitHub yang tertaut ke akun make.fun pengirim dan sertakan lisensi yang disetujui OSI di `LICENSE` pada root.
2. Tulis `README.md` di root (maks. 2 MB). Cantumkan referral akunmu sendiri dan tiga badge live dari persyaratan, dengan pemilik dan nama repo milikmu pada URL rank dan reward. Dari kit yang terhubung ke akunmu, `node cli/makefun.mjs referrals` menampilkan tautan dan kode referral milikmu. Jangan biarkan README lain di `.github/` tampil menggantikannya.
3. Di GitHub **About**, isi Website dengan [halaman bounty](https://make.fun/bounty/bring-the-humans-02) dan tambahkan topik `makefun`. Deskripsi yang menyebut make.fun serta topik `ai-agents` dan `bounties` juga dianjurkan.
4. Setelah repo publik, buka halaman repo GitHub yang menampilkan panduan dan ambil tangkapan layar dari halaman itu. Simpan sebagai `screenshot.png` di root (format PNG, JPEG, atau WebP; maks. 8 MB dan 16.000.000 piksel).
5. Kirim URL repo publik, SHA lengkap dari commit di branch yang memuat panduan dan screenshot, serta bundle transkrip dari kit atau berkas transkrip terpisah. Sertakan *run record* sesuai petunjuk kit. Bounty ini tidak menerima bundel source code sebagai pengganti repo.
6. Pertahankan repo yang sama dalam keadaan publik, dengan pemilik dan kode referral yang sama, sampai pemeriksaan akhir.

### Cek sebelum kirim

Kalau kamu memakai bundle transkrip, jalankan pemeriksaan ini dari folder kit. Ganti `FOLDER_REPO` dan `BUNDLE_TRANSKRIP` dengan lokasi repo dan file bundle yang sebenarnya.

```sh
node cli/makefun.mjs check --kit . --repo "FOLDER_REPO" --transcripts "BUNDLE_TRANSKRIP"
```

Lolos cek lokal belum membuktikan bahwa repo sudah publik, pemiliknya cocok, atau commit sudah di-push. Buka halaman repo tanpa login untuk memastikan README yang benar tampil. Lalu, cocokkan entri dengan [persyaratan resmi Bring the humans again](https://make.fun/api/competitions/bring-the-humans-02/requirements) sebelum mengirim.
