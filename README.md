# 🤖 Bot Eraspace - Discount & Stock Checker

Bot otomatis untuk mengecek produk diskon di Eraspace berdasarkan lokasi dan ketersediaan stock di toko terdekat.

## 📋 Fitur

- ✅ Cek produk diskon di Eraspace berdasarkan kategori
- 📍 Filter berdasarkan lokasi koordinat (latitude & longitude)
- 🏪 Cek ketersediaan stock di toko terdekat
- 💾 Export hasil ke file TXT
- 📊 Statistik lengkap hasil pencarian
- 🎯 Mode multi-kategori atau kategori spesifik

## 📦 Instalasi

```bash
# Clone repository
git clone https://github.com/codekuy/bot_eraspace.git
cd bot_eraspace

# Install dependencies
npm install
```

## 🔑 Dapatkan API Key

Bot ini memerlukan API Key dari Botnesia:

**👉 Dapatkan API Key di:** [https://botnesia.com/products/bot-eraspace](https://botnesia.com/products/bot-eraspace)

Atau kunjungi: [https://botnesia.com](https://botnesia.com)

> API Key akan otomatis diminta saat pertama kali menjalankan bot dan disimpan di file `apikey.txt`

## ⚠️ Penting - Pembatasan IP Address

**Bot ini hanya support 1 IP Address per API Key:**
- ✅ Satu API Key hanya bisa digunakan di 1 device/IP
- ❌ Tidak support multi-device atau multi-IP
- 🔄 Jika pindah device atau IP berubah, **wajib reset IP** di dashboard Botnesia

### Cara Reset IP:
1. Login ke [Botnesia.com](https://botnesia.com)
2. Masuk ke dashboard API Key
3. Pilih bot Eraspace yang aktif
4. Klik tombol **"Reset IP Address"**
5. Jalankan bot di device/IP baru

> **Note:** Setiap kali IP berubah (ganti WiFi, ganti device, dll), bot akan error. Harus reset IP terlebih dahulu.

## 🚀 Cara Penggunaan

### Metode 1: Mode Interaktif

```bash
npm start
```

Bot akan meminta:
1. Input koordinat lokasi (latitude & longitude)
2. Pilihan kategori produk

### Metode 2: Dengan Parameter Koordinat

```bash
node index.js -8.699558 115.180241
```

Kemudian pilih kategori yang diinginkan.

## 📍 Cara Mendapatkan Koordinat Lokasi

1. Buka [Google Maps](https://maps.google.com)
2. Klik kanan pada lokasi yang diinginkan
3. Klik koordinat yang muncul untuk menyalin
4. Format: `latitude, longitude` (contoh: `-8.699558, 115.180241`)

## 📁 Output

Hasil pencarian akan disimpan otomatis di folder `result/` dengan format nama file:
```
result/KATEGORI_TANGGAL_WAKTU.txt
```

### Contoh Format Output:

```
═══════════════════════════════════════════════════════════
🤖 BOT ERASPACE - HASIL CEK PRODUK DISKON + STOCK TOKO
═══════════════════════════════════════════════════════════

📍 Lokasi: -8.699558, 115.180241
📂 Kategori: Smartphone
📅 Tanggal: 05/11/2025 14:30:45
✅ Total: 15 produk dengan stock tersedia

═══════════════════════════════════════════════════════════

1. 📱 iPhone 15 Pro Max 256GB
   ═══════════════════════════════════════════════════════════
   📂 Kategori      : Smartphone
   💰 Harga Normal  : Rp 21.999.000
   🔥 Harga Diskon  : Rp 19.999.000
   🎉 DISKON        : 9% OFF
   📦 SKU           : IPHONE15PM256

   📍 STOCK TERSEDIA DI 3 TOKO:

      1. ✅ Eraspace Denpasar
         📍 Alamat  : Jl. Teuku Umar No. 123, Denpasar
         📏 Jarak   : 2.5 km

      2. ✅ Eraspace Mall Bali Galeria
         📍 Alamat  : Sunset Road, Kuta
         📏 Jarak   : 5.8 km

      3. ✅ Eraspace Level 21 Mall
         📍 Alamat  : Jl. Raya Kuta, Badung
         📏 Jarak   : 7.2 km
   ───────────────────────────────────────────────────────

2. 📱 Samsung Galaxy S24 Ultra
   ═══════════════════════════════════════════════════════════
   ...
```

File berisi informasi lengkap:
- Header dengan info lokasi dan tanggal
- Detail setiap produk dengan diskon
- Harga normal & harga diskon
- Persentase diskon
- SKU produk
- List toko dengan stock tersedia
- Alamat lengkap toko
- Jarak dari lokasi Anda

## 🛠️ Requirements

- Node.js 14.x atau lebih tinggi
- NPM atau Yarn
- API Key dari Botnesia

## 📝 Lisensi

ISC

## 👨‍💻 Author

Created by Ariel Septian

## 🔗 Links

- **Get API Key:** [https://botnesia.com/products/bot-eraspace](https://botnesia.com/products/bot-eraspace)
- **Botnesia Website:** [https://botnesia.com](https://botnesia.com)
- **Facebook:** [fb.com/arielseptian129](https://fb.com/arielseptian129)

## ❓ Support

Jika mengalami kendala, silakan hubungi support Botnesia atau kunjungi website resmi.

---

⭐ **Jangan lupa star repository ini jika bermanfaat!**
