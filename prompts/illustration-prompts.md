# Prompt Ilustrasi Editorial — 18 Slot Aktif

Prompt di bawah adalah prompt final per slot. Badan prompt ditulis dalam bahasa Inggris
agar cocok dengan model gambar; judul, catatan, dan batasan ditulis dalam bahasa Indonesia.

## Metadata generasi

| Field | Nilai |
|---|---|
| Fasilitas generasi | Subagent `image-generator` bawaan runtime lokal (tanpa dependency atau layanan eksternal baru) |
| Model internal | NOT AVAILABLE (tidak diekspos oleh runtime) |
| Seed | NOT AVAILABLE (tidak diekspos oleh runtime) |
| Durasi | NOT AVAILABLE |
| Token / usage | NOT AVAILABLE |
| Tanggal generasi | `2026-11-25` |
| Berkas keluaran | `9` slot `READY` (`masters/*.jpg` + `images/*.webp` terukur di `manifest.json`); `9` slot `PROMPT_ONLY` karena kuota model gambar habis (`HTTP 429 RESOURCE_EXHAUSTED`, tanpa dummy) |
| Optimasi delivery | Pillow `13.0.0`, `ImageOps.fit` (`LANCZOS`, downscale saja ke rasio slot eksak), `WEBP quality=86 method=6` |

Metadata yang tidak diekspos oleh runtime dicatat persis `NOT AVAILABLE` dan tidak diperkirakan.

## Art direction bersama

Scientific editorial illustration. Presisi, tenang, kedalaman isometrik terkendali, ruang
negatif cukup. Palet mengikuti token aktif: latar `#030a18` / `#0b1a33`, aksen `#6aaeff`,
`#35d9f2`, `#5b9bff`, aksen hangat `#e8804f`, tinta `#eef5ff`. Satu artwork harus bekerja
pada tema gelap (default) dan terang, sehingga kontras internal tidak bergantung pada latar.

Batasan bersama untuk semua slot:

- Tanpa teks, angka, label, watermark, logo, atau badge status di dalam gambar.
- Tanpa chart palsu, tangkapan layar dashboard, atau jumlah faktual.
- Tanpa geografi nyata, bendera, batas negara, anatomi ancestry, atau objek canon rekaan.
- Tanpa figur manusia, wajah, atau simbol keagamaan.
- Tidak menggambarkan proposal remodeling sebagai production.
- Tidak menggantikan hasil statistik, chart analitik, atau empty state.

## Slot

### 1. STATS_HOME_HERO — 16 / 9 — `stats-home-hero.webp`

Fungsi: ilustrasi observatorium utama beranda. Motif registry: `orbital`.

```
Scientific editorial illustration of an abstract observatory: a non-cartographic sphere
made of thin concentric shells, transparent observation layers orbiting it, and a small
archive of geometric record slabs resting on a quiet plinth. Controlled isometric depth,
generous negative space, precise hairline strokes, cool cobalt and cyan accents with one
warm ember accent. No text, no numbers, no labels, no logos, no flags, no maps, no
recognizable geography, no charts, no dashboard UI. Calm, exact, museum-plate restraint.
Wide 16:9 composition with the sphere off-center and clear space on the left for overlay
copy. Works on a near-black background and on a light background.
```

### 2. STATS_WORLD_OVERVIEW — 3 / 2 — `stats-world-overview.webp`

Fungsi: pengantar statistik planet. Motif registry: `contour`.

```
Scientific editorial illustration of an abstract planetary body rendered only as layered
contour bands and a neutral observation module hovering beside it. No continents, no
coastlines, no borders, no recognizable geography. Thin precise contour lines, controlled
isometric depth, generous negative space, cobalt and cyan accents. No text, no numbers, no
labels, no logos, no charts, no dashboard UI. 3:2 composition, calm and exact, readable on
both dark and light backgrounds.
```

### 3. STATS_COUNTRY_COMPARISON — 3 / 2 — `stats-country-comparison.webp`

Fungsi: perbandingan lintas negara. Motif registry: `lattice`.

```
Scientific editorial illustration of a neutral measurement lattice: an evenly spaced grid
of small nodes with two parallel vertical reference axes and a handful of highlighted
points, suggesting comparison between two abstract units without naming them. No flags, no
maps, no country shapes, no text, no numbers, no labels, no logos, no charts. Thin precise
strokes, controlled isometric depth, generous negative space, cobalt and cyan accents with
one warm accent. 3:2 composition, calm and exact, readable on dark and light backgrounds.
```

### 4. STATS_HISTORICAL_DYNAMICS — 16 / 9 — `stats-historical-dynamics.webp`

Fungsi: dinamika historis BAC. Motif registry: `chronology`.

```
Scientific editorial illustration of an abstract chronology: two smooth arcs sweeping
across the frame with small markers spaced along them and a faint baseline beneath, evoking
recorded intervals without any dates, numbers, or axis labels. No text, no numbers, no
labels, no logos, no charts, no dashboard UI. Thin precise strokes, controlled isometric
depth, generous negative space, cobalt and cyan accents. Wide 16:9 composition, calm and
exact, readable on dark and light backgrounds.
```

### 5. STATS_CLUSTERING_LAB — 3 / 2 — `stats-clustering-lab.webp`

Fungsi: konsep clustering. Motif registry: `clusters`.

```
Scientific editorial illustration of three loose groups of small geometric forms whose
boundaries are deliberately ambiguous: soft dashed envelopes that overlap, a few forms
sitting between groups, no hard partition. No text, no numbers, no labels, no logos, no
charts, no dashboard UI. Thin precise strokes, controlled isometric depth, generous
negative space, cobalt, cyan and warm accents. 3:2 composition, calm and exact, readable on
dark and light backgrounds.
```

### 6. STATS_DEPENDENCY_GRAPH — 3 / 2 — `stats-dependency-graph.webp`

Fungsi: relasi data. Motif registry: `network`.

```
Scientific editorial illustration of a layered modular network: a ring of small modules
connected by thin edges, converging downward into a single foundation block that reads as
an archive. Controlled isometric depth, precise hairline edges, generous negative space,
cobalt and cyan accents. No text, no numbers, no labels, no logos, no charts, no dashboard
UI, no arrows implying causality. 3:2 composition, calm and exact, readable on dark and
light backgrounds.
```

### 7. STATS_SOURCE_DRIFT — 3 / 2 — `stats-source-drift.webp`

Fungsi: perbandingan production dan remodeling. Motif registry: `twin-orbits`.

```
Scientific editorial illustration of two overlapping orbital rings of equal visual weight,
one cool and one warm, with a short ladder of neutral rungs between them suggesting measured
difference rather than hierarchy. Neither ring may look superior, newer, or approved. No
text, no numbers, no labels, no logos, no badges, no charts. Thin precise strokes,
controlled isometric depth, generous negative space. 3:2 composition, calm and exact,
readable on dark and light backgrounds.
```

### 8. STATS_REPORT_CENTER — 4 / 3 — `stats-report-center.webp`

Fungsi: pratinjau laporan dan ekspor. Motif registry: `documents`.

```
Scientific editorial illustration of one source node feeding a fanned stack of identical
document slabs of equal weight, each with abstract ruled lines and one small seal-like
rectangle, no readable text. Equal weight across outputs, no hierarchy, no numbers, no
labels, no logos, no charts, no dashboard UI. Thin precise strokes, controlled isometric
depth, generous negative space, cobalt and cyan accents. 4:3 composition, calm and exact,
readable on dark and light backgrounds.
```

### 9. CREATIVE_HOME_HERO — 16 / 9 — `creative-home-hero.webp`

Fungsi: ikhtisar Creative Intelligence. Motif registry: `constellation`.

```
Scientific editorial illustration of an abstract constellation of idea nodes: two soft
circular fields joined by a precise polyline, with a few brighter nodes and one warm node
marking a junction. No text, no numbers, no labels, no logos, no charts, no dashboard UI,
no recognizable constellation from real astronomy. Thin precise strokes, controlled
isometric depth, generous negative space, cobalt and cyan accents. Wide 16:9 composition,
calm and exact, readable on dark and light backgrounds.
```

### 10. CREATIVE_NARRATIVE_GRAPH — 3 / 2 — `creative-narrative-graph.webp`

Fungsi: graph relasi naratif. Motif registry: `network`.

```
Scientific editorial illustration of a narrative relationship graph: an irregular ring of
small nodes linked by thin edges, with one central node and a few longer cross-links that
stay clearly weaker than the ring. Co-occurrence, not causality: no arrowheads. No text, no
numbers, no labels, no logos, no charts. Thin precise strokes, controlled isometric depth,
generous negative space, cobalt and cyan accents. 3:2 composition, calm and exact, readable
on dark and light backgrounds.
```

### 11. CREATIVE_IDEATION_WORKSPACE — 3 / 2 — `creative-ideation-workspace.webp`

Fungsi: ruang ide dan brainstorming cerita. Motif registry: `prism`.

```
Scientific editorial illustration of a single beam entering a triangular prism and leaving
as three separated beams of different hue, evoking divergence of one idea into variants. No
text, no numbers, no labels, no logos, no charts, no dashboard UI. Thin precise strokes,
controlled isometric depth, generous negative space, cobalt, cyan and warm accents. 3:2
composition, calm and exact, readable on dark and light backgrounds.
```

### 12. CREATIVE_CONSISTENCY_AUDIT — 3 / 2 — `creative-consistency-audit.webp`

Fungsi: temuan konsistensi naratif. Motif registry: `scales`.

```
Scientific editorial illustration of a neutral balance: a thin vertical axis with a level
beam and two equal pans, each holding an abstract geometric mass of identical size. The beam
must read as level, not tilted. No text, no numbers, no labels, no logos, no badges, no
charts. Thin precise strokes, controlled isometric depth, generous negative space, cobalt
and cyan accents with one warm accent. 3:2 composition, calm and exact, readable on dark and
light backgrounds.
```

### 13. CREATIVE_STORY_REFACTOR — 3 / 2 — `creative-story-refactor.webp`

Fungsi: restrukturisasi dan refactor cerita. Motif registry: `blueprint`.

```
Scientific editorial illustration of a structural blueprint: one tall module on the left
connected by two clean routing paths to two smaller modules stacked on the right, drawn as
precise technical outlines with no dimensions or annotations. No text, no numbers, no
labels, no logos, no charts, no dashboard UI. Thin precise strokes, controlled isometric
depth, generous negative space, cobalt, cyan and warm accents. 3:2 composition, calm and
exact, readable on dark and light backgrounds.
```

### 14. CREATIVE_CANON_REMODEL — 3 / 2 — `creative-canon-remodel.webp`

Fungsi: remodeling canon dan skenario. Motif registry: `twin-orbits`.

```
Scientific editorial illustration of two equal orbital rings, one cool and one warm,
overlapping without either enclosing the other, with neutral rungs between them. The warm
ring must read as a parallel proposal of equal weight, never as an approved replacement. No
text, no numbers, no labels, no logos, no badges, no charts. Thin precise strokes,
controlled isometric depth, generous negative space. 3:2 composition, calm and exact,
readable on dark and light backgrounds.
```

### 15. CREATIVE_IMPACT_EXPLORER — 3 / 2 — `creative-impact-explorer.webp`

Fungsi: penjelajah konsekuensi dan dampak. Motif registry: `ripples`.

```
Scientific editorial illustration of concentric ripples spreading from a single small
source, with the outer rings dashed to show decreasing certainty rather than decreasing
importance. No text, no numbers, no labels, no logos, no charts, no dashboard UI. Thin
precise strokes, controlled isometric depth, generous negative space, cobalt, cyan and warm
accents. 3:2 composition, calm and exact, readable on dark and light backgrounds.
```

### 16. CREATIVE_DEVELOPMENT_ROADMAP — 16 / 9 — `creative-development-roadmap.webp`

Fungsi: roadmap dan peluang pengembangan kreatif. Motif registry: `chronology`.

```
Scientific editorial illustration of an abstract roadmap: a long horizontal sequence of
evenly spaced markers along a single gentle arc, with two short parallel arcs suggesting
alternative tracks. No dates, no numbers, no milestones labels, no text, no logos, no
charts. Thin precise strokes, controlled isometric depth, generous negative space, cobalt
and cyan accents. Wide 16:9 composition, calm and exact, readable on dark and light
backgrounds.
```

### 17. CREATIVE_DECISION_TREE — 3 / 2 — `creative-decision-tree.webp`

Fungsi: decision tree kreatif dan editorial interaktif. Motif registry: `branching`.

```
Scientific editorial illustration of a branching decision structure: one root node, a
single split node, three diamond decision gates, and four terminal nodes of equal size.
Branches are neutral; no branch may look recommended or highlighted as correct. No text, no
numbers, no labels, no logos, no charts, no dashboard UI. Thin precise strokes, controlled
isometric depth, generous negative space, cobalt, cyan and warm accents. 3:2 composition,
calm and exact, readable on dark and light backgrounds.
```

### 18. STATISTICAL_DECISION_TREE — 3 / 2 — `statistical-decision-tree.webp`

Fungsi: decision tree terawasi dengan guard. Motif registry: `branching`.

```
Scientific editorial illustration of a guarded branching structure: a root node, a split
node, three diamond gates each preceded by a thin shield-like outline, and four terminal
nodes of equal size. The guard outlines read as constraints, not as approval stamps. No
text, no numbers, no labels, no logos, no badges, no charts. Thin precise strokes,
controlled isometric depth, generous negative space, cobalt and cyan accents. 3:2
composition, calm and exact, readable on dark and light backgrounds.
```

## Derivatif responsif

Belum ada derivatif. Bila master tersedia, derivatif hanya boleh berasal dari master yang
sama dan mempertahankan rasio slot; jumlah derivatif ditentukan setelah master diukur.
