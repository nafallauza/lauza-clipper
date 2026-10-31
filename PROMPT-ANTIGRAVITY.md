# Prompt untuk Antigravity

Paket lokal sudah disiapkan di:
`/home/lauza/remotion-workspace/lauza-clipper`

Repo GitHub tujuan: `https://github.com/nafallauza/lauza-clipper`

Tugasmu: tinjau paket tersebut, lalu commit dan push hanya paket Lauza Clipper
ke repo tujuan. Jangan membuat atau mengunggah video dalam tugas ini.

1. Baca `SKILL.md`, `README.md`, `brand.json`, dan referensi yang ditautkan.
   Palette kuning/abu-abu/hitam sudah disepakati; Montserrat masih proposal.
   Jangan menulis bahwa sinkronisasi Timothy sudah beres. Jangan mengubah
   default koreksi video menjadi 100 ms; default di kit harus tetap nol.
2. Jika URL tujuan belum diisi, tanyakan URL kepada user sekali. Jangan
   menebak akun/repo dan jangan membuat repo baru tanpa instruksi user.
3. Periksa status Git workspace. Ada perubahan proyek lain di
   `remotion-workspace`; jangan ikutkan atau mengembalikan perubahan tersebut.
   Jangan memakai `git add .` atau `git add -A` di workspace sumber.
4. Gunakan checkout/staging terpisah di luar workspace sumber. Untuk repo
   tujuan kosong, tempatkan isi `lauza-clipper` di root repo, branch `main`.
   Untuk repo yang sudah berisi proyek lain, gunakan branch baru
   `feat/lauza-clipper-kit` dan letakkan paket di `skills/lauza-clipper/`.
   Pertahankan isi repo lain; jangan menimpa file yang sudah ada tanpa review.
5. Bawa hanya isi paket: skill, metadata agent, README/prompt, JSON, referensi,
   preview PNG, tiga font Montserrat OTF, OFL, dan `.gitignore`.
   Jangan bawa video Timothy, audio, PDF, ZIP referensi, node_modules, cache,
   model AI, `.env`, kredensial, folder `.git`, atau link instalasi lokal Codex.
6. Validasi JSON; cek link relatif serta keberadaan file font/preview/OFL.
   Jika validator skill Codex tersedia, jalankan `quick_validate.py` pada
   folder skill yang sebenarnya. Jangan menganggap template sebagai renderer
   atau skema upstream FCM. Jangan mengklaim telah merender video dari paket ini.
7. Tampilkan ringkasan file dan diff yang akan dipush. Setelah URL tujuan jelas
   dan review lokal lulus, lanjutkan commit serta push sesuai tugas ini.
   Commit message: `Add Lauza podcast clipper skill and visual kit`.
   Gunakan push biasa ke branch yang tepat; jangan force-push atau mengubah
   konfigurasi identitas Git global. Jika autentikasi/izin gagal, laporkan
   hambatan sebenarnya beserta langkah yang perlu dilakukan user.
8. Laporkan URL repo/branch, hash commit, file utama, dan hasil validasi.
   Untuk branch `feat/lauza-clipper-kit`, sertakan tautan compare/PR jika tersedia;
   jangan merge atau publish hal lain tanpa instruksi.
