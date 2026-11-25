# Reltroner Statistics — Illustration Resource

Aset ilustrasi editorial untuk situs statis `reltroner-statistics`. Repositori ini hanya
menyimpan berkas gambar, prompt, dan katalog; ia tidak menyimpan canon, angka statistik,
chart analitik, branding situs, atau keluaran build aplikasi.

## Status saat ini

| Item | Keadaan |
|---|---|
| Git repository | Ada. Branch `main` melacak `origin/main`. |
| Remote | `https://github.com/Reltroner/reltroner-statistics-resource.git` |
| Cakupan slot | `18` slot terdaftar (1:1): **`9` `READY`** (`images/*.webp` + `masters/*.jpg`), **`9` `PROMPT_ONLY`** (`IMAGE_GENERATION_QUOTA_EXHAUSTED` HTTP 429 — tanpa dummy). |
| Optimasi delivery | Pillow `13.0.0`, center-fit rasio slot eksak (downscale only, `LANCZOS`), `WEBP quality=86 method=6`. |
| Katalog | `manifest.json` (katalog resource memakai path relatif saja; pin full commit SHA 40 karakter disimpan di aplikasi setelah publikasi). |
| CDN | jsDelivr `https://cdn.jsdelivr.net/gh/Reltroner/reltroner-statistics-resource@<full-40-hex-sha>/images/<slug>.webp`. |

## Struktur repositori

```text
README.md
images/          # aset delivery WebP yang dipakai aplikasi (9 berkas READY)
masters/         # master JPEG asli terpilih tanpa modifikasi (9 berkas READY)
prompts/         # prompt final 18 slot dan metadata generasi aktual
manifest.json    # katalog path relatif + dimensi, ukuran byte, dan SHA-256 terukur
```

## Aturan nama berkas

Nama diturunkan dari ID slot aktif dengan normalisasi deterministik:

1. Ubah seluruh karakter menjadi huruf kecil.
2. Ganti setiap `_` dengan `-`.
3. Pertahankan hanya `a-z`, `0-9`, dan `-`.
4. Tambahkan ekstensi `.webp` di `images/` untuk aset delivery dan `.jpg` di `masters/` untuk master.

Contoh: `STATS_HOME_HERO` → `images/stats-home-hero.webp` (master: `masters/stats-home-hero.jpg`).

Pemeriksaan tabrakan dilakukan pada seluruh 18 ID aktif: 18 nama unik, 0 tabrakan.

## Inventaris aset delivery (`images/`)

| Slot ID | Status | Path | Dimensi | Rasio | Bytes | SHA-256 |
|---|---|---|---|---|---:|---|
| `STATS_HOME_HERO` | `READY` | `images/stats-home-hero.webp` | `1280×720` | `16 / 9` | `33,308` | `d55e9e5cf5158a07f972cb0d0c49ffdf9b7c7e93c5b8ccedd424e2945549a4cd` |
| `STATS_WORLD_OVERVIEW` | `READY` | `images/stats-world-overview.webp` | `1200×800` | `3 / 2` | `34,924` | `c02a3c9c26661247b58f75a5816910f5cd929db143db50c37acd8e804a38c1fb` |
| `STATS_COUNTRY_COMPARISON` | `READY` | `images/stats-country-comparison.webp` | `1200×800` | `3 / 2` | `34,120` | `b795eb12d57681bf120bf4a2bd55d4800dda253b10e99b4099e5571778175a68` |
| `STATS_HISTORICAL_DYNAMICS` | `READY` | `images/stats-historical-dynamics.webp` | `1280×720` | `16 / 9` | `17,354` | `67cb670456809d1602e745880c20f313d90f6c017a64238f39df2f5fca48e437` |
| `STATS_CLUSTERING_LAB` | `READY` | `images/stats-clustering-lab.webp` | `1200×800` | `3 / 2` | `57,282` | `5007a050913663f50b64a446c9f3168a16adb9d457023c43eabc44e9459a81ed` |
| `STATS_DEPENDENCY_GRAPH` | `READY` | `images/stats-dependency-graph.webp` | `1200×800` | `3 / 2` | `30,916` | `31e64766f6d87b16cbce9ca7054e0fd8fbff9216b4df537cc034f55bee9b01e2` |
| `STATS_SOURCE_DRIFT` | `READY` | `images/stats-source-drift.webp` | `1200×800` | `3 / 2` | `32,150` | `8f4fd5613b9b41d4ea56a2d6e8d4c46234b3ef3d654afbe937e02691a5d6ccbc` |
| `STATS_REPORT_CENTER` | `READY` | `images/stats-report-center.webp` | `1152×864` | `4 / 3` | `24,096` | `7ff2fceaa0302c37ed3a7c5897599150415f27c7de1477ce39681a7a5d67bf51` |
| `CREATIVE_HOME_HERO` | `READY` | `images/creative-home-hero.webp` | `1280×720` | `16 / 9` | `19,838` | `da0e78d607cdacf65c0a310b5d11af211e79b85b4cf418e8695eb9a4b4b1345b` |
| `CREATIVE_NARRATIVE_GRAPH` | `PROMPT_ONLY` | `images/creative-narrative-graph.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_IDEATION_WORKSPACE` | `PROMPT_ONLY` | `images/creative-ideation-workspace.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_CONSISTENCY_AUDIT` | `PROMPT_ONLY` | `images/creative-consistency-audit.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_STORY_REFACTOR` | `PROMPT_ONLY` | `images/creative-story-refactor.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_CANON_REMODEL` | `PROMPT_ONLY` | `images/creative-canon-remodel.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_IMPACT_EXPLORER` | `PROMPT_ONLY` | `images/creative-impact-explorer.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_DEVELOPMENT_ROADMAP` | `PROMPT_ONLY` | `images/creative-development-roadmap.webp` (belum ada) | — | `16 / 9` | — | Kuota model gambar habis (HTTP 429) |
| `CREATIVE_DECISION_TREE` | `PROMPT_ONLY` | `images/creative-decision-tree.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |
| `STATISTICAL_DECISION_TREE` | `PROMPT_ONLY` | `images/statistical-decision-tree.webp` (belum ada) | — | `3 / 2` | — | Kuota model gambar habis (HTTP 429) |

## Batas

- Tidak ada teks, angka, watermark, logo, atau badge status di dalam gambar.
- Tidak ada chart palsu, tangkapan layar dashboard palsu, atau jumlah faktual.
- Tidak ada geografi, bendera, anatomi ancestry, atau objek canon rekaan.
- Proposal remodeling tidak boleh divisualkan sebagai production.
- Ilustrasi tidak pernah menggantikan hasil statistik, chart, atau empty state.
