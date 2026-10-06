# 💰 Qianyuan-World — XIV. Economy & Market System (Sistem Ekonomi & Pasar Qianyuan)

> **Modul:** 13 — Economy Market System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Supply-Demand Driven — Currency Standardized
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (peta jarak & bursa pusat Yuanjing), `11_CROSS_REGION_ORGANIZATIONS.md` (Merchant Alliance & organisasi), `12_CULTIVATION_RESONANCE_SYSTEM.md` (tier material terobos), `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` (bahan & grade alkimia/tempa), `ECONOMY_ORACLE.md` (cheat-sheet harga instan)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Ekonomi

Sama seperti energi Qi yang tunduk pada formula `QiCap`, setiap harga komoditas, jasa, dan aset di dunia Qianyuan tunduk pada satu **Formula Harga Dinamis** yang terstandarisasi. Hal ini mencegah pengarangan harga sepihak oleh pemain maupun AI GM tanpa dasar kalkulasi resmi.

### Aturan Emas Anti-Cheat Ekonomi (Mandatory Enforced Rules)
1. **Larangan Deklarasi Sepihak**: Harga barang/jasa **TIDAK BOLEH** ditetapkan sepihak oleh pemain. Semua harga wajib dihitung AI GM menggunakan formula resmi.
2. **Item Origin Log / Ledger**: Setiap barang bernilai tinggi (**Tier 3+ / Grade Xuan ke atas**) wajib memiliki asal-usul yang sah (*Item Origin Log*) dari hasil quest, looting resmi, atau transaksi yang tercatat di log cerita. Barang tanpa origin **TIDAK BISA** diperjualbelikan atau dipakai untuk terobosan Realm.
3. **Stok Toko Terbatas**: Stok barang/bahan spiritual di setiap toko/kota dibatasi oleh kapasitas produksi wilayah. Pembelian borongan barang Tier tinggi tanpa alasan naratif kuat otomatis **DITOLAK**.
4. **Batas Tawar-Menawar (Haggling Ceiling)**: Tawar-menawar dibatasi sebesar ±5% hingga ±20% dari harga formula, tergantung pada sifat NPC pedagang.
5. **Hard Cap Fluktuasi Harga**: Fluktuasi harga akibat kelangkaan dan permintaan dibatasi pada rentang `[0,2× s/d 5,0×]` dari *Grade Value* dasar.

---

## 🪙 1. Mata Uang Resmi Qianyuan (Standardized Currency)

Sistem keuangan benua Qianyuan terstandarisasi berdasarkan ketetapan Kekaisaran Yuanjing dan Aliansi Pedagang Agung (*Grand Merchant Alliance*):

| Tier Mata Uang | Nama Mata Uang | Nilai Konversi Resmi | Penggunaan Utama |
|---|---|---|---|
| **Tier 1** | **Copper Tael / Koin Tembaga** | 1 (Satuan Dasar) | Transaksi harian rakyat biasa, makanan, penginapan murah. |
| **Tier 2** | **Silver Tael / Tael Perak** | 100 Copper Taels | Transaksi umum kota, upah jasa, herbal biasa, zirah standar. |
| **Tier 3** | **Gold Tael / Tael Emas** | 10 Silver Taels (1.000 Copper) | Transaksi besar, bahan tempa, pil kultivasi, jasa pengawalan. |
| **Tier 4** | **Spirit Stone Tier 1 (Low)** | 10 Silver Taels (1 Gold Tael) | Transaksi kultivator tingkat awal (Body Refining - Foundation). |
| **Tier 5** | **Spirit Stone Tier 2 (Mid)** | 100 Spirit Stone Tier 1 (1.000 Silver) | Transaksi bursa sekte, bahan terobos Core Formation/Nascent. |
| **Tier 6** | **Spirit Stone Tier 3 (High)** | 100 Spirit Stone Tier 2 (100.000 Silver)| Transaksi lelang teratas Yuanjing, relik kuno, pusaka tingkat dewa. |

> 📌 **Catatan Poin Kontribusi Sekte (*Sect Contribution Points*)**: Poin internal sekte digunakan khusus untuk menukar kitab, pil, dan fasilitas di dalam sekte. Poin ini **TIDAK BISA** dikonversi langsung ke Tael Perak/Emas untuk mencegah eksploitasi pencucian uang antar-sekte.

---

## 💎 2. Struktur Tier Base Value & Quality Grade

### 2.1 Tier Material & Base Value (Selaras dengan Tier Terobos `12_CULTIVATION_RESONANCE_SYSTEM.md`)

Setiap barang di dunia Qianyuan dikategorikan ke dalam 9 Tier material:

| Tier Barang | Tier Base Value (Copper Tael) | Konversi Praktis | Contoh Barang |
|---|---|---|---|
| **Tier 1** | 5 Copper | 5 Copper Taels | Herbal biasa, pedang besi desa, pakan ternak. |
| **Tier 2** | 50 Copper | 50 Copper Taels | Pil pemulih Qi ringan, zirah kulit dojo, obat luka luar. |
| **Tier 3** | 500 Copper | 5 Silver Taels | Pil penawar racun Grade 2, pedang baja tempa bermutu. |
| **Tier 4** | 5.000 Copper | 50 Silver Taels | Foundation Pill, senjata Cold Steel ber-Qi ringan. |
| **Tier 5** | 50.000 Copper | 5 Gold Taels / 50 SS-T1 | Golden Core Pill, Spirit Beast Collar, zirah batu hitam. |
| **Tier 6** | 500.000 Copper | 50 Gold Taels / 500 SS-T1 | Nascent Soul Pill, senjata Cold Steel Superior, perahu Lingzhou. |
| **Tier 7** | 5.000.000 Copper | 5 SS-T2 (500 Gold) | Bahan terobos Void Refinement, Spatial Shard, Anchor Talisman. |
| **Tier 8** | 50.000.000 Copper | 50 SS-T2 (5.000 Gold) | Bahan Tribulasi Petir, Kristal Es Inti Purba, Teratai Salju 100 Th. |
| **Tier 9** | 500.000.000 Copper | 500 SS-T2 / 5 SS-T3 | Fate Core Crystal, Kitab Prasasti Purba, Artefak Tingkat Dewa. |

```
TierBase(n) = 5 × 10^(n−1) Copper Taels
```

### 2.2 Quality Grade Multiplier

| Quality Grade | Nama Grade | Multiplier | Catatan Kualitas |
|---|---|---|---|
| **Grade 1** | **Fan-Grade (凡品)** | ×0,5 | Kualitas buatan amatir/cacat, efisiensi rendah. |
| **Grade 2** | **Huang-Grade (黄品)** | ×1,0 | Kualitas standar pasar / dojo biasa. |
| **Grade 3** | **Xuan-Grade (玄品)** | ×2,5 | Kualitas sekte menengah, ber-Qi murni. |
| **Grade 4** | **Di-Grade (地品)** | ×6,0 | Kualitas sekte besar, dibuat alchemist/penempa ahli. |
| **Grade 5** | **Tian-Grade (天品)** | ×15,0 | Kualitas master / pusaka sekte utama. |
| **Grade 6** | **Sheng-Grade (聖品)** | ×40,0 | Tingkat legendaris / relik purba tak ternilai. |

```
GradeValue(Tier, Grade) = TierBase(Tier) × GradeMultiplier(Grade)
```

---

## 📈 3. Formula Harga Dinamis (Dynamic Price Formula)

```
FinalPrice = GradeValue(Tier, Grade) × RegionScarcity × DemandIndex × EventModifier × ConditionModifier
FinalPrice = clamp(hasil, 0,2 × GradeValue, 5,0 × GradeValue)
```

### 3.1 Region Scarcity (Kelangkaan Wilayah)
- **Barang Lokal (Diproduksi di wilayah sendiri)**: ×0,6
- **Barang Impor Wilayah Tetangga (≤ 1.500 li)**: ×1,5
- **Barang Impor Wilayah Jauh (> 1.500 li)**: ×3,0
- **Barang dari Zona Anomali Terlarang (Fate Scarlands / Palung Abyss)**: ×5,0

### 3.2 Demand Index (Indeks Permintaan)
```
DemandIndex = clamp(0,5 + (ActiveBuyOrders − ActiveSupply) / ActiveSupply × 0,5, 0,5, 3,0)
```

- **Pasar Normal**: 1,0
- **Musim Paceklik / Musim Perang / Perluasan Wabah**: 1,5 s/d 3,0
- **Musim Panen Melimpah / Surplus**: 0,5 s/d 0,8

### 3.3 Condition Modifier (Kondisi Barang)
- Rusak / Cacat Ringan: ×0,7
- Kondisi Prima / Baru: ×1,0
- Barang Antik Verifikasi Arsip: ×1,5

---

## 🛠️ 4. Harga Jasa Resmi Qianyuan (Service Pricing)

### 4.1 Jasa Pengobatan Tabib (Golden Thread Medicine Hall & Tabib Rawa)
```
HealingFee = InjurySeverityBase × TabibRealmMultiplier
```

- **Luka Ringan / Pertolongan Pertama**: 10 s/d 50 Silver Taels
- **Luka Berat / Racun Miasma Rawa**: 100 s/d 500 Silver Taels
- **Penyembuhan Dantian Wound Trauma / Perbaikan Qi Deviation**: 5 s/d 50 Spirit Stones Tier 1

### 4.2 Jasa Pengawalan Karavan (Red Sand Caravan & Wan'an Escort)
```
EscortFee = (CargoValue × 5%) + (Jarak_li / 100 × 5 Silver Taels) × RiskMultiplier
```

- **Rute Aman (Vermilion / Central Plains)**: `RiskMultiplier = 1,0`
- **Rute Rawan Bandit / Gurun Ashen Sun**: `RiskMultiplier = 2,5`
- **Rute Perbatasan Scarlands / Badai Ngarai**: `RiskMultiplier = 5,0`

### 4.3 Jasa Informasi (Feather Wind Information Guild & Pos Tebing Bisik)
- Gosip / Informasi Umum Wilayah: 5 s/d 20 Silver Taels
- Informasi Rahasia Sekte / Lokasi Herba Langka: 100 s/d 500 Silver Taels
- Peta Navigasi Fate Scarlands / Rahasia Reruntuhan Purba: 10 s/d 50 Spirit Stones Tier 1

### 4.4 Kontrak Pembunuhan (Silent Blade Guild / Shadow Poison)
```
ContractFee = (TargetQiCap × 0,001 Copper Taels) + DifficultyBonus
```

- Floor minimum kontrak: 50 Silver Taels.

---

## 🏛️ 5. Harga Aset, Properti, & Transportasi

| Jenis Aset / Properti | Kisaran Harga Standar Bursa | Catatan Izin & Syarat |
|---|---|---|
| **Rumah Panggung / Pondok Kayu Desa** | 20 s/d 100 Silver Taels | Izin Kepala Desa lokal. |
| **Toko / Lapak Pasar Kota Utama** | 5 s/d 20 Gold Taels | Pajak bulanan Kekaisaran Yuanjing. |
| **Pendirian Dojo / Perguruan Cabang** | 500 Gold Taels + Sertifikat Dao Registry | Wajib terdaftar di Dao Registry Council (`11`). |
| **Perahu Dayung Rawa (*Mire Skiff*)** | 10 s/d 30 Silver Taels | Moda transportasi utama Nine-Reed Mire. |
| **Kapal Dagang Laut / Perang Maritim** | 50 s/d 500 Gold Taels | Galangan kapal Pelabuhan Star-Compass. |
| **Kapal Udara Lingzhou (*Spirit Airship*)** | 2.000 s/d 10.000 Gold Taels | Memerlukan izin penerbangan Kekaisaran. |

---

## 🤝 6. Batas Tawar-Menawar (Haggling Rules)

Pemain dapat melakukan tawar-menawar (*Haggling*) atas hasil `FinalPrice` melalui roleplay, dengan batasan persentase sesuai sifat NPC pedagang:

| Sifat / Karakteristik Pedagang NPC | Rentang Tawar Diizinkan |
|---|---|
| **Pedagang Ramah / Cerdik Menawar** (*Boss Green-Leaf, Nona Kedai*) | ±20% |
| **Pedagang Netral / Standar Bursa** (*Saudagar Han Jing, Boss Zhao*) | ±15% *(Default)* |
| **Pedagang Kaku / Keras Kepala** (*Master Hunter-Guan, Kepala Pos*) | ±5% |
| **Harga Mati (Formasi Otomatis / Pejabat Resmi Kekaisaran)** | 0% *(Tidak Bisa Ditawar)* |

---

## 📊 7. Integrasi Data Kekayaan 10 Wilayah Qianyuan-World

*(Selaras dengan Data Resmi Canon Modul `01`–`10`)*

| # | Wilayah Qianyuan-World | Total Kekayaan Regional | Karakteristik Komoditas Utama |
|---|---|---|---|
| 1 | **Ibu Kota Yuanjing** | ± 4,5 Miliar Tael | Pusat bursa finansial, lelang teratas, Bank Giok. |
| 2 | **Vermilion River Basin** | ± 720 Juta Tael | Murah untuk herba & ginseng; Mahal untuk mineral logam. |
| 3 | **Blackstone Skyreach** | ± 850 Juta Tael | Murah untuk bijih besi, zirah, & senjata tempa; Mahal untuk tanaman medis. |
| 4 | **Ashen Sun Expanse** | ± 420 Juta Tael | Murah untuk rempah api & kristal api; Sangat Mahal untuk air murni. |
| 5 | **Nine-Reed Mire** | ± 380 Juta Tael | Murah for racun & serangga spiritual; Mahal untuk makanan bersih. |
| 6 | **Astral Tide Sea** | ± 520 Juta Tael | Murah untuk Mutiara Bintang & hasil laut; Mahal untuk kayu tempa. |
| 7 | **Whispering Root Forest** | ± 360 Juta Tael | Murah untuk kayu purba & obat herba; Mahal untuk zirah besi. |
| 8 | **Frostglass Crown** | ± 290 Juta Tael | Murah untuk kristal es & Teratai Salju; Sangat Mahal untuk makanan segar. |
| 9 | **Hollow Gale Corridor** | ± 410 Juta Tael | Murah untuk Echo Stone & jasa kurir kilat; Sedang untuk barang umum. |
| 10 | **Fate Scarlands** | ± 850 Juta Tael | Sangat Mahal untuk relik anomali & *Spatial Shard*; Pakai barter. |

---

## 🛡️ 8. Checklist Validasi AI GM (Wajib Dicek Setiap Transaksi)

- [ ] Harga dihitung menggunakan formula `FinalPrice` (bukan klaim sepihak pemain)?
- [ ] Item Origin Log tervalidasi untuk barang Tier 3+ / Grade Xuan+?
- [ ] Region Scarcity dihitung presisi berdasarkan jarak peta dari wilayah produksi asal?
- [ ] Hasil `FinalPrice` berada dalam rentang clamp `[0,2× s/d 5,0×]` dari Grade Value?
- [ ] Tawar-menawar (*Haggling*) tidak melebihi persentase batas sifat NPC pedagang?
- [ ] Konversi mata uang menggunakan standar resmi Kekaisaran Yuanjing?
- [ ] Stok barang Tier tinggi tidak melebihi kapasitas logistik wilayah?

Jika **salah satu** poin di atas meragukan → Transaksi **DITOLAK TOTAL**. AI GM memberikan alasan teknis yang jelas kepada pemain.
