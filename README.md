# ARQR Brands · WebAR

AR Camera di browser untuk 5 produk **Tiffany & Co.** dan **adidas**. Scan kartu QR dengan kamera iPhone/Android,
website terbuka, lalu animasi 3D muncul di atas kartu. Tidak perlu install aplikasi.

**Website:** https://umbara19.github.io/arqr-brands/
**Preview tanpa kamera:** https://umbara19.github.io/arqr-brands/?preview=1

| Kartu (`cards/`) | Produk |
|---|---|
| `Card_tiffany-setting-ring.png` | The Tiffany® Setting Engagement Ring |
| `Card_tiffany-heart-tag.png` | Return to Tiffany® Heart Tag Pendant |
| `Card_tiffany-hardwear-bracelet.png` | Tiffany HardWear Link Bracelet |
| `Card_adidas-supernova.png` | adidas Supernova Running Shoes |
| `Card_adidas-trionda.png` | adidas Trionda Official Match Ball |

Cetak kartunya (sekitar 10–12 cm) atau tampilkan di layar lain, lalu scan QR-nya dengan kamera HP.

## Isi

- `index.html`, `app.js`, `style.css`: halaman WebAR (MindAR 1.2.5 + three.js 0.160 dari CDN).
- `targets.mind`: data pelacakan 5 kartu (urutan sama dengan `models/products.json`).
- `models/*.glb`: model 3D yang diekspor dari project Unity (`ARQR → WebAR → Export GLB`).
- `models/products.json`: nama produk, warna, dan parameter animasi (sama dengan prefab Unity).
- `tools/compile.html`: membuat ulang `targets.mind` dari gambar kartu (jalankan lewat `Tools/webar_server.py` di project Unity).

Model 3D-nya adalah prototipe bergaya untuk tugas kuliah, bukan model resmi brand.
