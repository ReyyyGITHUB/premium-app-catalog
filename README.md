# Premium App Catalog

**MVP platform for premium app sellers — visual catalog, manual QRIS payment, and chat-first checkout flow.**

Premium App Catalog adalah website katalog visual untuk penjual aplikasi premium yang ingin mengganti promosi berbasis chat menjadi storefront profesional dengan konversi langsung ke WhatsApp atau Telegram.

Tujuan utama produk ini adalah **mengurangi friksi jualan di chat**, meningkatkan **trust pembeli**, dan **menstandarkan format order** tanpa payment gateway.

---

## 🚀 Core Concept

> Link-in-bio versi e-commerce untuk penjual aplikasi premium.

Pembeli bisa melihat katalog, harga, dan stok tanpa login, lalu menyelesaikan transaksi via QRIS dan chat.

---

## ✨ MVP Features

### 🛍️ Storefront (Buyer Side)

- **Anonymous Browsing**  
  Pembeli bisa melihat produk tanpa login atau registrasi.

- **Visual Product Catalog**  
  Grid card berisi:
  - Icon aplikasi  
  - Nama & durasi  
  - Harga  
  - Label stok (Ready / Limited)

- **Smart Search**  
  Pencarian instan untuk menemukan aplikasi dengan cepat.

- **Product Detail Modal**  
  Detail lengkap produk + tombol **“Beli Sekarang”**.

---

### 🧑‍💼 Admin Dashboard (Seller Side)

- **Product Management**
  - Tambah, edit, dan hapus produk
  - Update harga & stok

- **Store Settings**
  - Nama toko & deskripsi
  - Nomor WhatsApp atau username Telegram
  - Upload / input URL gambar QRIS

- **Simple Auth**
  - Login admin dengan username & password statis (MVP)

---

## 💳 Payment Flow (Manual Verification)

Tanpa payment gateway untuk menghindari biaya admin dan kompleksitas integrasi.

### Flow:

1. Pembeli memilih produk
2. Checkout modal muncul:
   - Ringkasan pesanan
   - Gambar QRIS
3. Pembeli melakukan pembayaran
4. Konfirmasi via chat

### Confirmation Method (MVP Default)

- **Direct Chat Confirmation**  
  Tombol **“Saya Sudah Bayar”** akan mengarahkan ke WhatsApp / Telegram
  dengan template pesan otomatis:


> Upload bukti transfer di website disiapkan untuk tahap selanjutnya, bukan MVP.

---

## 💡 Why Use This Instead of Chat Only?

- **Visual Trust**  
Katalog profesional meningkatkan kredibilitas penjual.

- **Self-Service Buyer**  
Pembeli tidak perlu bertanya harga atau stok.

- **Standardized Orders**  
Penjual menerima format order yang rapi dan konsisten.

---

## 🧠 Technical Decisions

### Tech Stack

- React (Single Page Application)
- Tailwind CSS

### Data Persistence

- **Seller**
- Database (Firebase / sejenis)
- Produk & pengaturan toko

- **Buyer**
- localStorage
- Terakhir dilihat & histori pesanan (tanpa akun)

---

## 🗂️ Project Structure (Planned)


---

## 🧪 MVP Scope (Out of Scope)

- Payment gateway otomatis
- Multi-seller marketplace
- Akun pembeli
- Order tracking
- Role management admin

---

## 🛣️ Roadmap (Post-MVP)

- Upload bukti transfer via website
- Unique payment code
- Telegram Bot integration
- Multi-store support
- Order analytics dashboard

---

## 📌 Status

🚧 Active Development (MVP Stage)
