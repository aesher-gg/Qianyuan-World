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
5. 👤 **Bayangan / Yin (Siluman Tak Berwujud)**: Entitas siluman atau ilusi yang menyerang kesadaran batin dan energi Qi (*Qi Drain*) serta membingungkan indera arah.
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

Peluang disergap monster liar di wilayah terbuka dihitung per Jam perjalanan:

```
AmbushChance = BaseChance × RegionalDangerMod × TimeMod
```

- `BaseChance` = 2,5% per Jam perjalanan.

| Modifier | Nilai Multiplier | Catatan Aplikasi |
|---|---|---|
| `RegionalDangerMod` — Jalur Perdagangan Resmi | ×0,5 | Dikawal garnisun perbatasan atau karavan. |
| `RegionalDangerMod` — Wilayah Liar / Hutan / Rawa | ×2,0 | Medan belantara tanpa patroli resmi. |
| `RegionalDangerMod` — Zona Anomali Terlarang (*Scarlands/Abyss*) | ×4,0 | Distorsi ruang-waktu & miasma pekat. |
| `TimeMod` — Siang Hari | ×1,0 | Aktivitas monster normal. |
| `TimeMod` — Malam Hari | ×2,0 | Mayoritas monster nocturnal & siluman Yin lebih aktif. |

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

---

## 🌐 5. Katalog Beast Lintas Wilayah / Umum (Common Cross-Region Beasts)

Spesies binatang spiritual umum yang dapat ditemukan di berbagai wilayah benua Qianyuan (perbukitan, padang rumput, pinggir jalan karavan, dan hutan biasa):

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Spirit Wild Boar | 🐺 Spirit Beast | 1, Early (Body Refining) | 37 | 6 | Babi hutan berdaging keras di perbukitan umum. Menyergap dengan gundukan taring besi (*Posture Unstable*). | Umum: Daging Babi Ber-Qi (Tier 1) — Jarang: Taring Besi Liar (Tier 1) |
| Gray Wilderness Wolf | 🐺 Spirit Beast | 1, Mid (Body Refining) | 37 | 11 | Serigala padang rumput yang berburu dalam kelompok 3–6 ekor. Cepat dan mengintai dari semak-semak. | Umum: Bulu Serigala Abu (Tier 1) — Jarang: Taring Serigala Liar (Tier 1) |
| Iron-Claw Hawk | 🐺 Spirit Beast | 1, Late (Body Refining) | 50 | 15 | Elang perbukitan bercakar sekeras tembaga. Menukik cepat mencengkeram hewan kecil atau barang bawaan. | Umum: Bulu Elang Tembaga (Tier 1) — Jarang: Cakar Besi Elang (Tier 1) |
| Grass-Spotted Spirit Deer | 🐺 Spirit Beast | 1, Early (Body Refining) | 32 | 6 | Rusa rumput ber-Qi kayu murni. Sangat jinak dan lincah melarikan diri jika mendengar getaran langkah. | Umum: Daging Rusa Rumput (Tier 1) — Jarang: Tanduk Rusa Muda (Tier 1) |
| Mountain Stone Goat | 🐺 Spirit Beast | 1, Mid (Body Refining) | 56 | 9 | Kambing gunung berbelulang keras penjelajah tebing terjal. Menghentakkan tanduk keras jika disudutkan. | Umum: Kulit Kambing Gunung (Tier 1) — Jarang: Tanduk Batu Gunung (Tier 1) |
| Earth-Burrowing Rat | 🐛 Insect / Beast | 1, Early (Body Refining) | 37 | 6 | Tikus penggali tanah di sepanjang jalur karavan. Menggerogoti karung bekal dan akar herba spiritual. | Umum: Kulit Tikus Tanah (Tier 1) — Jarang: Gigi Penggali Batu (Tier 1) |
| Cloud-Rider Horse | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 30 | Kuda liar berkecepatan tinggi penghuni dataran tinggi. Dapat dijinakkan untuk tunggangan karavan cepat. | Umum: Daging Kuda Awan (Tier 1) — Jarang: Surai Kuda Awan (Tier 2) |
| Spirit Firefly Swarm | 🐛 Insect / Swarm | 1, Early (Body Refining) | 25 | 9 | Kawanan kunang-kunang pemancar Qi cahaya di pinggir hutan malam. Membingungkan pandangan musuh. | Umum: Serbuk Kunang-Kunang (Tier 1) — Jarang: Esens Cahaya Qi (Tier 1) |
| Phantom Cave Bat | 🦇 Spirit Beast / Swarm | 1, Mid (Body Refining) | 30 | 13 | Kelelawar gua malam pemancar gema getaran. Menyerang dalam kelompok saat obor dinyalakan. | Umum: Sayap Kelelawar Gua (Tier 1) — Jarang: Kelenjar Gema Malam (Tier 1) |
| Blood Leech | 🐛 Insect / Swarm | 1, Early (Body Refining) | 20 | 10 | Lintah penghisap darah di perairan tenang. Menempel tanpa terasa dan mengurangi Stamina -10/jam. | Umum: Cairan Lintah Darah (Tier 1) — Jarang: Esens Darah Murni (Tier 1) |
| Common River Crab | 🐺 Spirit Beast | 1, Early (Body Refining) | 31 | 6 | Kepiting sungai air tawar bersupit keras. Bersembunyi di balik batu sungai dangkal. | Umum: Daging Kepiting Sungai (Tier 1) — Jarang: Cangkang Kepiting Keras (Tier 1) |
| Wild Horned Bull | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 187 | 30 | Banteng bertanduk ganda penghuni padang rumput. Menundukkan kepala dan melakukan *Charge Attack*. | Umum: Daging Banteng Ber-Qi (Tier 1) — Jarang: Tanduk Banteng Liar (Tier 2) |
| Mist Rabbit | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Kelinci putih penyembur kabut tipis penyamar diri. Lincah dan melompat cepat ke dalam sarang tanah. | Umum: Bulu Kelinci Kabut (Tier 1) — Jarang: Mata Kelinci Kristal (Tier 1) |
| Wandering Crow | 🐺 Spirit Beast | 1, Mid (Body Refining) | 25 | 13 | Gagak pemakan bangkai ber-Qi kegelapan. Mengeluarkan suara nyaring yang memicu penalti *Evasion -5%*. | Umum: Bulu Gagak Pengembara (Tier 1) — Jarang: Paruh Gagak Mitos (Tier 1) |
| Common Poison Frog | 🐺 Spirit Beast | 1, Late (Body Refining) | 32 | 16 | Kodok beracun warna-warni di kolam hujan. Menyemburkan racun gatal jika tersentuh kulit terbuka. | Umum: Kulit Kodok Beracun (Tier 1) — Jarang: Kelenjar Racun Kodok (Tier 1) |

---

## 📖 6. Katalog Monster per Wilayah (Minimal 20 per Wilayah)

---

### 🏯 6.1 Ibu Kota Yuanjing & Perbatasan (`01`) — 24 Spesies
*(Rujukan: `01_WORLD_OVERVIEW_AND_CAPITAL.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Anjing Penjaga Perbatasan | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Menghuni pos gerbang luar 100 li dari Yuanjing. Peka terhadap miasma racun. | Umum: Kulit Anjing Perbatasan (Tier 1) — Jarang: Taring Pelacak (Tier 2) |
| Roh Prajurit Gerbang | 👻 Undead | 3, Early (Foundation Est.) | 312 | 112 | Arwah prajurit kuno penjaga benteng luar. Kebal senjata fisik biasa. | Umum: Serpihan Zirah Besi Kuno (Tier 2) — Jarang: Inti Roh Prajurit (Tier 3) |
| Kera Bambu Serat Giok | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Menghuni Lembah Bambu Serat Giok (150 li). Melemparkan buah bambu keras. | Umum: Bulu Kera Hijau (Tier 1) — Jarang: Bambu Serat Giok Muda (Tier 2) |
| Ular Kabut Serat Giok | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 168 | Bersembunyi di rumpun bambu, memancarkan kabut ilusi disorientasi arah. | Umum: Sisik Hijau Giok (Tier 2) — Jarang: Kelenjar Kabut Ilusi (Tier 3) |
| Jade Bamboo Viper | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 35 | Ular bambu berbisa tinggi di perbatasan luar Cincin 7. Patukannya menyuntikkan racun lumpuh. | Umum: Kulit Ular Bambu (Tier 1) — Jarang: Taring Bisa Bambu (Tier 2) |
| Imperial Hunting Hound | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 75 | Anjing pemburu keturunan militer di area latihan perbatasan. Cepat dan melacak aroma darah. | Umum: Bulu Anjing Pemburu (Tier 2) — Jarang: Taring Perak Pemburu (Tier 2) |
| Golden Feather Pheasant | 🐺 Spirit Beast | 1, Late (Body Refining) | 65 | 13 | Burung kuau berbulu emas di Lembah Bambu. Peka dan terbang memancarkan percikan cahaya Qi. | Umum: Bulu Emas Kuau (Tier 1) — Jarang: Paruh Kuau Emas (Tier 1) |
| Royal Guard Statue Golem | 🗿 Ancient Guardian | 3, Peak (Foundation Est.) | 1.171 | 225 | Golem batu pelindung makam bangsawan lama di perbatasan selatan Cincin 6. | Umum: Batu Zirah Kerajaan (Tier 3) — Jarang: Inti Golem Batu (Tier 3) |
| Stone Lion Guardian | 🗿 Ancient Guardian | 4, Early (Core Formation) | 4.687 | 750 | Patung singa batu hidup penjaga kuil purba 120 li dari Yuanjing. Hantaman cakar peremuk zirah. | Umum: Batu Singa Purba (Tier 3) — Jarang: Inti Singa Batu Tier 4 (Tier 4) |
| Mist Heron Outer | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 45 | Burung bangau pemakan ikan di danau Cincin 6. Menyemburkan kabut dingin. | Umum: Bulu Bangau Danau (Tier 1) — Jarang: Paruh Bangau Putih (Tier 2) |
| Wall-Crawling Gecko | 🐺 Spirit Beast | 1, Mid (Body Refining) | 37 | 9 | Tokek raksasa perayap tembok benteng luar Cincin 7. Menyemburkan lendir perekat kaki. | Umum: Kulit Tokek Tembok (Tier 1) — Jarang: Lendir Perekat (Tier 1) |
| Night Shadow Cat | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 45 | Kucing siluman berbulu hitam di lorong gelap Cincin 6. Cakar tajam pemutus urat. | Umum: Bulu Kucing Malam (Tier 1) — Jarang: Cakar Bayangan Kucing (Tier 2) |
| Iron-Hide Wild Boar | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 281 | 45 | Babi hutan berkulit tebal sekeras besi di pinggiran Lembah Bambu. Menyeruduk lurus. | Umum: Kulit Besi Babi (Tier 2) — Jarang: Taring Besi Babi (Tier 2) |
| Bamboo-Eating Panda | 🐺 Spirit Beast | 2, Peak (Qi Gathering) | 390 | 62 | Beruang panda penyuka bambu spiritual. Terlihat tenang namun memiliki pukulan cakar mematikan. | Umum: Bulu Panda Bambu (Tier 2) — Jarang: Empedu Panda Spiritual (Tier 2) |
| Spore Toad Outer | 🐺 Spirit Beast | 1, Late (Body Refining) | 40 | 21 | Kodok penyembur spora di rawa kecil luar perbatasan. Memicu gatal-gatal pada kulit. | Umum: Lendir Kodok Spora (Tier 1) — Jarang: Kelenjar Spora Luar (Tier 1) |
| Phantom Raven | 👤 Bayangan / Yin | 2, Mid (Qi Gathering) | 187 | 67 | Gagak arwah berbayangan gelap di makam tua Cincin 6. Menyerap energi Qi pengembara. | Umum: Bulu Gagak Arwah (Tier 1) — Jarang: Inti Bayangan Gagak (Tier 2) |
| Bronze-Shell Beetle | 🐛 Insect / Swarm | 1, Late (Body Refining) | 75 | 10 | Kumbang berspesimen cangkang perunggu di sekitar bengkel Cincin 5. Memakan sisa logam tempa. | Umum: Cangkang Perunggu (Tier 1) — Jarang: Serbuk Serangga Tempa (Tier 1) |
| White-Tail Deer | 🐺 Spirit Beast | 1, Mid (Body Refining) | 32 | 6 | Rusa bertanduk putih di hutan bambu kekaisaran. Pemalu dan sangat cepat berlari. | Umum: Daging Rusa Putih (Tier 1) — Jarang: Tanduk Rusa Emas (Tier 1) |
| Stream Fish Spirit | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Ikan mas kecil ber-Qi air murni di parit Cincin 1–3. Melompat dan memancarkan cahaya giok. | Umum: Daging Ikan Murni (Tier 1) — Jarang: Sisik Mas Giok (Tier 1) |
| Imperial Guard Falcon | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 112 | Elang terlatih milik Pasukan Pengawal Kekaisaran yang terlepas di perbatasan luar. | Umum: Bulu Elang Militer (Tier 2) — Jarang: Cakar Elang Kekaisaran (Tier 3) |
| Imperial Gold Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.406 | 421 | Anak naga emas bersisik logam kekaisaran di pegunungan perbatasan utara Cincin 4. | Umum: Sisik Naga Emas Muda (Tier 3) — Jarang: Darah Naga Emas Purba (Tier 3) |
| Jade Scale Serpent | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Ular bersisik hijau terang penunggu taman giok istana lama. | Umum: Kulit Ular Giok (Tier 1) — Jarang: Bisa Ular Giok (Tier 2) |
| Golden Lion Guard Golem | 🗿 Ancient Guardian | 4, Peak (Core Formation) | 11.718 | 2.812 | Golem singa emas raksasa penjaga gerbang gerhana kuno. | Umum: Logam Emas Purba (Tier 4) — Jarang: Inti Golem Singa Emas (Tier 4) |
| Golden Dragon Sovereign Purba | 🗿 Mitos / Sovereign | 8, Mid (Dao Integration) | 4.394.531 | 1.318.359 | Naga Emas Mitos purba penyeimbang takdir Kekaisaran Qianyuan di dasar Gunung Yuanjing. | Legendaris: Mutiara Naga Emas Mitos (Tier 8, bahan artefak Sheng-Grade Utama) |

---

### 🌊 6.2 Vermilion River Basin (`02`) — 24 Spesies
*(Rujukan: `02_VERMILION_RIVER_BASIN.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Vermilion Carp | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Ikan karper merah pemancar Wood Qi murni di Pelabuhan Zhuque. Pasif. | Umum: Daging Ikan Ber-Qi (Tier 1) — Jarang: Sisik Merah Vermilion (Tier 1) |
| Mud Crocodile | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 187 | 30 | Buaya rawa penyergap perahu kayu kecil di Dermaga Tiga Muara. | Umum: Kulit Buaya Lumpur (Tier 2) — Jarang: Taring Buaya Rawa (Tier 2) |
| Misty Heron | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 45 | Bangau raksasa penyembur angin embun di muara sungai. | Umum: Bulu Bangau Kabut (Tier 1) — Jarang: Paruh Bangau Tajam (Tier 2) |
| Giant Water Snake | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Ular air 12 meter di Lembah Embun Merah. Menjerat perenang dan perahu. | Umum: Kulit Ular Air (Tier 2) — Jarang: Inti Air Murni (Tier 3) |
| Teratai Lumpur Beracun | 🌿 Flora / Plant Creature | 3, Mid (Foundation Est.) | 468 | 168 | Teratai raksasa penembak duri racun pemutus Dantian di tepi rawa. | Umum: Batang Teratai Ber-Qi (Tier 2) — Jarang: Biji Teratai Lumpur Purba (Tier 3) |
| Hiu Sungai Vermilion | 🐺 Spirit Beast | 4, Early (Core Formation) | 3.125 | 937 | Predator puncak perairan dalam muara sungai. Gigi perobek lambung kapal. | Umum: Sirip Hiu Sungai (Tier 3) — Jarang: Inti Monster Air Tier 4 (Tier 4) |
| Crimson Turtle | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 375 | 40 | Penyu bercangkang merah keras di tepi Desa Bunga Embun. Bertahan tinggi. | Umum: Cangkang Penyu Merah (Tier 2) — Jarang: Daging Penyu Umur Panjang (Tier 2) |
| Water-Spout Python | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Ular piton semburan air di Jeram Tiga Muara. Menyemburkan gumpalan air deras. | Umum: Kulit Piton Air (Tier 2) — Jarang: Kelenjar Semburan Air (Tier 3) |
| Reed Heron | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Bangau sarang alang-alang sungai. Menusuk mata dengan paruh tajam. | Umum: Bulu Bangau Alang (Tier 1) — Jarang: Paruh Bangau Sungai (Tier 2) |
| Steam Toad | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Kodok raksasa penyembur uap air panas di muara hangat. | Umum: Lendir Kodok Uap (Tier 1) — Jarang: Kelenjar Uap Air (Tier 2) |
| Blue Shell Crab | 🐺 Spirit Beast | 1, Late (Body Refining) | 32 | 8 | Kepiting laut-sungai bersupit biru di muara Pelabuhan Zhuque. | Umum: Supit Kepiting Biru (Tier 1) — Jarang: Cangkang Biru Sungai (Tier 1) |
| Water-Spitting Fish | 🐺 Spirit Beast | 1, Mid (Body Refining) | 25 | 9 | Ikan kecil penembak tetesan air bertekanan tinggi dari sungai. | Umum: Daging Ikan Penembak (Tier 1) — Jarang: Sisik Air Tajam (Tier 1) |
| River Otter Spirit | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Berang-berang sungai pemutur jala nelayan. Lincah menyelam di arus keras. | Umum: Bulu Berang-Berang (Tier 1) — Jarang: Taring Berang Sungai (Tier 2) |
| Freshwater Eel | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Belut licin pemancar kejutan Qi air tipis di lumpur sungai. | Umum: Kulit Belut Licin (Tier 1) — Jarang: Lendir Kejutan Air (Tier 2) |
| Vermilion Water Dragonfly | 🐛 Insect / Swarm | 1, Late (Body Refining) | 20 | 14 | Capung merah berukuran lengan di atas ladang herba Dewflower. | Umum: Sayap Capung Merah (Tier 1) — Jarang: Mata Capung Vermilion (Tier 1) |
| Bog Crocodile Young | 🐺 Spirit Beast | 1, Late (Body Refining) | 75 | 12 | Anak buaya lumpur yang berburu mangsa kecil di rawa dangkal. | Umum: Kulit Buaya Muda (Tier 1) — Jarang: Taring Buaya Kecil (Tier 1) |
| Red Stream Salamander | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Kadal amfibi berwarna merah di tebing air terjun Lembah Embun. | Umum: Kulit Salamander Merah (Tier 1) — Jarang: Darah Salamander Air (Tier 2) |
| Marsh Water Spider | 🐛 Insect / Swarm | 2, Mid (Qi Gathering) | 150 | 67 | Laba-laba air pembentang jaring bening di permukaan sungai. | Umum: Benang Jaring Air (Tier 1) — Jarang: Kelenjar Jaring Sungai (Tier 2) |
| Mud Snail Spirit | 🐺 Spirit Beast | 1, Mid (Body Refining) | 37 | 6 | Siput raksasa bercangkang tebal di rawa teratai. Bergerak lambat. | Umum: Cangkang Siput Lumpur (Tier 1) — Jarang: Daging Siput Ber-Qi (Tier 1) |
| Ancient Vermilion Carp Boss | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 15.625 | 4.687 | Karper purba raksasa berumur 500 tahun di dasar Lembah Embun Merah. | Legendaris: Sisik Karper Purba Vermilion (Tier 5, bahan obat Sheng-Grade) |
| Vermilion River Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.125 | 337 | Anak naga sungai ber-Qi air murni yang meliuk di arus deras Vermilion. | Umum: Sisik Naga Sungai (Tier 3) — Jarang: Inti Air Naga Muda (Tier 3) |
| Vermilion Water Heron | 🐺 Spirit Beast | 1, Late (Body Refining) | 50 | 15 | Bangau bersayap kemerahan pemangsa ikan spiritual di muara sungai. | Umum: Bulu Bangau Merah (Tier 1) — Jarang: Paruh Bangau Sungai (Tier 1) |
| Jade Shell River Turtle | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 243 | 42 | Kura-kura air tawar cangkang hijau tebal di dasar batu kali. | Umum: Cangkang Kura Giok (Tier 2) — Jarang: Darah Kura Air Tawar (Tier 2) |
| Vermilion River Turtle Purba | 🗿 Mitos / Sovereign | 7, Peak (Void Refinement) | 1.464.843 | 292.968 | Kura-kura raksasa purba seukuran pulau penyangga muara Sungai Vermilion. | Legendaris: Cangkang Kura Purba Mitos (Tier 7, bahan formasi pertahanan utama) |

---

### ⛰️ 6.3 Blackstone Skyreach (`03`) — 24 Spesies
*(Rujukan: `03_BLACKSTONE_SKYREACH.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Iron-Eating Beetle | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 187 | 30 | Kumbang pemakan bijih besi di Gua Tambang Kuno. Menggerogoti zirah besi. | Umum: Cangkang Besi Hitam (Tier 1) — Jarang: Inti Kumbang Logam (Tier 2) |
| Cliff Falcon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 45 | Elang tebing bertepi sayap sekeras baja di Benteng Skyreach. | Umum: Bulu Baja Tebing (Tier 1) — Jarang: Cakar Elang Logam (Tier 2) |
| Stone Ridge Ape | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 468 | 75 | Kera raksasa bertubuh batu hitam penghuni Lembah Anvil. | Umum: Kulit Batu Kera (Tier 2) — Jarang: Batu Inti Magnetik (Tier 3) |
| Ironclad Bear | 🐺 Spirit Beast | 4, Early (Core Formation) | 4.687 | 750 | Beruang raksasa berdaging sekeras Cold Steel di Zona Inti Gua Tambang. | Umum: Empedu Beruang Alkimia (Tier 3) — Jarang: Kulit Besi Purba (Tier 4) |
| Golem Batu Hitam Purba | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 23.437 | 3.750 | Golem pelindung peninggalan penempa purba di kedalaman 3.000 meter. | Legendaris: Kristal Inti Bumi Purba (Tier 5, bahan zirah Tian-Grade) |
| Deep Steel Bat | 🦇 Spirit Beast / Swarm | 2, Mid (Qi Gathering) | 125 | 54 | Kelelawar cakar baja di lorong gua tambang bawah tanah. | Umum: Sayap Kelelawar Besi (Tier 1) — Jarang: Taring Steel Bat (Tier 2) |
| Magnet Ore Ant | 🐛 Insect / Swarm | 2, Late (Qi Gathering) | 250 | 48 | Kawanan semut pengangkut kristal magnetik di Zona Inti Gua Tambang. | Umum: Cangkang Semut Magnet (Tier 2) — Jarang: Serbuk Kristal Magnetik (Tier 2) |
| Ridge Lizard | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 187 | 30 | Kadal tebing perayap tebing batu terjal. Kulitnya menyerupai batu hitam. | Umum: Sisik Kadal Batu (Tier 1) — Jarang: Ekstrasi Kulit Batu (Tier 2) |
| Mountain Goat Iron | 🐺 Spirit Beast | 1, Peak (Body Refining) | 93 | 15 | Kambing gunung bertanduk besi keras di lereng Benteng Skyreach. | Umum: Daging Kambing Gunung (Tier 1) — Jarang: Tanduk Besi Kambing (Tier 1) |
| Boulder Turtle | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 703 | 112 | Penyu raksasa bertumpu cangkang batu tebal di Ngarai Batu Hitam Kelam. | Umum: Cangkang Batu Raksasa (Tier 2) — Jarang: Inti Bumi Penyu (Tier 3) |
| Rock Mantis | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Belalang sembah berbilah tangan sekeras batu pahat di Anvil Valley. | Umum: Bilah Tangan Mantis (Tier 1) — Jarang: Cangkang Mantis Batu (Tier 2) |
| Heavy Ore Scorpion | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 468 | 75 | Kalajengking bercangkang mineral berat di lorong tambang terlarang. | Umum: Cangkang Kalajengking Besi (Tier 2) — Jarang: Sengat Logam Berat (Tier 3) |
| Black Crag Panther | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Macan tutul berkulit hitam kelam di lereng tebing terjal perbatasan. | Umum: Kulit Macan Batu (Tier 2) — Jarang: Cakar Hitam Crag (Tier 3) |
| Ore-Gazer Owl | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 45 | Burung hantu ber-Mata kristal yang mendeteksi lokasi bijih logam murni. | Umum: Bulu Hantu Tambang (Tier 1) — Jarang: Mata Kristal Penambang (Tier 2) |
| Stone Wall Serpent | 🐺 Spirit Beast | 3, Late (Foundation Est.) | 625 | 150 | Ular batu meliuk di celah dinding gua tambang. Sisik sekeras batu tempa. | Umum: Sisik Ular Batu (Tier 2) — Jarang: Inti Bumi Ular (Tier 3) |
| Subterranean Mole | 🐺 Spirit Beast | 1, Late (Body Refining) | 56 | 12 | Tikus tahi lalat penggali lorong gua tambang bawah tanah. | Umum: Kulit Tikus Tambang (Tier 1) — Jarang: Cakar Penggali Batu (Tier 1) |
| Mountain Ridge Eagle | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 312 | 168 | Elang puncak pegunungan penyergap kambing batu dari udara. | Umum: Bulu Elang Gunung (Tier 2) — Jarang: Paruh Elang Batu (Tier 3) |
| Iron-Spined Porcupine | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 48 | Landak berduri duri besi tajam di lereng Pos Jembatan Rantai. | Umum: Duri Besi Landak (Tier 2) — Jarang: Kulit Duri Logam (Tier 2) |
| Magnet Golem Small | 🗿 Elemental | 3, Early (Foundation Est.) | 468 | 75 | Golem magnetik kecil buatan formasi pelindung tungku tempa purba. | Umum: Batu Magnetik Tempa (Tier 2) — Jarang: Inti Magnetik Kecil (Tier 3) |
| Deep Iron Centipede Purba | 🐛 Insect / Boss | 5, Early (Nascent Soul) | 23.437 | 3.750 | Lipan purba sepanjang 20 meter di Zona Inti Gua Tambang Kuno. | Legendaris: Cangkang Lipan Besi Purba (Tier 5, bahan zirah Sheng-Grade) |
| Blackstone Earth Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.687 | 281 | Anak naga bumi bersisik batu hitam tebal penghuni jurang tambang dalam. | Umum: Sisik Naga Batu Hitam (Tier 3) — Jarang: Tanduk Naga Bumi Muda (Tier 3) |
| Mountain Ridge Cliff Hawk | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 187 | 75 | Elang raksasa penyergap penambang di celah batu tinggi. | Umum: Bulu Elang Tebing (Tier 2) — Jarang: Cakar Tebing Hitam (Tier 2) |
| Deep Cavern Ore Spider | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 187 | 37 | Laba-laba pemakan bijih besi ber-Qi di lorong bawah tanah. | Umum: Benang Kawat Besi (Tier 1) — Jarang: Kelenjar Bijih Besi (Tier 2) |
| Skyreach Mountain Behemoth | 🗿 Mitos / Sovereign | 8, Early (Dao Integration) | 3.906.250 | 878.906 | Behemoth titan batu raksasa penghuni inti Gunung Blackstone Skyreach. | Legendaris: Inti Bumi Purba Behemoth (Tier 8, bahan artefak tanah Sheng-Grade) |

---

### 🏜️ 6.4 Ashen Sun Expanse (`04`) — 24 Spesies
*(Rujukan: `04_ASHEN_SUN_EXPANSE.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Dune Camel Wild | 🐺 Spirit Beast | 1, Early (Body Refining) | 22 | 9 | Unta liar gurun pasir penyimpan air spiritual. Pasif. | Umum: Daging Unta Gurun (Tier 1) — Jarang: Punuk Air Spiritual (Tier 1) |
| Flame-Viper | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 101 | 48 | Ular pasir merah bersisik panas penyuntik racun Dantian. | Umum: Kulit Ular Api (Tier 1) — Jarang: Kelenjar Racun Api Gurun (Tier 2) |
| Sun Lizard | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 101 | 58 | Kadal raksasa pemakan kristal api di Benteng Sandgate. | Umum: Sisik Kadal Sunfire (Tier 1) — Jarang: Inti Api Kecil (Tier 2) |
| Sandstorm Scorpion | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 253 | 146 | Kalajengking pasir sebesar kuda di Reruntuhan Buried Sun. | Umum: Cangkang Kalajengking Gurun (Tier 2) — Jarang: Sengat Racun Api (Tier 3) |
| Cacing Pasir Purba (Dune Worm) | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 105.468 | 30.468 | Cacing pasir purba 50 meter penyergap karavan dari bawah tanah. | Legendaris: Kulit Cacing Pasir Purba (Tier 6, bahan zirah Di-Grade) |
| Ash Cobra | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 135 | 73 | Kobra abu-abu bersembunyi di bawah debu panas rute karavan. | Umum: Kulit Kobra Abu (Tier 2) — Jarang: Bisa Kobra Surya (Tier 2) |
| Flame Ant Swarm | 🐛 Insect / Swarm | 1, Late (Body Refining) | 45 | 14 | Kawanan semut api penggali bukit pasir ber-Qi surya. | Umum: Cangkang Semut Api (Tier 1) — Jarang: Esens Api Semut (Tier 1) |
| Sun-Baked Eagle | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 253 | 146 | Elang gurun bercakar tajam penembus angin badai pasir. | Umum: Bulu Elang Surya (Tier 2) — Jarang: Cakar Api Elang (Tier 3) |
| Desert Hyena | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 101 | 48 | Hiena gurun berburu dalam kawanan 4–8 ekor di Lembah Pasir Merah. | Umum: Bulu Hiena Gurun (Tier 1) — Jarang: Taring Hiena Api (Tier 2) |
| Sunfire Salamander | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 379 | 219 | Salamander pemukim cairan pasir panas Sunfire Oasis. | Umum: Kulit Salamander Surya (Tier 2) — Jarang: Kelenjar Api Murni (Tier 3) |
| Quicksand Spider | 🐛 Insect / Swarm | 2, Mid (Qi Gathering) | 101 | 58 | Laba-laba pembuat sumur pasir hisap jebakan karavan. | Umum: Benang Pasir Isap (Tier 1) — Jarang: Kelenjar Racun Pasir (Tier 2) |
| Ash Vulture | 🐺 Spirit Beast | 1, Mid (Body Refining) | 22 | 11 | Burung pemakan bangkai di perbatasan Sandgate Post. | Umum: Bulu Burung Abu (Tier 1) — Jarang: Paruh Burung Gurun (Tier 1) |
| Dune Beetle | 🐛 Insect / Swarm | 1, Early (Body Refining) | 22 | 9 | Kumbang pendorong bola pasir panas di bukit pasir lepas. | Umum: Cangkang Kumbang Pasir (Tier 1) — Jarang: Serbuk Pasir Panas (Tier 1) |
| Sunfire Fox | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 135 | 73 | Rubah gurun berbulu emas pemikat ilusi fatamorgana. | Umum: Bulu Rubah Emas (Tier 2) — Jarang: Inti Ilusi Surya (Tier 2) |
| Flame Centipede Desert | 🐛 Insect / Swarm | 3, Mid (Foundation Est.) | 379 | 219 | Lipan api sepanjang 2 meter di Lembah Pasir Merah Kelam. | Umum: Cangkang Lipan Api (Tier 2) — Jarang: Sengat Api Lipan (Tier 3) |
| Sand-Prowler Cat | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 101 | 48 | Kucing liar gurun berlipat telinga penyergap burung pasir. | Umum: Bulu Kucing Gurun (Tier 1) — Jarang: Cakar Pasir Kucing (Tier 2) |
| Solar Chameleon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 101 | 58 | Bunglon gurun pembelok cahaya matahari penyamar diri. | Umum: Kulit Bunglon Surya (Tier 1) — Jarang: Esens Cahaya Bunglon (Tier 2) |
| Ash Rat Swarm | 🐛 Insect / Swarm | 1, Early (Body Refining) | 22 | 9 | Tikus abu gurun penggerogoti bahan bekal karavan. | Umum: Kulit Tikus Abu (Tier 1) — Jarang: Gigi Tikus Gurun (Tier 1) |
| Sunstone Golem Small | 🗿 Elemental | 3, Early (Foundation Est.) | 253 | 146 | Golem batu surya buatan Gua Reruntuhan Altar Api Purba. | Umum: Batu Surya Tempa (Tier 2) — Jarang: Inti Kristal Surya (Tier 3) |
| Flame Scorpion King Boss | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 14.062 | 6.093 | Raja kalajengking api purba penghuni Reruntuhan Buried Sun Palace. | Legendaris: Sengat Raja Kalajengking Purba (Tier 5, bahan senjata Di-Grade) |
| Sunfire Desert Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.012 | 450 | Anak naga padang pasir penyembur nafas api surya di gundukan pasir merah. | Umum: Sisik Naga Api Gurun (Tier 3) — Jarang: Kantong Api Naga Surya (Tier 3) |
| Sandstorm Vulture | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 125 | 56 | Burung pemakan bangkai ber-Qi panas penghuni bukit pasir. | Umum: Bulu Burung Pasir (Tier 1) — Jarang: Paruh Burung Gurun (Tier 2) |
| Desert Flame Viper | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 125 | 75 | Ular pasir berbisa menyengat yang bersembunyi di dalam pasir panas. | Umum: Kulit Ular Api (Tier 2) — Jarang: Bisa Api Gurun (Tier 2) |
| Ashen Phoenix Purba | 🗿 Mitos / Sovereign | 8, Late (Dao Integration) | 4.218.750 | 2.109.375 | Burung Phoenix api legendaris pemancar gelombang panas abadi Gurun Ashen Sun. | Legendaris: Bulu Phoenix Api Mitos (Tier 8, bahan piro-alkimia Sheng-Grade) |

---

### 🌿 6.5 Nine-Reed Mire (`05`) — 24 Spesies
*(Rujukan: `05_NINE_REED_MIRE.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Mud Leech | 🐛 Insect / Swarm | 1, Early (Body Refining) | 20 | 10 | Lintah mikro di Desa Mirewood. Penghisap Stamina (-10/jam). | Umum: Cairan Lintah Rawa (Tier 1) — Jarang: Esens Darah Lintah (Tier 1) |
| Swamp Toad | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 100 | 42 | Kodok raksasa penyembur lendir asam beracun perusak zirah. | Umum: Lendir Kodok Rawa (Tier 1) — Jarang: Kelenjar Racun Kodok (Tier 2) |
| Giant Poison Centipede | 🐛 Insect / Gu Swarm | 3, Early (Foundation Est.) | 250 | 131 | Lipan beracun 3 meter di Gua Sarang Serangga Spiritual. | Umum: Cangkang Duri Lipan (Tier 2) — Jarang: Inti Racun Lipan (Tier 3) |
| Miasma Python | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 375 | 196 | Ular miasma raksasa di Labirin Alang-Alang Sembilan. Melilit target. | Umum: Kulit Ular Miasma (Tier 2) — Jarang: Kantong Racun Murni (Tier 3) |
| Miasma Eel Purba | 🐺 Spirit Beast | 4, Early (Core Formation) | 2.500 | 1.312 | Belut listrik beracun di Reruntuhan Benteng Ular. Semburan listrik. | Umum: Kulit Belut Miasma (Tier 3) — Jarang: Inti Belut Beracun Tier 4 (Tier 4) |
| Toxic Mosquito Swarm | 🐛 Insect / Swarm | 1, Late (Body Refining) | 40 | 14 | Kawanan nyamuk rawa penyebar demam miasma di tepi rawa. | Umum: Sayap Nyamuk Rawa (Tier 1) — Jarang: Jarum Nyamuk Beracun (Tier 1) |
| Bog Crocodile | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 250 | 131 | Buaya rawa berlumut hijau di Rawa Teratai Kelam. | Umum: Kulit Buaya Rawa (Tier 2) — Jarang: Taring Buaya Miasma (Tier 3) |
| Violet Reed Serpent | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 133 | 65 | Ular bersisik ungu di antara semak alang-alang raksasa. | Umum: Kulit Ular Ungu (Tier 2) — Jarang: Bisa Ular Alang (Tier 2) |
| Mud Spider | 🐛 Insect / Swarm | 2, Mid (Qi Gathering) | 100 | 52 | Laba-laba pembentang jaring racun lumpur di pohon rawa. | Umum: Benang Jaring Lumpur (Tier 1) — Jarang: Kelenjar Racun Lumpur (Tier 2) |
| Rotting Willow Sentinel | 🌿 Flora / Plant Creature | 3, Mid (Foundation Est.) | 375 | 196 | Pohon dedalu busuk hidup penghuni Pos Rawa Beracun. | Umum: Kayu Dedalu Busuk (Tier 2) — Jarang: Biji Dedalu Miasma (Tier 3) |
| Poisonous Marsh Slug | 🐛 Insect / Swarm | 1, Mid (Body Refining) | 20 | 10 | Siput pelendir racun gatal perayap dahan rawa. | Umum: Lendir Siput Rawa (Tier 1) — Jarang: Esens Racun Siput (Tier 1) |
| Mire Crane | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 100 | 42 | Burung bangau pemakan lintah beracun di muara rawa. | Umum: Bulu Bangau Rawa (Tier 1) — Jarang: Paruh Bangau Beracun (Tier 2) |
| Black Water Snail | 🐺 Spirit Beast | 1, Late (Body Refining) | 40 | 10 | Siput cangkang hitam penyerap Qi air beracun di lumpur. | Umum: Cangkang Siput Hitam (Tier 1) — Jarang: Esens Air Rawa (Tier 1) |
| Swamp Lizard | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 100 | 52 | Kadal amfibi bersisik hijau tua di tepi perairan tenang. | Umum: Kulit Kadal Rawa (Tier 1) — Jarang: Kelenjar Kadal Beracun (Tier 2) |
| Green Gu Beetle | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 100 | 42 | Kumbang racun Gu pelubang kayu pohon rawa tua. | Umum: Cangkang Kumbang Gu (Tier 1) — Jarang: Serbuk Gu Hijau (Tier 2) |
| Mire Rat | 🐺 Spirit Beast | 1, Early (Body Refining) | 20 | 7 | Tikus rawa pembawa kuman penyakit di desa pemukiman. | Umum: Kulit Tikus Rawa (Tier 1) — Jarang: Gigi Tikus Beracun (Tier 1) |
| Bog Hydra Small | 🐺 Spirit Beast | 4, Early (Core Formation) | 2.500 | 1.312 | Ular kepala tiga kecil penghuni Zona Inti Rawa Sembilan. | Umum: Sisik Hydra Rawa (Tier 3) — Jarang: Inti Hydra Beracun Tier 4 (Tier 4) |
| Toxic Marsh Crab | 🐺 Spirit Beast | 1, Late (Body Refining) | 40 | 10 | Kepiting rawa bersupit racun korosif perusak logam. | Umum: Supit Kepiting Rawa (Tier 1) — Jarang: Cangkang Racun Crab (Tier 1) |
| Miasma Firefly Swarm | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 100 | 42 | Kawanan kunang-kunang rawa pemancar cahaya racun ilusi. | Umum: Serbuk Cahaya Rawa (Tier 1) — Jarang: Kelenjar Ilusi Miasma (Tier 2) |
| Purba Miasma Serpent Boss | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 105.468 | 32.812 | Ular purba raksasa penghuni inti Labirin Alang-Alang Sembilan. | Legendaris: Sisik Ular Purba Miasma (Tier 6, bahan zirah Sheng-Grade) |
| Poison Miasma Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 900 | 421 | Anak naga miasma bersisik hijau kehitaman penghuni rawa terlarang. | Umum: Sisik Naga Miasma (Tier 3) — Jarang: Inti Racun Naga Rawa (Tier 3) |
| Violet Swamp Toad | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 150 | 45 | Kodok racun warna ungu pelempar asam korosif di rawa dalam. | Umum: Lendir Kodok Ungu (Tier 1) — Jarang: Kelenjar Acid Purple (Tier 2) |
| Mud Miasma Swarm | 🐛 Insect / Swarm | 1, Late (Body Refining) | 35 | 12 | Kawanan serangga rawa pemakan Qi di balik rumpun alang-alang. | Umum: Sayap Serangga Rawa (Tier 1) — Jarang: Serbuk Miasma Green (Tier 1) |
| Nine-Headed Hydra Mitos | 🗿 Mitos / Sovereign | 7, Late (Void Refinement) | 625.000 | 351.562 | Hydra sembilan kepala purba penghuni titik terlarang Labirin Alang-Alang Sembilan. | Legendaris: Inti Racun Sembilan Kepala Mitos (Tier 7, bahan obat Sheng-Grade) |

---

### 🌊 6.6 Astral Tide Sea (`06`) — 24 Spesies
*(Rujukan: `06_ASTRAL_TIDE_SEA.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Star-Crab | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Kepiting pantai bersinar bercahaya bintang di Kepulauan Coral. | Umum: Cangkang Kepiting Bintang (Tier 1) — Jarang: Mutiara Bintang Kecil (Tier 1) |
| Spotted Coral Shark | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Hiu karang pencium darah di Benteng Pulau Coral. | Umum: Kulit Hiu Karang (Tier 1) — Jarang: Gigi Hiu Bintang (Tier 2) |
| Sea Serpent | 🐺 Spirit Beast | 4, Early (Core Formation) | 3.125 | 937 | Ular laut raksasa di Zona Arus Bintang Palung Abyss. | Umum: Sisik Ular Laut Bintang (Tier 3) — Jarang: Inti Mutiara Samudra (Tier 4) |
| Astral Whale Purba | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 78.125 | 23.437 | Paus purba raksasa 100 meter di Zona Palung Gelap. | Legendaris: Tulang Paus Bintang Purba (Tier 6, bahan perahu Lingzhou) |
| Tide Jellyfish | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Ubur-ubur bercahaya bintang pemancar sengatan listrik cair. | Umum: Lendir Ubur-Ubur (Tier 1) — Jarang: Esens Listrik Bintang (Tier 2) |
| Coral Turtle | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Penyu berselimut karang bercahaya di terumbu laut dangkal. | Umum: Cangkang Karang Laut (Tier 1) — Jarang: Mutiara Karang Bintang (Tier 2) |
| Starfire Flying Fish | 🐺 Spirit Beast | 1, Late (Body Refining) | 32 | 10 | Ikan terbang pemancar percikan cahaya bintang di atas gelombang. | Umum: Daging Ikan Terbang (Tier 1) — Jarang: Sayap Ikan Bintang (Tier 1) |
| Abyssal Octopus | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Gurita raksasa lengan tentakel penarik perahu di Palung Bintang. | Umum: Tentakel Gurita Laut (Tier 2) — Jarang: Tinta Hitam Abiss (Tier 3) |
| Flying Ray Astral | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 75 | Ikan pari melayang pembelah udara pantai Star-Compass Port. | Umum: Kulit Pari Bintang (Tier 2) — Jarang: Duri Pari Bintang (Tier 2) |
| Shell Guardian | 🗿 Ancient Guardian | 3, Early (Foundation Est.) | 312 | 93 | Golem cangkang kerang purba pelindung Reruntuhan Sunken Citadel. | Umum: Cangkang Purba Kerang (Tier 2) — Jarang: Mutiara Purba Samudra (Tier 3) |
| Deep-Sea Eel | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Belut laut dalam bertaring tajam di Zona Arus Bintang. | Umum: Kulit Belut Laut (Tier 2) — Jarang: Inti Air Bawah Laut (Tier 3) |
| Sea Anemone Spirit | 🌿 Flora / Creature | 2, Mid (Qi Gathering) | 187 | 56 | Anemon laut penembak jarum racun bius di terumbu karang. | Umum: Lendir Anemon Laut (Tier 1) — Jarang: Jarum Bius Anemon (Tier 2) |
| Blue Wave Dolphin | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 37 | Lumba-lumba penuntun perahu kargo yang ramah pada pelaut. | Umum: Kulit Lumba-Lumba (Tier 1) — Jarang: Inti Gelombang Laut (Tier 2) |
| Star-Claw Sea Otter | 🐺 Spirit Beast | 1, Mid (Body Refining) | 25 | 9 | Berang-berang laut pemecah cangkang kepiting bintang di pantai. | Umum: Bulu Berang Laut (Tier 1) — Jarang: Cakar Bintang Otter (Tier 1) |
| Astral Barracuda | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Ikan barakuda perenang cepat dalam kawanan penyerang perahu. | Umum: Daging Barakuda Bintang (Tier 1) — Jarang: Gigi Barakuda Laut (Tier 2) |
| Abyssal Sea Urchin | 🐛 Creature / Swarm | 1, Late (Body Refining) | 32 | 10 | Bulu babi berduri racun tajam di dasar terumbu karang. | Umum: Duri Bulu Babi (Tier 1) — Jarang: Esens Racun Urchin (Tier 1) |
| Tidal Water Elemental | 🔥 Elemental | 3, Mid (Foundation Est.) | 468 | 140 | Gumpalan elemental air pasang di perairan badai astral. | Umum: Batu Air Pasang (Tier 2) — Jarang: Inti Elemental Air (Tier 3) |
| Coral Mantis Shrimp | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 75 | Udang mantis bersupit pemicu ledakan tekanan air jarak dekat. | Umum: Cangkang Udang Mantis (Tier 2) — Jarang: Supit Pemecah Karang (Tier 2) |
| Manta Ray Purba | 🐺 Spirit Beast | 4, Early (Core Formation) | 3.125 | 937 | Pari purba bentang sayap 15 meter di kedalaman 600 meter. | Umum: Kulit Pari Purba (Tier 3) — Jarang: Inti Manta Bintang Tier 4 (Tier 4) |
| Kraken Palung Gelap Boss | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 78.125 | 23.437 | Monster cumi-cumi purba tentakel raksasa pemotong kapal perang. | Legendaris: Inti Samudra Purba Kraken (Tier 6, bahan artefak Sheng-Grade) |
| Astral Sea Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.125 | 337 | Anak naga laut bersisik cahaya bintang di perairan terumbu karang. | Umum: Sisik Naga Laut Bintang (Tier 3) — Jarang: Mutiara Naga Astral Muda (Tier 3) |
| Coral Reef Guardian Crab | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 150 | 45 | Kepiting raksasa berzirah karang keras penunggu dasar laut. | Umum: Cangkang Karang Keras (Tier 2) — Jarang: Supit Karang Bintang (Tier 2) |
| Astral Jellyfish Swarm | 🐛 Creature / Swarm | 2, Mid (Qi Gathering) | 112 | 33 | Kawanan ubur-ubur bintang pemancar aliran listrik penenang. | Umum: Lendir Bintang Laut (Tier 1) — Jarang: Kelenjar Listrik Astral (Tier 2) |
| Leviathan Astral Purba | 🗿 Mitos / Sovereign | 8, Mid (Dao Integration) | 3.515.625 | 1.318.359 | Leviathan bintang purba raksasa penyeimbang arus samudra astral Qianyuan. | Legendaris: Inti Bintang Mitos Leviathan (Tier 8, bahan kapal perang Sheng-Grade) |

---

### 🌲 6.7 Whispering Root Forest (`07`) — 24 Spesies
*(Rujukan: `07_WHISPERING_ROOT_FOREST.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Wood-Deer | 🐺 Spirit Beast | 1, Early (Body Refining) | 32 | 7 | Rusa spiritual berdaun hijau di Zona Luar Kanopi. Pasif. | Umum: Daging Rusa Herbal (Tier 1) — Jarang: Tanduk Kayu Serat (Tier 1) |
| Green Vine Snake | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 35 | Ular hijau tersamar dahan di Zona Tengah. Penyergap cepat. | Umum: Kulit Ular Dahan (Tier 1) — Jarang: Bisa Kayu Penenang (Tier 2) |
| Emerald Panther | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 243 | 53 | Macan tutul giok pemangsa cepat di jalur kanopi. *Stealth Attack*. | Umum: Kulit Macan Giok (Tier 2) — Jarang: Cakar Emerald Sharp (Tier 2) |
| Spore Wood Sentinel | 🌿 Flora / Plant Creature | 3, Early (Foundation Est.) | 406 | 89 | Pohon monster penembak spora beracun di Lembah Spora Hijau. | Umum: Kayu Spora Purba (Tier 2) — Jarang: Biji Spora Hijau Murni (Tier 3) |
| Ancient Bear | 🐺 Spirit Beast | 4, Early (Core Formation) | 4.062 | 890 | Beruang purba pelindung World Tree Sanctuary. Gelombang akar. | Umum: Empedu Beruang Purba (Tier 3) — Jarang: Inti Kehidupan Kayu Tier 4 (Tier 4) |
| Moss Bear | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 325 | 45 | Beruang berselimut lumut hijau di Zona Luar Kanopi. | Umum: Kulit Beruang Lumut (Tier 2) — Jarang: Empedu Beruang Kayu (Tier 2) |
| Vine Ape | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 243 | 53 | Kera perayap akar raksasa di Zona Tengah Whispering Root. | Umum: Bulu Kera Akar (Tier 1) — Jarang: Taring Kera Hutan (Tier 2) |
| Treant Sentinel | 🌿 Flora / Plant Creature | 3, Mid (Foundation Est.) | 609 | 134 | Monster pohon bergerak pelindung reruntuhan Kuil Akar Purba. | Umum: Kayu Serat Giok (Tier 2) — Jarang: Teras Kayu Purba (Tier 3) |
| Bark Beetle | 🐛 Insect / Swarm | 1, Late (Body Refining) | 48 | 12 | Kumbang penggerogoti kulit pohon purba di Pos Pengawas Kanopi. | Umum: Cangkang Kumbang Kayu (Tier 1) — Jarang: Serbuk Serangga Kayu (Tier 1) |
| Spirit Owl | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 35 | Burung hantu ber-Mata hijau pemantau hutan malam hari. | Umum: Bulu Hantu Hutan (Tier 1) — Jarang: Mata Hantu Kayu (Tier 2) |
| Green Canopy Hawk | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 325 | 67 | Elang penembak bulu daun tajam dari puncak kanopi pohon. | Umum: Bulu Elang Kanopi (Tier 2) — Jarang: Cakar Elang Giok (Tier 2) |
| Root-Bound Wolf | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 243 | 53 | Serigala bersimbiosis dengan akar kayu di perbatasan Desa Root-Bound. | Umum: Bulu Serigala Akar (Tier 1) — Jarang: Taring Kayu Serigala (Tier 2) |
| Leaf-Winged Butterfly | 🐛 Insect / Swarm | 1, Early (Body Refining) | 32 | 7 | Kupu-kupu penyesat pandangan ber-Qi penenang di kebun herbal. | Umum: Serbuk Sayap Kupu (Tier 1) — Jarang: Esens Bunga Hutan (Tier 1) |
| Forest Wild Boar | 🐺 Spirit Beast | 1, Late (Body Refining) | 48 | 12 | Babi hutan bertanduk kayu keras di semak belukar liar. | Umum: Daging Babi Hutan (Tier 1) — Jarang: Taring Kayu Babi (Tier 1) |
| Wood Chameleon | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 162 | 35 | Bunglon pohon pemutar warna kulit penyamar diri di dahan. | Umum: Kulit Bunglon Kayu (Tier 1) — Jarang: Kelenjar Ilusi Pohon (Tier 2) |
| Poisonous Mushroom Creature | 🌿 Flora / Creature | 2, Mid (Qi Gathering) | 243 | 53 | Jamur monster pelempar kabut spora pemicu pengurasan *Stamina -15*. | Umum: Batang Jamur Spora (Tier 1) — Jarang: Esens Racun Jamur (Tier 2) |
| Canopy Squirrel | 🐺 Spirit Beast | 1, Mid (Body Refining) | 32 | 9 | Tupai lincah pengumpul biji tanaman obat spiritual. | Umum: Bulu Tupai Kanopi (Tier 1) — Jarang: Biji Obat Simpanan (Tier 1) |
| Emerald Snake Small | 🐺 Spirit Beast | 1, Late (Body Refining) | 48 | 12 | Anak ular giok bersisik bening di rawa kecil hutan. | Umum: Kulit Ular Giok Kecil (Tier 1) — Jarang: Bisa Giok Muda (Tier 1) |
| Ancient Tree Guardian Boss | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 20.312 | 3.750 | Pelindung purba berbentuk pohon raksasa 30 meter di Sanctuary. | Legendaris: Teras Kayu Purba World Tree (Tier 5, bahan tongkat Sheng-Grade) |
| Great Emerald Panther King Boss | 🐺 Spirit Beast / Boss | 4, Mid (Core Formation) | 6.093 | 1.335 | Raja macan giok purba pemimpin kawanan panther Zona Inti. | Legendaris: Inti Macan Giok Purba Tier 4 (Tier 4, bahan artefak Di-Grade) |
| Verdant Wood Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.462 | 337 | Anak naga kayu bersisik serat daun giok penghuni rimba suci Whispering Root. | Umum: Sisik Naga Kayu Purba (Tier 3) — Jarang: Darah Naga Life Qi (Tier 3) |
| Ancient Tree Bark Beetle | 🐛 Insect / Swarm | 2, Mid (Qi Gathering) | 146 | 33 | Kumbang raksasa pelubang kayu pohon purba penyerap getah spiritual. | Umum: Cangkang Kumbang Kayu (Tier 1) — Jarang: Serbuk Getah Purba (Tier 2) |
| Whispering Moss Panther | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 195 | 45 | Macan tutul berselimut lumut hijau berjalan tanpa suara di kanopi hutan. | Umum: Kulit Macan Lumut (Tier 2) — Jarang: Cakar Bisikan Kayu (Tier 2) |
| World Tree Dragon Sovereign Purba | 🗿 Mitos / Sovereign | 8, Peak (Dao Integration) | 7.628.906 | 1.757.812 | Naga Kayu Mitos purba raksasa penjaga urat kehidupan Pohon Dunia Qianyuan. | Legendaris: Teras Naga Kayu Mitos (Tier 8, bahan artefak kehidupan Sheng-Grade) |

---

### ❄️ 6.8 Frostglass Crown (`08`) — 24 Spesies
*(Rujukan: `08_FROSTGLASS_CROWN.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Ice-Crystal Wolf | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Serigala es berbulu bening di Desa Gletser Bening. Berburu kawanan. | Umum: Bulu Serigala Es (Tier 2) — Jarang: Kristal Es Serigala (Tier 3) |
| Frost Snow Ape | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Kera salju raksasa di tebing gletser terjal. Melempar es keras. | Umum: Kulit Kera Salju (Tier 2) — Jarang: Taring Es Abadi (Tier 3) |
| Glacier Eagle | 🐺 Spirit Beast | 3, Late (Foundation Est.) | 625 | 187 | Elang raksasa bercakar kristal es penembus badai salju. | Umum: Bulu Elang Gletser (Tier 2) — Jarang: Cakar Kristal Es (Tier 3) |
| Frostglass Centipede | 🐛 Insect / Gu Swarm | 4, Early (Core Formation) | 3.125 | 937 | Lipan es bening sekeras kaca di Gua Meditasi Inti Es. | Umum: Cangkang Kaca Es (Tier 3) — Jarang: Inti Es Purba Tier 4 (Tier 4) |
| Eternal Snow Leopard | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Macan tutul salju pemicu pendarahan dingin *Chill Effect*. | Umum: Kulit Macan Salju (Tier 2) — Jarang: Cakar Es Abadi (Tier 3) |
| Ice Core Golem | 🗿 Elemental | 4, Early (Core Formation) | 3.125 | 937 | Golem buatan dari kristal es purba di Reruntuhan Menara Pedang. | Umum: Batu Kristal Es (Tier 3) — Jarang: Inti Golem Es Tier 4 (Tier 4) |
| Blizzard Owl | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 75 | Burung hantu salju ber-Mata bening pemicu angin badai es. | Umum: Bulu Hantu Salju (Tier 2) — Jarang: Mata Kristal Es (Tier 2) |
| Frost Mammoth | 🐺 Spirit Beast | 4, Mid (Core Formation) | 4.687 | 1.406 | Gajah purba berselimut es di lembah salju bawah pemicu gempa es. | Umum: Gading Es Purba (Tier 3) — Jarang: Kulit Mammoth Es (Tier 4) |
| Glacial Spider | 🐛 Insect / Swarm | 3, Early (Foundation Est.) | 312 | 93 | Laba-laba pembentang jaring es bening membekukan di gua. | Umum: Benang Jaring Es (Tier 2) — Jarang: Kelenjar Beku Spider (Tier 3) |
| Cold Steel Beetle | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 125 | 37 | Kumbang cangkang baja dingin pemakan batu gletser abadi. | Umum: Cangkang Baja Cold (Tier 1) — Jarang: Serbuk Es Kumbang (Tier 2) |
| Snow Hare Spirit | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 7 | Kelinci salju lincah perayap lorong gletser bening. Pasif. | Umum: Bulu Kelinci Salju (Tier 1) — Jarang: Daging Kelinci Es (Tier 1) |
| Ice Ridge Fox | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 56 | Rubah salju bertulang bening pemikat ilusi badai dingin. | Umum: Bulu Rubah Salju (Tier 1) — Jarang: Inti Ilusi Es (Tier 2) |
| Frostbite Bat | 🦇 Spirit Beast / Swarm | 2, Late (Qi Gathering) | 250 | 75 | Kelelawar es penarik kehangatan fisik pengembara malam. | Umum: Sayap Kelelawar Es (Tier 2) — Jarang: Kelenjar Pembeku Bat (Tier 2) |
| Glacier Serpent | 🐺 Spirit Beast | 3, Late (Foundation Est.) | 625 | 187 | Ular es panjang meliuk di dalam celah gletser bening licin. | Umum: Sisik Ular Es (Tier 2) — Jarang: Inti Es Gletser (Tier 3) |
| Cold Mist Dragonfly | 🐛 Insect / Swarm | 1, Late (Body Refining) | 32 | 10 | Capung es pembawa uap dingin di Puncak Meditasi Keheningan. | Umum: Sayap Capung Es (Tier 1) — Jarang: Esens Embun Cold (Tier 1) |
| Frozen Sentinel Statues | 🗿 Ancient Guardian | 3, Peak (Foundation Est.) | 781 | 225 | Patung prajurit es pelindung gerbang Benteng Salju Frost-Edge. | Umum: Batu Es Zirah (Tier 2) — Jarang: Inti Patung Es (Tier 3) |
| Snow Stalker Lynx | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 93 | Kucing liar salju pemicu serangan kejutan di semak es. | Umum: Kulit Lynx Salju (Tier 2) — Jarang: Cakar Lynx Gletser (Tier 3) |
| Ice Crystal Stag | 🐺 Spirit Beast | 2, Peak (Qi Gathering) | 312 | 62 | Rusa bertanduk kristal es murni pemikat cahaya malam. | Umum: Daging Rusa Es (Tier 2) — Jarang: Tanduk Kristal Es (Tier 2) |
| Glacial Wurm Small | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 140 | Cacing es gletser pelubang tebing es bening bawah tanah. | Umum: Lendir Beku Wurm (Tier 2) — Jarang: Kulit Cacing Es (Tier 3) |
| Dragon-Ice Purba Boss | 🗿 Ancient Guardian | 6, Early (Soul Formation) | 78.125 | 23.437 | Naga es purba terlelap di kedalaman Gua Meditasi Inti Es Purba. | Legendaris: Sisik Naga Es Purba (Tier 6, bahan zirah Sheng-Grade) |
| Frost-Marrow Ice Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.125 | 337 | Anak naga es bersisik kristal beku di lereng Pegunungan Frostglass. | Umum: Sisik Naga Es Beku (Tier 3) — Jarang: Inti Sumsum Es Naga (Tier 3) |
| Frostglass Snow Leopard | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 150 | 45 | Macan tutul salju berbulu perak penyergap di tengah badai es. | Umum: Bulu Macan Salju (Tier 2) — Jarang: Cakar Kristal Es (Tier 2) |
| Ice-Spire Falcon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 112 | 33 | Elang bersayap kristal es pemotong angin dingin puncak pegunungan. | Umum: Bulu Elang Es (Tier 1) — Jarang: Paruh Kristal Beku (Tier 2) |
| Absolute Zero Glacial Dragon Mitos | 🗿 Mitos / Sovereign | 8, Mid (Dao Integration) | 3.515.625 | 1.318.359 | Naga Es Abadi Mitos penyimpan rahasia pembekuan total di dasar Puncak Frostglass. | Legendaris: Inti Es Abadi Mitos Dragon (Tier 8, bahan artefak es Sheng-Grade) |

---

### 🌪️ 6.9 Hollow Gale Corridor (`09`) — 24 Spesies
*(Rujukan: `09_HOLLOW_GALE_CORRIDOR.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Wind-Runner Swift | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 8 | Burung kecil berkecepatan tinggi di jembatan gantung tali. | Umum: Bulu Angin Cepat (Tier 1) — Jarang: Paruh Burung Swift (Tier 1) |
| Hollow Canyon Lizard | 🐺 Spirit Beast | 2, Early (Qi Gathering) | 125 | 45 | Kadal tebing perayap dinding batu ngarai. Penyamar diri. | Umum: Kulit Kadal Ngarai (Tier 1) — Jarang: Cakar Perayap Tebing (Tier 2) |
| Gale Falcon | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 67 | Elang pemangsa berkecepatan tinggi di Pos Tebing Bisik. | Umum: Bulu Elang Topan (Tier 1) — Jarang: Inti Angin Ngarai (Tier 2) |
| Echo Bat | 🦇 Spirit Beast / Swarm | 2, Late (Qi Gathering) | 250 | 90 | Kelelawar raksasa pemancar serangan *Sonic Disorientation*. | Umum: Sayap Kelelawar Gema (Tier 2) — Jarang: Kelenjar Suara Gema (Tier 2) |
| Sonic Bat Swarm | 🦇 Spirit Beast / Swarm | 2, Early (Qi Gathering) | 125 | 45 | Kawanan kelelawar kecil pemancar getaran gelombang suara. | Umum: Sayap Kelelawar Suara (Tier 1) — Jarang: Serbuk Suara Gema (Tier 2) |
| Cliff Hawk | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 67 | Elang tebing penyergap penjelajah jembatan gantung tali. | Umum: Bulu Elang Tebing (Tier 1) — Jarang: Cakar Hawk Ngarai (Tier 2) |
| Sound-Wave Cicada | 🐛 Insect / Swarm | 1, Late (Body Refining) | 32 | 12 | Tonggeret pemancar derik gema suara pemicu pengurasan *Stamina -10*. | Umum: Sayap Tonggeret Gema (Tier 1) — Jarang: Kelenjar Suara Cicada (Tier 1) |
| Canyon Viper | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 90 | Ular tebing bersembunyi di lubang batu berongga Kota Wind-Gale. | Umum: Kulit Ular Ngarai (Tier 2) — Jarang: Bisa Angin Kobra (Tier 2) |
| Wind-Blade Leopard | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 135 | Macan tutul angin penyergap cepat tanpa getaran suara. | Umum: Kulit Macan Angin (Tier 2) — Jarang: Cakar Wind Blade (Tier 3) |
| Wind Elemental Swarm | 🔥 Elemental | 2, Mid (Qi Gathering) | 187 | 67 | Pusaran elemental angin kecil pemotong pakaian pengembara. | Umum: Batu Angin Topan (Tier 1) — Jarang: Inti Elemental Angin (Tier 2) |
| Canyon Goat Swift | 🐺 Spirit Beast | 1, Mid (Body Refining) | 25 | 10 | Kambing ngarai lincah penjelajah dinding batu curam. | Umum: Daging Kambing Ngarai (Tier 1) — Jarang: Tanduk Kambing Angin (Tier 1) |
| Echo Spider | 🐛 Insect / Swarm | 2, Early (Qi Gathering) | 125 | 45 | Laba-laba pembentang benang getar gema suara di gua batu. | Umum: Benang Getar Gema (Tier 1) — Jarang: Kelenjar Suara Spider (Tier 2) |
| Gale Swallow | 🐺 Spirit Beast | 1, Early (Body Refining) | 25 | 8 | Burung layang-layang pemotong arus angin kencang ngarai. | Umum: Bulu Layang Topan (Tier 1) — Jarang: Paruh Layang Angin (Tier 1) |
| Canyon Gryphon Small | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 468 | 202 | Makhluk garuda kecil berkepala elang bertubuh singa ngarai. | Umum: Bulu Garuda Ngarai (Tier 2) — Jarang: Cakar Garuda Angin (Tier 3) |
| Hollow Stone Golem | 🗿 Ancient Guardian | 3, Late (Foundation Est.) | 625 | 225 | Golem batu berongga pelindung Reruntuhan Menara Angin Purba. | Umum: Batu Berongga Tempa (Tier 2) — Jarang: Inti Golem Angin (Tier 3) |
| Wind-Steed Horse | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 250 | 90 | Kuda liar ber-Qi angin kencang penjelajah dataran tinggi. | Umum: Daging Kuda Angin (Tier 2) — Jarang: Surai Kuda Topan (Tier 2) |
| Sound Serpent | 🐺 Spirit Beast | 3, Early (Foundation Est.) | 312 | 135 | Ular gema pemancar desisan suara gelombang pemotong perisai. | Umum: Sisik Ular Suara (Tier 2) — Jarang: Kelenjar Desis Gema (Tier 3) |
| Gale Dragonfly | 🐛 Insect / Swarm | 1, Mid (Body Refining) | 25 | 10 | Capung raksasa berkecepatan angin kencang di tebing lembah. | Umum: Sayap Capung Topan (Tier 1) — Jarang: Mata Capung Angin (Tier 1) |
| Canyon Stalker Cat | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 187 | 67 | Kucing liar ngarai berbulu warna batu penyamar dinding tebing. | Umum: Bulu Kucing Ngarai (Tier 1) — Jarang: Cakar Stalker Tebing (Tier 2) |
| Great Gale Falcon King Boss | 🐺 Spirit Beast / Boss | 4, Early (Core Formation) | 3.125 | 1.350 | Raja elang topan raksasa pemimpin kawanan elang Lembah Gema. | Legendaris: Inti Elang Topan Purba Tier 4 (Tier 4, bahan artefak Di-Grade) |
| Gale Wind Dragon Fledgling | 🐺 Spirit Beast | 3, Mid (Foundation Est.) | 1.068 | 371 | Anak naga angin bersayap gelombang suara di tebing Hollow Gale. | Umum: Sisik Naga Angin Topan (Tier 3) — Jarang: Kelenjar Suara Naga (Tier 3) |
| Sonic Echo Eagle | 🐺 Spirit Beast | 2, Late (Qi Gathering) | 142 | 49 | Elang raksasa pemancar jeritan gelombang suara di ngarai batu. | Umum: Bulu Elang Gema (Tier 2) — Jarang: Paruh Suara Topan (Tier 2) |
| Canyon Wind Serpent | 🐺 Spirit Beast | 2, Mid (Qi Gathering) | 106 | 37 | Ular angin melayang penjelajah lorong-lorong batu berongga. | Umum: Kulit Ular Angin (Tier 1) — Jarang: Bisa Gema Ngarai (Tier 2) |
| Heavenly Tempest Dragon Mitos | 🗿 Mitos / Sovereign | 8, Early (Dao Integration) | 2.226.562 | 791.015 | Naga Badai Topan Mitos pemanggil arus badai angin ngarai Koridor Gale. | Legendaris: Mutiara Badai Topan Mitos (Tier 8, bahan artefak angin Sheng-Grade) |

---

### 🌀 6.10 Fate Scarlands (`10`) — 24 Spesies
*(Rujukan: `10_FATE_SCARLANDS.md`)*

| Monster | Kategori | Tier (Realm Setara) | HP | Attack Power | Kemampuan & Deskripsi | Loot Drop |
|---|---|---|---|---|---|---|
| Scar-Gazer | 👤 Bayangan / Anomali | 4, Mid (Core Formation) | 2.656 | 843 | Monster bermata satu raksasa memicu ilusi *Memory Erosion*. | Umum: Serpihan Mata Anomali (Tier 3) — Jarang: Inti Mutasi Batin (Tier 4) |
| Spatial Anomaly Serpent | 🐺 Spirit Beast Mutasi | 5, Early (Nascent Soul) | 13.281 | 4.218 | Ular mutasi perayap celah ruang di Reruntuhan Kota Terbalik. | Umum: Sisik Belah Ruang (Tier 4) — Jarang: Spatial Shard Purba (Tier 5) |
| Chrono-Beast | 🗿 Ancient Guardian | 7, Early (Void Refinement) | 332.031 | 105.468 | Binatang purba pelindung Celah Takdir. Memperlambat waktu $-60\%$. | Legendaris: Fate Core Crystal (Tier 7, bahan terobos Dao Integration) |
| Mutated Void Beast | 🗿 Ancient Guardian / Calamity | 7, Mid (Void Refinement) | 498.046 | 158.203 | Monster tanpa wujud tetap melompat antar-dimensi ruang. | Legendaris: Inti Kehampaan Anomali Tier 7 (Tier 7, bahan senjata Sheng-Grade) |
| Distortion Phantom | 👤 Bayangan / Yin | 4, Early (Core Formation) | 1.770 | 562 | Bayangan arwah terdistorsi di Lembah Bayangan Terbalik. | Umum: Serpihan Arwah Distorsi (Tier 3) — Jarang: Esens Bayangan Fate (Tier 4) |
| Fate-Eating Moth | 🐛 Insect / Swarm | 3, Late (Foundation Est.) | 500 | 175 | Ngengat pemakan energi benang Takdir di Zona Keretakan Ruang. | Umum: Serbuk Sayap Takdir (Tier 2) — Jarang: Kelenjar Pemakan Fate (Tier 3) |
| Void Spider | 🐛 Insect / Swarm | 4, Early (Core Formation) | 1.770 | 562 | Laba-laba pembentang jaring celah ruang tak kasat mata. | Umum: Benang Ruang Kehampaan (Tier 3) — Jarang: Kelenjar Belah Ruang (Tier 4) |
| Time-Warped Wolf | 🐺 Spirit Beast Mutasi | 4, Mid (Core Formation) | 2.656 | 843 | Serigala mutasi bergerak dalam dua linimasa waktu berbeda. | Umum: Bulu Serigala Waktu (Tier 3) — Jarang: Taring Belah Distorsi (Tier 4) |
| Anomaly Golem | 🗿 Ancient Guardian | 5, Early (Nascent Soul) | 13.281 | 4.218 | Golem gabungan batu dan pecahan energi distorsi Takdir. | Umum: Batu Mutasi Anomali (Tier 4) — Jarang: Inti Golem Fate (Tier 5) |
| Mutated Crow | 🐺 Spirit Beast Mutasi | 3, Early (Foundation Est.) | 250 | 87 | Gagak berkepala gila pemancar gelombang guncangan batin. | Umum: Bulu Gagak Mutasi (Tier 2) — Jarang: Paruh Gagak Anomali (Tier 3) |
| Scar-Bound Hound | 🐺 Spirit Beast Mutasi | 3, Mid (Foundation Est.) | 375 | 131 | Anjing mutasi berkulit keretakan ruang di Pos Perbatasan Scarlands. | Umum: Kulit Anjing Mutasi (Tier 2) — Jarang: Taring Belah Ruang (Tier 3) |
| Chrono Dragonfly | 🐛 Insect / Swarm | 2, Late (Qi Gathering) | 200 | 70 | Capung pemancar aura percepatan/perlambatan gerak lokal. | Umum: Sayap Capung Waktu (Tier 2) — Jarang: Esens Cahaya Chrono (Tier 2) |
| Fate-Warped Snake | 🐺 Spirit Beast Mutasi | 4, Late (Core Formation) | 3.541 | 1.125 | Ular mutasi penyerap keberuntungan roll pemicu status *Bad Luck*. | Umum: Sisik Ular Takdir (Tier 3) — Jarang: Bisa Mutasi Fate (Tier 4) |
| Spatial Rift Lizard | 🐺 Spirit Beast Mutasi | 3, Late (Foundation Est.) | 500 | 175 | Kadal amfibi melompati jarak 10 langkah instan lewat celah ruang. | Umum: Kulit Kadal Ruang (Tier 2) — Jarang: Cakar Belah Dimensi (Tier 3) |
| Void Parasite | 🐛 Insect / Swarm | 3, Early (Foundation Est.) | 250 | 87 | Parasit mikro penempel meridian pemicu kebocoran QiCap. | Umum: Cairan Parasit Kehampaan (Tier 2) — Jarang: Inti Parasit Anomali (Tier 3) |
| Mutated Bear | 🐺 Spirit Beast Mutasi | 5, Mid (Nascent Soul) | 19.921 | 6.328 | Beruang mutasi dua kepala penembak sinar gelombang Fate Qi. | Umum: Empedu Beruang Mutasi (Tier 4) — Jarang: Inti Beruang Fate Tier 5 (Tier 5) |
| Chrono-Stalker Cat | 🐺 Spirit Beast Mutasi | 4, Early (Core Formation) | 1.770 | 562 | Kucing pemburu yang menyerang 1 detik sebelum langkah kakinya terlihat. | Umum: Bulu Kucing Waktu (Tier 3) — Jarang: Cakar Stalker Chrono (Tier 4) |
| Scarland Vulture | 🐺 Spirit Beast Mutasi | 2, Peak (Qi Gathering) | 250 | 70 | Burung bangau pemakan sisa daging mahluk anomali terdistorsi. | Umum: Bulu Burung Anomali (Tier 2) — Jarang: Paruh Vulture Fate (Tier 2) |
| Spatial Worm Small | 🐛 Insect / Swarm | 3, Mid (Foundation Est.) | 375 | 131 | Cacing belah ruang penggali terowongan linimasa waktu bawah tanah. | Umum: Lendir Belah Ruang (Tier 2) — Jarang: Kulit Cacing Dimensi (Tier 3) |
| Lord of Anomaly Boss | 🗿 Ancient Guardian / Calamity | 8, Early (Dao Integration) | 1.660.156 | 527.343 | Penguasa anomali takdir raksasa di pusat Celah Takdir Purba. | Legendaris: Inti Takdir Purba Dao Integration (Tier 8, bahan terobos Tribulation) |
| Chrono Rift Dragon Fledgling | 🐺 Spirit Beast Mutasi | 3, Mid (Foundation Est.) | 956 | 379 | Anak naga mutasi ruang-waktu bersisik ungu keemasan di Celah Takdir. | Umum: Sisik Naga Celah Takdir (Tier 3) — Jarang: Inti Ruang-Waktu Naga (Tier 3) |
| Temporal Scar Phantom | 👤 Bayangan / Anomali | 3, Late (Foundation Est.) | 318 | 126 | Bayangan arwah linimasa masa lalu yang terjebak di zona keretakan. | Umum: Serpihan Arwah Waktu (Tier 2) — Jarang: Esens Distorsi Temporal (Tier 3) |
| Scarland Anomaly Wyrm | 🐺 Spirit Beast Mutasi | 4, Mid (Core Formation) | 2.390 | 759 | Cacing naga mutasi raksasa pembelah batas dimensi tanah. | Umum: Kulit Wyrm Anomali (Tier 3) — Jarang: Inti Belah Ruang Wyrm (Tier 4) |
| Primordial Chrono-Dragon Mitos | 🗿 Mitos / Sovereign | 9, Early (Tribulation Transcendence) | 8.300.781 | 2.490.234 | Naga Waktu Mitos purba teragung penguasa linimasa dan keretakan takdir Qianyuan-World. | Legendaris: Inti Naga Waktu Purba Tribulation (Tier 9, bahan obat/artefak Mitos Tertinggi) |

---

## 🛡️ 7. Checklist Anti-Cheat Monster (Wajib Dicek AI-GM)

- [ ] HP dan Attack Power monster dihitung dari formula `MonsterHP` dan `MonsterAttackPower` di §1, bukan klaim sepihak?
- [ ] Kemunculan penyergapan (*Ambush*) dilempar via formula `AmbushChance` (§3) oleh AI GM, bukan diatur sepihak pemain?
- [ ] Monster Calamity (Tier 6+) hanya muncul di habitat resmi sesuai canon (`01`–`10`), tidak di lokasi aman?
- [ ] Loot hanya didapat setelah monster benar-benar dikalahkan dalam roleplay dan dicatat di *Item Origin Log* (`13`)?
- [ ] Serangan ultimate monster (> 1,5× Attack Power) dibatasi cooldown minimal 3 ronde pertempuran?
- [ ] Respawn monster unik/boss dibatasi cooldown naratif wajar, tidak di-farming berulang dalam waktu singkat?

Jika **salah satu** poin di atas meragukan → Encounter / Loot **DIKOREKSI OTOMATIS** oleh AI GM.

---

## 🗺️ 8. Integrasi dengan Sistem Lain

- **Dengan Sistem Hukum Kultivasi (`12`)**: `MonsterQiCap` menggunakan tabel QiCap yang sama, dan loot monster dipetakan langsung ke Bahan Terobosan Realm per Hukum.
- **Dengan Sistem Ekonomi (`13`)**: Seluruh loot monster tunduk pada Tier & Grade Value serta formula `FinalPrice` saat ditransaksikan di bursa.
- **Dengan Sistem Vitalitas & HP (`14`)**: Damage monster mengurangi HP karakter secara presisi dan dapat memicu status *Wound/Trauma*.
- **Dengan Sistem Pertempuran Taktis (`15`)**: Monster dan kultivator bertarung menggunakan sistem *Initiative*, *Action Economy*, dan *Posture/Position* yang identik.
- **Dengan Sistem Beast Bond (`19`)**: Spirit Beast liar dari kategori 🐺 dapat dijinakkan dan diikat menjadi pasangan bertarung jika memenuhi syarat *Trust* dan *Taming Chance*.

---

## 📊 9. Ringkasan Jumlah Monster per Wilayah Qianyuan-World

| Wilayah Qianyuan-World | Jumlah Spesies Canon | Threat Level Tertinggi |
|---|---|---|
| **Ibu Kota Yuanjing & Perbatasan (`01`)** | 24 Spesies | 🖤 Black (Tier 8 — Golden Dragon Sovereign Purba) |
| **Vermilion River Basin (`02`)** | 24 Spesies | 🖤 Black (Tier 7 — Vermilion River Turtle Purba) |
| **Blackstone Skyreach (`03`)** | 24 Spesies | 🖤 Black (Tier 8 — Skyreach Mountain Behemoth) |
| **Ashen Sun Expanse (`04`)** | 24 Spesies | 🖤 Black (Tier 8 — Ashen Phoenix Purba) |
| **Nine-Reed Mire (`05`)** | 24 Spesies | 🖤 Black (Tier 7 — Nine-Headed Hydra Mitos) |
| **Astral Tide Sea (`06`)** | 24 Spesies | 🖤 Black (Tier 8 — Leviathan Astral Purba) |
| **Whispering Root Forest (`07`)** | 24 Spesies | 🖤 Black (Tier 8 — World Tree Dragon Sovereign Purba) |
| **Frostglass Crown (`08`)** | 24 Spesies | 🖤 Black (Tier 8 — Absolute Zero Glacial Dragon Mitos) |
| **Hollow Gale Corridor (`09`)** | 24 Spesies | 🖤 Black (Tier 8 — Heavenly Tempest Dragon Mitos) |
| **Fate Scarlands (`10`)** | 24 Spesies | 🖤 Black (Tier 9 — Primordial Chrono-Dragon Mitos) |
| **Monster Lintas Wilayah / Umum (§5)** | 15 Spesies | 🟡 Yellow (Tier 2 — Wild Horned Bull & Cloud-Rider Horse) |

---

## 🎯 10. Panduan Penggunaan untuk AI GM

### 10.1 Memilih Monster yang Tepat
1. **Tentukan wilayah** tempat pemain berada saat ini (misal: *Nine-Reed Mire*).
2. **Pilih spesies monster** dari katalog wilayah tersebut yang sesuai dengan Threat Level dan Realm pemain.
3. **Lempar `AmbushChance`** (§3) untuk menentukan apakah terjadi penyergapan tiba-tiba.

### 10.2 Menjalankan Pertarungan
1. **Gunakan formula** dari `15_COMBAT_TACTICAL_SYSTEM.md` untuk resolusi pertempuran.
2. **Hitung `MonsterHP` & `MonsterAttackPower`** menggunakan formula §1.
3. **Serangan Ultimate Monster**: Boleh menggunakan 1,5× s/d 3,0× Attack Power sekali per pertarungan (cooldown 3 ronde).

### 10.3 Menentukan Loot
1. Setelah monster dikalahkan, lempar `BaseDropRate` (§4).
2. Tentukan material yang berhasil didapat dan catat ke *Item Origin Log* (`13`).
