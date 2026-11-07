Dokumentasi Kegiatan Workshop: Building with AI, Managing Change with GitHub

Nama Lengkap: Rafli Andhika

Deskripsi Singkat

Repository ini berisi catatan, rangkuman materi, serta alur kerja yang dipelajari selama mengikuti workshop "Building with AI, Managing Change with GitHub". Repository ini digunakan untuk mendokumentasikan pemahaman mengenai penggunaan AI untuk pengembangan aplikasi sederhana serta manajemen versi kode menggunakan Git dan GitHub.

Tujuan & Kegunaan

Dokumentasi & Portofolio: Menyimpan rekam jejak praktik pembelajaran pembuatan aplikasi berbasis AI dan integrasi Git/GitHub.

Referensi Mandiri: Sebagai panduan praktis untuk melakukan setup Git, SSH key, prompt engineering, serta version control di masa depan.

Kolaborasi & Repositori Kode: Menyimpan kode sumber (source code) proyek Student Task Planner yang dibangun selama sesi workshop.

Informasi Kegiatan Workshop

Nama Workshop: Building with AI, Managing Change with GitHub

Narasumber / Pembicara: Nugi Farhan (Senior Product Designer / UX Advisor)

Tanggal & Waktu: 7 november 2026

Dokumentasi & Rangkuman Materi

1. Materi & Topik Utama

Workshop ini membahas dua pilar utama dalam pengembangan perangkat lunak modern:

Prompt Engineering (Building with AI): Teknik merancang instruksi yang tepat agar AI menghasilkan kode/solusi yang relevan dan siap pakai.

Git & GitHub (Managing Change): Konsep sistem kontrol versi terdistribusi, alur kerja Git lokal, integrasi ke GitHub online, serta konfigurasi keamanan (SSH Key).

Studi Kasus: Pembuatan aplikasi Student Task Planner memanfaatkan AI dan pengelolaan kodenya dengan Git/GitHub.

2. Catatan & Rangkuman Materi

A. Prompt Engineering (Building with AI)

Pengertian: Prompting adalah cara merancang masukan/instruksi agar model AI memberikan jawaban yang akurat, relevan, dan efisien.

Struktur Prompt yang Baik:

Role: Menentukan peran AI (misal: "You are helping me build a beginner-friendly student task planner...").

Task/Goal: Tujuan utama yang ingin dicapai.

Context: Latar belakang dan kebutuhan spesifik pengguna.

Constraints: Batasan teknis (misal: "Use HTML, CSS, and vanilla JavaScript without external libraries").

Format/Output: Bentuk luaran yang diharapkan (misal: "Provide complete code for each file").

Keuntungan Prompt Engineering: Meningkatkan performa model AI, mengurangi bias/respons ofensif, meningkatkan kontrol & keterprediksian, serta memberikan pengalaman pengguna yang lebih baik.

B. Git & GitHub Fundamentals

Perbedaan Git & GitHub:

Git: Distributed Version Control System (DVCS) lokal untuk melacak perubahan file.

GitHub: Platform berbasis web untuk menyimpan repositori Git secara online dan memfasilitasi kolaborasi.

Tiga Area Utama Git (Git Workflow):

Working Directory: Direktori kerja tempat file proyek dibuat dan dimodifikasi secara lokal.

Staging Area (Index): Area tempat menampung perubahan file sebelum disimpan secara permanen.

Git Directory (Repository): Tempat simpanan metadata dan basis data objek proyek yang sudah di-commit.

C. Perintah Dasar Git & GitHub

Setup Identitas:

git config --global user.name "Nama Anda"
git config --global user.email "email@example.com"


Alur Perubahan Lokal:

git init : Memulai repositori baru.

git add . atau git add -A : Memindahkan seluruh file/perubahan ke Staging Area.

git commit -m 'catatan perubahan' : Menyimpan riwayat perubahan dari Staging Area ke Repository lokal.

Integrasi Remote (GitHub):

git remote add <name> <url> : Menghubungkan repositori lokal ke repositori remote.

git push origin main : Mengunggah commit lokal ke repositori GitHub online.

git pull origin main : Mengambil dan menggabungkan perubahan terbaru dari remote ke lokal.

D. Autentikasi Keamanan (SSH Key Setup)

Membuat SSH Key berbasis Ed25519 untuk autentikasi aman ke GitHub:

ssh-keygen -t ed25519 -C "email@domain.com"


Mengaktifkan SSH Agent & mendaftarkan key pada macOS Keychain (~/.ssh/config).

Menambahkan Public Key (pbcopy < ~/.ssh/id_ed25519.pub) ke pengaturan SSH Keys di GitHub.

Verifikasi koneksi menggunakan perintah:

ssh -T git@github.com
