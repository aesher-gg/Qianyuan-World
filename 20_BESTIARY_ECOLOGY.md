# 🐺 Qianyuan-World — XXI. Bestiary & Ecology (Database Ekologi, Monster, & Spirit Beast)

> **Modul:** 20 — Bestiary Ecology
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Formula-Driven Stats — Habitat & Threat Standardized
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01`–`10` (modul regional), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap sebagai basis stats), `13_ECONOMY_MARKET_SYSTEM.md` (loot & grade value), `15_COMBAT_TACTICAL_SYSTEM.md` (resolusi pertempuran), `19_BEAST_BOND_SYSTEM.md` (penjinakan & kontrak)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Bestiarium

Bestiary Ecology adalah database canon dan panduan ekologi alam liar bagi seluruh binatang spiritual (*Spirit Beast*), monster, dan makhluk gaib di benua Qianyuan. Statistik tempur monster (HP dan Attack Power) tidak dikarang secara sepihak, melainkan diturunkan secara presisi dari formula `QiCap` Realm yang setara.

### Aturan Emas Anti-Cheat Bestiarium (Mandatory Enforced Rules)
1. **Statistik Terikat Formula**: HP dan Attack Power monster **WAJIB** dihitung menggunakan formula resmi `MonsterHP` dan `MonsterAttackPower`. Klaim monster dengan HP/Damage berlebihan tanpa alur cerita sah otomatis **DITOLAK**.
2. **Ambush Chance Dilempar AI GM**: Kemunculan monster liar (*Random Encounter*) atau penyergapan (*Ambush*) dilempar oleh AI GM menggunakan formula `AmbushChance`. Pemain **TIDAK BISA** menentukan sendiri ada/tidaknya monster di wilayah liar.
3. **Item Origin Log untuk Loot**: Seluruh material, kulit, kelenjar racun, dan *Spirit Core* yang didapat dari pembunuhan monster wajib dicatat ke log inventory (*Item Origin Log*) sebelum dapat diperjualbelikan (`13`) atau dipakai untuk alkimia (`16`).
4. **Pembatasan Cooldown Serangan Ultimate**: Serangan mematikan khas monster ($> 1,5\times \text{ Attack Power}$) dibatasi cooldown minimal 3 ronde pertempuran.

---

## 🎲 1. Formula Baku Statistik Monster (Monster Combat Formulas)

Statistik dasar monster dan binatang spiritual liar diturunkan dari `QiCap` Realm yang setara (`12`):

```
MonsterHP = QiCap(realm, stage) × 0,5 × LawHPMultiplier(element)
MonsterAttackPower = QiCap(realm, stage) × 0,15 × LawAttackMultiplier(element)
```

- `LawHPMultiplier`: Elemen Earth/Metal = ×1,5 | Wood/Life = ×1,3 | Water/Star/Ice = ×1,0 | Fire/Sun = ×0,9 | Poison/Blood = ×0,8.
- `LawAttackMultiplier`: Elemen Poison/Blood = ×1,4 | Fire/Sun = ×1,3 | Wind/Sound = ×1,2 | Water/Ice = ×1,0 | Earth/Metal = ×0,8.

---

## 🎯 2. Formula Kemunculan & Penyergapan (Ambush Chance)

Peluang disergap monster liar di wilayah terbuka dihitung per Shichen perjalanan:

```
AmbushChance = clamp(BaseChance × RegionalDangerMod × TimeMod, 5%, 80%)
```

- `BaseChance`: 5% per Shichen perjalanan.
- `RegionalDangerMod`: Jalur Perdagangan Aman = ×0.5 | Wilayah Liar Biasa = ×1.0 | Hutan Belantara / Rawa = ×2.0 | Zona Anomali Terlarang (*Scarlands/Abyss*) = ×4.0.
- `TimeMod`: Siang Hari = ×1.0 | Malam Hari = ×2.0 (monster nocturnal lebih aktif).

---

## 💎 3. Sistem Drop Loot & Rate Rarity

Loot dapat dipanen dari monster yang berhasil dikalahkan dalam pertempuran sah:

```
LootDropRate = BaseDropRate(rarity)
```

| Tingkat Rarity Loot | BaseDropRate | Contoh Material Loot |
|---|---|---|
| **Common (Umum)** | 70% – 90% | Daging ber-Qi, kulit kasar, bulu binatang, taring biasa. |
| **Rare (Jarang)** | 20% – 40% | Inti Monster (*Spirit Core*), kelenjar racun murni, sisik keras. |
| **Legendary / Boss** | 5% – 15% (100% Kill Pertama) | Kristal Purba Tier 7+, tanduk purba, esens jiwa monster. |

---

## 🛑 4. Standar Tingkat Bahaya (Threat Level Standard)

| Threat Level | Kategori Bahaya | Syarat Tim / Kultivator Disarankan |
|---|---|---|
| 🟢 **Green (Rendah)** | Monster Tingkat Awal (Tier 1–2). | Kultivator *Body Refining* / *Qi Gathering* (Realm 1–2). |
| 🟡 **Yellow (Sedang)** | Monster Tingkat Menengah (Tier 3). | Kultivator *Foundation Establishment* (Realm 3) atau tim 3 orang. |
| 🔴 **Red (Tinggi)** | Monster Tingkat Tinggi / Ganas (Tier 4–5). | Kultivator *Core Formation* / *Nascent Soul* (Realm 4–5). |
| 🖤 **Black (Calamity)** | Ancaman Bencana Wilayah / Boss Purba (Tier 6+).| Tetua Sekte / Kultivator *Soul Formation* / *Void Refinement* (Realm 6+). |

---

## 🌍 5. Katalog Monster & Spirit Beast Lintas Wilayah / Umum (Common Cross-Region)

Makhluk-makhluk berikut umum dijumpai melintasi berbagai wilayah benua Qianyuan-World:

| Nama Monster / Beast | Tier / Threat | Habitat Umum | Elemen Qi | HP | Attack | Loot Utama |
|---|---|---|---|---|---|---|
| **Babi Hutan Hutan (Wild Boar)** | Tier 1 / Green | Pinggiran Hutan / Desa | None | 25 | 7 | Daging Sega, Gading Babi (Tier 1). |
| **Gagak Spiritual (Spirit Raven)** | Tier 1 / Green | Pegunungan / Kota | Wind Qi | 20 | 6 | Bulu Hitam, Inti Qi Kecil (Tier 1). |
| **Serigala Malam (Night Wolf)** | Tier 2 / Green | Hutan Malam / Ngarai | Wind Qi | 125 | 37 | Kulit Serigala, Taring Tajam (Tier 2). |
| **Ular Lumpur (Mud Viper)** | Tier 2 / Green | Rawa / Tepi Sungai | Water + Poison | 100 | 42 | Bisa Ular Rawa, Kulit Ular (Tier 2). |
| **Kera Batu (Rock Ape)** | Tier 2 / Green | Perbukitan Batu | Earth Qi | 187 | 30 | Kulit Kera Batu, Batu Inti (Tier 2). |
| **Kawanan Lebah Spiritual (Spirit Bee)**| Tier 2 / Green | Kebun Herbal / Hutan | Wood Qi | 100 | 37 | Madu Spiritual, Sengat Lebah (Tier 2). |
| **Roh Pengembara (Wandering Ghost)** | Tier 3 / Yellow | Bekas Medan Perang | Fate Qi | 312 | 112 | Serpihan Baju Zirah, Inti Roh (Tier 3). |
| **Kumbang Pemakan Besi (Iron Beetle)** | Tier 2 / Green | Gua Tambang / Gunung | Metal Qi | 187 | 30 | Cangkang Besi, Bijih Mentah (Tier 2). |
| **Lipan Raksasa (Giant Centipede)** | Tier 3 / Yellow | Gua Tanah / Rawa | Poison Qi | 250 | 131 | Kelenjar Racun, Cangkang Duri (Tier 3). |
| **Rubah Ilusi (Mirage Fox)** | Tier 3 / Yellow | Hutan Kabut / Lembah | Star Qi | 312 | 93 | Bulu Rubah Giok, Inti Ilusi (Tier 3). |

---

## 🗺️ 6. Katalog Monster per 10 Wilayah Qianyuan-World

### 🏯 6.1 Ibu Kota Yuanjing & Perbatasan (`01`)
- **Anjing Penjaga Perbatasan (Gate Hound)** | Tier 2 (Green) | HP 125 | Attack 37 | Elemen: Earth Qi.
- **Roh Prajurit Gerbang (Gate Spirit)** | Tier 3 (Yellow) | HP 312 | Attack 112 | Elemen: Metal Qi.

### 🌊 6.2 Vermilion River Basin (`02`)
- **Vermilion Carp** | Tier 1 (Green) | HP 25 | Attack 7 | Elemen: Water Qi.
- **Mud Crocodile** | Tier 2 (Green) | HP 187 | Attack 30 | Elemen: Water + Earth Qi.
- **Misty Heron** | Tier 2 (Green) | HP 125 | Attack 45 | Elemen: Wind Qi.
- **Giant Water Snake** | Tier 3 (Yellow) | HP 312 | Attack 93 | Elemen: Water Qi.

### ⛰️ 6.3 Blackstone Skyreach (`03`)
- **Iron-Eating Beetle** | Tier 2 (Green) | HP 187 | Attack 30 | Elemen: Metal Qi.
- **Cliff Falcon** | Tier 2 (Green) | HP 125 | Attack 45 | Elemen: Wind Qi.
- **Stone Ridge Ape** | Tier 3 (Yellow) | HP 468 | Attack 75 | Elemen: Earth Qi.
- **Ironclad Bear** | Tier 4 (Red) | HP 4.687 | Attack 750 | Elemen: Earth + Metal Qi.

### 🏜️ 6.4 Ashen Sun Expanse (`04`)
- **Dune Camel** | Tier 1 (Green) | HP 25 | Attack 7 | Elemen: Sun Qi.
- **Flame-Viper** | Tier 2 (Green) | HP 112 | Attack 48 | Elemen: Fire Qi.
- **Sun Lizard** | Tier 2 (Green) | HP 112 | Attack 48 | Elemen: Fire + Sun Qi.
- **Sandstorm Scorpion** | Tier 3 (Yellow) | HP 281 | Attack 121 | Elemen: Fire + Sun Qi.

### 🌿 6.5 Nine-Reed Mire (`05`)
- **Mud Leech** | Tier 1 (Green) | HP 20 | Attack 10 | Elemen: Poison Qi.
- **Swamp Toad** | Tier 2 (Green) | HP 100 | Attack 42 | Elemen: Water + Poison Qi.
- **Giant Poison Centipede** | Tier 3 (Yellow) | HP 250 | Attack 131 | Elemen: Poison Qi.
- **Miasma Python** | Tier 3 (Yellow) | HP 250 | Attack 131 | Elemen: Water + Poison Qi.
- **Miasma Eel** | Tier 4 (Red) | HP 2.500 | Attack 1.312 | Elemen: Poison Qi.

### 🌊 6.6 Astral Tide Sea (`06`)
- **Star-Crab** | Tier 1 (Green) | HP 25 | Attack 7 | Elemen: Water Qi.
- **Spotted Coral Shark** | Tier 2 (Green) | HP 125 | Attack 37 | Elemen: Water Qi.
- **Sea Serpent** | Tier 4 (Red) | HP 3.125 | Attack 937 | Elemen: Water + Star Qi.
- **Astral Whale (Purba)** | Tier 6 (Black) | HP 78.125 | Attack 23.437 | Elemen: Water + Star Qi.

### 🌲 6.7 Whispering Root Forest (`07`)
- **Wood-Deer** | Tier 1 (Green) | HP 32 | Attack 7 | Elemen: Life Qi.
- **Green Vine Snake** | Tier 2 (Green) | HP 162 | Attack 35 | Elemen: Wood Qi.
- **Emerald Panther** | Tier 2 (Green) | HP 162 | Attack 42 | Elemen: Wood Qi.
- **Spore Wood Sentinel** | Tier 3 (Yellow) | HP 406 | Attack 89 | Elemen: Wood Qi.
- **Ancient Bear** | Tier 4 (Red) | HP 4.062 | Attack 890 | Elemen: Wood + Life Qi.

### ❄️ 6.8 Frostglass Crown (`08`)
- **Ice-Crystal Wolf** | Tier 3 (Yellow) | HP 312 | Attack 93 | Elemen: Ice Qi.
- **Frost Snow Ape** | Tier 3 (Yellow) | HP 312 | Attack 93 | Elemen: Ice + Stillness Qi.
- **Glacier Eagle** | Tier 3 (Yellow) | HP 312 | Attack 112 | Elemen: Ice + Wind Qi.
- **Frostglass Centipede** | Tier 4 (Red) | HP 3.125 | Attack 937 | Elemen: Ice Qi.

### 🌪️ 6.9 Hollow Gale Corridor (`09`)
- **Wind-Runner Swift** | Tier 1 (Green) | HP 25 | Attack 8 | Elemen: Wind Qi.
- **Hollow Canyon Lizard** | Tier 2 (Green) | HP 125 | Attack 45 | Elemen: Wind Qi.
- **Gale Falcon** | Tier 2 (Green) | HP 125 | Attack 45 | Elemen: Wind Qi.
- **Echo Bat** | Tier 2 (Green) | HP 125 | Attack 45 | Elemen: Sound Qi.

### 🌀 6.10 Fate Scarlands (`10`)
- **Scar-Gazer** | Tier 4 (Red) | HP 2.656 | Attack 843 | Elemen: Mutated Qi.
- **Chrono-Beast** | Tier 7 (Red) | HP 332.031 | Attack 105.468 | Elemen: Fate Qi.
- **Mutated Void Beast** | Tier 7 (Red) | HP 332.031 | Attack 105.468 | Elemen: Fate + Mutated Qi.
- **Spatial Anomaly Serpent** | Tier 8 (Black) | HP 1.660.156 | Attack 527.343 | Elemen: Fate Qi.

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Dicek Setiap Encounter)

- [ ] HP & Attack Power monster dihitung dari formula `MonsterHP` dan `MonsterAttackPower`?
- [ ] Kemunculan penyergapan (*Ambush*) dilempar menggunakan formula `AmbushChance`?
- [ ] Loot yang dipanen setelah pertempuran tercatat di *Item Origin Log* (`13`)?
- [ ] Monster tingkat Calamity (Tier 6+) hanya muncul di habitat resmi sesuai canon?
- [ ] Cooldown serangan ultimate khas monster (3 ronde) ditaati selama pertempuran?

Jika **salah satu** poin di atas meragukan → Encounter / Loot **DIKOREKSI OTOMATIS** oleh AI GM.
