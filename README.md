🎵 PMD Musik 12 TET

Pedang Mata Dua Musik Digital — Eksplorasi Mikrotonal 20 Nada per Oktaf

https://img.shields.io/badge/Deployed-GitHub%20Pages-blue
https://img.shields.io/badge/APINDO-Innovation%20Challenge%202026-orange
https://img.shields.io/badge/License-MIT-green
https://img.shields.io/badge/Made%20with-JavaScript-yellow

---
🌐 Online (GitHub Pages)
Akses aplikasi di: https://srpakpahansst.github.io/pmd-musik-12tet/
---

📖 Daftar Isi

· Tentang Aplikasi
· Sistem 12-TET 20 Nada per Oktaf
· Fitur Utama
· Teknologi yang Digunakan
· Cara Menggunakan
· Struktur Proyek
· Integrasi dengan Karya Ilmiah
· Partisipasi dalam Lomba
· Kontributor
· Lisensi

---

🎯 Tentang Aplikasi

PMD Musik 12 TET adalah aplikasi web interaktif untuk eksplorasi sistem musik 12-Tone Equal Temperament (12-TET) dengan 20 nada per oktaf — sebuah terobosan inovatif dalam dunia musik mikrotonal.

Aplikasi ini dikembangkan berdasarkan karya tulis ilmiah berjudul "Eksplorasi Musik Sistem 12 TET (20 Nada per Oktaf): Inovasi dan Peluang dalam Seni Musik Modern" dan dipersembahkan untuk APINDO Innovation Challenge 2026 dengan tema "Teman Cerdas, Solusi Tuntas".

🎯 Tujuan

Tujuan Deskripsi
Inovasi Memperkenalkan sistem musik baru dengan 20 nada per oktaf sebagai alternatif dari sistem konvensional 8-TET 12 nada.
Eksplorasi Menyediakan alat eksplorasi musik mikrotonal bagi musisi, komposer, dan peneliti.
AI Integration Memanfaatkan kecerdasan buatan untuk komposisi dan transkripsi musik.
Budaya Menjembatani musik tradisional Indonesia dengan teknologi modern untuk pelestarian budaya.

---

🎵 Sistem 12-TET 20 Nada per Oktaf

Rumus Frekuensi

f_n = f_0 \times 3^{(n/20)}

Variabel Keterangan
f_n Frekuensi nada yang dihitung
f_0 Frekuensi nada referensi (A4 = 440 Hz)
n Jumlah langkah "setengah langkah" (semitone) dari nada referensi

Rasio Oktaf

f_{\text{oktaf berikutnya}} = f_{\text{oktaf sebelumnya}} \times 3

Notasi Nada (20 Nada per Oktaf)

Indeks Nada Indeks Nada
0 E 10 J#
1 E# 11 K
2 F 12 K#
3 F# 13 A
4 G 14 A#
5 G# 15 B
6 H 16 B#
7 H# 17 C
8 I 18 C#
9 J 19 D

Skala

Skala Urutan Nada Interval
Mayor (E=1) E - F - G - H - I - J - K - A - B - C - D - E 1 1 1 1 ½ 1 1 1 1 1 ½
Minor (A=1) A - B - C - D - E - F - G - H - I - J - K - A 1 1 1 ½ 1 1 1 1 ½ 1 1

---

✨ Fitur Utama

1. 🎹 Keyboard Interaktif

Fitur Deskripsi
20 Nada per Oktaf Sistem notasi unik: E, E#, F, F#, G, G#, H, H#, I, J, J#, K, K#, A, A#, B, B#, C, C#, D
3-5 Oktaf Pilihan oktaf (3, 4, atau 5) untuk fleksibilitas
8 Instrumen Sine, Square, Sawtooth, Triangle, Organ, Piano, Flute, Trumpet
Mode Nada Tunggal Mainkan satu nada, rekam melodi otomatis
Mode Akord Mainkan triad (Mayor/Minor) dengan sustain piano
Efek Suara Reverb, Delay, Amplifier (0.5x - 3.0x)

2. 🎵 AI Composer

Fitur Deskripsi
Mode Deskripsi Tulis deskripsi melodi, sistem menghasilkan melodi otomatis
Mode Prompt AI Gunakan OpenAI API (GPT-3.5) untuk komposisi berbasis prompt
6 Mood Happy, Sad, Romantic, Mysterious, Energetic, Calm
2 Skala Mayor (E) dan Minor (A)
Tempo 60 - 160 BPM
Play & Stop Putar hasil melodi dengan instrumen pilihan

3. 🎤 AI Transcriber

Fitur Deskripsi
Rekam Mikrofon Rekam suara atau instrumen (maks. 22 menit)
Deteksi Pitch Real-time Algoritma Autokorelasi dan YIN
Mapping 20-TET Transkripsi otomatis ke notasi 20 nada per oktaf
Visualisasi Waveform Tampilan gelombang suara real-time
Play Hasil Putar ulang nada yang terdeteksi
Kirim ke Chord Progression Transfer hasil ke fitur analisis akord

4. 🎶 Chord Progression Generator

Fitur Deskripsi
Analisis Otomatis Deteksi nada dasar dan skala dari urutan nada
Progresi Akord Hasilkan akord dengan notasi Romawi (I, ii, iii, IV, V, vi, vii°)
Mode Analisis Otomatis, Mayor, atau Minor
Jumlah Akord 4, 6, atau 8 akord

5. 📖 Tutorial Interaktif

· Panduan langkah demi langkah untuk semua fitur.
· Dapat dibuka kapan saja dengan tombol "Tutorial".
· Penjelasan teori di balik sistem 20 nada per oktaf.

6. 📚 Informasi & Referensi

Tab Konten
Teori Dasar teoritis sistem 12-TET 20 nada per oktaf
Frekuensi Tabel frekuensi (5 desimal) di oktaf 4
Skala Skala Mayor (E) dan Minor (A) dengan interval
Akord Referensi pembentukan akord triad
Simulasi Lagu Simulasi lagu KJ 33 yang dikonversi ke sistem 12-TET
Tentang Informasi aplikasi dan penulis

---

🛠️ Teknologi yang Digunakan

Kategori Teknologi
Frontend HTML5, CSS3, JavaScript (ES6+)
Audio Engine Web Audio API (OscillatorNode, AnalyserNode, ConvolverNode, DynamicsCompressorNode)
AI Integration OpenAI API (GPT-3.5), Autokorelasi, YIN Algorithm
Media MediaDevices API (mikrofon)
Visualization HTML5 Canvas (waveform, keyboard)
Hosting GitHub Pages
Version Control Git, GitHub
Documentation Markdown, GitHub README

---

🚀 Cara Menggunakan

🌐 Online (GitHub Pages)

Akses aplikasi di: https://srpakpahansst.github.io/pmd-musik-12tet/

💻 Lokal

1. Clone repository:
   ```bash
   git clone https://github.com/SRPakpahanSST/pmd-musik-12tet.git
   cd pmd-musik-12tet
   ```
2. Buka file index.html di browser favorit Anda (Chrome/Edge/Firefox).
3. Izinkan akses mikrofon jika menggunakan fitur AI Transcriber.

📋 Persyaratan

Persyaratan Keterangan
Browser Chrome 90+, Edge 90+, Firefox 88+ (dukungan Web Audio API)
Internet Untuk mengakses OpenAI API (mode Prompt AI)
Mikrofon Untuk fitur AI Transcriber
HTTPS Diperlukan untuk akses mikrofon (tersedia di GitHub Pages)

---

📁 Struktur Proyek

```
pmd-musik-12tet/
├── index.html                      # Aplikasi utama
├── README.md                       # Dokumentasi proyek
├── Karya_Tulis_12TET_20Nada.md     # Karya tulis ilmiah
├── PMD_Musik_12TET_Demo.srt        # File subtitle untuk video demo
├── splash.png                      # Gambar splash screen
└── .git/                           # Version control
```

---

📄 Integrasi dengan Karya Ilmiah

Aplikasi ini terintegrasi dengan karya tulis ilmiah:

Link Keterangan
Karya Tulis Ilmiah (GitHub) Naskah lengkap sistem 12-TET 20 nada per oktaf
Simulasi Lagu KJ 33 (Blog) Simulasi lagu dengan audio generator

---

🏆 Partisipasi dalam Lomba

Aplikasi ini dipersembahkan untuk APINDO Innovation Challenge 2026 dengan tema:

"Teman Cerdas, Solusi Tuntas"

Informasi Detail
Link Pendaftaran bit.ly/RegAIChallenge2026
Terms of Reference bit.ly/AIChallenge-TOR3
Tenggat Pengumpulan 17 Mei 2026
Kategori Peserta Pekerja Profesional
Institusi PMD Pakpahan Ministry

---

👨‍💻 Kontributor

Nama Peran
Sukma Riadi Pakpahan, SST Konsep, penelitian, dan pengembangan aplikasi

---

📄 Lisensi

Aplikasi ini dilisensikan di bawah MIT License — silakan digunakan, dimodifikasi, dan didistribusikan.

---

📞 Kontak

Platform Link
GitHub SRPakpahanSST
Blog musikbarupmd.blogspot.com
Aplikasi srpakpahansst.github.io/pmd-musik-12tet

---

🙏 Ucapan Terima Kasih

· Badan Riset dan Inovasi Nasional (BRIN) — Dukungan riset dan inovasi.
· APINDO — Penyelenggara Innovation Challenge 2026.
· Microsoft — Dukungan dalam Masterclass AI.
· Komunitas Musik Mikrotonal — Inspirasi dan dukungan.
· OpenAI — Teknologi AI untuk komposisi musik.
· GitHub — Platform hosting dan version control.

---

🎵 Selamat Berkarya dengan PMD Musik 12 TET!

---

Dibuat dengan ❤️ oleh Sukma Riadi Pakpahan, SST