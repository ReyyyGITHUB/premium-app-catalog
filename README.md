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
  Grid card berisi icon aplikasi, nama, durasi, harga, dan label stok.
- **Smart Search**  
  Pencarian instan untuk menemukan aplikasi tertentu.
- **Product Detail Modal**  
  Info lengkap produk dan tombol **“Beli Sekarang”**.

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

### Flow

1. Pembeli memilih produk
2. Checkout modal muncul:
   - Ringkasan pesanan
   - Gambar QRIS
3. Pembeli melakukan pembayaran
4. Konfirmasi via chat

### Confirmation Method (MVP Default)

Tombol **“Saya Sudah Bayar”** akan mengarahkan ke WhatsApp / Telegram dengan template pesan otomatis:

```text
Halo, saya sudah bayar pesanan:
- Produk: {{product_name}}
- Harga: {{price}}
- Durasi: {{duration}}
