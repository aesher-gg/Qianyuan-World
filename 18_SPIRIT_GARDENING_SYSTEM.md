# 🌿 Qianyuan-World — XIX. Spirit Gardening System (Sistem Kebun & Budidaya Tanaman Spiritual)

> **Modul:** 18 — Spirit Gardening System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Growth-Time Realism — Soil & Element Aligned
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak & time-skip), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (peta jarak & arus Qi), `13_ECONOMY_MARKET_SYSTEM.md` (harga hasil panen herba), `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` (resep alkimia & bahan pil), `17_ROLES_PROFESSIONS_SYSTEM.md` (profesi Farmer/Petani Herbal)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Pertanian

Sistem Kebun Spiritual (*Spirit Gardening*) di Qianyuan-World mengatur budidaya, perawatan, persilangan mutasi (*Crossbreeding*), dan panen herba obat spiritual. Sistem ini merupakan fondasi utama pasokan bahan mentah bagi disiplin Alkimia (`16`) dan penopang ekonomi pertanian benua Qianyuan.

### Aturan Emas Anti-Cheat Pertanian (Mandatory Enforced Rules)
1. **Syarat Asal-Usul Benih (Seed Origin Log)**: Benih spiritual bernilai tinggi (**Tier 3+ / Grade Xuan ke atas**) wajib memiliki riwayat asal-usul (*Seed Origin Log*) dari hasil pencarian di wilayah liar, pembelian bursa, atau hadiah quest. Benih tanpa origin **TIDAK BISA** ditanam.
2. **Larangan Panen Instan**: Pertumbuhan tanaman spiritual terikat pada waktu dunia Qianyuan (Shichen/Hari/Bulan). Pemain **TIDAK BISA** memanen tanaman secara instan tanpa penggunaan cairan nutrisi alkimia (*Nutrient Liquid*) atau formasi percepatan yang tervalidasi.
3. **Kesesuaian Element Tanah & Qi**: Tanaman elemen tertentu (misal: Bunga Api) memerlukan *Spirit Soil* dan *Qi Density* yang selaras. Menanam di tanah yang tidak cocok menyebabkan pembusukan akar (*Root Rot*).
4. **Resiko Hama & Bencana Kebun**: Kebun yang ditinggal tanpa perawatan atau perlindungan formasi berisiko diserang serangga spiritual (*Spirit Pests*) atau infeksi jamur miasma.
5. **Akselerasi Tervalidasi & Integrasi Time-Skip**: Semua bentuk percepatan tumbuh (Cairan Nutrisi, Formasi, Air Spiritual, dan Time-Skip Retret Kultivasi AI GM) wajib dihitung menggunakan formula *Spirit Catalysis* yang transparan.

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

## ⏳ 2. Formula Masa Tumbuh & Akselerasi (Growth & Catalysis Mechanics)

Pertumbuhan tanaman spiritual dihitung berdasarkan durasi waktu terkompresi in-game Qianyuan, dikombinasikan dengan mekanisme *Spirit Catalysis* (Akselerasi Katalis Qi):

```
ActualGrowthDays = BaseGrowthDays(Tier) × SoilMultiplier × EnvironmentMod / CatalysisMultiplier
```

### 2.1 Durasi Dasar Pertumbuhan (Base Growth Days per Tier)

| Tier Herba | Base Growth Days (Durasi Dasar) | Syarat Minimum Spirit Soil Grade | Syarat Khusus Tambahan |
|---|---|---|---|
| **Tier 1** | **1 – 2 Hari** | Grade 1 (Low-Grade Earth) | Tidak ada |
| **Tier 2** | **3 – 5 Hari** | Grade 1 (Low-Grade Earth) | Tidak ada |
| **Tier 3** | **7 – 10 Hari** | Grade 2 (Vermilion Wood Mud) | Kepadatan Qi Lokal ≥ 1.0× |
| **Tier 4** | **15 – 20 Hari** | Grade 2 (Vermilion Wood Mud) | Kepadatan Qi Lokal ≥ 1.2× |
| **Tier 5** | **30 Hari (1 Bulan Qianyuan)** | Grade 3 / Grade 4 Soil | Formasi Pengumpul Qi Grade 2+ |
| **Tier 6** | **60 – 90 Hari (2–3 Bulan)** | Grade 4 / Grade 5 Soil | Keselarasan Elemen Wilayah Murni |
| **Tier 7** | **120 – 180 Hari (4–6 Bulan)** | Grade 5 Soil | Syarat Anomali Lingkungan Khusus (Anomali Miasma/Gletser) |
| **Tier 8** | **180 – 270 Hari (6–9 Bulan)** | Grade 6 (Astral Star Sand) | Formasi Akselerasi Bintang + Ritual Qi |
| **Tier 9** | **270 Hari (1 Tahun Qianyuan)** | Grade 6 (Astral Star Sand) | Resonansi Hukum Dao & Segel Perlindungan |

### 2.2 Faktor Modifikator Pertumbuhan

- **SoilMultiplier**:
  - Tanah Selaras (Matching Element Soil): `0.8`
  - Tanah Netral (Standard Soil): `1.0`
  - Tanah Tidak Cocok (Mismatched Element): `2.0` (Plus risiko pembusukan akar *Root Rot* 30% per Shichen).
- **EnvironmentMod**:
  - Di dalam Wilayah Asal / Habitat Alami: `0.85`
  - Di luar Wilayah Asal tanpa Formasi Penyesuai: `1.3`

---

## 🧪 3. Sistem Katalis Pertumbuhan (Spirit Catalysis & Care Systems)

Guna menghindari durasi penantian real-time yang terlalu lama dalam roleplay, pemain dapat mengombinasikan berbagai metode percepatan (*Catalysis Factors*):

```
CatalysisMultiplier = 1.0 + AirSpiritualMod + NutrientLiquidMod + FormationMod + WorkerMod
```

### 3.1 Penyiraman Air Spiritual (Spirit Water Nourishment)
- **Air Sungai Vermilion / Air Hujan Murni**: `+0.15` (Memotong waktu ~13%).
- **Air Gletser Abadi / Air Laut Bintang**: `+0.25` (Memotong waktu ~20%).

### 3.2 Cairan Nutrisi Alkimia (Nutrient Liquids — `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md`)
- **Nutrient Liquid Grade 1 (Cairan Nutrisi Dasar)**: `+0.25`
- **Nutrient Liquid Grade 2 (Cairan Nutrisi Menengah)**: `+0.50`
- **Nutrient Liquid Grade 3 (Cairan Nutrisi Unggul)**: `+0.80`
- **Nutrient Liquid Grade 4 (Cairan Nutrisi Esensial)**: `+1.20`
- **Nutrient Liquid Grade 5 (Cairan Nutrisi Murni Agung)**: `+1.80`

*(Catatan: Pemberian Cairan Nutrisi maksimal 1 kali per fase pertumbuhan tanaman untuk mencegah keracunan aura / Over-Nourishment).*

### 3.3 Formasi Percepatan Kebun (Spirit Acceleration Array — `16`)
- **Formasi Pengumpul Qi Kebun Grade 1–2**: `+0.30`
- **Formasi Pengumpul Qi Kebun Grade 3–4**: `+0.60`
- **Formasi Pengumpul Qi Kebun Grade 5+**: `+1.00`

### 3.4 Bantuan Serangga Penyerbuk & Petani Ahli (Spirit Bees & Caretaker)
- **Koloni Lebah Spiritual (Spirit Bees Pollination)**: `+0.20` + Bonus Kualitas Hasil Panen *Flawless Quality* `+20%`.
- **Petani Herbal Berprofesi Farmer (Role `17`)**: `+0.10` per tingkat Profesi Farmer.

> 💡 **Batas Maksimal Akselerasi Total**: Kombinasi seluruh katalis di atas dibatasi maksimal **4.0× Multiplier** (Memotong durasi hingga **75% dari waktu dasar**). Contoh: Herba Tier 5 (30 hari dasar) dengan akselerasi penuh dapat dipanen hanya dalam **7.5 hari**.

### 3.5 Integrasi Otomatis Time-Skip Retret Kultivasi AI GM
Sesuai aturan `00_CORE_RULES_AI_GM.md` §1.8, saat pemain melakukan retret kultivasi murni (skip waktu hingga 1 bulan per prompt):
- Pertumbuhan seluruh tanaman spiritual di kebun milik pemain **otomatis berjalan secara simultan** sesuai durasi retret.
- AI GM wajib menghitung akumulasi kemajuan tumbuh tanaman dan mengecek status kebun (pemberian nutrisi otomatis jika ada penjaga kebun/formasi otomatis, atau risiko hama jika kebun ditinggalkan tanpa perlindungan).

---

## 🐛 4. Hama Spiritual, Miasma Jamur, & Mutasi Persilangan (Hybrid Crossbreeding)

### 4.1 Hama & Bencana Kebun (Pests & Diseases)
- **Serangga Pemakan Akar (Spirit Root Beetle)**: Menggerogoti akar tanaman spiritual. Memicu status *Withered* (penalti hasil panen -50%).
- **Miasma Jamur Busuk (Rot Spore Miasma)**: Infeksi jamur beracun yang menular antar-petak kebun. Memerlukan obat semprot herbal *Pesticide Spray* dari Alchemist.
- **Hama Tikus Penggali (Earth-Burrowing Rat)**: Menggerogoti umbi herba bawah tanah. Memerlukan formasi perangkap atau pembasmian manual.

### 4.2 Mutasi Persilangan (Hybrid Crossbreeding)
Menanam dua spesies herba berunsur elemen berbeda pada petak tanah bersilangan dengan bantuan *Nutrient Liquid Grade 3+* memicu peluang mutasi `15%`:
- *Contoh*: Vermilion Ginseng (Fire/Wood) + Snow Lotus (Ice) → **Mutiara Teratai Api Es (Hybrid Herb Tier 5)**.

---

## 🌸 5. Katalog Lengkap Herba Spiritual Lintas Wilayah Qianyuan-World (Tier 1 s/d Tier 9)

*(Selaras dengan Data Canon Wilayah Modul `02`–`10` & Resep Alkimia `16`)*

---

### 🌐 5.0 Herba Umum Lintas Wilayah (Cross-Region Common Herbs)

Herba yang dapat ditemukan atau dibudidayakan di sebagian besar wilayah benua Qianyuan.

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Gale Grass (Rumput Angin)** | Tier 1 | Padang rumput umum (Wind Qi) | Bahan dasar *Basic Qi Pill* & ramuan stamina | Grade 1 Soil, mudah tumbuh |
| 2 | **Water Dew Flower (Bunga Embun Air)** | Tier 1 | Tepi sungai & danau (Water Qi) | Bahan *Basic Qi Pill* & salep pembersih luka | Grade 1 Soil, menyukai penyiraman air murni |
| 3 | **Spirit Iron Herb (Rumput Besi Jiwa)** | Tier 2 | Tepi perbukitan cadas (Metal Qi) | Bahan salep penguat kulit & campuran jimat | Grade 1 Soil, membutuhkan abu logam |
| 4 | **Sun-Dew Blossom (Bunga Embun Matahari)** | Tier 2 | Lembah terbuka hangat (Sun Qi) | Bahan ramuan penghangat & pil pemulih fokus | Grade 1 Soil, butuh paparan sinar matahari |
| 5 | **Five-Element Vine (Akar Akar Lima Elemen)** | Tier 3 | Hutan lebat campuran (All Elements) | Bahan *Universal Meridian Pill* & tali jimat | Grade 2 Soil, butuh pupuk lima elemen |
| 6 | **Spirit Purifying Lotus (Teratai Pemurni Spirit)**| Tier 4 | Danau pegunungan murni (Clear Qi) | Bahan *Soul Cleansing Pill* & penawar racun | Grade 2 Soil + Air Gletser Murni |

---

### 🌊 5.1 Vermilion River Basin (Lembah Sungai Vermilion — `02`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Vermilion Ginseng (Ginseng Merah)** | Tier 2 | Tepian sungai Vermilion (Wood/Fire Qi) | Bahan utama *Foundation Pill* (Tier 2) | Grade 2 Soil (Vermilion Wood Mud) |
| 2 | **Jade Dewflower (Bunga Embun Giok)** | Tier 3 | Rawa lembah Vermilion (Water Qi) | Bahan utama *Golden Core Pill* (Tier 3) | Grade 2 Soil + Penyiraman Air Sungai |
| 3 | **Red Lantern Blossom (Bunga Lentera Merah)** | Tier 1 | Ladang pedesaan Vermilion (Fire Qi) | Bahan pil penerang malam & salep luka hangat | Grade 1 Soil, mudah beradaptasi |
| 4 | **River Willow Root (Akar Dedalu Sungai)** | Tier 4 | Dasar delta sungai (Water/Wood Qi) | Bahan *River Resilience Pill* & penguat lambung kapal | Grade 2 Soil + Formasi Saluran Air |
| 5 | **Vermilion Lotus of Life (Teratai Merah Kehidupan)** | Tier 6 | Hulu rawa tua Vermilion (Wood/Life Qi) | Bahan *Life Extension Pill* & regenerasi organ | Grade 4 Soil + Air Murni Suci |
| 6 | **Grand Vermilion Dragon Stem (Batang Naga Vermilion)**| Tier 8 | Inti Mata Air Vermilion (Fire/Wood/Fate Qi) | Bahan *Immortal Foundation Essence* (Tier 8) | Grade 6 Soil + Resonansi Arus Sungai Utama |

---

### ⛰️ 5.2 Blackstone Skyreach (Pegunungan Skyreach — `03`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Blackstone Root (Akar Batu Hitam)** | Tier 3 | Cadas jurang Skyreach (Earth/Metal Qi) | Bahan campuran tempa *Cold Steel Armor* & pil ketahanan | Grade 2 Soil + Abu Mineral Logam |
| 2 | **Ironclad Lichen (Lumut Zirah Besi)** | Tier 1 | Dinding tebing terik (Earth Qi) | Salep pengeras kulit & penambal retakan zirah | Grade 1 Soil, menyukai tempat kering |
| 3 | **Skyreach Cloud Moss (Lumut Awan Skyreach)** | Tier 2 | Puncak tebing berkabut (Wind/Earth Qi) | Bahan *Cloud Foot Pill* (Kecepatan Gerak) | Grade 1 Soil + Uap Kabut Pagi |
| 4 | **Titan Ore Fungus (Jamur Bijih Titan)** | Tier 5 | Gua tambang dalam (Metal/Earth Qi) | Bahan *Titan Strength Pill* & campuran peleburan emas | Grade 3 Soil + Lingkungan Lemab Gua |
| 5 | **Gale-Edge Blossom (Bunga Belati Runcing)** | Tier 4 | Celah angin puncak Skyreach (Metal/Wind Qi) | Bahan pelapis mata pedang & *Sharpness Talisman Ink* | Grade 2 Soil + Terpaan Angin Kencang |
| 6 | **Skyreach Earth-Core Ginseng (Ginseng Inti Earth Skyreach)**| Tier 7 | Inti kedalaman tebing Skyreach (Earth/Fate Qi) | Bahan *Earth Core Breakthrough Pill* (Tier 7) | Grade 5 Soil + Tekanan Beban Bebatu |

---

### 🏜️ 5.3 Ashen Sun Expanse (Gurun Pasir Ashen Sun — `04`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Ashen Berry (Buah Pasir Emas)** | Tier 3 | Oase gurun Ashen Sun (Fire/Sun Qi) | Bahan *Fire Core Pill* & minyak penyegar stamina | Grade 3 Soil (Ashen Flame Soil) |
| 2 | **Sunfire Cactus (Kaktus Api Matahari)** | Tier 2 | Buana pasir terik (Fire Qi) | Penawar racun dingin & bahan minyak pelumas senjata | Grade 1 Soil + Panas Terik Cahaya |
| 3 | **Scorched Sand Vine (Akar Pasir Hangus)** | Tier 1 | Bukit pasir geser (Earth/Fire Qi) | Bahan tali peningkat cengkeraman & salep memar | Grade 1 Soil, sangat tahan kering |
| 4 | **Solar Bloom Rose (Mawar Surya Abadi)** | Tier 5 | Kawah pasir pijar (Sun/Fire Qi) | Bahan *Solar Refinement Pill* & elixir pemurni Dantian | Grade 3 Soil + Formasi Cermin Surya |
| 5 | **Blazing Flame Orchid (Anggrek Kobaran Api)** | Tier 4 | Retakan batu magma (Fire Qi) | Bahan *Flame Burst Talisman Ink* & pil kekebalan api | Grade 3 Soil + Abu Volkanik |
| 6 | **Ashen Sun Phoenix Fruit (Buah Phoenix Ashen Sun)**| Tier 8 | Inti Gurun Pasir Pijar (Fire/Sun/Fate Qi) | Bahan *Phoenix Rebirth Elixir* (Pemulihan Mati Suri) | Grade 6 Soil + Resonansi Panas Ekstrem |

---

### 🐸 5.4 Nine-Reed Mire (Rawa-Rawa Beracun Nine-Reed — `05`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Mire Blood Orchid (Anggrek Darah Rawa)** | Tier 4 | Rawa dalam Nine-Reed (Water/Poison Qi) | Bahan obat racun & *Blood Renewal Pill* | Grade 5 Soil (Nine-Reed Toxic Silt) |
| 2 | **Toxic Reed Sprout (Tunas Buluh Beracun)** | Tier 1 | Pinggiran perairan rawa (Poison Qi) | Bahan dasar racun panah & pil pemicu muntah | Grade 1 Soil, butuh air rawa |
| 3 | **Gloom-Shroom (Jamur Keheningan Rawa)** | Tier 2 | Bawah pepohonan lapuk rawa (Water/Poison Qi) | Bahan *Drowsiness Powder* & penenang jiwa | Grade 1 Soil + Miasma Ringan |
| 4 | **Nine-Toxic Nightshade (Kecubung Sembilan Racun)**| Tier 5 | Rawa tenggelam tua (Poison/Dark Qi) | Bahan *Corrosive Poison Pill* & pelarut zirah | Grade 5 Soil + Uap Miasma Pekat |
| 5 | **Purifying Mire Reed (Buluh Pemurni Rawa)** | Tier 3 | Pulau kecil tengah rawa (Water/Wood Qi) | Bahan penawar racun rawa & obat gangguan usus | Grade 2 Soil + Air Rawa Murni |
| 6 | **Hydra Poison Vine (Akar Racun Hydra Sembilan Kepala)**| Tier 7 | Inti Rawa Mati (Poison/Water/Fate Qi) | Bahan *Nine-Toxins Soul Severing Pill* (Tier 7) | Grade 5 Soil + Konsentrasi Miasma Abadi |

---

### 🌌 5.5 Astral Tide Sea (Lautan & Kepulauan Astral — `06`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Star Herb (Mutiara Laut Bintang)** | Tier 4 | Terumbu karang dangkal (Water/Star Qi) | Bahan *Astral Navigation Essence* & pil konsentrasi | Grade 6 Soil (Astral Star Sand) |
| 2 | **Tide Kelp (Rumput Laut Arus Astral)** | Tier 1 | Pantai kepulauan Astral (Water Qi) | Pakan lezat beast air & bahan obat pembersih darah | Grade 1 Soil + Air Laut Bergaram |
| 3 | **Moonlit Coral Blossom (Bunga Karang Rembulan)**| Tier 3 | Karang dalam malam hari (Star/Water Qi) | Bahan *Moonlight Clarity Pill* (Fokus & Batin) | Grade 2 Soil + Cahaya Rembulan |
| 4 | **Astral Tide Algae (Ganggang Pasang Astral)** | Tier 2 | Tepi ceruk pulau astral (Water/Star Qi) | Bahan tinta jimat pelindung ombak & obat pusing | Grade 1 Soil + Air Laut Astral |
| 5 | **Starlight Lotus (Teratai Cahaya Bintang)** | Tier 6 | Danau kawah pulau astral (Star Qi) | Bahan *Astral Breakthrough Pill* & pemurni Dantian | Grade 6 Soil + Formasi Pengumpul Bintang |
| 6 | **Celestial Astral Sea-Core Blossom (Bunga Inti Laut Astral)**| Tier 9 | Inti Palung Laut Astral (Water/Star/Fate Qi) | Bahan *Immortal Ascension Pill* (Tier 9) | Grade 6 Soil + Cahaya Rasi Bintang Murni |

---

### 🌲 5.6 Whispering Root Forest (Hutan Purba Whispering Root — `07`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Green Spore House (Rumah Spora Hijau)** | Tier 2 | Bawah pohon purba (Wood/Life Qi) | Salep luka luar & penawar racun miasma | Grade 1 Soil + Kelembapan Hutan |
| 2 | **Whispering Moss (Lumut Bisikan Hutan)** | Tier 1 | Batang pohon tua (Wood/Sound Qi) | Bahan obat pereda ketulian & jimat pendengar | Grade 1 Soil + Kelembapan Tinggi |
| 3 | **Root-Heart Ginseng (Ginseng Teras Akar)** | Tier 4 | Inti akar pohon purba (Wood/Life Qi) | Bahan *Life Essence Pill* & pemulihan Vitalitas | Grade 2 Soil (Vermilion Wood Mud) |
| 4 | **Wood-Spirit Treant Flower (Bunga Spirit Treant)**| Tier 3 | Pelepah pohon raksasa (Wood Qi) | Bahan *Wood Resonant Pill* & pakan beast kayu | Grade 2 Soil + Pupuk Kayu Lapuk |
| 5 | **Ancient Life Tree Sapling (Tunas Pohon Hayat Kuno)**| Tier 7 | Pusat Hutan Whispering (Wood/Life/Fate Qi) | Bahan *Soul Restoration Pill* & penumbuh organ | Grade 5 Soil + Uap Life Qi Murni |
| 6 | **Myriad-Year Whispering Root (Akar Bisikan Purba Sejuta Tahun)**| Tier 9 | Kedalaman Inti Hutan Purba (Wood/Fate Qi) | Bahan *Dao Integration Essence Pill* (Tier 9) | Grade 6 Soil + Resonansi Roh Hutan |

---

### ❄️ 5.7 Frostglass Crown (Pegunungan Salju Frostglass — `08`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Snow Lotus (Bunga Teratai Salju)** | Tier 5 | Puncak gletser abadi (Ice/Stillness Qi) | Bahan *Soul Refinement Pill* (Tier 5) | Grade 4 Soil (Frost Ice Mud) |
| 2 | **Frost Pine Needle (Jarum Pinus Salju)** | Tier 1 | Lereng bawah Frostglass (Ice Qi) | Bahan teh penyegar fokus & minyak gosok hening | Grade 1 Soil + Suhu Dingin |
| 3 | **Glacier Orchid (Anggrek Gletser Es)** | Tier 3 | Ceruk es puncak pegunungan (Ice Qi) | Bahan *Ice Resistance Pill* & pelapis pedang es | Grade 4 Soil + Air Es Murni |
| 4 | **Crystal Frost Plum (Bunga Plum Kristal Es)** | Tier 4 | Lereng terjal Frostglass (Ice/Stillness Qi) | Bahan *Mind Freezing Pill* & obat penenang amarah | Grade 4 Soil + Suhu Beku Ekstrem |
| 5 | **Eternal Cold-Marrow Fungus (Jamur Sumsum Dingin)**| Tier 6 | Dinding gua gletser abadi (Ice/Stillness Qi) | Bahan *Cold Core Breakthrough Pill* (Tier 6) | Grade 4 Soil + Pembekuan Lingkungan |
| 6 | **Absolute Zero Glacial Plum (Plum Es Nol Mutlak)**| Tier 8 | Inti Puncak Gletser Frostglass (Ice/Fate Qi) | Bahan *Heavenly Tribulation Shield Pill* (Tier 8) | Grade 6 Soil + Suhu Pembekuan Jiwa |

---

### 🌪️ 5.8 Hollow Gale Corridor (Koridor Ngarai Angin Hollow Gale — `09`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Echo Grass (Rumput Gema Angin)** | Tier 2 | Ngarai angin Hollow Gale (Wind/Sound Qi) | Bahan pembuatan *Echo Stone* komunikasi | Grade 1 Soil + Terpaan Angin |
| 2 | **Gale-Spur Blossom (Bunga Duri Angin Topan)** | Tier 1 | Tebing ngarai berbatu (Wind Qi) | Bahan obat penyegar nafas & ramuan kelincahan | Grade 1 Soil, menyukai tempat tinggi |
| 3 | **Sound-Echo Fern (Paku-Pakuan Gema Suara)** | Tier 3 | Gua ngarai bergema (Sound/Wind Qi) | Bahan *Sonic Disruption Powder* & jimat tuli | Grade 2 Soil + Resonansi Suara |
| 4 | **Feather-Wind Vine (Akar Bulu Angin)** | Tier 4 | Gelatan tebing ngarai (Wind Qi) | Bahan *Feather Body Pill* (Penyeringan Bobot) | Grade 2 Soil + Aliran Angin Deras |
| 5 | **Hollow Wind Lotus (Teratai Angin Kehampaan)** | Tier 6 | Inti pusaran ngarai angin (Wind/Void Qi) | Bahan *Wind Severing Pill* & jimat teleportasi pendek | Grade 5 Soil + Formasi Pusaran Angin |
| 6 | **Nine-Gale Tempest Blossom (Bunga Badai Sembilan Angin)**| Tier 7 | Puncak Pusaran Ngarai Utama (Wind/Sound/Fate Qi)| Bahan *Tempest Breakthrough Pill* (Tier 7) | Grade 5 Soil + Terpaan Badai Angin Topan |

---

### 🔮 5.9 Fate Scarlands (Wilayah Anomali Fate Scarlands — `10`)

| # | Nama Tanaman Spiritual | Tier | Habitat & Elemen Qi | Kegunaan Utama Alkimia & Crafting (`16`) | Syarat Tanah & Akselerasi Khusus |
|---|---|---|---|---|---|
| 1 | **Void Berry (Buah Anomali Scar)** | Tier 7 | Zona distorsi Fate Scarlands (Fate/Void Qi) | Bahan *Spatial Anchor Pill* (Tier 7) | Grade 6 Soil (Astral Star Sand) |
| 2 | **Scar Weaved Grass (Rumput Tenun Takdir)** | Tier 2 | Perbatasan Fate Scarlands (Fate Qi) | Bahan *Fate Anchoring Talisman Ink* | Grade 1 Soil + Distorsi Ringan |
| 3 | **Distortion Blossom (Bunga Distorsi Ruang)** | Tier 4 | Zone retakan Fate Scarlands (Void/Fate Qi) | Bahan *Spatial Concealment Powder* | Grade 6 Soil + Anomali Ruang |
| 4 | **Memory-Erosion Mushroom (Jamur Pengikis Ingatan)**| Tier 3 | Kawah anomali Scarlands (Fate Qi) | Bahan obat penenang emosi & racun pemudar ingatan | Grade 2 Soil + Miasma Distorsi |
| 5 | **Fate-Rewind Lily (Bunga Bakung Pembalik Takdir)**| Tier 8 | Inti Anomali Retakan Ruang (Fate Qi) | Bahan *Fate Reversal Pill* (Menetralkan Backlash) | Grade 6 Soil + Resonansi Garis Takdir |
| 6 | **Chaos Void World-Tree Seedling (Benih Pohon Dunia)**| Tier 9 | Inti Kedalaman Anomali Ruang (Fate/Void Qi) | Bahan *Immortal Ascension Pill* & Pusaka Dunia | Grade 6 Soil + Segel Ruang Hampa |

---

## 🛡️ 6. Checklist Validasi AI GM (Wajib Dicek Setiap Siklus Kebun)

- [ ] Benih Tier 3+ memiliki riwayat asal-usul yang sah (*Seed Origin Log*)?
- [ ] Kualitas tanah (*Spirit Soil Grade*) sesuai dengan syarat elemen benih?
- [ ] Waktu pertumbuhan dihitung berdasarkan durasi kompresi in-game Qianyuan dengan menerapkan rumus `ActualGrowthDays` & `CatalysisMultiplier`?
- [ ] Akselerasi total dari cairan nutrisi, air spiritual, dan formasi tidak melebihi batas maksimal **4.0× Multiplier**?
- [ ] Jika melakukan Time-Skip Retret Kultivasi, pertumbuhan kebun dihitung bersamaan dengan durasi retret pemain?
- [ ] Hasil panen yang diperoleh dicatat ke log inventory beserta Quality Grade-nya?

Jika **salah satu** poin di atas meragukan → Proses Pertanian **DITOLAK TOTAL**. AI GM memberikan alasan teknis yang jelas kepada pemain.
