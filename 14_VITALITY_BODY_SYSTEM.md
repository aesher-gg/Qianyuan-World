# ❤️ Qianyuan-World — XV. Vitality & Body System (Sistem Vitalitas, Tubuh, & Kelangsungan Hidup)

> **Modul:** 14 — Vitality Body System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Survival & Injury Realism
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (ikhtisar dunia), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap & breakthrough), `13_ECONOMY_MARKET_SYSTEM.md` (harga pengobatan Tabib & makanan), `15_COMBAT_TACTICAL_SYSTEM.md` (penerapan damage & trauma pertarungan)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Vitalitas

Sama seperti energi Qi yang tunduk pada `QiCap` dan harga yang tunduk pada `FinalPrice`, daya tahan fisik (*HP*), status luka, dan rasa lapar (*Satiety*) di dunia Qianyuan tunduk pada formula mekanis yang ketat. Pemain **TIDAK BOLEH** mengarang sendiri angka HP, regenerasi ajaib instan, atau kekebalan dari cedera fisik tanpa dasar item/jasa medis resmi.

### Aturan Emas Anti-Cheat Vitalitas & Kelaparan (Mandatory Enforced Rules)
1. **Larangan Deklarasi HP Sepihak**: Maksimal HP karakter dihitung otomatis oleh AI GM menggunakan formula `HPMax(realm, stage, law)`. Klaim nilai HP di atas formula otomatis **DITOLAK**.
2. **Log Kerusakan Bertimestamp**: Setiap luka (*Wound*), trauma batin (*Trauma*), dan pengurangan HP akibat pertarungan atau racun wajib dicatat di log percakapan bertimestamp dan tidak bisa diedit mundur.
3. **Pengobatan Medis Terintegrasi**: Penyembuhan luka berat (*Major/Severe Wound*) dan trauma Dantian hanya bisa dipulihkan lewat ramuan alkimia (*Pills*) atau jasa Tabib resmi yang tunduk pada Sistem Ekonomi (`13_ECONOMY_MARKET_SYSTEM.md`).
4. **Kelaparan Berdasarkan Waktu (*Satiety Decay*)**: Penurunan tingkat kenyang (*Satiety*) dihitung per Jam berdasarkan *Fasting Multiplier* Realm karakter, bukan klaim sepihak pemain.
5. **Pembaruan Otomatis Terobosan**: Terobosan Realm (*Breakthrough*) secara otomatis memperbarui nilai Max HP, Max Stamina, dan Fasting Multiplier karakter, serta memicu pemulihan HP dan Qi penuh.

---

## 📊 1. Atribut Vitalitas Utama (Core Vital Attributes)

Setiap karakter di dunia Qianyuan memiliki 4 Atribut Vitalitas Utama yang dicatat di blok Profil Karakter:

* **HP (Hit Points / Health)**: Daya tahan hidup fisik utama. Jika HP mencapai 0, karakter masuk ke kondisi pingsan/kritis (*Dying State*).
* **Qi (Spiritual Energy)**: Energi batin Dantian untuk merapalkan jurus, membentuk perisai aura, dan melakukan kultivasi.
* **Stamina**: Energi fisik untuk berlari, bertahan dalam pertarungan jarak dekat, dan menahan kondisi lingkungan ekstrem.
* **Satiety (Tingkat Kekenyangan)**: Skala nutrisi fisik (0 s/d 100). Memengaruhi kecepatan regenerasi fisik.

---

## 🩸 2. Formula HP Universal & Law HP Multiplier

### 2.1 Formula Dasar HP Qianyuan
```
HPBase(realm, stage) = BasePhysicalVitality + (QiCap(realm, stage) × K_HP)
BasePhysicalVitality = 100 HP (Daya tahan fisik dasar raga manusia)
K_HP = 1,0 (Konstanta Vitalitas Universal)

HPMax(realm, stage, law) = HPBase(realm, stage) × LawHPMultiplier(law)
```

> 📌 **Ketentuan Khusus Mortal (Non-Kultivator)**: Manusia biasa / Mortal yang belum berkultivasi (sebelum memasuki Realm 1) memiliki **`QiCap = 0`**. Maka `HPBase` untuk Mortal murni adalah `100 + (0 × 1,0) = 100 HP`.

### 2.2 Law HP Multiplier per Jalur Hukum Qianyuan

| Jalur Hukum Kultivasi (`12`) | LawHPMultiplier | Alasan Filosofis & Karakteristik |
|---|---|---|
| **Hukum Zirah Batu Hitam & Logam** (*Earth/Metal Qi*) | ×1,5 | Penempaan raga keras — sangat tahan banting, HP Max tertinggi. |
| **Hukum Raga Serat Kayu & Kehidupan** (*Wood/Life Qi*) | ×1,3 | Vitalitas serat kayu — pemulihan sel cepat, daya tahan tinggi. |
| **Hukum Gelombang Samudra & Bintang** (*Water/Star Qi*) | ×1,0 | Baseline standar — seimbang antara pertahanan dan kelenturan. |
| **Hukum Pedang Es & Keheningan** (*Ice/Stillness Qi*) | ×1,0 | Baseline standar — fokus pada ketenangan batin dan kebekuan. |
| **Hukum Angin Topan & Gema Suara** (*Wind/Sound Qi*) | ×0,95 | Lincah dan fleksibel — sedikit lebih tipis demi kecepatan. |
| **Hukum Matahari Membara & Api** (*Fire/Sun Qi*) | ×0,9 | Agresif dan ofensif — fokus pada daya hancur ketimbang HP. |
| **Hukum Anomali Ruang & Takdir** (*Fate/Mutated Qi*) | ×0,85 | Unik dan tidak stabil — memicu risiko fluktuasi Dantian. |
| **Hukum Racun Miasma & Anggrek Darah** (*Poison/Blood Qi*)| ×0,8 | Jalur racun beracun — trade-off klasik kekuatan racun besar, raga rapuh. |

---

### 📈 2.3 Tabel Skala HP Maksimal per Realm (Jalur Hukum Netral ×1,0)

| Realm & Stage Kultivasi | QiCap (`12`) | Formula HPBase | HPMax (Hukum Netral ×1,0) |
|---|---|---|---|
| **Mortal (Non-Kultivator)** | **0** | `100 + (0 × 1,0)` | **100 HP** |
| **Body Refining Early Stage (Realm 1)** | **50** | `100 + (50 × 1,0)` | **150 HP** |
| **Body Refining Mid Stage** | **75** | `100 + (75 × 1,0)` | **175 HP** |
| **Body Refining Late Stage** | **100** | `100 + (100 × 1,0)` | **200 HP** |
| **Body Refining Peak Stage** | **125** | `100 + (125 × 1,0)` | **225 HP** |
| **Qi Gathering Early Stage (Realm 2)** | **250** | `100 + (250 × 1,0)` | **350 HP** |
| **Qi Gathering Peak Stage** | **625** | `100 + (625 × 1,0)` | **725 HP** |
| **Foundation Est. Early Stage (Realm 3)** | **1.250** | `100 + (1.250 × 1,0)` | **1.350 HP** |
| **Foundation Est. Peak Stage** | **3.125** | `100 + (3.125 × 1,0)` | **3.225 HP** |
| **Core Formation Early Stage (Realm 4)** | **6.250** | `100 + (6.250 × 1,0)` | **6.350 HP** |
| **Core Formation Peak Stage** | **15.625** | `100 + (15.625 × 1,0)` | **15.725 HP** |
| **Nascent Soul Early Stage (Realm 5)** | **31.250** | `100 + (31.250 × 1,0)` | **31.350 HP** |
| **Soul Formation Early Stage (Realm 6)** | **156.250** | `100 + (156.250 × 1,0)` | **156.350 HP** |

---

## 🤕 3. Status Kondisi HP & Ambang Bahaya

| % HP Tersisa | Status Kondisi | Efek Mekanis & Penalti |
|---|---|---|
| **100% s/d 50%** | **Sehat (Healthy)** | Kondisi prima, tidak ada penalti. |
| **49% s/d 20%** | **Terluka (Wounded)** | Penalti Output Qi -10%, penalti Evasion -10%. |
| **19% s/d 1%** | **Kritis (Critical)** | Penalti Output Qi -30%, penalti Evasion -25%, risiko *Qi Deviation* ringan. |
| **0%** | **Pingsan / Dying State** | Tak sadarkan diri. Wajib mendapat pertolongan medis dalam 4 Jam. |
| **-1% s/d -30%** | **Nyaris Mati (Near Death)**| Memerlukan Tabib Realm ≥ Realm karakter; jika gagal → *Permanent Dantian Trauma*. |
| **Di bawah -50%** | **Kematian Permanen** | Overkill ekstrem tervalidasi GM (karakter tewas permanen). |

---

## 🩹 4. Luka Fisik (Wound), Trauma Dantian, & Efek Racun

### 4.1 Kategori Luka Fisik (Wound)
* **Minor Wound (Luka Ringan)**: Memar / goresan senjata ringan. Penalti Max Stamina -10%.
* **Major Wound (Luka Berat)**: Tebasan dalam / patah tulang ekstremitas. Penalti Max HP -25%, penalti Movement Speed -20%.
* **Severe Wound (Luka Parah)**: Kerusakan organ dalam / pendarahan hebat. Penalti Max HP -50%, penalti seluruh statistik tempur -40%.

### 4.2 Trauma Dantian & Jiwa (Trauma)
* **Dantian Shock**: Gangguan aliran Qi akibat hentakan intim atau *Backlash*. Penalti Kecepatan Pemulihan Qi -50%.
* **Soul Trauma**: Kerusakan jiwa batin akibat serangan mental/ilusi. Penalti Max Qi -30%.

### 4.3 Racun & Pendarahan (Poison & Bleeding)
* **Poison Status (Sengatan Racun)**: Mengurangi HP sebesar 2,5 s/d 15 poin per Jam tergantung grade racun (*Minor / Moderate / Lethal*) hingga diminumi *Antidote Pill*.
* **Bleeding (Pendarahan)**: Mengurangi HP dan Stamina sebesar 5 poin per turn pertempuran hingga dibalut dengan perban/salep.

---

## 🌾 5. Sistem Kelaparan & Fasting Multiplier (Bi Gu / 辟谷)

Trope xianxia klasik: seiring meningkatnya Realm kultivasi, kultivator mampu menyerap energi Qi lingkungan untuk menggantikan makanan fisik (*Bi Gu / 辟谷*).

```
DecayRatePerHour(realm) = BaseDecayRate / FastingMultiplier(realm)
BaseDecayRate = 12,5 Satiety Points per Jam (Mortal biasa kehilangan kenyang penuh dalam 8 Jam)
```

### 📊 Fasting Multiplier per Realm Qianyuan

| Realm Kultivasi | FastingMultiplier | Waktu Sampai Lapar (Satiety < 30) |
|---|---|---|
| **0 — Non-Kultivator (Mortal)** | ×1,0 | 8 Jam |
| **1 — Body Refining Realm (Qi-Guan)** | ×1,5 | 12 Jam |
| **2 — Qi Gathering Realm (Qi-Ji)** | ×3,0 | 24 Jam (1 Hari) |
| **3 — Foundation Establishment (Zhu-Ji)** | ×10,0 | 80 Jam (~3,3 Hari) |
| **4 — Core Formation Realm (Jie-Dan)** | ×30,0 | 240 Jam (10 Hari) |
| **5 — Nascent Soul Realm (Yuan-Ying)** | ×100,0 | 800 Jam (~33 Hari / 1 Bulan) |
| **6 — Soul Formation Realm (Hua-Shen)** | ×500,0 | 4.000 Jam (~5 Bulan) |
| **7 — Void Refinement Realm (Lian-Xu)** | ×2.000,0 | 16.000 Jam (~1,8 Tahun) |
| **8 — Dao Integration Realm (He-Dao)** | ×10.000,0 | 80.000 Jam (~9 Tahun) |
| **9 — Tribulation Transcendence (Du-Jie)**| **Tak Terbatas** | **Bi Gu Sempurna** (Tidak butuh makan selamanya). |

### 🥣 Status Efek Satiety
* **Satiety 70 s/d 100 (Kenyang)**: Bonus regenerasi Stamina & Qi +10%.
* **Satiety 30 s/d 69 (Normal)**: Kondisi fisik biasa.
* **Satiety 10 s/d 29 (Lapar)**: Penalti Max Stamina -25%, penalti Kecepatan Pemulihan Qi -20%.
* **Satiety 0 (Kelaparan Kritis)**: Pengurangan HP sebesar 2,5 poin per Jam, **TIDAK BISA** melakukan terobosan Realm atau regenerasi Qi alami.

---

## 🛌 6. Mekanik Istirahat & Pemulihan (Rest & Recovery)

* **Short Rest (2 Jam)**: Memulihkan Stamina sebesar 30%, memulihkan Qi sebesar 25%. Memerlukan konsumsi 1 porsi makanan/air.
* **Long Rest (8 Jam)**: Memulihkan HP sebesar 50%, memulihkan Qi & Stamina penuh.
* **Pengobatan Tabib / Pill Alkimia**: Diperlukan untuk memulihkan *Major/Severe Wound*, menyembuhkan *Dantian Shock*, atau menghilangkan racun mematikan.

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Diperiksa Setiap Turn)

- [ ] Max HP dihitung otomatis berdasarkan formula `HPMax(realm, stage, law)`?
- [ ] Mortal murni (sebelum Realm 1) menggunakan `QiCap = 0` (`HPMax = 100 HP`)?
- [ ] Kerusakan HP, status Wound, dan Trauma dicatat di log bertimestamp?
- [ ] Penurunan Satiety dihitung presisi sesuai Fasting Multiplier Realm karakter?
- [ ] Penyembuhan luka berat dan trauma menggunakan pill/jasa tabib tervalidasi Sistem Ekonomi?
- [ ] Terobosan Realm memperbarui statistik Max HP, memulihkan HP/Qi penuh, dan memperbarui Fasting Multiplier?

Jika **salah satu** poin di atas meragukan → Status Vitalitas **DIKOREKSI OTOMATIS** oleh AI GM.
