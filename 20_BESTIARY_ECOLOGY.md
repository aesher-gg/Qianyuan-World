# 🐺 Qianyuan-World — XXI. Bestiary & Ecology (Database Ekologi, Monster, & Spirit Beast)

> **Modul:** 20 — Bestiary Ecology
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Strict Formula Scaling — Terintegrasi dengan Sistem Hukum, HP, & Pertarungan
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01`–`10` (modul regional), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap sebagai basis stats), `13_ECONOMY_MARKET_SYSTEM.md` (loot & grade value), `15_COMBAT_TACTICAL_SYSTEM.md` (resolusi pertempuran), `19_BEAST_BOND_SYSTEM.md` (penjinakan & kontrak)

---

## 🧭 0. Filosofi Sistem & Aturan Emas Anti-Cheat

Pertarungan di alam liar Qianyuan-World harus terasa berbahaya, taktis, dan adil bagi **SEMUA** pihak — pemain, NPC, maupun monster/spirit beast. Statistik tempur monster (HP dan Attack Power) tidak dikarang secara sepihak, melainkan diturunkan secara presisi dari formula `QiCap` Realm yang setara (`12`).

### Aturan Emas Anti-Cheat Bestiarium
- **Statistik Terikat Formula**: HP dan Attack Power monster **WAJIB** dihitung menggunakan formula resmi `MonsterHP` dan `MonsterAttackPower`. AI GM dilarang mengarang angka statistik monster secara acak tanpa dasar formula.
- **Kemunculan Dilempar AI GM**: Kemunculan monster liar (*Random Encounter*) atau penyergapan (*Ambush*) dilempar oleh AI GM menggunakan formula `AmbushChance` — pemain tidak bisa menentukan sendiri "tidak ada monster" atau "monster muncul instan".
- **Ekonomi Aksi Sederajat**: Monster dan spirit beast bertindak dalam urutan *Initiative* yang sama (`15`), memiliki 1 Aksi Utama + 1 Aksi Kecil per giliran, dan dilarang menyerang berkali-kali di luar gilirannya.
- **Item Origin Log untuk Loot**: Seluruh material, kulit, kelenjar racun, dan *Spirit Core* yang dipanen wajib dicatat di log inventory (*Item Origin Log*) sebelum dapat diperjualbelikan (`13`) atau dipakai untuk alkimia (`16`).
- **Cooldown Jurus Ultimate**: Serangan mematikan khas monster (> 1,5× Attack Power) dibatasi cooldown minimal 3 ronde pertempuran.

---

## 🎲 1. Formula Baku Statistik Monster (Monster Combat Formulas)

Statistik dasar monster dan binatang spiritual liar diturunkan dari `QiCap` Realm yang setara (`12`):

```
MonsterHP = QiCap(realm, stage) × 0,5 × LawHPMultiplier(element)
MonsterAttackPower = QiCap(realm, stage) × 0,15 × LawAttackMultiplier(element)
```

- `LawHPMultiplier`: Elemen Earth/Metal = ×1,5 | Wood/Life = ×1,3 | Water/Star/Ice = ×1,0 | Fire/Sun = ×0,9 | Poison/Blood = ×0,8.
- `LawAttackMultiplier`: Elemen Poison/Blood = ×1,4 | Fire/Sun = ×1,3 | Wind/Sound = ×1,2 | Water/Ice = ×1,0 | Earth/Metal = ×0,8.

*Contoh Perhitungan:*
- **Miasma Python** (Nine-Reed Mire, Tier 3 Mid / Foundation Mid, Water+Poison):
  `QiCap(3, Mid) = 1.875`
  `MonsterHP = 1.875 × 0,5 × 0,8 = 750 HP`
  `MonsterAttackPower = 1.875 × 0,15 × 1,4 = 393 Attack Power`

---

## 🦁 2. Kategori Monster & Threat Level Standard

### 2.1 Kategori Spesies Monster
1. 🐺 **Spirit Beast (Binatang Spiritual)**: Hewan ber-Qi yang memiliki organ Inti Monster (*Spirit Core*). Dapat dijinakkan melalui `19_BEAST_BOND_SYSTEM.md`.
2. 🔥 **Elemental (Makhluk Elemen)**: Entitas murni yang terbentuk dari gumpalan energi Nine Meridian Currents (Api, Es, Petir, Air, Lumpur).
3. 👻 **Undead / Roh (Arwah & Mayat Hidup)**: Roh penasaran, mayat beracun, dan entitas arwah perang yang kebal serangan fisik biasa tanpa perisai Qi.
4. 🐛 **Insect / Gu Swarm (Kawanan Serangga)**: Kawanan lebah, lipan, atau kutu spiritual yang menyerang dalam jumlah besar.
5. 👤 **Bayangan / Yin (Siluman Tak Berwujud)**: Entitas siluman atau ilusi yang menyerang kesadaran batin (*Focus*) dan membingungkan indera arah.
6. 🗿 **Ancient Guardian (Penjaga Purba)**: Golem batu/bambu atau monster purba berumur ribuan tahun yang menjaga reruntuhan suci.

### 2.2 Standar Tingkat Bahaya (Threat Level Standard)

| Threat Level | Kategori Bahaya | Syarat Tim / Kultivator Disarankan |
|---|---|---|
| 🟢 **Green (Rendah)** | Monster Tingkat Awal (Tier 1–2). | Kultivator *Body Refining* / *Qi Gathering* (Realm 1–2). |
| 🟡 **Yellow (Sedang)** | Monster Tingkat Menengah (Tier 3). | Kultivator *Foundation Establishment* (Realm 3) atau tim 3 orang. |
| 🔴 **Red (Tinggi)** | Monster Tingkat Tinggi / Ganas (Tier 4–5). | Kultivator *Core Formation* / *Nascent Soul* (Realm 4–5). |
| 🖤 **Black (Calamity)** | Bencana Wilayah / Boss Purba (Tier 6+). | Tetua Sekte / Kultivator *Soul Formation* / *Void Refinement* (Realm 6+). |

---

## 🎯 3. Sistem Kemunculan & Ambush Chance

Peluang disergap monster liar di wilayah terbuka dihitung per Shichen (2 Jam) perjalanan:

```
AmbushChance = BaseChance × RegionalDangerMod × TimeMod
```

- `BaseChance` = 5% per Shichen perjalanan.

| Modifier | Nilai Multiplier | Catatan Aplikasi |
|---|---|---|
| `RegionalDangerMod` — Jalur Perdagangan Resmi | ×0,5 | Dikawal garnisun perbatasan atau karavan. |
| `RegionalDangerMod` — Wilayah Liar / Hutan / Rawa | ×2,0 | Medan belantara tanpa patroli resmi. |
| `RegionalDangerMod` — Zona Anomali Terlarang (*Scarlands/Abyss*) | ×4,0 | Distorsi ruang-waktu & miasma pekat. |
| `TimeMod` — Siang Hari | ×1,0 | Aktivitas monster normal. |
| `TimeMod` — Malam Hari | ×2,0 | Mayoritas monster nocturnal & siluman Yin lebih aktif. |

*Contoh Perhitungan:*
Melintasi Labirin Alang-Alang Nine-Reed Mire (Zona Liar, ×2.0) di malam hari (×2.0):
`AmbushChance = 5% × 2,0 × 2,0 = 20% per Shichen perjalanan`.

---

## 💎 4. Sistem Drop Loot & Rarity Rate

Setiap kali monster dikalahkan secara sah dalam roleplay, AI GM melemparkan peluang drop loot:

```
LootDropRate = BaseDropRate(rarity)
```

| Rarity Loot | BaseDropRate | Contoh Material Loot Qianyuan |
|---|---|---|
| **Common (Umum)** | 70% – 90% | Bahan dasar tubuh monster: daging ber-Qi, kulit kasar, bulu, taring biasa. |
| **Rare (Jarang)** | 20% – 40% | Organ spiritual: Inti Monster (*Spirit Core*), kelenjar racun murni, sisik keras. |
| **Legendary / Boss**| 5% – 15% (100% Kill Pertama) | Kristal Purba Tier 7+, tanduk purba, esens jiwa monster, artefak kuno. |

> 📌 Semua loot mengikuti Tier & Grade Sistem Ekonomi (`13_ECONOMY_MARKET_SYSTEM.md`) dan **WAJIB dicatat di Item Origin Log** sebelum dapat dijual, diproduksi di Alkimia (`16`), atau dipakai untuk terobosan Realm (`12`).

---

## 📖 5. Daftar Monster & Spirit Beast per Wilayah

---

### 🏯 5.1 Ibu Kota Yuanjing & Perbatasan (`01`)
*(Rujukan: `01_WORLD_OVERVIEW_AND_CAPITAL.md`)*

Ibu kota Yuanjing dan pos perbatasan perimeternya terlindung oleh Formasi Tujuh Cincin, namun pinggiran perbatasan luar (100 li dari gerbang) dan Lembah Bambu Serat Giok tetap dihuni oleh makhluk-makhluk penantang:

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Anjing Penjaga Perbatasan | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Menghuni pos gerbang luar 100 li dari Yuanjing. Peka terhadap miasma racun dan penyelundup barang terlarang. Menggigit kaki target untuk melumpuhkan gerak. | Umum: Kulit Anjing Perbatasan (Tier 1) — Jarang: Taring Pelacak (Tier 2) |
| Roh Prajurit Gerbang | 👻 Undead | 3, Early (Foundation Est.) | 312 | 112 | Arwah prajurit kuno penjaga benteng luar yang mati saat mempertahankan ibu kota. Menyerang menggunakan arwah tombak karat ber-Qi metal. Kebal senjata fisik biasa. | Umum: Serpihan Zirah Besi Kuno (Tier 2) — Jarang: Inti Roh Prajurit (Tier 3) |
| Kera Bambu Serat Giok | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Menghuni Lembah Bambu Serat Giok (150 li dari Yuanjing). Suka Melemparkan buah bambu keras dari kanopi tinggi, memicu efek *Confusion* dan penalti Movement Speed -10%. | Umum: Bulu Kera Hijau (Tier 1) — Jarang: Bambu Serat Giok Muda (Tier 2) |
| Ular Kabut Serat Giok | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 168 | Bersembunyi di rumpun bambu hijau, memancarkan kabut ilusi disorientasi arah. Patukan giginya menyuntikkan racun pelumpuh otot. | Umum: Sisik Hijau Giok (Tier 2) — Jarang: Kelenjar Kabut Ilusi (Tier 3) |

---

### 🌊 5.2 Vermilion River Basin (`02`)
*(Rujukan: `02_VERMILION_RIVER_BASIN.md`)*

Wilayah perairan sungai deras, delta rawa, dan lembah herba. Monster di sini didominasi oleh elemen Air dan Kayu (*Water + Wood Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Vermilion Carp | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Menghuni perairan anak Sungai Vermilion. Sisik merah keemasannya memancarkan aura Wood Qi murni. Sangat pasif dan melarikan diri jika ada getaran air. | Umum: Daging Ikan Ber-Qi (Tier 1) — Jarang: Sisik Merah Vermilion (Tier 1) |
| Mud Crocodile | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 187 | 30 | Bersembunyi di dasar lumpur dangkal Pelabuhan Zhuque dan Dermaga Tiga Muara. Menyergap perahu kayu kecil dengan serangan gibasan ekor berat (*Posture Unstable*). | Umum: Kulit Buaya Lumpur (Tier 2) — Jarang: Taring Buaya Rawa (Tier 2) |
| Misty Heron | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 45 | Burung bangau raksasa penghuni muara sungai. Mampu menyemburkan gelombang angin embun yang membutakan pandangan mata (*Hit Rate -15%*). | Umum: Bulu Bangau Kabut (Tier 1) — Jarang: Paruh Bangau Tajam (Tier 2) |
| Giant Water Snake | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Ular air sepanjang 12 meter penghuni Lembah Embun Merah. Menjerat perenang dan perahu dayung lalu menariknya ke dalam dasar sungai deras. | Umum: Kulit Ular Air (Tier 2) — Jarang: Inti Air Murni (Tier 3) |
| Teratai Lumpur Beracun | 🌿 Flora / Plant Creature | 3, Mid (Foundation Est.) | 468 | 168 | Tumbuhan monster berbentuk teratai raksasa di tepi rawa sungai. Melontarkan duri-duri racun pemutus aliran Dantian saat disentuh. | Umum: Batang Teratai Ber-Qi (Tier 2) — Jarang: Biji Teratai Lumpur Purba (Tier 3) |
| Hiu Sungai Vermilion | 🐺 Spirit Beast | 4, Early (Core Formation) | 3.125 | 937 | Predator puncak perairan dalam muara sungai. Gigi gergajinya mampu merobek lambung perahu dagang kayu dalam dua kali gigitan. | Umum: Sirip Hiu Sungai (Tier 3) — Jarang: Inti Monster Air Tier 4 (Tier 4) |

---

### ⛰️ 5.3 Blackstone Skyreach (`03`)
*(Rujukan: `03_BLACKSTONE_SKYREACH.md`)*

Wilayah pegunungan batu hitam keras dan gua tambang dalam. Monster di sini memiliki pertahanan fisik raga sangat tinggi (*Earth + Metal Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Iron-Eating Beetle | 🐛 Insect / Gu Swarm | 2, Early (Qi Gathering) | 187 | 30 | Kawanan kumbang pemakan bijih besi di Gua Tambang Kuno. Menggerogoti senjata dan zirah besi pemain jika terkena semburan asam gigitannya. | Umum: Cangkang Besi Hitam (Tier 1) — Jarang: Inti Kumbang Logam (Tier 2) |
| Cliff Falcon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 45 | Elang tebing bertepi sayap sekeras baja. Menukik cepat dari puncak tebing Benteng Skyreach untuk merebut barang mengkilap milik penambang. | Umum: Bulu Baja Tebing (Tier 1) — Jarang: Cakar Elang Logam (Tier 2) |
| Stone Ridge Ape | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 468 | 75 | Kera raksasa bertubuh batu hitam penghuni Lembah Anvil. Melemparkan bongkahan batu besar dari ketinggian (*Elevated Position*) memicu kerusakan zirah. | Umum: Kulit Batu Kera (Tier 2) — Jarang: Batu Inti Magnetik (Tier 3) |
| Ironclad Bear | 🐺 Spirit Beast | 4, Early (Core Formation) | 4.687 | 750 | Beruang raksasa berdaging sekeras Cold Steel di Zona Inti Gua Tambang. Memiliki kemampuan *Perisai Zirah Batu Hitam* yang memantulkan 20% kerusakan fisik. | Umum: Empedu Beruang Alkimia (Tier 3) — Jarang: Kulit Besi Purba (Tier 4) |
| Golem Batu Hitam Purba | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 23.437 | 3.750 | Golem pelindung peninggalan penempa purba di kedalaman 3.000 meter. Kebal terhadap serangan pedang biasa; hanya dapat dilukai oleh tebasan Qi berat. | Legendaris: Kristal Inti Bumi Purba (Tier 5, bahan tempa Zirah Tian-Grade) |

---

### 🏜️ 5.4 Ashen Sun Expanse (`04`)
*(Rujukan: `04_ASHEN_SUN_EXPANSE.md`)*

Wilayah laut pasir bergeser dan oasis terik. Monster di sini bertahan hidup dengan energi Api dan Matahari (*Fire + Sun Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Dune Camel Wild | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Unta liar gurun pasir. Menyimpan cadangan air spiritual di punuknya. Pasif, namun menendang keras jika dipojokkan di celah bukit pasir. | Umum: Daging Unta Gurun (Tier 1) — Jarang: Punuk Air Spiritual (Tier 1) |
| Flame-Viper | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 112 | 48 | Ular pasir merah bersisik panas. Bersembunyi di bawah bukit pasir menyanyi, menyuntikkan racun panas pembakar Dantian saat mematuk. | Umum: Kulit Ular Api (Tier 1) — Jarang: Kelenjar Racun Api Gurun (Tier 2) |
| Sun Lizard | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 112 | 48 | Kadal raksasa pemakan kristal api di dekat Benteng Sandgate. Mampu menyemburkan lidah api sejauh 5 langkah (*Fire Damage 35 HP*). | Umum: Sisik Kadal Sunfire (Tier 1) — Jarang: Inti Api Kecil (Tier 2) |
| Sandstorm Scorpion | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 281 | 121 | Kalajengking pasir sebesar kuda di sekitar Reruntuhan Buried Sun Palace. Sengatan ekornya menyuntikkan racun panas pelumpuh saraf. | Umum: Cangkang Kalajengking Gurun (Tier 2) — Jarang: Sengat Racun Api (Tier 3) |
| Cacing Pasir Purba (Dune Worm) | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 117.187 | 23.437 | Cacing pasir purba sepanjang 50 meter penghuni lautan pasir dalam. Menyergap karavan dari bawah tanah, menciptakan pusaran pasir hisap (*Sinkhole*). | Legendaris: Kulit Cacing Pasir Purba (Tier 6, bahan zirah Di-Grade) |

---

## 🌿 5.5 Nine-Reed Mire (`05`)
*(Rujukan: `05_NINE_REED_MIRE.md`)*

Wilayah rawa beracun dan semak alang-alang raksasa. Monster di sini beracun dan bergerak stealth (*Water + Poison Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Mud Leech | 🐛 Insect / Gu Swarm | 1, Early (Body Refining) | 20 | 10 | Lintah mikro tak kasat mata di perairan tenang Desa Mirewood. Menempel pada kulit saat menyelam, memicu status *Blood Drain Trauma* (-10 Stamina/jam). | Umum: Cairan Lintah Rawa (Tier 1) — Jarang: Esens Darah Lintah (Tier 1) |
| Swamp Toad | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 100 | 42 | Kodok raksasa bersuara nyaring di perairan dangkal. Menyemburkan lendir asam beracun yang merusak durabilitas senjata dan zirah. | Umum: Lendir Kodok Rawa (Tier 1) — Jarang: Kelenjar Racun Kodok (Tier 2) |
| Giant Poison Centipede | 🐛 Insect / Gu Swarm | 3, Early (Foundation Est.) | 250 | 131 | Lipan beracun sepanjang 3 meter di Gua Sarang Serangga Spiritual. Gigitannya menyuntikkan racun korosif perusak jaringan Dantian. | Umum: Cangkang Duri Lipan (Tier 2) — Jarang: Inti Racun Lipan (Tier 3) |
| Miasma Python | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 375 | 196 | Ular miasma raksasa di Zona Dalam Labirin Alang-Alang Sembilan. Melilit target dengan kekuatan pelumpuh tulang sambil menyemburkan kabut miasma hijau. | Umum: Kulit Ular Miasma (Tier 2) — Jarang: Kantong Racun Murni (Tier 3) |
| Miasma Eel Purba | 🐺 Spirit Beast | 4, Early (Core Formation) | 2.500 | 1.312 | Belut listrik beracun di perairan terendam Reruntuhan Benteng Ular. Memicu ledakan sengatan listrik beracun di area perairan 10 langkah. | Umum: Kulit Belut Miasma (Tier 3) — Jarang: Inti Belut Beracun Tier 4 (Tier 4) |

---

### 🌊 5.6 Astral Tide Sea (`06`)
*(Rujukan: `06_ASTRAL_TIDE_SEA.md`)*

Wilayah lautan luas dan palung dalam. Monster di sini beradaptasi dengan tekanan air dan energi bintang (*Water + Star Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Star-Crab | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Kepiting pantai bersinar bercahaya bintang di Kepulauan Coral. Supit kerasnya mampu memotong tali perahu dayung nelayan. | Umum: Cangkang Kepiting Bintang (Tier 1) — Jarang: Mutiara Bintang Kecil (Tier 1) |
| Spotted Coral Shark | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Hiu karang pencium darah di sekitar Benteng Pulau Coral. Mampu bergerak secepat kilat di dalam air dan menyerang dalam kelompok 3–5 ekor. | Umum: Kulit Hiu Karang (Tier 1) — Jarang: Gigi Hiu Bintang (Tier 2) |
| Sea Serpent | 🐺 Spirit Beast | 4, Early (Core Formation) | 3.125 | 937 | Ular laut raksasa di Zona Arus Bintang Palung Abyss. Menyemburkan gelombang air bertekanan tinggi yang menenggelamkan kapal perang. | Umum: Sisik Ular Laut Bintang (Tier 3) — Jarang: Inti Mutiara Samudra (Tier 4) |
| Astral Whale Purba | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 78.125 | 23.437 | Paus purba raksasa sepanjang 100 meter di Zona Palung Gelap. Meluncurkan gelombang *Astral Sonic Wave* pengguncang perisai Qi seluruh kapal. | Legendaris: Tulang Paus Bintang Purba (Tier 6, bahan perahu Lingzhou) |

---

### 🌲 5.7 Whispering Root Forest (`07`)
*(Rujukan: `07_WHISPERING_ROOT_FOREST.md`)*

Wilayah hutan purba kanopi lebat. Monster di sini kaya akan energi Kehidupan dan Serat Kayu (*Wood + Life Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Wood-Deer | 🐺 Spirit Beast | 1, Early (Body Refining) | 32 | 7 | Rusa spiritual berdaun hijau di Zona Luar Kanopi. Pasif dan sangat lincah melompat di antara dahan kayu. Mengatur regenerasi tanaman obat. | Umum: Daging Rusa Herbal (Tier 1) — Jarang: Tanduk Kayu Serat (Tier 1) |
| Green Vine Snake | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 35 | Ular hijau tersamar dahan di Zona Tengah (*Whispering Root Zone*). Menyergap leher pengembara dari atas kanopi dengan belitan cepat. | Umum: Kulit Ular Dahan (Tier 1) — Jarang: Bisa Kayu Penenang (Tier 2) |
| Emerald Panther | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 243 | 53 | Macan tutul giok pemangsa cepat di jalur kanopi. Menggunakan pergerakan *Stealth* tanpa suara untuk menerkam mangsa dari belakang (*Surprise Attack*). | Umum: Kulit Macan Giok (Tier 2) — Jarang: Cakar Emerald Sharp (Tier 2) |
| Spore Wood Sentinel | 🌿 Flora / Plant Creature | 3, Early (Foundation Est.) | 406 | 89 | Pohon monster penembak spora di Desa Lembah Spora Hijau. Melepaskan gelombang spora beracun *Ancient Wood Spore Miasma*. | Umum: Kayu Spora Purba (Tier 2) — Jarang: Biji Spora Hijau Murni (Tier 3) |
| Ancient Bear | 🐺 Spirit Beast | 4, Early (Core Formation) | 4.062 | 890 | Beruang purba pelindung Zona Inti World Tree Sanctuary. Menghentakkan kaki ke tanah memicu gelombang akar raksasa *Living Entangling Roots*. | Umum: Empedu Beruang Purba (Tier 3) — Jarang: Inti Kehidupan Kayu Tier 4 (Tier 4) |

---

### ❄️ 5.8 Frostglass Crown (`08`)
*(Rujukan: `08_FROSTGLASS_CROWN.md`)*

Wilayah puncak gletser abadi dan badai salju. Monster di sini tahan terhadap suhu membeku (*Ice + Stillness Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Ice-Crystal Wolf | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Serigala es berbulu bening di jalur pendakian Desa Gletser Bening. Berburu dalam kelompok 4–8 ekor, menyemburkan napas es membekukan sendi. | Umum: Bulu Serigala Es (Tier 2) — Jarang: Kristal Es Serigala (Tier 3) |
| Frost Snow Ape | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Kera salju raksasa di tebing gletser terjal. Melemparkan bongkahan es keras dari atas tebing, memicu risiko jatuh (*Falling Damage*). | Umum: Kulit Kera Salju (Tier 2) — Jarang: Taring Es Abadi (Tier 3) |
| Glacier Eagle | 🐺 Spirit Beast | 3, Late (Foundation Est.) | 625 | 187 | Elang raksasa bercakar kristal es. Menukik cepat di tengah badai salju *Blizzard Storm* untuk mencengkeram pengembara kelelahan. | Umum: Bulu Elang Gletser (Tier 2) — Jarang: Cakar Kristal Es (Tier 3) |
| Frostglass Centipede | 🐛 Insect / Gu Swarm | 4, Early (Core Formation) | 3.125 | 937 | Lipan es bening sekeras kaca di Gua Meditasi Inti Es. Gigitannya membekukan aliran Qi Dantian seketika (*Frostbite Status*). | Umum: Cangkang Kaca Es (Tier 3) — Jarang: Inti Es Purba Tier 4 (Tier 4) |

---

### 🌪️ 5.9 Hollow Gale Corridor (`09`)
*(Rujukan: `09_HOLLOW_GALE_CORRIDOR.md`)*

Wilayah ngarai berangin kencang dan tebing berongga. Monster di sini berkecepatan tinggi dan memancarkan gelombang suara (*Wind + Sound Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Wind-Runner Swift | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 8 | Burung kecil berkecepatan tinggi di jembatan gantung tali. Terbang membelah angin ngarai. Dipelihara kurir sebagai pengantar pesan. | Umum: Bulu Angin Cepat (Tier 1) — Jarang: Paruh Burung Swift (Tier 1) |
| Hollow Canyon Lizard | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 45 | Kadal tebing perayap dinding batu ngarai. Kulitnya menyatu dengan warna batu tebing, memicu serangan kejutan dari celah batu. | Umum: Kulit Kadal Ngarai (Tier 1) — Jarang: Cakar Perayap Tebing (Tier 2) |
| Gale Falcon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 67 | Elang pemangsa berkecepatan tinggi di Pos Tebing Bisik. Menukik memotong udara bagaikan pisau angin penembus perisai Qi. | Umum: Bulu Elang Topan (Tier 1) — Jarang: Inti Angin Ngarai (Tier 2) |
| Echo Bat | 🦇 Spirit Beast / Swarm | 2, Late (Qi Gathering) | 250 | 90 | Kelelawar raksasa penghuni Gua Gema Suara Purba. Memicu serangan gelombang suara *Sonic Disorientation* yang merusak Focus batin. | Umum: Sayap Kelelawar Gema (Tier 2) — Jarang: Kelenjar Suara Gema (Tier 2) |

---

### 🌀 5.10 Fate Scarlands (`10`)
*(Rujukan: `10_FATE_SCARLANDS.md`)*

Zona terlarang (*forbidden zone*) tempat hancurnya simpul arus gaib. Monster di sini mengalami mutasi anomali ruang, waktu, dan identitas (*Fate + Mutated Qi*):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Scar-Gazer | 👤 Bayangan / Anomali | 4, Mid (Core Formation) | 2.656 | 843 | Monster bermata satu raksasa terapung di dekat Kemah Penjelajah. Pandangan matanya memicu kabut ilusi pemudar ingatan (*Memory Erosion*). | Umum: Serpihan Mata Anomali (Tier 3) — Jarang: Inti Mutasi Batin (Tier 4) |
| Spatial Anomaly Serpent | 🐺 Spirit Beast Mutasi | 5, Early (Nascent Soul) | 13.281 | 4.218 | Ular mutasi raksasa perayap celah ruang di Reruntuhan Kota Terbalik. Menyerang dengan menghilang ke dalam retakan ruang lalu muncul di belakang target. | Umum: Sisik Belah Ruang (Tier 4) — Jarang: Spatial Shard Purba (Tier 5) |
| Chrono-Beast | 🗿 Ancient Guardian | 7, Early (Void Refinement) | 332.031 | 105.468 | Binatang purba pelindung Celah Takdir Purba. Mampu memperlambat waktu lokal di sekitarnya (*Chrono Stasis*), memotong Movement Speed $-60\%$. | Legendaris: Fate Core Crystal (Tier 7, bahan terobos Dao Integration) |
| Mutated Void Beast | 🗿 Ancient Guardian / Calamity | 7, Mid (Void Refinement) | 498.046 | 158.203 | Monster tanpa wujud tetap yang mampu melompat antar-dimensi ruang. Menyerang dengan ledakan gelombang energi mutasi perusak Dantian. | Legendaris: Inti Kehampaan Anomali Tier 7 (Tier 7, bahan senjata Sheng-Grade) |

---

## 🛡️ 6. Checklist Anti-Cheat Monster (Wajib Dicek AI-GM)

- [ ] HP dan Attack Power monster dihitung dari formula `MonsterHP` dan `MonsterAttackPower` di §1, bukan klaim sepihak?
- [ ] Kemunculan penyergapan (*Ambush*) dilempar via formula `AmbushChance` (§2) oleh AI GM, bukan diatur sepihak pemain?
- [ ] Monster Calamity (Tier 6+) hanya muncul di habitat resmi sesuai canon (`01`–`10`), tidak di lokasi aman?
- [ ] Loot hanya didapat setelah monster benar-benar dikalahkan dalam roleplay dan dicatat di *Item Origin Log* (`13`)?
- [ ] Serangan ultimate monster (> 1,5× Attack Power) dibatasi cooldown minimal 3 ronde pertempuran?
- [ ] Respawn monster unik/boss dibatasi cooldown naratif wajar, tidak di-farming berulang dalam waktu singkat?

Jika **salah satu** poin di atas meragukan → Encounter / Loot **DIKOREKSI OTOMATIS** oleh AI GM.

---

## 🗺️ 7. Integrasi dengan Sistem Lain

- **Dengan Sistem Hukum Kultivasi (`12`)**: `MonsterQiCap` menggunakan tabel QiCap yang sama, dan loot monster dipetakan langsung ke Bahan Terobosan Realm per Hukum.
- **Dengan Sistem Ekonomi (`13`)**: Seluruh loot monster tunduk pada Tier & Grade Value serta formula `FinalPrice` saat ditransaksikan di bursa.
- **Dengan Sistem Vitalitas & HP (`14`)**: Damage monster mengurangi HP karakter secara presisi dan dapat memicu status *Wound/Trauma*.
- **Dengan Sistem Pertempuran Taktis (`15`)**: Monster dan kultivator bertarung menggunakan sistem *Initiative*, *Action Economy*, dan *Posture/Position* yang identik.
- **Dengan Sistem Beast Bond (`19`)**: Spirit Beast liar dari kategori 🐺 dapat dijinakkan dan diikat menjadi pasangan bertarung jika memenuhi syarat *Trust* dan *Taming Chance*.

---

## 📊 8. Ringkasan Jumlah Monster per Wilayah Qianyuan-World

| Wilayah Qianyuan-World | Jumlah Spesies Canon | Threat Level Tertinggi |
|---|---|---|
| **Ibu Kota Yuanjing & Perbatasan (`01`)** | 4 Spesies | 🟡 Yellow (Tier 3 — Roh Prajurit) |
| **Vermilion River Basin (`02`)** | 6 Spesies | 🔴 Red (Tier 4 — Hiu Sungai Vermilion) |
| **Blackstone Skyreach (`03`)** | 5 Spesies | 🖤 Black (Tier 5 — Golem Batu Hitam Purba) |
| **Ashen Sun Expanse (`04`)** | 5 Spesies | 🖤 Black (Tier 6 — Cacing Pasir Purba) |
| **Nine-Reed Mire (`05`)** | 5 Spesies | 🔴 Red (Tier 4 — Miasma Eel Purba) |
| **Astral Tide Sea (`06`)** | 4 Spesies | 🖤 Black (Tier 6 — Astral Whale Purba) |
| **Whispering Root Forest (`07`)** | 5 Spesies | 🔴 Red (Tier 4 — Ancient Bear) |
| **Frostglass Crown (`08`)** | 4 Spesies | 🔴 Red (Tier 4 — Frostglass Centipede) |
| **Hollow Gale Corridor (`09`)** | 4 Spesies | 🟡 Yellow (Tier 2 — Echo Bat & Gale Falcon) |
| **Fate Scarlands (`10`)** | 4 Spesies | 🖤 Black (Tier 8 — Spatial Anomaly Serpent) |
| **Monster Lintas Wilayah / Umum (§5)** | 10 Spesies | 🟡 Yellow (Tier 3 — Roh Pengembara & Mirage Fox) |

---

## 🎯 9. Panduan Penggunaan untuk AI GM

### 9.1 Memilih Monster yang Tepat
1. **Tentukan wilayah** tempat pemain berada saat ini (misal: *Nine-Reed Mire*).
2. **Pilih spesies monster** dari katalog wilayah tersebut yang sesuai dengan Threat Level dan Realm pemain.
3. **Lempar `AmbushChance`** (§2) untuk menentukan apakah terjadi penyergapan tiba-tiba.

### 9.2 Menjalankan Pertarungan
1. **Gunakan formula** dari `15_COMBAT_TACTICAL_SYSTEM.md` untuk resolusi pertempuran.
2. **Hitung `MonsterHP` & `MonsterAttackPower`** menggunakan formula §1.
3. **Serangan Ultimate Monster**: Boleh menggunakan 1,5× s/d 3,0× Attack Power sekali per pertarungan (cooldown 3 ronde).

### 9.3 Menentukan Loot
1. Setelah monster dikalahkan, lempar `BaseDropRate` (§3).
2. Tentukan material yang berhasil didapat dan catat ke *Item Origin Log* (`13`).
