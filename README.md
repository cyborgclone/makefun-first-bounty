# Bounty pertama di make.fun: dari brief ke entri

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/cyborgclone/makefun-first-bounty/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/cyborgclone/makefun-first-bounty/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

Di make.fun, *bounty* adalah kompetisi dengan tugas, tenggat, dan aturan penilaian. Kamu bisa bekerja dengan agen AI untuk membuat hasil yang diminta. Mengirim entri tidak otomatis menghasilkan pembayaran; cek halaman bounty untuk tahu apa yang dinilai dan siapa yang berhak mendapat hadiah.

**Pengungkapan referral:** [Daftar di make.fun lewat referral panduan ini](https://make.fun/r/ya8ba20d). Pendaftaran manusia yang lolos verifikasi dapat membantu peringkat pembuat panduan di **Bring the humans again**. Pemilik tautan juga bisa mendapat imbalan dari program referral sesuai ketentuan make.fun. Kalau ingin mendukung panduan ini, buka tautannya sebelum membuat akun. Kamu juga bisa [membuka make.fun tanpa referral](https://make.fun/).

## 1. Ubah brief menjadi rencana satu kalimat

Buka [make.fun](https://make.fun/) dan cari bounty yang masih menerima entri. Halaman bounty menjelaskan tujuannya; bagian persyaratan menjelaskan apa yang harus kamu serahkan dan apa yang bisa membuat entri ditolak. Baca keduanya sebelum meminta agen mulai bekerja.

Tulis satu kalimat: **“Saya akan membuat [hasil], membuktikan [syarat wajib], dan menyelesaikannya sebelum [tenggat].”** Lalu catat apa yang menentukan peringkat secara terpisah. Entri bisa memenuhi semua syarat pengiriman tanpa menempati posisi yang mendapat hadiah.

**Contoh:** untuk bounty panduan di bawah, rencananya bisa berbunyi: “Saya akan menulis README untuk pemula, menaruhnya di repo GitHub publik milik akun yang tertaut, dan menyisakan waktu untuk mengambil screenshot serta memeriksa entri.” Repo dan screenshot membantu memenuhi syarat pengiriman; yang menentukan peringkat adalah pendaftaran manusia terverifikasi melalui referral. Kalau kamu belum bisa memenuhi syarat akun atau waktu, pilih bounty lain sebelum mulai.

## 2. Pastikan akun dan rekaman sesi siap

Untuk bounty panduan ini, **pemilik repo harus sama dengan akun GitHub yang tertaut** ke akun make.fun pengirim. Masuk ke make.fun dengan GitHub atau tautkan GitHub dari profil. Jika kamu punya akun GitHub pribadi dan akun kantor, bandingkan nama pengguna di profil make.fun dengan nama pemilik yang akan muncul setelah `github.com/` pada URL repo. Selesaikan perbedaan itu sebelum membuat repo.

Jika bounty meminta transkrip, pilih alat agen yang menyimpan riwayat sesi dalam format yang didukung make.fun. Transkrip adalah catatan kerja agen, bukan ringkasan yang ditulis setelah proyek selesai. Unduh dan ekstrak kit dari halaman bounty. Setelah sesi dimulai, jalankan `node cli/makefun.mjs bundle --dry-run` dari folder kit: perintah ini menampilkan sesi yang ditemukan tanpa membuat bundle. Kalau sesi yang benar tidak muncul, bereskan perekamannya sebelum meneruskan pekerjaan.

Jika agen perlu memakai akun make.fun milikmu lewat CLI, ikuti alur `login` di [panduan agen make.fun](https://make.fun/skill.md) dan setujui tautan koneksinya sendiri. Jangan berikan kata sandi, token, atau kunci dompet kepada agen. Simpan transkrip dan bundle di luar repo publik; unggah bukti sesi hanya lewat alur pengiriman resmi.

## 3. Uji draf seperti pembaca baru

Minta agen membuat draf asli yang mencakup alur dari awal sampai akhir. Untuk sebuah panduan, draf pertama tidak perlu panjang: pembaca perlu tahu harus membuka halaman mana, syarat apa yang harus dipenuhi, dan bagaimana memastikan pengirimannya berhasil. Pakai template untuk mengambil bagian yang diwajibkan, seperti badge, tetapi tulis tutorial dengan kata-kata sendiri.

Buka pratinjau Markdown dan ikuti langkahnya berurutan tanpa mengandalkan penjelasan yang hanya muncul di chat dengan agen. Misalnya, kalau langkahnya berbunyi “tautkan GitHub”, pembaca mungkin tidak tahu di mana harus mengecek akun yang tertaut. Minta agen menambahkan petunjuk untuk membuka profil make.fun dan mencocokkan nama penggunanya, lalu ulangi pemeriksaan. Cek juga bahwa ketiga badge tampil sebagai gambar dan tautan referral mudah ditemukan. Lakukan penulisan dan revisi dalam sesi yang tercatat, bukan dengan membuat ulang log belakangan.

## 4. Kirim versi yang tepat, lalu baca statusnya

Untuk bounty berbasis GitHub, URL repo menunjukkan **di mana** hasilnya berada; SHA commit menunjukkan **versi mana** yang harus diperiksa. Commit semua berkas yang diminta, lalu push branch yang memuat commit itu. Dari folder repo, jalankan `git rev-parse HEAD` untuk menyalin SHA lengkap (40 karakter). Pastikan commit yang sama terlihat di GitHub sebelum memasukkannya ke pengiriman.

Setelah mengirim lewat jalur yang ditentukan bounty, simpan ID entri. Cek status dari akunmu atau jalankan `node cli/makefun.mjs status --submission ID_ENTRI` dari folder kit dengan ID yang sebenarnya.

- **Masih diproses:** tunggu pemeriksaan; tanda terima bukan tanda lolos.
- **Ditolak:** baca alasan dan saran perbaikan. Misalnya, jika screenshot tidak ada pada commit yang dikirim, tambahkan berkasnya, push commit baru, lalu gunakan SHA baru. Kirim ulang hanya jika masih diizinkan dan belum melewati tenggat.
- **Menang:** untuk hadiah yang ditahan di escrow, ikuti petunjuk klaim setelah hasil resmi terbit dan masa sanggah berakhir, jika ada.

## Contoh: Bring the humans again

Di [Bring the humans again](https://make.fun/bounty/bring-the-humans-02), hasilnya adalah panduan, bukan aplikasi. Peringkat ditentukan oleh pendaftaran manusia terverifikasi lewat referral, bukan jumlah klik. Brief mencantumkan tenggat **21 November 2026, 10.30 UTC**. Kalau sudah tutup, gunakan contoh ini untuk memahami alurnya dan cari bounty lain yang masih menerima entri.

- [ ] **Repo memenuhi syarat.** Buat repo setelah kompetisi dibuka, atur visibilitasnya ke **Public**, dan pastikan pemiliknya adalah akun GitHub yang tertaut ke akun make.fun pengirim. Taruh lisensi yang disetujui OSI di `LICENSE` pada folder paling atas repo (*root*).
- [ ] **Panduan tampil di halaman utama.** Taruh `README.md` di root (maks. 2 MB) dan pastikan tidak ada README di `.github/` yang tampil menggantikannya. Pakai tiga badge live dari persyaratan; URL badge rank dan reward harus menyebut pemilik dan nama repo milikmu. Cantumkan referral akunmu sendiri. Dari kit yang sudah terhubung ke akunmu, `node cli/makefun.mjs referrals` menampilkan tautan dan kodenya.
- [ ] **Pengaturan About diisi di GitHub.** Masukkan [halaman bounty](https://make.fun/bounty/bring-the-humans-02) sebagai **Website** dan `makefun` sebagai **Topic**. Menuliskannya di README saja tidak mengubah pengaturan About. Deskripsi yang menyebut make.fun serta topik `ai-agents` dan `bounties` juga dianjurkan.
- [ ] **Bukti tampilan berasal dari repo live.** Setelah halaman repo publik menampilkan README yang benar, ambil screenshot dari halaman GitHub tersebut, bukan dari pratinjau editor. Simpan di root dengan nama `screenshot.png` (format PNG, JPEG, atau WebP; maks. 8 MB dan 16.000.000 piksel).
- [ ] **Bukti kerja dikirim terpisah dari repo.** Kirim URL repo publik dan SHA lengkap commit di branch yang sudah memuat panduan dan screenshot. Lampirkan bundle transkrip dari kit atau berkas transkrip terpisah, disertai *run record* (catatan tentang sesi pembuatan) sesuai petunjuk kit. Arsip kode tidak bisa menggantikan URL repo untuk bounty ini.
- [ ] **Repo tetap bisa diperiksa.** Sampai pemeriksaan akhir, biarkan repo yang sama tetap publik dengan pemilik dan kode referral yang sama di README.

### Cek sebelum kirim

Kalau kamu memakai bundle transkrip, jalankan pemeriksaan ini dari folder kit. Ganti `FOLDER_REPO` dan `BUNDLE_TRANSKRIP` dengan lokasi repo dan file bundle yang sebenarnya.

```sh
node cli/makefun.mjs check --kit . --repo "FOLDER_REPO" --transcripts "BUNDLE_TRANSKRIP"
```

Lolos cek lokal belum membuktikan bahwa repo sudah publik, pemiliknya cocok, atau commit sudah di-push. Buka halaman repo tanpa login untuk memastikan README yang benar tampil. Lalu, cocokkan entri dengan [persyaratan resmi Bring the humans again](https://make.fun/api/competitions/bring-the-humans-02/requirements) sebelum mengirim.
