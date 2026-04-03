# Contributing to AutoGoPay

Terima kasih atas minat Anda untuk berkontribusi ke AutoGoPay! 🎉

## Menambahkan Logo Toko Anda

Jika Anda menggunakan AutoGoPay untuk bisnis Anda dan ingin menampilkan logo toko di landing page kami, ikuti langkah-langkah berikut:

### Persyaratan Logo

1. **Format**: PNG atau SVG dengan background transparan
2. **Ukuran**: 100x100 pixels (akan di-resize otomatis jika lebih besar)
3. **Kualitas**: Logo harus jelas dan berkualitas tinggi
4. **Konten**: Logo harus merepresentasikan bisnis yang sah dan aktif menggunakan AutoGoPay

### Cara Menambahkan Logo

1. **Fork repository ini**
   ```bash
   git clone https://github.com/AutoFTbot/AutoGopay.git
   cd AutoGopay
   ```

2. **Tambahkan logo Anda**
   - Upload logo ke folder `logos/` di root repository
   - Nama file: `nama-toko.png` atau `nama-toko.svg` (lowercase, gunakan dash untuk spasi)
   - Contoh: `logos/toko-saya.png`

3. **Update file stores.json**
   - Edit file `logos/stores.json`
   - Tambahkan informasi toko Anda dengan URL GitHub raw:
   ```json
   {
     "name": "Nama Toko Anda",
     "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/toko-saya.png",
     "website": "https://tokosaya.com",
     "description": "Deskripsi singkat toko Anda"
   }
   ```

4. **Buat Pull Request**
   - Commit perubahan Anda
   ```bash
   git add logos/toko-saya.png
   git add logos/stores.json
   git commit -m "Add [Nama Toko] logo"
   git push origin main
   ```
   - Buat Pull Request ke repository utama
   - Jelaskan bisnis Anda dan bagaimana Anda menggunakan AutoGoPay

### Review Process

- Setiap Pull Request akan di-review oleh maintainer
- Logo akan di-approve jika memenuhi persyaratan dan bisnis terbukti aktif menggunakan AutoGoPay
- Proses review biasanya memakan waktu 1-3 hari kerja
- Kami berhak menolak logo yang tidak sesuai dengan guidelines

### Contoh Struktur Repository

```
AutoGopay/
├── logos/                    
│   ├── stores.json         
│   ├── example-store.svg
│   ├── toko-elektronik.png
│   ├── warung-kopi.svg
│   └── toko-saya.png        # Logo Anda
└── CONTRIBUTING.md
```

### Contoh stores.json

```json
[
  {
    "name": "Example Store",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/example-store.svg",
    "website": "https://example.com",
    "description": "Contoh toko yang menggunakan AutoGoPay untuk payment gateway"
  },
  {
    "name": "Toko Elektronik",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/toko-elektronik.png",
    "website": "https://tokoelektronik.com",
    "description": "Toko elektronik terpercaya sejak 2020"
  },
  {
    "name": "Warung Kopi",
    "logo": "https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/warung-kopi.svg",
    "website": "https://warungkopi.id",
    "description": "Kopi berkualitas dengan harga terjangkau"
  }
]
```

### Format URL Logo

Logo akan diambil dari GitHub raw URL dengan format:
```
https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/[nama-file]
```

Contoh:
- `https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/example-store.svg`
- `https://raw.githubusercontent.com/AutoFTbot/AutoGopay/main/logos/toko-saya.png`

## Aturan Umum

- Logo tidak boleh mengandung konten yang menyinggung, ilegal, atau tidak pantas
- Logo harus milik Anda atau Anda memiliki izin untuk menggunakannya
- Kami berhak menghapus logo kapan saja jika ditemukan pelanggaran
- Dengan mengirimkan logo, Anda setuju bahwa logo akan ditampilkan di website AutoGoPay

## Pertanyaan?

Jika Anda memiliki pertanyaan, silakan hubungi kami melalui:
- Telegram: [@AutoGopayBot](https://t.me/AutoGopayBot)
- GitHub Issues: [Create an issue](https://github.com/AutoFTbot/AutoGopay/issues)

---

Terima kasih telah menggunakan AutoGoPay! 🚀
