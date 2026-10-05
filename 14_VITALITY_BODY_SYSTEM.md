# ❤️ Qianyuan-World — XV. Vitality & Body System (Sistem Vitalitas, Tubuh, & Kelangsungan Hidup)

> **Modul:** 14 — Vitality Body System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Law-Specific Scaling — Survival & Injury Realism
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (ikhtisar dunia), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap sebagai basis HP), `13_ECONOMY_MARKET_SYSTEM.md` (harga pengobatan Tabib & makanan), `15_COMBAT_TACTICAL_SYSTEM.md` (penerapan damage & trauma pertarungan)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Vitalitas

Sama seperti energi Qi yang tunduk pada `QiCap` dan harga yang tunduk pada `FinalPrice`, daya tahan fisik (*HP*), status luka, dan rasa lapar (*Satiety*) di dunia Qianyuan tunduk pada formula mekanis yang ketat. Pemain **TIDAK BOLEH** mengarang sendiri angka HP, regenerasi ajaib instan, atau kekebalan dari cedera fisik tanpa dasar item/jasa medis resmi.

### Aturan Emas Anti-Cheat Vitalitas & Kelaparan (Mandatory Enforced Rules)
1. **Larangan Deklarasi HP Sepihak**: Maksimal HP karakter dihitung otomatis oleh AI GM menggunakan formula `HP(realm, stage, law)`. Klaim nilai HP di atas formula otomatis **DITOLAK**.
2. **Log Kerusakan Bertimestamp**: Setiap luka (*Wound*), trauma batin (*Trauma*), dan pengurangan HP akibat pertarungan atau racun wajib dicatat di log percakapan bertimestamp dan tidak bisa diedit mundur.
3. **Pengobatan Medis Terintegrasi**: Penyembuhan luka berat (*Major/Severe Wound*) dan trauma Dantian hanya bisa dipulihkan lewat ramuan alkimia (*Pills*) atau jasa Tabib resmi yang tunduk pada Sistem Ekonomi (`13_ECONOMY_MARKET_SYSTEM.md`).
4. **Kelaparan Berdasarkan Waktu (*Satiety Decay*)**: Penurunan tingkat kenyang (*Satiety*) dihitung per Shichen berdasarkan *Fasting Multiplier* Realm karakter, bukan klaim sepihak pemain.
5. **Pembaruan Otomatis Terobosan**: Terobosan Realm (*Breakthrough*) secara otomatis memperbarui nilai Max HP, Max Stamina, dan Fasting Multiplier karakter.

---

## 📊 1. Atribut Vitalitas Utama (Core Vital Attributes)

Setiap karakter di dunia Qianyuan memiliki 7 Atribut Vitalitas Utama yang dicatat di blok Profil Karakter:

* **HP (Hit Points / Health)**: Daya tahan hidup fisik utama. Jika HP mencapai 0, karakter masuk ke kondisi pingsan/kritis (*Dying State*).
* **Qi (Spiritual Energy)**: Energi batin Dantian untuk merapalkan jurus, membentuk perisai aura, dan melakukan kultivasi.
* **Stamina**: Energi fisik untuk berlari, bertahan dalam pertarungan jarak dekat, dan menahan kondisi lingkungan ekstrem.
* **Satiety (Tingkat Kekenyangan)**: Skala nutrisi fisik ($0 \text{ s/d } 100$). Memengaruhi kecepatan regenerasi fisik.
* **Focus (Konsentrasi Batin)**: Ketahanan mental ($0 \text{ s/d } 100$) terhadap serangan ilusi, intimidasi, dan kelelahan pikiran.
* **Resolve (Tekad Batin)**: Ketahanan moral ($0 \text{ s/d } 100$) untuk bertahan hidup saat berada dalam kondisi kritis/nyaris mati.
* **Fatigue (Keletihan Tubuh)**: Akumulasi kelelahan fisik ($0 \text{ s/d } 100$). Fatigue tinggi menurunkan regenerasi Stamina dan Qi.

---

## 🩸 2. Formula HP Universal & Law HP Multiplier

### 2.1 Formula Dasar HP Qianyuan
$$\text{HPBase}(\text{realm}, \text{stage}) = \text{QiCap}(\text{realm}, \text{stage}) \times K_{\text{HP}} + \text{PhysicalBonus}$$

- $K_{\text{HP}} = 0,5$ (Konstanta Vitalitas Universal Qianyuan).
- $\text{PhysicalBonus}$: Bonus ketahanan fisik khusus Body Refining Stage ($+20 \text{ s/d } +100 \text{ HP}$).

$$\text{HP}(\text{realm}, \text{stage}, \text{law}) = \text{HPBase}(\text{realm}, \text{stage}) \times \text{LawHPMultiplier}(\text{law})$$

### 2.2 Law HP Multiplier per Jalur Hukum Qianyuan

| Jalur Hukum Kultivasi (`12`) | LawHPMultiplier | Alasan Filosofis & Karakteristik |
|---|---|---|
| **Hukum Zirah Batu Hitam & Logam** (*Earth/Metal Qi*) | $\times 1,5$ | Penempaan raga keras — sangat tahan banting, HP Max tertinggi. |
| **Hukum Raga Serat Kayu & Kehidupan** (*Wood/Life Qi*) | $\times 1,3$ | Vitalitas serat kayu — pemulihan sel cepat, daya tahan tinggi. |
| **Hukum Gelombang Samudra & Bintang** (*Water/Star Qi*) | $\times 1,0$ | Baseline standar — seimbang antara pertahanan dan kelenturan. |
| **Hukum Pedang Es & Keheningan** (*Ice/Stillness Qi*) | $\times 1,0$ | Baseline standar — fokus pada ketenangan batin dan kebekuan. |
| **Hukum Angin Topan & Gema Suara** (*Wind/Sound Qi*) | $\times 0,95$ | Lincah dan fleksibel — sedikit lebih tipis demi kecepatan. |
| **Hukum Matahari Membara & Api** (*Fire/Sun Qi*) | $\times 0,9$ | Agresif dan ofensif — fokus pada daya hancur ketimbang HP. |
| **Hukum Anomali Ruang & Takdir** (*Fate/Mutated Qi*) | $\times 0,85$ | Unik dan tidak stabil — memicu risiko fluktuasi Dantian. |
| **Hukum Racun Miasma & Anggrek Darah** (*Poison/Blood Qi*)| $\times 0,8$ | Jalur racun beracun — trade-off klasik kekuatan racun besar, raga rapuh. |

---

## 🤕 3. Status Kondisi HP & Ambang Bahaya

| % HP Tersisa | Status Kondisi | Efek Mekanis & Penalti |
|---|---|---|
| **$100\% \text{ s/d } 50\%$** | **Sehat (Healthy)** | Kondisi prima, tidak ada penalti. |
| **$49\% \text{ s/d } 20\%$** | **Terluka (Wounded)** | Penalti Output Qi $-10\%$, penalti Evasion $-10\%$. |
| **$19\% \text{ s/d } 1\%$** | **Kritis (Critical)** | Penalti Output Qi $-30\%$, penalti Evasion $-25\%$, risiko *Qi Deviation* ringan. |
| **$0\%$** | **Pingsan / Dying State** | Tak sadarkan diri. Wajib mendapat pertolongan medis dalam 2 Shichen. |
| **$-1\% \text{ s/d } -30\%$** | **Nyaris Mati (Near Death)**| Memerlukan Tabib Realm $\ge$ Realm karakter; jika gagal $\to$ *Permanent Dantian Trauma*. |
| **Di bawah $-50\%$** | **Kematian Permanen** | Overkill ekstrem tervalidasi GM (karakter tewas permanen). |

---

## 🩹 4. Luka Fisik (Wound), Trauma Dantian, & Efek Racun

### 4.1 Categories Luka Fisik (Wound)
* **Minor Wound (Luka Ringan)**: Memar / goresan senjata ringan. Penalti Max Stamina $-10\%$.
* **Major Wound (Luka Berat)**: Tebasan dalam / patah tulang ekstremitas. Penalti Max HP $-25\%$, penalti Movement Speed $-20\%$.
* **Severe Wound (Luka Parah)**: Kerusakan organ dalam / pendarahan hebat. Penalti Max HP $-50\%$, penalti seluruh statistik tempur $-40\%$.

### 4.2 Trauma Bantian & Jiwa (Trauma)
* **Dantian Shock**: Gangguan aliran Qi akibat hentakan intim atau *Backlash*. Penalti Kecepatan Pemulihan Qi $-50\%$.
* **Soul Trauma**: Kerusakan jiwa batin akibat serangan mental/ilusi. Penalti Max Focus $-30\%$.

### 4.3 Racun & Pendarahan (Poison & Bleeding)
* **Poison Status (Sengatan Racun)**: Mengurangi HP sebesar $5 \text{ s/d } 30$ poin per Shichen tergantung grade racun (*Minor / Moderate / Lethal*) hingga diminumi *Antidote Pill*.
* **Bleeding (Pendarahan)**: Mengurangi HP dan Stamina sebesar $5$ poin per turn pertempuran hingga dibalut dengan perban/salep.

---

## 🌾 5. Sistem Kelaparan & Fasting Multiplier (Bi Gu / 辟谷)

Trope xianxia klasik: seiring meningkatnya Realm kultivasi, kultivator mampu menyerap energi Qi lingkungan untuk menggantikan makanan fisik (*Bi Gu / 辟谷*).

$$\text{DecayRatePerShichen}(\text{realm}) = \frac{\text{BaseDecayRate}}{\text{FastingMultiplier}(\text{realm})}$$

- $\text{BaseDecayRate} = 25 \text{ Satiety Points per Shichen}$ (Mortal biasa kehilangan kenyang penuh dalam 4 Shichen / 8 Jam).

### 📊 Fasting Multiplier per Realm Qianyuan

| Realm Kultivasi | FastingMultiplier | Waktu Sampai Lapar (Satiety < 30) |
|---|---|---|
| **0 — Non-Kultivator (Mortal)** | $\times 1,0$ | 4 Shichen (8 Jam) |
| **1 — Body Refining Realm (Qi-Guan)** | $\times 1,5$ | 6 Shichen (12 Jam) |
| **2 — Qi Gathering Realm (Qi-Ji)** | $\times 3,0$ | 12 Shichen (24 Jam / 1 Hari) |
| **3 — Foundation Establishment (Zhu-Ji)** | $\times 10,0$ | 40 Shichen (3,3 Hari) |
| **4 — Core Formation Realm (Jie-Dan)** | $\times 30,0$ | 120 Shichen (10 Hari) |
| **5 — Nascent Soul Realm (Yuan-Ying)** | $\times 100,0$ | 400 Shichen (33 Hari / 1 Bulan) |
| **6 — Soul Formation Realm (Hua-Shen)** | $\times 500,0$ | 2.000 Shichen (~5 Bulan) |
| **7 — Void Refinement Realm (Lian-Xu)** | $\times 2.000,0$ | 8.000 Shichen (~1,8 Tahun) |
| **8 — Dao Integration Realm (He-Dao)** | $\times 10.000,0$ | 40.000 Shichen (~9 Tahun) |
| **9 — Tribulation Transcendence (Du-Jie)**| **Tak Terbatas** | **Bi Gu Sempurna** (Tidak butuh makan selamanya). |

### 🥣 Status Efek Satiety
* **Satiety $70 \text{ s/d } 100$ (Kenyang)**: Bonus regenerasi Stamina & Qi $+10\%$.
* **Satiety $30 \text{ s/d } 69$ (Normal)**: Kondisi fisik biasa.
* **Satiety $10 \text{ s/d } 29$ (Lapar)**: Penalti Max Stamina $-25\%$, penalti Focus $-10$.
* **Satiety $0$ (Kelaparan Kritis)**: Pengurangan HP sebesar $5 \text{ poin per Shichen}$, **TIDAK BISA** melakukan terobosan Realm atau regenerasi Qi alami.

---

## 🛌 6. Mekanik Istirahat & Pemulihan (Rest & Recovery)

* **Short Rest (1 Shichen / 2 Jam)**: Memulihkan Stamina sebesar $30\%$, memulihkan Qi sebesar $25\%$. Memerlukan konsumsi $1 \text{ porsi makanan/air}$.
* **Long Rest (4 Shichen / 8 Jam)**: Memulihkan HP sebesar $50\%$, memulihkan Qi & Stamina penuh, serta mengurangi Fatigue sebesar $50 \text{ poin}$.
* **Pengobatan Tabib / Pill Alkimia**: Diperlukan untuk memulihkan *Major/Severe Wound*, menyembuhkan *Dantian Shock*, atau menghilangkan racun mematikan.

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Diperiksa Setiap Turn)

- [ ] Max HP dihitung otomatis berdasarkan formula `HP(realm, stage, law)`?
- [ ] Kerusakan HP, status Wound, dan Trauma dicatat di log bertimestamp?
- [ ] Penurunan Satiety dihitung presisi sesuai Fasting Multiplier Realm karakter?
- [ ] Penyembuhan luka berat dan trauma menggunakan pill/jasa tabib tervalidasi Sistem Ekonomi?
- [ ] Terobosan Realm memperbarui statistik Max HP dan Fasting Multiplier secara otomatis?

Jika **salah satu** poin di atas meragukan $\to$ Status Vitalitas **DIKOREKSI OTOMATIS** oleh AI GM.
