# Proton Live Showroom — Landing Page

Landing page interaktif untuk sales advisor automotif: pilih model, viewer kereta (drag untuk tilt), kalkulator loan & trade-in, warna ready stock, CTA WhatsApp, dan responsive mobile.

## 📁 Struktur fail
```
live-showroom/
├─ index.html            ← halaman utama
├─ README.md
└─ assets/
   └─ img/
      ├─ saga.webp
      ├─ persona.webp
      ├─ iriz.webp
      ├─ s70.webp        ← sementara guna gambar Saga
      ├─ x50.webp
      ├─ x70.webp
      ├─ x90.webp
      └─ emas7.webp
```
> Kekalkan struktur folder ini. `index.html` merujuk gambar melalui `assets/img/...`, jadi folder `assets` mesti diupload sekali.

---

## 🚀 Upload ke GitHub Pages

### Cara A — Web GitHub (drag folder)
1. [github.com](https://github.com) → **New repository** → nama cth `live-showroom` → **Public** → **Create repository**.
2. Dalam repo → **Add file → Upload files**.
3. **Drag masuk kesemua kandungan** folder ini sekali gus — termasuk `index.html`, `README.md`, dan folder `assets` (boleh drag folder terus; GitHub akan kekalkan struktur).
4. **Commit changes**.
5. **Settings → Pages → Source: Deploy from a branch → Branch: `main` / `(root)` → Save**.
6. Tunggu ~1–2 minit. Live di:
   ```
   https://<username-anda>.github.io/live-showroom/
   ```

### Cara B — GitHub Desktop (kalau drag folder bermasalah)
1. Pasang **GitHub Desktop** → **File → New repository** (atau clone repo kosong).
2. Salin kesemua fail + folder `assets` ke dalam folder repo tempatan.
3. **Commit** → **Push origin**.
4. Aktifkan Pages seperti langkah 5–6 di atas.

### Cara C — Git command line
```bash
git init
git add .
git commit -m "Live Showroom landing page"
git branch -M main
git remote add origin https://github.com/<username>/live-showroom.git
git push -u origin main
```

---

## ✏️ Kemas kini kandungan
Dalam `index.html` (bahagian `<script>`, cari `const MODELS = {...}`):

| Nak tukar | Cari |
|---|---|
| Harga OTR / booking / gaji | `otr`, `book`, `salary` dalam `MODELS` |
| Warna | `MODELS[...].colors` |
| Kadar faedah loan | `const FLAT_RATE = 0.03;` (3% flat — sahkan dgn bank) |
| Nombor WhatsApp | `const WA_NUMBER = "60139383476";` |
| Nama advisor | cari `OLIVE` |
| Gambar model | ganti fail dalam `assets/img/` (kekalkan nama sama) |

**Sebelum go-live:**
- Ganti `assets/img/s70.webp` dengan gambar S70 sebenar.
- Sahkan semua harga & warna.
- Untuk 360° penuh: sediakan 24–36 frame/model (viewer sedia menyokong).

---
*Dibina oleh RankUp Digital.*
