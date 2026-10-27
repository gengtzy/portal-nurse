# Portal Layanan Keperawatan · RSUD Welas Asih

Portal web statis berbasis HTML5 & Vanilla CSS murni sebagai gerbang utama (*hub*) layanan digital keperawatan RSUD Welas Asih Provinsi Jawa Barat, khususnya Ruang Rawat Inap Umar Bin Khattab 2.

---

## 🎯 Navigasi Kartu Aplikasi

1. **Card 1: Aplikasi Nurse Recharge**
   - **Tujuan**: `https://nurse-questionnaire-ecru.vercel.app/`
   - **Deskripsi**: Platform pendampingan psikologis, evaluasi burnout MBI terstandarisasi (Pre & Post test), intervensi relaksasi *Butterfly Hug* 🦋, mini game katarsis "Hancurkan Stres", kartu apresiasi rekan (*Thank You Card*), dan panel analitik Kepala Ruangan.

2. **Card 2: Supervisi Keperawatan Ruang UBK 2**
   - **Tujuan**: `https://supervisi-keperawatan-ruang-ubk-2-1.ai.studio/`
   - **Target**: `_blank` (Tab baru)
   - **Deskripsi**: Penjaminan mutu asuhan keperawatan, keselamatan pasien (IPSG), kepatuhan SPO klinis, bimbingan reflektif dengan *Voice Note*, dan pengesahan Berita Acara Tanda Tangan Digital resmi.

---

## 📁 Struktur Direktori

```text
portal/
├── index.html              # Halaman web statis utama
├── css/
│   └── style.css           # Modern Vanilla CSS design system
├── images/
│   └── logo_welas_asih.png # Logo institusi RSUD Welas Asih
├── vercel.json             # Konfigurasi Vercel (cleanUrls & security headers)
└── README.md               # Dokumentasi dan panduan deployment
```

---

## 🚀 Panduan Deploy ke Vercel (Sangat Mudah & Cepat)

Karena portal ini murni **HTML & CSS statis tanpa build step (Zero-Config Static)**, proses deploy ke Vercel hanya memakan waktu beberapa detik:

### Langkah 1: Push ke GitHub Repository
Di terminal folder `c:\Client_Project\nurse_kuisionere\portal`:
```bash
git add .
git commit -m "feat: initial static portal for nursing services"
git push origin main
```

### Langkah 2: Deploy di Vercel Dashboard
1. Buka [vercel.com/dashboard](https://vercel.com/dashboard) dan login.
2. Klik tombol **"Add New..."** &rarr; pilih **"Project"**.
3. Pada daftar Git Repository, cari dan klik **"Import"** pada repo **`gengtzy/portal-nurse`**.
4. Di halaman konfigurasi project:
   - **Framework Preset**: Biarkan otomatis terdeteksi **"Other"** (Static HTML).
   - **Root Directory**: `./` (Default).
   - **Build Command**: Kosongkan (tidak perlu build script apa pun).
   - **Output Directory**: Kosongkan (langsung melayani file root).
5. Klik **"Deploy"**.
6. Selesai! Dalam waktu ~10-15 detik, website portal Anda sudah aktif dengan URL publik Vercel (misal: `https://portal-nurse-xxx.vercel.app`).

### Alternatif: Deploy via Vercel CLI
Jika memiliki Vercel CLI di komputer Anda:
```bash
# Jalankan di folder portal
vercel

# Untuk deploy langsung ke production domain
vercel --prod
```
