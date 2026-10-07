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
| **Grade 1** | Low-Grade Earth (Tanah Kebun Biasa) | Tier 1 – 2 | Tanah subur umum, tidak ber-Qi murni. |
| **Grade 2** | Vermilion Wood Mud (Lumpur Kayu Vermilion) | Tier 3 – 4 | Wood Qi + Water Qi (*Vermilion Basin / Whispering Forest*). |
| **Grade 3** | Ashen Flame Soil (Tanah Abu Membara) | Tier 4 – 5 | Fire Qi + Sun Qi (*Ashen Sun Expanse*). |
| **Grade 4** | Frost Ice Mud (Lumpur Es Abadi) | Tier 5 – 6 | Ice Qi + Stillness Qi (*Frostglass Crown*). |
| **Grade 5** | Nine-Reed Toxic Silt (Endapan Rawa Beracun) | Tier 6 – 7 | Water Qi + Poison Qi (*Nine-Reed Mire*). |
| **Grade 6** | Astral Star Sand (Pasir Bintang Astral) | Tier 8 – 9 | Star Qi + Fate Qi (*Astral Tide Sea / Fate Scarlands*). |

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
- `BaseGrowthDays(Tier)`: Tier 1 = 3 Hari | Tier 2 = 7 Hari | Tier 3 = 15 Hari | Tier 4 = 30 Hari (1 Bulan) | Tier 5 = 90 Hari (3 Bulan) | Tier 6 = 270 Hari (9 Bulan / 1 Tahun Qianyuan) | Tier 7 = 3 Tahun | Tier 8 = 9 Tahun | Tier 9 = 27+ Tahun Qianyuan.
- `SoilMultiplier`: Tanah cocok = `0.8` | Tanah biasa = `1.0` | Tanah tidak cocok = `2.0` (risiko busuk).
- `CareEfficiencyMod`: Penyiraman air spiritual rutin & pupuk alkimia = `1.5`.

---

## 🌿 3. Klasifikasi Tier Herba Spiritual Qianyuan-World (Tier 1 – 9)

Herba spiritual di Benua Qianyuan memiliki tingkatan usia spiritual (*Spiritual Age*), konsentrasi Qi, dan kelangkaan tersendiri dari Tier 1 hingga Tier 9:

| Tier Herba | Usia Spiritual / Kematangan | Tingkat Kelangkaan | Kegunaan Utama Alkimia (`16`) |
|---|---|---|---|
| **Tier 1** | 1–10 Tahun | Common (Sangat Umum) | Salep obat luar, ramuan Stamina, & pembersih racun ringan. |
| **Tier 2** | 10–50 Tahun | Uncommon (Umum) | Pil pemulihan HP/Qi tingkat dasar & obat stamina petualang. |
| **Tier 3** | 50–100 Tahun | Rare (Jarang) | Pil penguat Dantian, pemurni darah, & salep organ dalam. |
| **Tier 4** | 100–300 Tahun | Very Rare (Sangat Jarang) | Bahan utama *Foundation Pill* & *Golden Core Pill* (`16`). |
| **Tier 5** | 300–500 Tahun | Epic (Langka) | Pil pemurni Inti Qi, penawar racun miasma berat, & obat jiwa. |
| **Tier 6** | 500–1.000 Tahun | Legendary (Sangat Langka) | Bahan utama *Soul Formation Pill* & penjelajah terobos Realm. |
| **Tier 7** | 1.000–3.000 Tahun | Purba / Ancient | Pil rekonstruksi Dantian hancur & penembus batas kehampaan. |
| **Tier 8** | 3.000–9.000 Tahun | Mythical / Transcendent | Bahan *Dao Integration Pill* & penarik pencerahan hukum benua. |
| **Tier 9** | 9.000+ Tahun | Celestial / Tribulation | Herba Mitos penahan petir Tribulasi Kesengsaraan Langit (`12`). |

---

## 🌐 4. Katalog Herba Spiritual Lintas Wilayah / Umum (Common Cross-Region Herbs)

Tanaman obat spiritual umum yang tumbuh subur di berbagai daratan, tepi jalan karavan, dan lembah perbukitan benua Qianyuan:

| Tier | Nama Herba Spiritual | Elemen Qi | Habitat Umum | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Embun Pagi (Morning Dew Grass)** | Water / Earth | Tepi padang rumput & ladang desa | Bahan obat penutup luka luar & pemulih Stamina ringan. |
| **T2** | **Akar Wangi Penenang (Fragrant Calming Root)** | Wood Qi | Perbukitan & pinggir hutan | Salep pereda nyeri otot & bahan pil penenang batin. |
| **T3** | **Bunga Giok Penyambung Tulang (Jade Bone Flower)** | Earth + Wood | Lereng gunung batu umum | Pembalut luka patah tulang (*Bone Fracture Trauma*) & salep Zirah. |
| **T4** | **Buah Merah Pemurni Darah (Blood Cleansing Berry)**| Wood + Water | Lembah subur benua | Bahan ramuan pemurni sirkulasi darah & peningkat HP Max. |
| **T5** | **Ginseng Lima Warna (Five-Element Ginseng)** | Multi-Element | Hutan tua terisolasi | Bahan pemurni Dantian & peningkat regenerasi Qi alami. |
| **T6** | **Teratai Perak Umur Panjang (Silver Longevity Lotus)**| Water + Ice | Danau pekat & mata air gunung | Bahan pil perpanjang usia (*Longevity Pill*) & penawar racun. |
| **T7** | **Jamur Lingzhi Purba Sembilan Warna** | Wood + Life Qi | Reruntuhan batu purba | Bahan rekonstruksi organ dalam hancur & terobos Realm. |
| **T8** | **Buah Jiwa Keabadian (Celestial Soul Fruit)** | Fate + Star Qi | Puncak gunung terisolasi benua | Bahan *Dao Integration Pill* & peningkat Focus murni. |
| **T9** | **Bunga Embun Langit Mitos (Heavenly Dew Blossom)**| Multi-Element | Celah terlarang benua | Herba mitos penahan sengatan petir Tribulasi Langit (`12`). |

---

## 📖 5. Katalog Herba Spiritual Spesifik per Wilayah (Tier 1–9)

---

### 4.1 Hama & Bencana Kebun (Pests & Diseases)
- **Serangga Pemakan Akar (Spirit Root Beetle)**: Menggerogoti akar tanaman spiritual. Memicu status *Withered* (penalti hasil panen -50%).
- **Miasma Jamur Busuk (Rot Spore Miasma)**: Infeksi jamur beracun yang menular antar-petak kebun. Memerlukan obat semprot herbal *Pesticide Spray* dari Alchemist.
- **Hama Tikus Penggali (Earth-Burrowing Rat)**: Menggerogoti umbi herba bawah tanah. Memerlukan formasi perangkap atau pembasmian manual.
### 🌊 5.1 Vermilion River Basin (`02` — Water + Wood Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Embun Sungai** | Tepi anak Sungai Vermilion | 3 Hari | Salep penyembuh pendarahan luar & pembersih racun air. |
| **T2** | **Ginseng Vermilion** | Ladang Desa Bunga Embun (`02`) | 7 Hari | Bahan utama *Foundation Pill* (Tier 2) & penyegar Qi. |
| **T3** | **Bunga Teratai Embun Giok** | Muara Pelabuhan Zhuque | 15 Hari | Bahan *Golden Core Pill* (Tier 3) & salep luka organ. |
| **T4** | **Buah Air Jernih (Clear Water Berry)**| Dermaga Tiga Muara | 30 Hari | Bahan ramuan penawar racun lumpur rawa & pemurni meridian. |
| **T5** | **Teratai Embun Merah (Crimson Stream Lotus)**| Lembah Embun Merah | 90 Hari | Bahan *Soul Refinement Pill* & pelindung Dantian. |
| **T6** | **Akar Sungai Purba (Ancient River Root)**| Gua Reruntuhan Kuil Air Purba | 270 Hari | Bahan pemurnian *Soul Formation Pill* & obat trauma dalam. |
| **T7** | **Teratai Air Abadi (Eternal Stream Water Lotus)**| Dasar Rawa Teratai Kelam | 3 Tahun | Bahan pil rekonstruksi Dantian & pemurni racun darah. |
| **T8** | **Bunga Arus Sembilan Muara** | Titik pusat konvergensi sungai | 9 Tahun | Bahan *Dao Integration Pill* berunsur Air Murni. |
| **T9** | **Mutiara Jiwa Teratai Vermilion Purba**| Mata air purba Lembah Embun Merah | 27+ Tahun | Herba mitos penyembuh kelumpuhan total & penahan petir. |

---

## 🌸 5. Katalog Lengkap Herba Spiritual Lintas Wilayah Qianyuan-World (Tier 1 s/d Tier 9)
### ⛰️ 5.2 Blackstone Skyreach (`03` — Earth + Metal Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Batu Hitam (Blackstone Grass)** | Tebing terjal Benteng Skyreach | 3 Hari | Bahan tempa pelapis baja & salep kulit tahan gesekan. |
| **T2** | **Akar Batu Hitam (Blackstone Root)** | Lereng Anvil Valley (`03`) | 7 Hari | Bahan campuran tempa senjata Cold Steel & Heavy Iron. |
| **T3** | **Bunga Besi Berat (Heavy Iron Blossom)**| Zona Luar Gua Tambang Kuno | 15 Hari | Bahan ramuan penguat tulang (*Bone Tempering Elixir*). |
| **T4** | **Kristal Tambang Emas (Gold Ore Herb)**| Zona Tengah Deep Steel | 30 Hari | Bahan pil penembus zirah (*Armor Piercing Pill*). |
| **T5** | **Teratai Besi Abadi (Eternal Iron Lotus)**| Zona Inti Core Magnet | 90 Hari | Bahan *Metal Core Pill* & pelindung raga keras. |
| **T6** | **Buah Inti Bumi (Earth Core Fruit)** | Gua Reruntuhan Tungku Purba | 270 Hari | Bahan *Soul Formation Pill* berunsur Pertahanan Raga. |
| **T7** | **Akar Bintang Magnetik Purba** | kedalaman 3.000m Gua Tambang | 3 Tahun | Bahan obat rekonstruksi Zirah Raga & pemurni Metal Qi. |
| **T8** | **Jamur Karang Batu Purba** | Ngarai Batu Hitam Kelam | 9 Tahun | Bahan *Dao Integration Pill* berunsur Earth Qi murni. |
| **T9** | **Buah Inti Gunung Hitam Mitos** | Puncak tertinggi Skyreach Citadel | 27+ Tahun | Herba mitos pelindung tubuh dari kehancuran fisik total. |

---

### 🏜️ 5.3 Ashen Sun Expanse (`04` — Fire + Sun Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Pasir Panas (Warm Sand Grass)**| Bukit pasir lepas luar oasis | 3 Hari | Salep penahan sengatan dingin & pemurni keringat. |
| **T2** | **Buah Pasir Emas (Ashen Berry)** | Kota Sunfire Oasis (`04`) | 7 Hari | Bahan *Fire Core Pill* & minyak penyegar dehidrasi. |
| **T3** | **Bunga Api Surya (Sunfire Flower)** | Benteng Sandgate Post | 15 Hari | Bahan ramuan penghangat Dantian & pemurni Fire Qi. |
| **T4** | **Buah Kristal Api Gurun (Flame Crystal Fruit)**| Pos Pengawas Sumur Batu | 30 Hari | Bahan pil peledak serangan elemen Api (*Fire Burst Pill*). |
| **T5** | **Teratai Api Pasir Merah (Red Sand Lotus)**| Lembah Pasir Merah Kelam | 90 Hari | Bahan *Sunfire Core Pill* & penawar racun es murni. |
| **T6** | **Akar Abu Membara (Ashen Flame Root)**| Reruntuhan Buried Sun Palace | 270 Hari | Bahan *Soul Formation Pill* berunsur Api Murni. |
| **T7** | **Bunga Matahari Purba (Ancient Sun Blossom)**| Gua Altar Api Purba | 3 Tahun | Bahan obat pemurni energi *Sun Qi* & rekonstruksi Dantian. |
| **T8** | **Teratai Api Surya Abadi** | Pusat kawah pasir panas gurun | 9 Tahun | Bahan *Dao Integration Pill* berunsur Fire Qi murni. |
| **T9** | **Mutiara Inti Api Surya Purba Mitos**| Dasar lautan pasir Ashen Sun | 27+ Tahun | Herba mitos pemurni energi surya penembus batas Realm. |

---

### 🌿 5.4 Nine-Reed Mire (`05` — Water + Poison Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Alang Rawa (Swamp Reed Grass)**| Tepi rawa Desa Mirewood | 3 Hari | Bahan penawar gatal & obat pendarahan rawa ringan. |
| **T2** | **Jamur Spora Rawa (Mire Spore Mushroom)**| Pos Rawa Beracun (`05`) | 7 Hari | Bahan salep luka luar & penawar racun miasma sedang. |
| **T3** | **Bunga Teratai Racun (Toxic Reed Lotus)**| Labirin Alang-Alang Sembilan | 15 Hari | Bahan racikan racun pelumpuh & pil *Poison Resistance*. |
| **T4** | **Anggrek Darah Rawa (Blood Orchid)**| Rawa Teratai Kelam | 30 Hari | Bahan obat racun murni & *Blood Renewal Pill*. |
| **T5** | **Jamur Miasma Hijau (Green Miasma Fungus)**| Gua Sarang Serangga Spiritual | 90 Hari | Bahan *Poison Core Pill* & emulsi racun korosif. |
| **T6** | **Akar Rawa Beracun Purba** | Reruntuhan Benteng Ular Purba | 270 Hari | Bahan *Soul Formation Pill* berunsur Poison Qi murni. |
| **T7** | **Teratai Darah Kelam Purba** | Kedalaman inti Rawa Sembilan | 3 Tahun | Bahan obat rekonstruksi pembuluh darah & racun Dantian. |
| **T8** | **Bunga Spora Miasma Purba** | Pusat sarang racun terlarang | 9 Tahun | Bahan *Dao Integration Pill* berunsur Water + Poison. |
| **T9** | **Buah Jiwa Teratai Racun Purba Mitos**| Titik simpul miasma Nine-Reed Mire | 27+ Tahun | Herba mitos penawar seluruh racun mematikan di benua. |

---

### 🌊 5.5 Astral Tide Sea (`06` — Water + Star Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Karang Bintang (Star Coral Grass)**| Pantai Kepulauan Coral | 3 Hari | Salep luka air garam & pemurni napas bawah laut. |
| **T2** | **Mutiara Laut Bintang (Star Herb)** | Pelabuhan Star-Compass (`06`)| 7 Hari | Bahan *Astral Navigation Essence* & obat penerang mata. |
| **T3** | **Bunga Cahaya Astral (Astral Light Blossom)**| Mercusuar Formasi Bintang | 15 Hari | Bahan ramuan peningkat Focus malam hari & perisai Qi. |
| **T4** | **Buah Bintang Samudra (Ocean Star Fruit)**| Benteng Pulau Coral | 30 Hari | Bahan *Star Core Pill* & obat pelindung tekanan air. |
| **T5** | **Teratai Bintang Karang (Star Coral Lotus)**| Zona Terumbu Karang Abyss | 90 Hari | Bahan *Astral Refinement Pill* & pemurni energi batin. |
| **T6** | **Akar Laut Bintang Purba** | Zona Arus Bintang Palung Abyss | 270 Hari | Bahan *Soul Formation Pill* berunsur Star Qi murni. |
| **T7** | **Kristal Bintang Samudra Purba** | Reruntuhan Sunken Citadel | 3 Tahun | Bahan obat penembus ilusi laut & rekonstruksi Dantian. |
| **T8** | **Bunga Rasi Bintang Purba** | Zona Palung Gelap kedalaman 2000m| 9 Tahun | Bahan *Dao Integration Pill* berunsur Star Qi murni. |
| **T9** | **Mutiara Bintang Sembilan Samudra Mitos**| Dasar Palung Bintang Bawah Laut | 27+ Tahun | Herba mitos pemanggil hujan cahaya bintang penembus batas. |

---

### 🌲 5.6 Whispering Root Forest (`07` — Wood + Life Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Dahan Hijau (Green Branch Grass)**| Zona Luar Kanopi Hutan | 3 Hari | Bahan balut luka dahan & salep pemulih Stamina. |
| **T2** | **Rumah Spora Hijau (Green Spore House)**| Desa Root-Bound (`07`) | 7 Hari | Salep luka luar & penawar racun miasma hutan. |
| **T3** | **Akar Kayu Serat Giok (Jade Wood Root)**| Wood-Heart Lodge | 15 Hari | Bahan ramuan pemulihan fisik & penguat serat otot. |
| **T4** | **Buah Vitalitas Hutan (Forest Vitality Fruit)**| Desa Lembah Spora Hijau | 30 Hari | Bahan *Life Renewal Pill* & pemulih HP masif instan. |
| **T5** | **Teratai Kehidupan Purba (Ancient Life Lotus)**| Ancient Tree Sanctuary | 90 Hari | Bahan *Wood Core Pill* & penyembuh trauma organ berat. |
| **T6** | **Kayu Serat Giok Abadi** | Reruntuhan Kuil Akar Purba | 270 Hari | Bahan *Soul Formation Pill* berunsur Life Qi murni. |
| **T7** | **Akar World Tree Purba** | Kedalaman World Tree Ancestor | 3 Tahun | Bahan obat rekonstruksi organ dalam & pemulih Dantian. |
| **T8** | **Buah Jiwa Kehidupan Hutan** | Inti Kanopi Hutan Purba | 9 Tahun | Bahan *Dao Integration Pill* berunsur Wood + Life Qi. |
| **T9** | **Bunga Embun World Tree Ancestor Mitos**| Puncak World Tree Ancestor | 27+ Tahun | Herba mitos pemurni kehidupan abadi & penahan Tribulasi. |

---

### ❄️ 5.7 Frostglass Crown (`08` — Ice + Stillness Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Es Gletser (Glacier Ice Grass)**| Lereng Desa Gletser Bening | 3 Hari | Salep pereda demam panas & penghangat batin dingin. |
| **T2** | **Bunga Teratai Salju Muda (Young Snow Lotus)**| Benteng Salju Frost-Edge (`08`)| 7 Hari | Bahan ramuan penahan hipotermia & pemurni Ice Qi. |
| **T3** | **Buah Kristal Es (Ice Crystal Fruit)** | Pos Pengawas Gletser Bening | 15 Hari | Bahan *Glacial Shield Pill* & obat pembeku darah. |
| **T4** | **Akar Es Abadi (Eternal Ice Root)** | Puncak Meditasi Keheningan | 30 Hari | Bahan *Stillness Mind Pill* & pelindung gangguan emosi. |
| **T5** | **Bunga Teratai Salju Purba (Snow Lotus)**| Gua Meditasi Es Abadi | 90 Hari | Bahan utama *Soul Refinement Pill* (Tier 5). |
| **T6** | **Bunga Keheningan Es (Stillness Ice Blossom)**| Gua Meditasi Inti Es Purba | 270 Hari | Bahan *Soul Formation Pill* berunsur Ice + Stillness Qi. |
| **T7** | **Kristal Teratai Es Abadi Purba** | Reruntuhan Menara Pedang Beku | 3 Tahun | Bahan obat pemurni Niat Pedang Es & rekonstruksi Dantian. |
| **T8** | **Buah Jiwa Gletser Purba** | Puncak gletser tertinggi Frostglass| 9 Tahun | Bahan *Dao Integration Pill* berunsur Ice Qi murni. |
| **T9** | **Mutiara Es Keheningan Abadi Mitos** | Dasar gletser abadi Frostglass Crown| 27+ Tahun | Herba mitos pembeku aliran waktu batin & penahan petir. |

---

### 🌪️ 5.8 Hollow Gale Corridor (`09` — Wind + Sound Qi)

| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Angin Ngarai (Canyon Wind Grass)**| Jembatan gantung tali ngarai | 3 Hari | Bahan minyak penyegar kelincahan *Movement Speed*. |
| **T2** | **Rumput Gema Angin (Echo Grass)** | Kota Wind-Gale (`09`) | 7 Hari | Bahan pembuatan *Echo Stone* komunikasi & obat telinga. |
| **T3** | **Buah Sayap Topan (Gale Wing Fruit)** | Pos Tebing Bisik | 15 Hari | Bahan *Wind Glide Pill* & peningkat respon refleks. |
| **T4** | **Bunga Suara Gema (Sonic Echo Blossom)** | Lembah Gema | 30 Hari | Bahan ramuan pemurni gelombang suara & penawar stun. |
| **T5** | **Teratai Angin Ngarai (Canyon Gale Lotus)**| Benteng Ngarai Gale Haven | 90 Hari | Bahan *Gale Core Pill* & pelindung dari gema merobek. |
| **T6** | **Akar Topan Purba (Ancient Gale Root)** | Gua Pemindai Suara Benua | 270 Hari | Bahan *Soul Formation Pill* berunsur Wind + Sound Qi. |
| **T7** | **Bunga Gema Suara Purba** | Gua Gema Suara Purba | 3 Tahun | Bahan obat penyembuh kerusakan gendang telinga & Focus. |
| **T8** | **Buah Kecepatan Angin Abadi** | Reruntuhan Menara Angin Purba | 9 Tahun | Bahan *Dao Integration Pill* berunsur Wind Qi murni. |
| **T9** | **Mutiara Badai Topan Purba Mitos** | Titik simpul badai angin ngarai | 27+ Tahun | Herba mitos pemanggil gelombang topan pelindung benua. |

---

### 🌀 5.9 Fate Scarlands (`10` — Fate + Mutated Qi)

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
| Tier | Nama Herba Spiritual | Habitat Utama Wilayah | Waktu Tumbuh | Kegunaan Alkimia (`16`) |
|---|---|---|---|---|
| **T1** | **Rumput Celah Ruang (Rift Space Grass)**| Perbatasan Pos Pengawas Scarlands| 3 Hari | Bahan minyak pelumas peralatan & pemurni disorientasi. |
| **T2** | **Buah Anomali Scar (Void Berry)** | Kemah Penjelajah Scarlands (`10`)| 7 Hari | Bahan *Spatial Anchor Pill* (Tier 2) & obat mata. |
| **T3** | **Bunga Mutasi Takdir (Fate Mutation Flower)**| Reruntuhan Kota Terbalik | 15 Hari | Bahan ramuan penstabil ilusi *Memory Erosion*. |
| **T4** | **Akar Belah Dimensi (Spatial Split Root)**| Celah Takdir Purba | 30 Hari | Bahan pil pelindung distorsi ruang (*Void Protection*). |
| **T5** | **Teratai Distorsi Ruang (Spatial Rift Lotus)**| Lembah Bayangan Terbalik | 90 Hari | Bahan *Fate Core Pill* & obat penyambung meridian. |
| **T6** | **Buah Waktu Chrono (Chrono Fruit)** | Celah Waktu Terisolasi | 270 Hari | Bahan *Soul Formation Pill* berunsur Fate + Time Qi. |
| **T7** | **Kristal Takdir Purba** | Inti Anomali Ruang Scarlands | 3 Tahun | Bahan obat rekonstruksi Dantian terdistorsi & Fate Qi. |
| **T8** | **Bunga Keretakan Takdir Abadi** | Puncak Celah Takdir Purba | 9 Tahun | Bahan *Dao Integration Pill* berunsur Fate Qi murni. |
| **T9** | **Mutiara Kehampaan Anomali Purba Mitos**| Pusat anomali utama Fate Scarlands | 27+ Tahun | Herba mitos penstabil keretakan dimensi ruang benua. |

---

## 🛡️ 6. Checklist Validasi AI GM (Wajib Dicek Setiap Siklus Kebun)

- [ ] Benih Tier 3+ memiliki riwayat asal-usul yang sah (*Seed Origin Log*)?
- [ ] Kualitas tanah (*Spirit Soil Grade*) sesuai dengan syarat elemen benih?
- [ ] Waktu pertumbuhan dihitung berdasarkan durasi kompresi in-game Qianyuan dengan menerapkan rumus `ActualGrowthDays` & `CatalysisMultiplier`?
- [ ] Akselerasi total dari cairan nutrisi, air spiritual, dan formasi tidak melebihi batas maksimal **4.0× Multiplier**?
- [ ] Jika melakukan Time-Skip Retret Kultivasi, pertumbuhan kebun dihitung bersamaan dengan durasi retret pemain?
- [ ] Hasil panen yang diperoleh dicatat ke log inventory beserta Quality Grade-nya?

Jika **salah satu** poin di atas meragukan → Proses Pertanian **DITOLAK TOTAL**. AI GM memberikan alasan teknis yang jelas kepada pemain.
