# Reltroner Statistics — Illustration Resource

Aset ilustrasi editorial untuk situs statis `reltroner-statistics`. Repositori ini hanya
menyimpan berkas gambar, prompt, dan katalog; ia tidak menyimpan canon, angka statistik,
chart analitik, atau keluaran build aplikasi.

## Status saat ini

| Item | Keadaan |
|---|---|
| Git repository | Ada. Di-bootstrap dengan `git init -b main`; branch `main` melacak `origin/main`. |
| Remote | `https://github.com/Reltroner/reltroner-statistics-resource.git` |
| Aset gambar | NOT AVAILABLE — belum ada berkas gambar. |
| Fasilitas generasi | NOT AVAILABLE — tidak ada kredensial penyedia gambar dan tidak ada runtime generasi lokal. |
| CDN pin | NOT AVAILABLE — belum ada aset untuk dipin. Mekanisme jsDelivr `gh/<owner>/<repo>@<full-sha>` sudah diverifikasi byte-identik untuk berkas teks di repositori ini. |

Karena belum ada aset, `images/`, `masters/`, dan `manifest.json` sengaja belum dibuat.
Membuat katalog tanpa berkas terukur akan menjadi data rekaan.

## Struktur yang diusulkan

```
README.md
images/          # aset delivery yang dipakai aplikasi
masters/         # master final terpilih, bila ada
prompts/         # prompt final dan metadata generasi yang benar-benar tersedia
manifest.json    # katalog path relatif + metadata terukur
```

Hanya `README.md` dan `prompts/` yang dibuat pada tahap ini.

## Aturan nama berkas

Nama diturunkan dari ID slot aktif dengan normalisasi deterministik:

1. Ubah seluruh karakter menjadi huruf kecil.
2. Ganti setiap `_` dengan `-`.
3. Pertahankan hanya `a-z`, `0-9`, dan `-`.
4. Tambahkan ekstensi sesuai format delivery (`.webp` untuk aset utama).

Contoh: `STATS_HOME_HERO` → `stats-home-hero.webp`.

Pemeriksaan tabrakan dilakukan pada seluruh 18 ID aktif: 18 nama unik, 0 tabrakan.

## Batas

- Tidak ada teks, angka, watermark, logo, atau badge status di dalam gambar.
- Tidak ada chart palsu, tangkapan layar dashboard palsu, atau jumlah faktual.
- Tidak ada geografi, bendera, anatomi ancestry, atau objek canon rekaan.
- Proposal remodeling tidak boleh divisualkan sebagai production.
- Ilustrasi tidak pernah menggantikan hasil statistik, chart, atau empty state.
