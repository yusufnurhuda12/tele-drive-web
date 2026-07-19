# Telegram Drive - Site Document Manager

Aplikasi web modern (Sistem Informasi Manajemen Dokumen) untuk mengunggah dokumen *site* secara aman ke Telegram Cloud. Dibangun dengan Next.js dan didesain khusus untuk memudahkan pencarian file langsung dari Telegram maupun dari Web Dashboard.

## 🚀 Fitur Utama
- **Modern UI/UX**: Antarmuka estetis dengan desain *Glassmorphism* dan *Dark Mode*.
- **Live Spreadsheet Validation**: Mengecek dan memvalidasi `Site ID` secara *real-time* langsung dari Google Sheets.
- **Checklist Terintegrasi**: Fitur *remarks* cepat untuk menandai kekurangan (ATP, NMS, RET, SALES PART).
- **Auto-Caption Telegram**: Pengiriman dokumen ke Telegram lengkap dengan format `#SiteID` yang membuat dokumen sangat mudah dicari (searchable) di aplikasi Telegram.
- **Sistem Login**: Terintegrasi dengan NextAuth.js untuk otorisasi akses Admin.

## 💻 Tech Stack
- **Framework**: Next.js 14 (App Router)
- **Frontend**: React 18, Lucide React (Icons), Vanilla CSS
- **Backend**: Next.js API Routes, Node.js Buffer
- **Database**: Vercel Postgres (Disiapkan)
- **Integrasi Pihak Ketiga**: Telegram Bot API, Google Sheets (CSV Export)

## ⚙️ Persyaratan Environment Variables
Agar aplikasi dapat berjalan dan terhubung dengan Telegram, Anda wajib mengatur *Environment Variables* berikut di pengaturan hosting (Vercel):

| Variable Name | Deskripsi |
| :--- | :--- |
| `TELEGRAM_BOT_TOKEN` | Token Bot Telegram Anda (didapatkan dari @BotFather). |
| `TELEGRAM_CHAT_ID` | ID Grup atau Channel tempat dokumen akan dikirimkan. |

## 🌐 Panduan Deployment (Vercel)
Aplikasi ini sudah dikonfigurasi untuk *zero-config deployment* di Vercel.
1. *Push* kode ini ke repository GitHub Anda.
2. Login ke [Vercel](https://vercel.com/) dan buat proyek baru (*Import* repository ini).
3. Masukkan `TELEGRAM_BOT_TOKEN` dan `TELEGRAM_CHAT_ID` di menu **Environment Variables** Vercel.
4. Klik **Deploy**. Selesai!

---
*Dibuat untuk mempermudah manajemen dokumen tim lapangan secara cepat, efisien, dan tanpa batas kapasitas (Telegram Cloud).*
