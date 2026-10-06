# 🌿 Qianyuan-World — XIX. Spirit Gardening System (Sistem Kebun & Budidaya Tanaman Spiritual)

> **Modul:** 18 — Spirit Gardening System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Growth-Time Realism — Soil & Element Aligned
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (peta jarak & arus Qi), `13_ECONOMY_MARKET_SYSTEM.md` (harga hasil panen herba), `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` (resep alkimia & bahan pil), `17_ROLES_PROFESSIONS_SYSTEM.md` (profesi Farmer/Petani Herbal)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Pertanian

Sistem Kebun Spiritual (*Spirit Gardening*) di Qianyuan-World mengatur budidaya, perawatan, persilangan mutasi (*Crossbreeding*), dan panen herba obat spiritual. Sistem ini merupakan fondasi utama pasokan bahan mentah bagi disiplin Alkimia (`16`) dan penopang ekonomi pertanian benua Qianyuan.

### Aturan Emas Anti-Cheat Pertanian (Mandatory Enforced Rules)
1. **Syarat Asal-Usul Benih (Seed Origin Log)**: Benih spiritual bernilai tinggi (**Tier 3+ / Grade Xuan ke atas**) wajib memiliki riwayat asal-usul (*Seed Origin Log*) dari hasil pencarian di wilayah liar, pembelian bursa, atau hadiah quest. Benih tanpa origin **TIDAK BISA** ditanam.
2. **Larangan Panen Instan**: Pertumbuhan tanaman spiritual terikat pada waktu dunia Qianyuan (Shichen/Hari/Bulan). Pemain **TIDAK BISA** memanen tanaman secara instan tanpa penggunaan cairan nutrisi alkimia (*Nutrient Liquid*) atau formasi percepatan yang tervalidasi.
3. **Kesesuaian Element Tanah & Qi**: Tanaman elemen tertentu (misal: Bunga Api) memerlukan *Spirit Soil* dan *Qi Density* yang selaras. Menanam di tanah yang tidak cocok menyebabkan pembusukan akar (*Root Rot*).
4. **Resiko Hama & Bencana Kebun**: Kebun yang ditinggal tanpa perawatan atau perlindungan formasi berisiko diserang serangga spiritual (*Spirit Pests*) atau infeksi jamur miasma.

---

## ⛰️ 1. Kategori Tanah Spiritual (Spirit Soil Grades & Element Affinities)

Kualitas tanah spiritual (*Spirit Soil*) menentukan batas Tier benih yang dapat tumbuh serta mempengaruhi kecepatan regenerasi hara kebun:

| Soil Grade | Nama Jenis Tanah | Batas Tier Benih | Kecocokan Elemen Qi Utama |
|---|---|---|---|
| **Grade 1** | **Low-Grade Earth (Tanah Kebun Biasa)** | Tier 1 – 2 | Tanah subur umum, tidak ber-Qi murni. |
| **Grade 2** | **Vermilion Wood Mud (Lumpur Kayu Vermilion)** | Tier 3 – 4 | Wood Qi + Water Qi (*Vermilion Basin / Whispering Forest*). |
| **Grade 3** | **Ashen Flame Soil (Tanah Abu Membara)** | Tier 4 – 5 | Fire Qi + Sun Qi (*Ashen Sun Expanse*). |
| **Grade 4** | **Frost Ice Mud (Lumpur Es Abadi)** | Tier 5 – 6 | Ice Qi + Stillness Qi (*Frostglass Crown*). |
| **Grade 5** | **Nine-Reed Toxic Silt (Endapan Rawa Beracun)** | Tier 6 – 7 | Water Qi + Poison Qi (*Nine-Reed Mire*). |
| **Grade 6** | **Astral Star Sand (Pasir Bintang Astral)** | Tier 8 – 9 | Star Qi + Fate Qi (*Astral Tide Sea / Fate Scarlands*). |

---

## ⏳ 2. Formula Waktu Tumbuh & Perawatan (Growth & Care Mechanics)

Pertumbuhan tanaman spiritual dihitung berdasarkan durasi waktu in-game Qianyuan:

```
GrowthDuration (Hari) = BaseGrowthDays(Tier) × SoilMultiplier × QiDensityMod / CareEfficiencyMod
```

- `BaseGrowthDays(Tier)`: Tier 1 = 3 Hari | Tier 2 = 7 Hari | Tier 3 = 15 Hari | Tier 4 = 30 Hari (1 Bulan) | Tier 5 = 90 Hari (3 Bulan) | Tier 6 = 270 Hari (9 Bulan / 1 Tahun Qianyuan) | Tier 7+ = 3+ Tahun Qianyuan.
- `SoilMultiplier`: Tanah cocok = `0.8` | Tanah biasa = `1.0` | Tanah tidak cocok = `2.0` (risiko busuk).
- `CareEfficiencyMod`: Penyiraman air spiritual rutin & pupuk alkimia = `1.5`.

---

## 🐝 3. Sistem Nutrisi, Air Spiritual, & Penyerbukan

1. **Penyiraman Air Spiritual (Spirit Water Nourishment)**:
   - Menyiram kebun dengan air gletser murni (*Melted Glacier Water*) atau air laut bintang meningkatkan *CareEfficiencyMod* sebesar `+25%`.
2. **Penggunaan Pupuk Alkimia (Nutrient Liquids — `16`)**:
   - Cairan nutrisi buatan Alchemist mampu memotong waktu tumbuh sebesar `20% s/d 50%` tergantung Grade cairan.
3. **Bantuan Serangga Penyerbuk (Spirit Bees Pollination)**:
   - Memelihara kawanan lebah spiritual (*Spirit Bees*) di sekitar kebun memberikan bonus *Flawless Harvest Quality* sebesar `+20%`.

---

## 🐛 4. Hama Spiritual, Miasma Jamur, & Mutasi Persilangan (Hybrid Crossbreeding)

### 4.1 Hama & Bencana Kebun (Pests & Diseases)
- **Serangga Pemakan Roots (Spirit Root Beetle)**: Menggerogoti akar tanaman spiritual. Memicu status *Withered* (penalti hasil panen -50%).
- **Miasma Jamur Busuk (Rot Spore Miasma)**: Infeksi jamur beracun yang menular antar-petak kebun. Memerlukan obat semprot herbal *Pesticide Spray* dari Alchemist.

### 4.2 Mutasi Persilangan (Hybrid Crossbreeding)
Menanam dua spesies herba berunsur elemen berbeda pada petak tanah bersilangan dengan bantuan *Nutrient Liquid Grade 3+* memicu peluang mutasi `15%`:
- *Contoh*: Vermilion Ginseng (Fire/Wood) + Snow Lotus (Ice) → **Mutiara Teratai Api Es (Hybrid Herb Tier 5)**.

---

## 🌸 5. Katalog 10 Tanaman Spiritual Khas Wilayah Qianyuan-World

*(Selaras dengan Data Canon Wilayah Modul `02`–`10` & Resep Alkimia `16`)*

| # | Nama Tanaman Spiritual | Tier Herb | Habitat Wilayah Utama | Kegunaan Utama Alkimia (`16`) |
|---|---|---|---|---|
| 1 | **Ginseng Vermilion** | Tier 2 | Vermilion River Basin (`02`) | Bahan utama *Foundation Pill* (Tier 2). |
| 2 | **Bunga Teratai Embun Giok** | Tier 3 | Vermilion River Basin (`02`) | Bahan *Golden Core Pill* (Tier 3). |
| 3 | **Rumah Spora Hijau** | Tier 2 | Whispering Root Forest (`07`)| Salep luka luar & penawar racun miasma. |
| 4 | **Bunga Teratai Salju (Snow Lotus)**| Tier 5 | Frostglass Crown (`08`) | Bahan *Soul Refinement Pill* (Tier 5). |
| 5 | **Bunga Anggrek Darah Rawa** | Tier 4 | Nine-Reed Mire (`05`) | Bahan obat racun & *Blood Renewal Pill*. |
| 6 | **Buah Pasir Emas (Ashen Berry)** | Tier 3 | Ashen Sun Expanse (`04`) | Bahan *Fire Core Pill* & minyak penyegar. |
| 7 | **Rumput Gema Angin (Echo Grass)** | Tier 2 | Hollow Gale Corridor (`09`) | Bahan pembuatan *Echo Stone* komunikasi. |
| 8 | **Mutiara Laut Bintang (Star Herb)**| Tier 4 | Astral Tide Sea (`06`) | Bahan *Astral Navigation Essence*. |
| 9 | **Akar Batu Hitam (Blackstone Root)**| Tier 3 | Blackstone Skyreach (`03`) | Bahan campuran tempa senjata Cold Steel. |
| 10| **Buah Anomali Scar (Void Berry)** | Tier 7 | Fate Scarlands (`10`) | Bahan *Spatial Anchor Pill* (Tier 7). |

---

## 🛡️ 6. Checklist Validasi AI GM (Wajib Dicek Setiap Siklus Kebun)

- [ ] Benih Tier 3+ memiliki riwayat asal-usul yang sah (*Seed Origin Log*)?
- [ ] Kualitas tanah (*Spirit Soil Grade*) sesuai dengan syarat elemen benih?
- [ ] Waktu pertumbuhan dihitung jujur berdasarkan durasi in-game Qianyuan (Shichen/Hari/Bulan)?
- [ ] Penggunaan cairan percepatan panen tervalidasi dari inventory Alchemist (`16`)?
- [ ] Hasil panen yang diperoleh dicatat ke log inventory beserta Quality Grade-nya?

Jika **salah satu** poin di atas meragukan → Proses Pertanian **DITOLAK TOTAL**. AI GM memberikan alasan teknis yang jelas kepada pemain.
