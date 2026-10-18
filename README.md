# XaviOS Web: situs penjelasan proyek

Website animasi yang menjelaskan **XaviOS Hybrid Glass**: Xavi Glass, Xavi Band, Chip 1:1,
Integration Core, Sukuna AI, dan pipeline voice (STT, TTS, RVC).
Stack: React 19, Vite 6, **framer-motion**. Semua gambar adalah SVG animasi buatan sendiri.

## Menjalankan

```bash
npm install          # sudah memasang framer-motion (lihat package.json)
npm run dev          # http://localhost:5173
npm run build        # hasil di dist/
npm run preview
```

Butuh Node.js 18+. Kalau mau memasang framer-motion manual: `npm i framer-motion`.

## Struktur

- `src/App.jsx`: semua section dan animasi (scroll reveal, counter, tilt, tab, pipeline)
- `src/art.jsx`: ilustrasi SVG (Glass, Band, Chip) dan diagram hub animasi
- `src/index.css`: gaya glass dan responsif
- `src/main.jsx`: entry, `MotionConfig reducedMotion="user"` (menghormati pengaturan reduced motion)

## Catatan

Konten mengikuti master prompt refactor XaviOS. Situs ini menjelaskan target arsitektur,
bukan bukti bahwa tiap modul sudah berjalan di hardware nyata.
