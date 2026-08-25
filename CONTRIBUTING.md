🤝 Panduan Kontribusi — PMD Musik 12 TET

Terima kasih atas minat Anda untuk berkontribusi pada PMD Musik 12 TET! Aplikasi ini adalah proyek open-source untuk eksplorasi sistem musik mikrotonal 12-TET 20 nada per oktaf, dan setiap kontribusi sangat dihargai.

Sebelum memulai, mohon baca panduan ini dengan saksama untuk memastikan kontribusi Anda dapat diproses dengan lancar.

---

📋 Daftar Isi

· Cara Melaporkan Masalah (Issue)
· Cara Mengajukan Permintaan Fitur
· Panduan Pull Request
· Standar Koding
· Cara Menjalankan Proyek Secara Lokal
· Struktur Proyek
· Pedoman Pengujian
· Etika Kontribusi
· Lisensi

---

🐛 Cara Melaporkan Masalah (Issue)

Jika Anda menemukan bug atau masalah dalam aplikasi, silakan buat Issue di GitHub dengan mengikuti template berikut:

Format Laporan Bug

```markdown
**Judul:** [Deskripsi singkat masalah]

**Deskripsi:**
- Jelaskan masalah secara detail.
- Sebutkan langkah-langkah untuk mereproduksi bug.

**Lingkungan:**
- Browser: [misal: Chrome 120, Firefox 115]
- Sistem Operasi: [misal: Windows 11, macOS Sonoma]
- Versi Aplikasi: [commit hash atau tag]

**Perilaku yang Diharapkan:**
- Jelaskan apa yang seharusnya terjadi.

**Perilaku Aktual:**
- Jelaskan apa yang sebenarnya terjadi.

**Lampiran:**
- Screenshot atau video (jika ada).
- Error log dari Console browser (F12).
```

Contoh Issue yang Baik

```markdown
**Judul:** Tombol "Play Hasil" di AI Transcriber tidak mengeluarkan suara

**Deskripsi:**
Setelah merekam suara dan mendapatkan hasil transkripsi, ketika tombol "Play Hasil" diklik, tidak ada suara yang keluar. Tidak ada error di console.

**Langkah Reproduksi:**
1. Buka tab AI Transcriber.
2. Klik tombol mikrofon dan rekam suara "do-re-mi".
3. Hentikan rekaman.
4. Klik tombol "Play Hasil".

**Lingkungan:**
- Browser: Chrome 120
- OS: Windows 11
- Commit: f02799f

**Perilaku yang Diharapkan:**
Suara nada hasil transkripsi terdengar.

**Perilaku Aktual:**
Tidak ada suara sama sekali.
```

---

💡 Cara Mengajukan Permintaan Fitur

Jika Anda memiliki ide untuk fitur baru, silakan buat Issue dengan label enhancement.

Format Permintaan Fitur

```markdown
**Judul:** [Nama fitur yang diusulkan]

**Deskripsi:**
- Jelaskan fitur yang Anda usulkan secara detail.
- Mengapa fitur ini penting untuk aplikasi?

**Manfaat:**
- Siapa yang akan diuntungkan oleh fitur ini?
- Bagaimana fitur ini meningkatkan pengalaman pengguna?

**Alternatif:**
- Apakah ada cara lain untuk mencapai tujuan yang sama?

**Contoh Penggunaan:**
- Berikan skenario penggunaan fitur ini.
```

---

🔧 Panduan Pull Request

1. Fork Repository

1. Buka repository: https://github.com/SRPakpahanSST/pmd-musik-12tet
2. Klik tombol Fork di pojok kanan atas.
3. Clone fork Anda ke lokal:
   ```bash
   git clone https://github.com/[username-anda]/pmd-musik-12tet.git
   cd pmd-musik-12tet
   ```

2. Buat Branch Baru

```bash
# Untuk fitur baru
git checkout -b feat/nama-fitur

# Untuk perbaikan bug
git checkout -b fix/nama-bug

# Untuk dokumentasi
git checkout -b docs/nama-perubahan
```

3. Lakukan Perubahan

· Ikuti Standar Koding di bawah.
· Pastikan perubahan Anda tidak merusak fungsionalitas yang ada.
· Jika menambahkan fitur baru, perbarui dokumentasi yang relevan.

4. Commit dan Push

```bash
git add .
git commit -m "feat: tambahkan fitur [deskripsi singkat]"
git push origin feat/nama-fitur
```

Format Pesan Commit:

Prefix Keterangan
feat: Fitur baru
fix: Perbaikan bug
docs: Perubahan dokumentasi
style: Perubahan style (CSS, formatting)
refactor: Refaktor kode tanpa perubahan fungsional
test: Penambahan atau perbaikan test
chore: Tugas maintenance (build, dependencies)

Contoh:

```bash
git commit -m "feat: tambahkan dukungan untuk instrumen saxophone"
git commit -m "fix: perbaiki volume play hasil di AI Transcriber"
git commit -m "docs: perbarui README dengan instruksi instalasi"
```

5. Buat Pull Request

1. Buka repository fork Anda di GitHub.
2. Klik tombol Compare & pull request.
3. Isi judul dan deskripsi PR dengan jelas.
4. Hubungkan PR dengan Issue terkait (jika ada): Closes #123.
5. Klik Create pull request.

6. Review dan Merge

· Tim akan meninjau PR Anda dalam 1-3 hari kerja.
· Jika ada perubahan yang diminta, lakukan dan push ulang ke branch yang sama.
· Setelah disetujui, PR akan di-merge ke branch main.

---

📝 Standar Koding

JavaScript (ES6+)

Aspek Standar
Indentasi 4 spasi (bukan tab)
String Gunakan single quotes '...' kecuali untuk template literal
Semicolon Wajib di akhir setiap statement
Nama Variabel camelCase: myVariable
Nama Fungsi camelCase: function myFunction()
Nama Kelas PascalCase: class MyClass
Konstanta UPPER_SNAKE_CASE: const MAX_NOTES = 20
Async/Await Gunakan async/await daripada .then()
Console Hapus console.log sebelum commit (kecuali untuk debugging sementara)

Contoh:

```javascript
// ✅ Baik
function playSingleNote(frequency, duration) {
    const ctx = initAudio();
    const oscillator = ctx.createOscillator();
    oscillator.frequency.setValueAtTime(frequency, ctx.currentTime);
    return oscillator;
}

// ❌ Buruk
function playSingleNote(frequency, duration){
  const ctx=initAudio()
  var osc=ctx.createOscillator()
  osc.frequency.setValueAtTime(frequency,ctx.currentTime)
  return osc
}
```

HTML

Aspek Standar
Indentasi 2 spasi
Attribute Gunakan double quotes "..."
ID & Class kebab-case: my-element, btn-primary
Semantic Elements Gunakan <header>, <nav>, <main>, <section>, <footer>

Contoh:

```html
<!-- ✅ Baik -->
<div class="keyboard-wrapper">
    <button class="btn btn-primary" id="playBtn">▶ Play</button>
</div>

<!-- ❌ Buruk -->
<div class="keyboard_wrapper">
    <Button class='btn btn-primary' id=playBtn>Play</Button>
</div>
```

CSS

Aspek Standar
Indentasi 4 spasi
Selector Gunakan class selector (bukan ID) untuk styling
Unit Gunakan rem untuk font-size, px untuk border/outline
Warna Gunakan variabel CSS untuk warna utama

Contoh:

```css
/* ✅ Baik */
.keyboard-wrapper {
    background: var(--bg-dark);
    padding: 1rem;
    border-radius: 12px;
}

/* ❌ Buruk */
#keyboardWrapper{
background:#1a1a2e;
padding:10px;
border-radius:12px;
}
```

---

🚀 Cara Menjalankan Proyek Secara Lokal

Persyaratan

Perangkat Lunak Versi
Browser Chrome 90+, Edge 90+, Firefox 88+
Git 2.30+
Editor VS Code (rekomendasi)

Langkah-langkah

1. Clone repository:
   ```bash
   git clone https://github.com/SRPakpahanSST/pmd-musik-12tet.git
   cd pmd-musik-12tet
   ```
2. Buka dengan browser:
   ```bash
   # Cara termudah: double-click index.html
   # Atau gunakan Live Server di VS Code
   ```
3. Untuk pengembangan:
   · Buka index.html di browser.
   · Buka Developer Tools (F12) untuk debugging.
   · Perubahan pada file akan terlihat setelah refresh browser.
4. Testing fitur mikrofon:
   · Gunakan HTTPS atau localhost (browser memerlukan secure context).
   · GitHub Pages sudah menyediakan HTTPS secara otomatis.

---

📁 Struktur Proyek

```
pmd-musik-12tet/
├── index.html                      # Aplikasi utama (HTML + CSS + JavaScript inline)
├── README.md                       # Dokumentasi proyek
├── CONTRIBUTING.md                 # Panduan kontribusi (file ini)
├── Karya_Tulis_12TET_20Nada.md     # Karya tulis ilmiah
├── PMD_Musik_12TET_Demo.srt        # File subtitle untuk video demo
├── splash.png                      # Gambar splash screen
└── .git/                           # Version control (jangan diubah)
```

Catatan: Aplikasi ini menggunakan single-file architecture (index.html berisi semua kode). Jika kontribusi Anda besar, pertimbangkan untuk memisahkan CSS dan JavaScript ke file terpisah.

---

🧪 Pedoman Pengujian

Sebelum Mengirim Pull Request

1. Uji di Chrome dan Firefox (minimal).
2. Uji di HP (resolusi layar kecil).
3. Uji fitur audio (pastikan suara keluar).
4. Uji AI Transcriber (pastikan deteksi pitch berfungsi).
5. Uji mode Akord (pastikan sustain dan pergantian akord berjalan).
6. Cek Console (pastikan tidak ada error JavaScript).
7. Cek Responsif (pastikan UI tidak pecah di layar kecil).

Fitur yang Harus Diuji

Fitur Yang Diuji
Splash Screen Tombol "Mulai" berfungsi
Keyboard Semua tuts mengeluarkan suara, rekam melodi
Instrumen Semua 8 instrumen berbunyi
Efek Reverb, Delay, Amplifier
AI Composer Generate dan Play
AI Transcriber Rekam, transkripsi, Play Hasil
Chord Progression Generate dari hasil transkripsi
Info Panel Semua tab menampilkan konten
Tutorial Navigasi slide berfungsi

---

🤝 Etika Kontribusi

Hal Keterangan
Bersikap sopan Hormati pendapat dan kontribusi orang lain.
Jangan spam Hindari PR atau Issue yang tidak relevan.
Hargai waktu Review PR bisa memakan waktu 1-3 hari.
Berikan konteks Jelaskan dengan jelas apa yang Anda ubah dan mengapa.
Test dulu Pastikan perubahan Anda tidak merusak fitur lain.

---

📄 Lisensi

Dengan berkontribusi ke proyek ini, Anda setuju bahwa kontribusi Anda akan dilisensikan di bawah MIT License yang sama dengan proyek ini.

---

📞 Kontak

Jika Anda memiliki pertanyaan lebih lanjut, silakan hubungi:

Platform Link
GitHub Issues Buat Issue
Email [sukma.riadi.pakpahan@gmail.com]
Blog musikbarupmd.blogspot.com

---

Terima kasih atas kontribusi Anda untuk memajukan musik mikrotonal! 🎵