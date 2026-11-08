# ✈️ B-21 Raider 3D — Penampil Struktur Pesawat Interaktif

Website 3D interaktif untuk menjelajahi struktur pesawat pembom siluman **B-21 Raider**, dibuat dengan **Three.js** (WebGL) tanpa framework dan tanpa build step.

**Live demo:** https://b21-raider-3d.vercel.app

> Model 3D ini adalah rekonstruksi ilustratif berdasarkan foto publik, bukan data resmi. Sebagian besar data teknis B-21 masih dirahasiakan.

## Fitur

- **21 komponen, 74.432 segitiga**: rangka & kulit, kokpit, mesin turbofan, saluran udara S-duct, spar & rusuk sayap, permukaan kendali, roda pendarat, ruang bom, dan livery.
- **4 mode tampilan**: Solid, X-Ray, Wireframe, dan Warna Sistem.
- **Exploded view**: urai komponen dengan slider.
- **Potongan penampang**: belah pesawat secara memanjang, melintang, atau horizontal.
- **Daftar komponen**: cari, sembunyikan, isolasi, fokus kamera, dan lihat detail setiap bagian.
- **Animasi**: roda pendarat naik/turun, pintu ruang bom & peluncur putar, kipas mesin.
- **Simulasi misi**: lepas landas, awan & kota muncul di bawah jalur, peluncuran senjata dengan efek ledakan bergaya game, lengkap dengan HUD ketinggian, kecepatan, dan amunisi.
- **Preset kamera** (isometrik, atas, bawah, depan, samping, belakang), screenshot, dan tautan tampilan lewat URL hash (`#cam=…&mode=xray&explode=50`).
- **Responsif** untuk desktop dan mobile.

## Kontrol

| Aksi | Kontrol |
|---|---|
| Putar | Seret mouse / satu jari |
| Zoom | Scroll / pinch |
| Geser | Klik kanan + seret |
| Detail komponen | Klik bagian pesawat |
| Terbang / mendarat | `T` |
| Luncurkan senjata | `Spasi` |
| Isi ulang senjata | `R` |

## Menjalankan Secara Lokal

Cukup sajikan folder ini lewat server statis (diperlukan karena memakai ES modules):

```bash
npx serve .
# atau
python -m http.server 8000
```

Lalu buka `http://localhost:8000`.

## Teknologi

- Three.js 0.160 (OrbitControls, RoomEnvironment, CSS2DRenderer) via import map dari CDN
- JavaScript (ES modules), HTML5, CSS3
- Deploy di Vercel

---

<div align="center">

**Built with ❤️ by [whympxx](https://github.com/whympxx)**

</div>
