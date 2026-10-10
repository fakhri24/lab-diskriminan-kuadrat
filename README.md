# 📐 Lab Visual Interaktif: Diskriminan & Jenis Akar Persamaan Kuadrat

Media Pembelajaran Interaktif Matematika **SMA Fase E (Kelas X) • Kurikulum Merdeka** berbasis *Single-File Application* (HTML5, Tailwind CSS, KaTeX, HTML5 Canvas 2D, dan Web Speech API).

🌐 **Live Demo (GitHub Pages):** [https://fakhri24.github.io/lab-diskriminan-kuadrat/](https://fakhri24.github.io/lab-diskriminan-kuadrat/)  
*(Tautan alternatif/alias: https://github.com/fakhri24/lab-diskriminan-kuadrat)*

---

## 🎯 Capaian Pembelajaran & Tujuan (Fase E)

1. **Menganalisis Peran Koefisien**: Menyelidiki pengaruh koefisien $a$, $b$, dan konstanta $c$ terhadap bentuk kurva parabola $f(x) = ax^2 + bx + c$.
2. **Kalkulasi & Sifat Diskriminan**: Memahami asal-usul dan signifikansi nilai diskriminan $D = b^2 - 4ac$ dari rumus kuadrat (Rumus ABC) $x = \frac{-b \pm \sqrt{D}}{2a}$.
3. **Klasifikasi 3 Jenis Akar**:
   - 🟢 **$D > 0$**: Memiliki dua akar real berbeda ($x_1 \neq x_2$), kurva memotong sumbu-X di 2 titik.
   - 🟡 **$D = 0$**: Memiliki satu akar real kembar ($x_1 = x_2$), kurva menyinggung sumbu-X di 1 titik (titik puncak).
   - 🔴 **$D < 0$**: Tidak memiliki akar real (akar imajiner/kompleks), kurva melayang di atas atau di bawah sumbu-X (Definit Positif / Negatif).
4. **Teorema Vieta & Titik Karakteristik**: Menemukan hubungan jumlah akar ($x_1 + x_2 = -\frac{b}{a}$), hasil kali akar ($x_1 \cdot x_2 = \frac{c}{a}$), koordinat titik puncak $\left(-\frac{b}{2a}, -\frac{D}{4a}\right)$, serta persamaan sumbu simetri $x = -\frac{b}{2a}$.

---

## ✨ Fitur-Fitur Utama

### 1. 🎛️ Panel Kontrol Koefisien Presisi & Sinkronisasi 2-Arah
- **Slider Parameter $a$**: Rentang $-5$ s.d. $5$ (step $0.5$). Otomatis melewati nilai $0$ agar selalu memenuhi syarat fungsi kuadrat ($a \neq 0$).
- **Slider Parameter $b$ & $c$**: Rentang $-10$ s.d. $10$ (step $1$).
- **Input Angka Numerik Langsung**: Tersinkronisasi secara real-time dengan tombol stepper $(+)$ dan $(-)$.
- **Tombol Preset Cepat (Quick Presets)**:
  - $D > 0$ (Dua Akar Real)
  - $D = 0$ (Akar Kembar)
  - $D < 0$ (Akar Imajiner)
  - Akar Simetris ($b = 0$)
  - Parabola Terbuka ke Bawah ($a < 0$)
  - Definit Positif ($a > 0, D < 0$)

### 2. 📝 Display Matematis & Teorema Vieta Dinamis (KaTeX)
- Formula bentuk umum $ax^2 + bx + c = 0$ ter-render rapi dan adaptif tanda aljabarnya.
- Penjabaran langkah per langkah substitusi numerik rumus diskriminan $D = b^2 - 4ac$.
- Status Badge responsif penentu jenis akar.
- Penampilan akar $x_1$ dan $x_2$ dalam format desimal maupun bentuk pecahan / radikal eksak matematika.
- Kalkulasi dan pembuktian langsung Teorema Vieta (Jumlah dan Hasil Kali Akar).

### 3. 📈 Visualisasi Grafik Parabola Interaktif (HTML5 Canvas 2D)
- Koordinat kartesius responsif dengan sumbu X & Y, grid garis adaptif, dan angka skala dinamis.
- Kurva parabola dirender halus dengan efek visual glowing gradient.
- Penandaan titik krusial berwarna kontras:
  - 🟢 **Titik Potong Sumbu-X**: $(x_1, 0)$ dan $(x_2, 0)$
  - 🟣 **Titik Potong Sumbu-Y**: $(0, c)$
  - 🟡 **Titik Puncak**: $(x_p, y_p) = \left(-\frac{b}{2a}, -\frac{D}{4a}\right)$ dengan keterangan minimum/maksimum
  - 🔵 **Garis Sumbu Simetri**: Garis putus-putus $x = -\frac{b}{2a}$
- Tool inspeksi kursor mouse: Pelacak titik dinamis $(x, f(x))$ pada kurva dengan floating tooltip.
- Fitur Zoom In, Zoom Out, Auto-Fit, dan Ekspor Gambar PNG beresolusi tinggi.

### 4. 🔊 Aksesibilitas Suara AI (Web Speech API)
- Tombol **"Dengarkan Penjelasan AI"**: Narasi audio otomatis dalam Bahasa Indonesia menggunakan `window.speechSynthesis` bawaan peramban.
- Menjelaskan makna koefisien, arah kurva, perhitungan diskriminan, jenis akar, dan interpretasi geometrisnya secara bertutur ramah siswa.
- Dilengkapi transkrip teks langsung untuk kemudahan membaca bagi siswa.

### 5. 🎮 Matriks Geometris 6 Kondisi & Misi Tantangan Siswa
- Matriks interaktif 6 sel ($a > 0$ vs $a < 0$ dan $D > 0, D = 0, D < 0$) dengan highlight aktif real-time.
- Misi eksplorasi mandiri peserta didik dengan validasi kondisi interaktif.

---

## 🚀 Cara Menjalankan

Aplikasi ini bersifat **Single-File Zero Build Application**:
1. Cukup unduh atau clone repositori ini:
   ```bash
   git clone https://github.com/fakhri24/lab-diskriminan-kuadrat.git
   ```
2. Buka berkas `index.html` langsung di peramban web modern apa pun (Google Chrome, Edge, Safari, Firefox) via double-click (`file://`).
3. Tidak memerlukan Node.js, npm build step, maupun server backend.

---

## 🛠️ Tumpukan Teknologi
- **HTML5 & CSS3**
- **Tailwind CSS v3** (via CDN)
- **KaTeX v0.16.11** (via CDN)
- **HTML5 Canvas 2D API** (Native JavaScript)
- **Web Speech API** (SpeechSynthesis)

---

## 📄 Lisensi
MIT License © 2026 Fakhri Fadllillah • Media Pembelajaran Matematika SMA Fase E.
