# Proton Live Showroom — Landing Page (flat / root version)

**Semua fail berada di ROOT — TIADA folder.** Ini elak masalah "folder flatten" masa upload ke GitHub, dan gambar akan sentiasa jumpa.

```
index.html
README.md
.nojekyll
saga.webp  persona.webp  iriz.webp  s70.webp
x50.webp   x70.webp      x90.webp   emas7.webp
```

---

## ✅ Cara paling cepat betulkan website sedia ada

Repo anda sudah ada fail `.webp` di root. Anda cuma perlu **ganti `index.html`**:

1. Buka repo `protonshowroom` di GitHub.
2. Klik fail **`index.html`** → ikon **pensil (Edit)** → padam semua → tampal kandungan `index.html` baru ini.
   *(atau: **Add file → Upload files** → drag `index.html` baru → ia akan menggantikan yang lama → Commit)*
3. **Commit changes.**
4. Tunggu ~1 minit, kemudian buka website di telefon dan **refresh kuat** (tarik-ke-bawah untuk reload, atau clear cache) — gambar akan muncul.

> Kenapa tadi gambar tak keluar: `index.html` lama mencari gambar dalam `assets/img/…`, tetapi fail `.webp` berada di root repo. Versi baru ini merujuk gambar terus di root (`x50.webp`), jadi ia padan.

---

## 🔁 Atau mulakan bersih (upload semua sekali)

1. Padam fail lama dalam repo (atau buat repo baru).
2. **Add file → Upload files** → drag **kesemua fail dalam pakej ini** (semua di root, tiada folder) → **Commit**.
3. **Settings → Pages → Deploy from a branch → `main` / `(root)` → Save**.

---

## 📱 Nota mobile
- Versi ini sudah responsive (1 kolum di telefon, model jadi chip scroll, WhatsApp button terapung).
- Kalau masih nampak versi lama di telefon: itu **cache**. Cuba buka dalam tab peribadi/incognito atau clear cache browser. GitHub Pages juga ambil masa 1–2 minit untuk kemas kini.

## ✏️ Kemas kini kandungan
Dalam `index.html` (`<script>`, cari `const MODELS`): harga (`otr`), warna (`colors`), kadar loan (`FLAT_RATE = 0.03`), nombor WhatsApp (`WA_NUMBER`).
Ganti gambar: timpa fail `.webp` dengan nama sama. **S70** kini guna gambar Saga — ganti `s70.webp` bila ada gambar sebenar.

---
*Dibina oleh RankUp Digital.*
