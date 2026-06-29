# Final Project IMK Kelompok 9
| Nama           | NRP        | Kelas     | Tim |
| ---            | ---        | ----------| --- |
| Umi Lailatul Khotimah | 5025241062 | Interaksi Manusia dan Komputer (A)       | A |
| Nabilah Bunga  | 5025241073           | Interaksi Manusia dan Komputer (A)       | A |
| Callista Fidelya  | 5025241086 | Interaksi Manusia dan Komputer (A)       | A |
| Willy Marcelius | 5025241096 | Interaksi Manusia dan Komputer (A)       | B |
| Rendy Tanuwijaya | 5025241099           | Interaksi Manusia dan Komputer (A)       | B |

## Tim A (Pasar Hanacaraka)

### Anggota Tim
| Nama           | NRP        | Kelas     |
| ---            | ---        | ----------|
| Umi Lailatul Khotimah | 5025241062 | Interaksi Manusia dan Komputer (A)     
| Nabilah Bunga  | 5025241073           | Interaksi Manusia dan Komputer (A)  
| Callista Fidelya  | 5025241086 | Interaksi Manusia dan Komputer (A)       

DOMAIN APLIKASI : https://nabilahbunga26.github.io/IMK9APASARHANACARAKA/

VIDEO : https://drive.google.com/drive/folders/1jg_Knq2vDVSJEWoqBetLESjnzyqCnIFw?usp=sharing

Pasar Hanacaraka adalah aplikasi permainan edukasi interaktif yang dirancang untuk membantu siswa, guru, dan pengguna umum dalam mempelajari aksara Jawa (Hanacaraka) secara menyenangkan melalui simulasi jual-beli di pasar tradisional.

### Arsitektur & Teknologi

Aplikasi ini dikembangkan menggunakan tumpukan teknologi modern untuk performa yang optimal dan pengalaman pengguna yang lancar:

*   **Frontend**: React 18+ dengan Vite sebagai alat pembangunan (build tool).
*   **Styling**: Tailwind CSS untuk antarmuka yang responsif, bersih, dan modern.
*   **Backend & Database**: Firebase (Firestore) untuk persistensi data pengguna dan Firebase Authentication untuk sistem login yang aman.
*   **Bahasa Pemrograman**: TypeScript untuk memastikan keamanan tipe (type safety) di seluruh basis kode.

### Alur Aplikasi (User Journey)

1.  **Peluncuran (Splash Screen)**: Pengguna disambut dengan animasi splash screen yang dilengkapi indikator loading visual.
2.  **Onboarding**: Pengguna baru akan dipandu melalui carousel interaktif untuk memahami konsep dasar game dan cara bermain.
3.  **Autentikasi**: Pengguna dapat memilih untuk:
    - **Mendaftar/Masuk**: Menggunakan email atau akun sosial untuk menyimpan progres secara permanen.
    - **Mode Tamu**: Bermain langsung dengan batasan progres tidak tersimpan (tersedia informasi transparan mengenai batasan ini).
    - **Pemulihan Akun**: Tersedia fitur 'Lupa Password' pada halaman login.
4.  **Pemilihan Peran**: Pengguna memilih peran sebagai **Pembeli** (berbelanja barang di pasar) atau **Penjual** (melayani pembeli). Tersedia penjelasan (tooltip/modal) untuk setiap peran.
5.  **Pemilihan Level**: Pengguna memilih level belanja (dasar, menengah, mahir). Level yang belum terbuka (locked) memiliki indikator visual gembok yang jelas.
6.  **Pemilihan Warung**: Pengguna memilih jenis warung (misal: Jamu, Buah). Warung yang terkunci tidak dapat diakses dan memberikan umpan balik (toast) kepada pengguna.
7.  **Gameplay**:
    - **Mode Penjual**: Melayani pembeli dengan mencocokkan aksara.
    - **Mode Pembeli**: Berbelanja barang di pasar dengan mengenali aksara.
    - **Mode Belajar**: Latihan menulis aksara dengan panduan *stroke order*.
    - **Kontrol**: Pengguna dapat melakukan pause permainan kapan saja.
8.  **Progres & Pencapaian**: Pengguna dapat memantau progres pribadi, peringkat di leaderboard, serta berbelanja item di toko menggunakan koin yang didapat.

### Fitur Utama

- **Sistem Autentikasi Firebase**: Mendukung pendaftaran, login, lupa password, dan mode tamu yang aman.
- **Simulasi Pasar Interaktif**: Berbagai jenis warung dengan mekanisme gameplay jual-beli yang berbeda untuk penjual dan pembeli.
- **Sistem Pembelajaran Aksara**: Visualisasi aksara Jawa yang ramah edukasi, termasuk panduan *stroke order* untuk penulisan yang benar.
- **Sistem Ekonomi & Progresi**: Mekanisme perolehan Koin dan XP (Experience Points) untuk naik level dan membuka fitur baru.
- **Sistem Toko & Upgrade**: Toko dalam game untuk membeli item peningkatan atau membuka konten eksklusif, dengan tampilan saldo koin yang persisten.
- **Manajemen Pengalaman (UX)**:
    - **Onboarding Carousel**: Panduan interaktif untuk pengguna baru.
    - **Kontrol Gameplay**: Tombol pause, dialog konfirmasi aksi (undo/confirm), dan fitur zoom aksara.
    - **Visual Feedback**: Indikator loading, toast/snackbar untuk aksi terkunci, dan UI yang responsif.
- **Leaderboard & Rapor**: Peringkat global dan statistik kemajuan pribadi pengguna.
- **Navigasi Intuitif**: Bottom navigation bar untuk berpindah antar modul (Pasar, Belajar, Toko, Rapor).

### Laporan Revisi Heuristik (15 Poin)

Aplikasi ini telah diperbarui secara menyeluruh berdasarkan evaluasi heuristik untuk meningkatkan pengalaman pengguna:

1.  **Splash Screen**: Telah ditambahkan indikator loading visual.
2.  **Login/Register (Lupa Password)**: Telah ditambahkan jalur pemulihan kata sandi.
3.  **Register (Konfirmasi Password)**: Field konfirmasi kata sandi ('Ulangi Kata Sandi') telah ditambahkan.
4.  **Pilih Peran**: Penjelasan singkat (tooltip/modal) telah ditambahkan pada peran 'Pembeli' dan 'Penjual'.
5.  **Pilih Level Belanja**: Visual gembok dan label keterangannya telah diterapkan.
6.  **Pilih Warung**: Interaksi pada warung yang terkunci telah dinonaktifkan, disertai pesan umpan balik (toast).
7.  **Gameplay Penjual (Aksara)**: Fitur tap-to-enlarge pada balon kata aksara telah ditambahkan.
8.  **Gameplay Pembeli (Undo/Konfirmasi)**: Dialog konfirmasi telah diimplementasikan sebelum aksi krusial.
9.  **Mode Belajar (Stroke Order)**: Panduan urutan penulisan aksara telah ditambahkan.
10. **Rapor / Leaderboard**: Halaman rapor telah disesuaikan agar menampilkan progres pribadi sebagai tampilan default.
11. **Toko / Reward**: Saldo koin pengguna kini ditampilkan secara persisten pada halaman Toko.
12. **Bottom Navigation**: Ikon navigasi untuk Rapor telah diperbarui menjadi ikon badge/piala.
13. **Gameplay (Pause)**: Tombol pause yang jelas kini tersedia selama gameplay.
14. **Seluruh Aplikasi (Onboarding)**: Onboarding carousel telah ditambahkan saat first-time launch.
15. **Login / Register (Mode Tamu)**: Informasi batasan fitur 'Mode Tamu' telah dijelaskan secara transparan.

### Cara Menjalankan Aplikasi

Aplikasi ini berjalan dalam lingkungan Node.js. Berikut adalah cara untuk menjalankannya di lingkungan pengembangan:

1.  **Instalasi Dependensi**: Pastikan Anda berada di direktori akar proyek, kemudian jalankan:
    ```bash
    npm install
    ```
2.  **Menjalankan Server Pengembangan**:
    ```bash
    npm run dev
    ```
    Aplikasi akan tersedia secara lokal (biasanya di `http://localhost:3000`).

3.  **Membangun untuk Produksi**:
    ```bash
    npm run build
    ```
=======
# IMK9APASARHANACARAKA
>>>>>>> 600eec0cbc3f2c3b986a07053114c3691e33fc3b

## Tim B (Chrono Thread - Game Based Learning)

### Anggota Tim
| Nama           | NRP        | Kelas     |
| ---            | ---        | ----------|
| Willy Marcelius | 5025241096 | Interaksi Manusia dan Komputer (A)       |
| Rendy Tanuwijaya | 5025241099           | Interaksi Manusia dan Komputer (A)       |

### Link Deploy Aplikasi
```
https://chrono-thread-1011441607029.asia-southeast1.run.app/
```

### Link Demo Prototype dan Dev
```
https://youtu.be/EvcBUxP9rHg
```

### Link Prototype Figma 
```
https://www.figma.com/design/KiAzxVFFFoaWLsfQEMcYFA/Untitled?node-id=0-1&t=2xsiM1T9MGmS9dQl-1
```

### Deskripsi Project

Chrono-Thread adalah aplikasi game berbasis cognitive training yang dirancang sebagai media latihan kognitif interaktif untuk generasi muda. Melalui dua mode permainan — Visual Puzzle dan Logika & Urutan — pengguna dapat melatih fokus visual dan memori prosedural secara menyenangkan, kapan saja dan di mana saja.

Chrono-Thread merupakan bagian dari tugas akhir mata kuliah Interaksi Manusia dan Komputer (IMK) yang dikerjakan oleh Kelompok 9 Tim B. Aplikasi ini dikembangkan menggunakan pendekatan User-Centered Design (UCD), mulai dari riset pengguna, pembuatan persona, perancangan wireframe, hingga evaluasi heuristik dan iterasi prototipe high-fidelity.

### Tujuan Aplikasi
- Menyediakan media latihan kognitif yang dapat dimainkan di sela-sela aktivitas padat
- Melatih fokus visual dan memori prosedural melalui pendekatan game
- Membangun kebiasaan latihan otak yang konsisten melalui sistem gamifikasi

### Laporan Revisi Heuristik
Aplikasi ini telah diperbarui berdasarkan evaluasi heuristik oleh Kelompok 8 menggunakan Nielsen's 10 Usability Heuristics:

1. Splash Screen — Ditambahkan progress bar dengan persentase numerik  
2. Login (Mode Tamu) — Ditambahkan tombol "Coba Tanpa Akun" beserta keterangan batasannya  
3. Sign Up (Validasi Real-Time) — Ditambahkan inline validation pada setiap field (format email, kekuatan password, kecocokan konfirmasi)  
4. Home Dashboard — Bagian "Aktivitas Terakhir" dibuat collapsible untuk mengurangi kepadatan informasi  
5. Pilih Game (Label) — Kode internal FR-01/FR-02 dihapus dari tampilan, diganti label kognitif: "Fokus Visual" dan "Memori Prosedural"  
6. Pilih Game (Kesulitan) — Ditambahkan deskripsi singkat tiap level kesulitan (jumlah soal, waktu, kompleksitas)  
7. Gameplay (Indikator Nyawa) — Ditambahkan indikator ♥♥♥ agar pengguna memahami konsekuensi jawaban salah  
8. Gameplay (Pause) — Ditambahkan Pause Menu dengan opsi Lanjut, Ulangi, dan Keluar ke Home  
9. Feedback Jawaban Salah — Diperluas dengan penjelasan alasan salah dan highlight jawaban benar  
10. Logika & Urutan (Affordance) — Ditambahkan ikon grip ⠿ dan tombol ▲▼ sebagai alternatif drag-and-drop, touch target diperbesar ke 44dp  
11. Hasil / Skor — Ditambahkan tombol "Lihat Review Jawaban"  
12. Review Jawaban — Ditambahkan screen baru dengan detail tiap soal dan penjelasan jawaban salah  
13. Progress Tracking — Ditambahkan filter rentang waktu: 7 Hari / 30 Hari / Semua  
14. Profil — Ditambahkan Edit Profil, akses ulang Tutorial & Onboarding, dan opsi Hapus Akun  
15. Bottom Navigation — Label "MAIN" diganti menjadi "GAME" agar lebih deskriptif  

### Alur Aplikasi (User Journey)

1. Splash Screen — Animasi pembuka dengan progress bar dan persentase loading
2. Onboarding — 3 slide interaktif saat first launch: pengenalan app, sistem XP & streak, dan dua mode game
3. Autentikasi — Pengguna dapat:
    - **Mendaftar / Masuk dengan Email** → progres tersimpan permanen
   - **Mode Tamu** → bermain langsung tanpa akun (progres tidak tersimpan)
   - **Lupa Password** → jalur pemulihan akun
4. Home Dashboard — Menampilkan level & XP, streak harian, dan tantangan hari ini sebagai quick access
5. Pilih Game & Kesulitan — Memilih mode permainan (Visual Puzzle / Logika & Urutan) beserta level kesulitan (Mudah / Sedang / Sulit) yang dilengkapi deskripsi jumlah soal dan waktu
6. Gameplay — Bermain dengan indikator timer, skor, progress soal, dan nyawa (♥♥♥). Pause tersedia kapan saja
7. Feedback Real-Time — Setiap jawaban langsung diberi respons: penjelasan mengapa salah dan highlight jawaban benar
8. Hasil & Review — Menampilkan skor akhir, XP didapat, notifikasi naik level, dan opsi melihat review tiap soal
9. Progress & Profil — Memantau grafik skor, badge pencapaian, riwayat sesi, serta mengatur akun dan preferensi

### Fitur Utama

#### Mode Permainan
- Visual Puzzle — Melatih fokus dan pengenalan pola visual
- Logika & Urutan — Melatih memori prosedural dan pemikiran algoritmik

#### Sistem Gamifikasi
- XP & Level — Kumpulkan poin pengalaman dan naik level setiap sesi
- Streak Harian — Bonus XP untuk pengguna yang bermain setiap hari
- Badge Pencapaian — Koleksi lencana sebagai bukti perkembangan kognitif

#### Progress & Feedback
- Progress Tracker — Grafik skor mingguan dengan filter 7 hari / 30 hari / semua
- Feedback Real-Time — Penjelasan langsung mengapa jawaban salah + highlight jawaban benar
- Review Jawaban — Analisis detail tiap soal setelah sesi selesai

#### Kenyamanan Pengguna
- Dark Mode sebagai tema default (ramah mata untuk penggunaan malam)
- Onboarding 3 Slide untuk pengguna baru
- Pause Menu dengan opsi Lanjut, Ulangi, dan Keluar
- Mode masuk tanpa akun untuk mencoba tanpa perlu membuat akun

### Instalasi dan Pengaturan Lokal

Pastikan Anda telah menginstal **Node.js (v18 atau versi lebih tinggi)** di perangkat Anda.

#### 1. Klon & Ekstrak
Ekstrak atau arahkan terminal ke direktori proyek Anda:
```bash
cd chrono-thread
```

#### 2. Instal Dependensi
Instal seluruh paket konfigurasi dependensi yang diperlukan:
```bash
npm install
```

#### 3. Jalankan Server Pengembangan (Dev Server)
Jalankan server pengembangan lokal pada alamat `http://localhost:3000`:
```bash
npm run dev
```

#### 4. Kompilasi Produksi Langsung
Kompilasi aset aplikasi web menjadi modul statis teroptimasi yang siap dideploy pada direktori `/dist`:
```bash
npm run build
```
