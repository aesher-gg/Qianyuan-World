# ⚔️ Qianyuan-World — XVI. Combat Tactical System (Sistem Pertempuran & Taktik Qianyuan)

> **Modul:** 15 — Combat Tactical System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Turn-Based Tactical — Position & Posture Driven
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap sebagai basis Attack/Defense), `14_VITALITY_BODY_SYSTEM.md` (damage mengurangi HP & pemicuan trauma), `20_BESTIARY_ECOLOGY.md` (monster dan monster attack power)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Pertempuran

Pertarungan di dunia Qianyuan ditentukan secara seimbang dan adil bagi semua pihak — pemain, NPC, maupun monster liar. Pertarungan tidak ditentukan hanya oleh tingkatan Realm murni, melainkan juga oleh postur bertarung (*Posture*), taktik posisi (*Position*), jarak (*Distance*), kondisi medan (*Terrain*), serta pengelolaan energi Qi dan Stamina.

### Aturan Emas Anti-Cheat Pertempuran (Mandatory Enforced Rules)
1. **Aturan Giliran Wajib Bergantian**: Pertarungan berjalan berbasis giliran (*Turn-Based*). Setiap karakter bertindak berurutan berdasarkan skor *Initiative*. Tidak ada pihak yang dapat menyerang terus-menerus di luar gilirannya.
2. **Larangan Menentukan Aksi Musuh**: Pemain **TIDAK PERNAH** menentukan sendiri hasil serangan, hit/miss, atau kerusakan pada musuh. AI GM yang mengeksekusi kalkulasi formula dan menentukan reaksi NPC.
3. **Batas Ekonomi Aksi (Action Economy Ceiling)**: Satu giliran karakter **HANYA** mendapatkan tepat **1 Aksi Utama + 1 Aksi Kecil**. Deskripsi naratif serangan bertubi-tubi tetap dihitung sebagai 1 Aksi Utama dengan 1 kali resolusi damage.
4. **Log Pertempuran Bertimestamp**: Seluruh pengurangan HP, konsumsi Qi/Stamina, pemicuan status luka, dan giliran dicatat di log pertempuran bertimestamp dan tidak dapat diedit mundur.
5. **Kepatuhan Sifat NPC**: NPC dan monster **WAJIB** bertindak sesuai Karakteristik & Sifat yang tercantum pada tabel canon (misal: NPC penakut memilih bertindak defensif atau kabur).

---

## 🎲 1. Struktur Giliran (Initiative & Turn Order)

### 1.1 Formula Initiative
```
InitiativeScore = (RealmIndex × 100 + StageBonus) + Random(1–20)
```

- `RealmIndex`: 1 s/d 9 (Body Refining = 1, Qi Gathering = 2, dst).
- `StageBonus`: Early = 0, Mid = 10, Late = 20, Peak = 30.
- `Random(1–20)`: Dadu inisiatif yang dilempar AI GM di awal setiap ronde pertempuran.

### 1.2 Struktur Ronde Pertempuran
Satu Ronde Pertempuran adalah putaran di mana **setiap** karakter yang terlibat mendapatkan tepat 1 giliran. Inisiatif dilempar ulang pada setiap ronde baru untuk menjaga dinamika pertempuran.

---

## ⚡ 2. Ekonomi Aksi (Action Economy) — Inti Anti-Spam

Setiap giliran, setiap petarung mendapat alokasi aksi berikut:

### 2.1 Aksi Utama (Main Action) — Pilih Salah Satu:
- **Serang (Attack)**: Menggunakan serangan biasa, teknik andalan, atau jurus ultimate dari *Law Origin Log* yang sah.
- **Bertahan (Defend)**: Mengambil postur defensif untuk mengaktifkan *Active Defense Bonus*.
- **Gunakan Item / Pill**: Meminum obat penyembuh / memicu jimat (*Talisman*) dari inventory tervalidasi.
- **Kabur (Escape)**: Mencoba melarikan diri dari area pertempuran.
- **Merapalkan Formasi / Pemicuan Alat**: Mengaktifkan formasi penyegel atau alat spiritual.

### 2.2 Aksi Kecil (Minor Action) — Pilih Salah Satu:
- **Reposisi Kecil**: Berpindah jarak dekat (misal: melangkah mundur 2 langkah).
- **Bicara Singkat**: Ucapan 1 kalimat pendek yang tidak mengonsumsi Qi.
- **Tukar Equipment**: Memindahkan 1 senjata atau aksesoris antara slot terpakai dan inventory.

---

## 🗡️ 3. Formula Serangan & Damage (Damage Resolution)

### 3.1 Attack Power Karakter (Player & NPC Kultivator)
```
AttackPower(realm, stage, law) = QiCap(realm, stage) × 0,15 × LawAttackMultiplier(law)
```

| Jalur Hukum Kultivasi (`12`) | LawAttackMultiplier | Karakteristik Ofensif |
|---|---|---|
| **Hukum Racun Miasma & Anggrek Darah** (*Poison/Blood*) | ×1,4 | Ofensif racun tertinggi, pembusuk Dantian musuh. |
| **Hukum Matahari Membara & Api** (*Fire/Sun Qi*) | ×1,3 | Ofensif panas destruktif, pembakar perisai Qi. |
| **Hukum Angin Topan & Gema Suara** (*Wind/Sound Qi*) | ×1,2 | Serangan gelombang suara penetrasi tinggi. |
| **Hukum Gelombang Samudra & Bintang** (*Water/Star Qi*) | ×1,0 | Baseline standar seimbang. |
| **Hukum Pedang Es & Keheningan Abadi** (*Ice/Stillness*) | ×1,0 | Baseline standar dengan kontrol pembekuan. |
| **Hukum Raga Serat Kayu & Kehidupan** (*Wood/Life Qi*) | ×0,95 | Tahan banting, pemulihan tinggi, ofensif sedang. |
| **Hukum Anomali Ruang & Takdir** (*Fate/Mutated Qi*) | ×0,9 | Unik, manipulasi celah ruang dan waktu. |
| **Hukum Zirah Batu Hitam & Logam** (*Earth/Metal Qi*) | ×0,8 | Pertahanan raga terkuat, ofensif lebih rendah. |

### 3.2 Resolusi Final Damage
```
RawDamage = AttackPower(penyerang) × TechniqueTierBonus × PostureDamageMod × PositionDamageMod × HitConfirmed
FinalDamage = max(0, RawDamage − TotalDefense(bertahan))
```

- `TechniqueTierBonus`: Serangan Biasa = ×1.0 | Teknik Andalan (Signature) = ×1.5 | Jurus Ultimate = ×3.0.
- `HitConfirmed`: 1 jika serangan berhasil mengenai target, 0 jika meleset (*Miss*).

### 3.3 Peluang Kena (Hit Chance)
```
HitChance = clamp(70% + (RealmIndex_penyerang − RealmIndex_bertahan) × 5% + PositionHitMod + PostureHitMod, 10%, 95%)
```

---

## 🛡️ 4. Formula Pertahanan & Cooldown Jurus

### 4.1 Passive and Active Defense
```
PassiveDefense(realm, stage) = QiCap(realm, stage) × 0,05
ActiveDefenseBonus = QiCap(realm, stage) × 0,10
TotalDefense = PassiveDefense + (ActiveDefenseBonus jika memilih Aksi Utama "Bertahan", 0 jika tidak)
```

- **Passive Defense**: Selalu aktif secara otomatis melingkupi tubuh karakter.
- **Active Defense Bonus**: Hanya aktif saat karakter mengeksekusi Aksi Utama "Bertahan".

### 4.2 Cooldown Jurus Ultimate
- **Teknik Andalan (Signature ×1,5)**: Dapat digunakan setiap turn selama Qi mencukupi.
- **Jurus Ultimate (×3,0)**: Wajib menjalani **Cooldown 3 Ronde** setelah dieksekusi.

---

## 🧘 5. Status Posture & Taktik Posisi (Position & Distance)

### 5.1 Status Posture Tempur (Posture States)

| Status Posture | Bonus Mekanis | Penalti Mekanis |
|---|---|---|
| **Neutral Posture** | Seimbang, tanpa bonus. | Tanpa penalti. |
| **Offensive Posture** | Bonus Damage +20%. | Penalti Evasion & Defense -15%. |
| **Defensive Posture** | Bonus Active Defense +30%. | Penalti Damage -20%. |
| **Evasive Posture** | Bonus Evasion +30%. | Penalti Accuracy/Hit Rate -15%. |
| **Charging Posture** | Mengumpulkan Qi untuk Ultimate. | Rentan terhadap serangan sela (*Counter Interrupt*). |
| **Broken Posture** | - | Pertahanan hancur! Menerima Critical Damage +50% selama 1 turn. |

### 5.2 Taktik Posisi (Position States)
- **Ground Neutral**: Posisi berdiri biasa di tanah datar.
- **Elevated (Posisi Tinggi)**: Berada di atas tebing/pohon. Bonus Accuracy +15%, Bonus Damage Jarak Jauh +10%.
- **Concealed (Tersamar / Sembunyi)**: Berada di balik semak/kabut. Bonus Surprise Attack / Ambush +30%.
- **Cornered (Tersudut)**: Terjebak di dinding tebing. Penalti Evasion -25%.
- **Flanked / Surrounded (Dikeroyok)**: Diserang dari banyak sisi. Penalti Defense -20%.

### 5.3 Distance (Jarak Tempur)
- **Close Range (Melee)**: Jarak pisau, belati, pukulan telapak tangan.
- **Mid Range**: Jarak pedang, tombak, cambuk, serangan Qi jarak pendek.
- **Far Range**: Jarak busur panah, senjata lempar, serangan jarak jauh elemen Qi.

---

## 🔋 6. Biaya Qi per Aksi & Pukulan Kosong (Mortal Strike)

| Jenis Aksi Serangan | Konsumsi Biaya Qi |
|---|---|
| **Serangan Biasa** | `QiCap × 5%` |
| **Teknik Andalan (Signature)** | `QiCap × 12%` |
| **Jurus Ultimate** | `QiCap × 25%` (Cooldown 3 Ronde) |

### Pukulan Kosong (Mortal Strike) saat Qi = 0
Jika energi Qi karakter habis (`0 Qi`), karakter hanya dapat mengeksekusi **Pukulan Kosong (Mortal Strike)** tanpa energi batin:
```
MortalStrikeDamage = AttackPower × 0,3
```
- Penalti Hit Rate -15%, tanpa *TechniqueTierBonus*.

---

## 🏃 7. Mekanik Kabur (Escape) & Pertempuran Kelompok

### 7.1 Formula Peluang Kabur (Escape Chance)
```
EscapeChance = clamp(50% + (RealmIndex_kabur − RealmIndex_pengejar) × 5%, 10%, 90%)
```

- jika Aksi "Kabur" **GAGAL**, pihak lawan mendapatkan **Serangan Kesempatan (Opportunity Attack)** gratis di luar gilirannya.

### 7.2 Pertempuran Kelompok (Multi-Combatant)
- Seluruh petarung (pemain, sekutu, banyak musuh) dimasukkan ke dalam **satu urutan Initiative bersama**.
- Jika dikeroyok, setiap musuh mendapatkan giliran independennya sendiri sesuai Initiative.

---

## 🌿 8. Pengaruh Kondisi Medan & Lingkungan (Terrain Interactions)

- **Mud / Swamp (Rawa Berlumpur)**: Penalti Movement Speed & Evasion -20% (kecuali pengguna teknik Air/Rawa).
- **High Wind (Badai Angin Kencang)**: Penalti Akurasi Senjata Panah -20%.
- **Extreme Heat / Cold (Suhu Ekstrem)**: Pengeluaran Stamina melonjak +25% per turn.

---

## 🛡️ 9. Checklist Validasi AI GM (Wajib Dicek Setiap Turn Pertempuran)

- [ ] Urutan Initiative ditetapkan di awal ronde dan dipatuhi ketat?
- [ ] Setiap karakter hanya melakukan 1 Aksi Utama + 1 Aksi Kecil per giliran?
- [ ] Penentuan Hit/Miss dan Damage dilakukan oleh AI GM menggunakan formula resmi?
- [ ] Biaya Qi dikurangi dan Cooldown Jurus Ultimate (3 ronde) ditaati?
- [ ] Modifikator Posture, Position, dan Terrain dihitung ke dalam Final Damage?
- [ ] NPC dan monster bertindak sesuai Karakteristik & Sifat canon masing-masing?

Jika **salah satu** poin di atas meragukan → Eksekusi Aksi **DIULANG SEGERA** oleh AI GM sesuai mekanik resmi.
