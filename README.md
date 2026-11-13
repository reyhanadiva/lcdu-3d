# LCDU — arsip hero 3D

Arsip (cadangan) landing page LCDU **dengan hero 3D** (`hero/diorama.js`: Kubah Shakhrah & Masjid Qibli, three.js r160,
bloom, GSAP). Repo utama [`reyhanadiva/lcdu`](https://github.com/reyhanadiva/lcdu) sejak November 2026 hanya memakai
hero **Foto** (`hero/lentera-hd.js`); varian 3D dipindahkan ke sini untuk jaga-jaga.

- **Asal snapshot**: `reyhanadiva/lcdu` commit `b6e428ed29330b96c4b9ebf4853f1d8b3820ee90`
  ("Dokumentasi aliran benang…"), disalin utuh tanpa `.git` dan `node_modules`.
- **Status**: arsip, tidak dikembangkan lagi. Section setelah hero di sini bisa tertinggal dari repo utama.
- Dokumentasi proyek asli: `README-proyek.md` dan `CLAUDE.md` (keadaan saat snapshot).

## Menjalankan

```bash
python3 -m http.server 8000
```

Buka `http://localhost:8000/?hero=diorama` (3D) atau `?hero=lentera-hd` (Foto). Modul ES butuh server, bukan `file://`.
Alat pengembang: `?debug-perf`, `?tier=0|1|2`, `?hero=diorama&edit-lights`, `?hero=diorama&debug-veg`.

Alat aset 3D (opsional): `cd tools && npm install && npm run models` — lihat `tools/README.md`.

## Lisensi pihak ketiga

three.js (MIT) di `vendor/three/`; GSAP (lisensi standar GreenSock, bukan MIT) di `vendor/gsap/`;
Lenis (MIT) di `vendor/lenis/`. Model Kubah & Qibli dibuat dari gambar ChatGPT lalu diubah ke 3D dengan TRELLIS.2 (MIT).
