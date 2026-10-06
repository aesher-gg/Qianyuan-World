# 📇 Qianyuan-World — Players Database Index & Template Save Standar

> **Modul:** Players Index (`players.md`)
> **Fungsi:** Katalog direktori pemain aktif dan format baku template save karakter awal di dalam direktori `players/`.
> **Sifat Wajib:** READ-ONLY bagi AI GM selama roleplay berlangsung. AI GM memanggil file spesifik di `players/` HANYA saat karakter baru dimuat pertama kali (Jalur A di `00_CORE_RULES_AI_GM.md`).
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.6 (3 jalur input pemain), `12_CULTIVATION_RESONANCE_SYSTEM.md` (kalkulasi QiCap), `13_ECONOMY_MARKET_SYSTEM.md` (mata uang & item), `17_ROLES_PROFESSIONS_SYSTEM.md` (role & profesi)

---

## 📇 1. Overview & Aturan Read-Only Katalog

`players.md` dan file individual di direktori `players/` murni merupakan **katalog template data awal** karakter. Konsekuensi teknis bagi AI Game Master:

1. **Sifat Read-Only**: AI GM **TIDAK PERNAH** menulis, mengedit, merevisi, atau memperbarui isi file `players.md` maupun file di direktori `players/`. File-file ini hanya dapat diubah secara manual oleh pemilik repository (admin/developer).
2. **Prosedur Fetch Awal (Jalur A)**: Saat pemain menyebutkan nama karakter terdaftar atau mengirimkan link RAW file di `players/`, AI GM melakukan *fetch* satu kali untuk memuat statistik awal karakter sebagai titik mulai narasi.
3. **Pencatatan Perkembangan**: Setelah roleplay berjalan, seluruh perkembangan karakter (HP, Qi, Item, Exp, Level, Waktu World) dicatat dan ditransfer secara dinamis murni lewat **blok "Profil Karakter"** di dalam percakapan pada setiap giliran balasan (§2 di `00`).

---

## 📋 2. Player Directory Registry (Katalog Pemain Terdaftar)

| Player ID | Character Name | Starting Region | Realm & Primary Role | File Path | Raw Link | Status |
|---|---|---|---|---|---|---|
| `PLR-001` | **Lin Feng** | Vermilion River Basin (`02`) | Body Refining Early · Martial Swordsman | `players/Lin_Feng.md` | `https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Lin_Feng.md` | 🟢 Ready to Load |
| `PLR-002` | **Ye Chen** | Blackstone Skyreach (`03`) | Body Refining Early · Forge Blacksmith | `players/Ye_Chen.md` | `https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Ye_Chen.md` | 🟢 Ready to Load |

---

## 📄 3. Save File Format Template Standard (`players/<character_name>.md`)

Setiap pembuatan file save karakter baru di direktori `players/<character_name>.md` wajib menggunakan struktur baku sebagai berikut:

```markdown
# 📜 CHARACTER SAVE FILE: [CHARACTER NAME]

## 1. Basic Info
- **Player ID**: [Misal: PLR-001]
- **Character Name**: [Nama Karakter]
- **Origin / Background**: [Asal-usul / Background Cerita Singkat]
- **Primary Role**: [Role Utama per `17` - Misal: Combat Swordsman]
- **Secondary Role**: [Profesi Sekunder per `17` - Misal: Alchemist / Blacksmith]
- **Social Role**: [Kedudukan Sosial - Misal: Sanxiu / Wandering Cultivator]

## 2. Cultivation Profile
- **Realm**: [Major Realm per `12` - Misal: Body Refining Realm]
- **Stage**: [Stage per `12` - Early / Mid / Late / Peak]
- **Qi Capacity (QiCap)**: [Formula: `QiCap = RealmBase × StageMultiplier` per `12`]
- **Meridian Pattern**: [Pola Meridian Terbuka - Misal: 3/9 Meridian Currents]
- **Dao Resonance**: [Resonansi Elemen Utama - Misal: Water + Wood Qi]
- **Insight Points**: [5 / 100]

## 3. Vital Attributes
- **HP**: [Formula: `HPMax = QiCap × 0.5 + PhysicalBonus` per `14`]
- **Qi**: [Sama dengan QiCap saat penuh]
- **Stamina**: [100 / 100]
- **Satiety**: [100 / 100]
- **Focus**: [100 / 100]
- **Resolve**: [100 / 100]
- **Fatigue**: [0 / 100]
- **Status Luka / Trauma**: Normal / Non-Wounded

## 4. Equipment & Inventory
- **Senjata Utama**: [Nama Senjata - Tier / Grade Value per `13`]
- **Zirah / Pelindung**: [Nama Zirah / Pakaian Ber-Qi]
- **Aksesoris**: [Cincin Pouch / Liontin Identitas]
- **Mata Uang**: [Gold Taels] × X | [Silver Taels] × XX | [Copper Taels] × XXX | [Spirit Stones Tier 1] × XX

**Inventory (Tas / Pouch)**:
- [Item 1 - Kuantitas - Deskripsi Singkat]
- [Item 2 - Kuantitas - Deskripsi Singkat]

## 5. Techniques & Arts
1. [Nama Jurus 1] - Element: [Elemen] - Mastery: [Basic / Proficient / Master]
2. [Nama Jurus 2] - Element: [Elemen] - Mastery: [Basic / Proficient / Master]

## 6. Location & World State
- **Current Region**: [Misal: Vermilion River Basin (`02`)]
- **Specific Location**: [Misal: Kota Vermilion Port / Pelabuhan Zhuque]
- **Current World Date**: Bulan [1–9], Tanggal [1–30], Shichen [1–12]
```

---

## 🛠️ 4. Panduan Inisiasi Karakter Baru AI GM

Saat AI GM menerima giliran pertama dari pemain, AI GM wajib mengidentifikasi Jalur Input Karakter (§1.6 di `00`):

1. **Jalur A (Karakter Katalog Terdaftar)**: AI GM membaca file di `players/<character_name>.md`, memuat seluruh nilai atribut di atas ke dalam blok "Profil Karakter" di balasan pertama, dan menarasikan awal kedatangan karakter di lokasi spesifik.
2. **Jalur B (Melanjutkan Sesi Sebelumnya)**: AI GM mengambil data dari blok "Profil Karakter" terakhir yang ditempelkan pemain tanpa menyentuh folder `players/`.
3. **Jalur C (Karakter Spontan Baru)**: AI GM menggunakan statistik default awal untuk *Body Refining Realm Early Stage*:
   - `QiCap`: **50**
   - `HPMax`: **25** (`50 × 0.5`)
   - `Stamina`: **100** | `Satiety`: **100** | `Focus`: **100** | `Resolve`: **100** | `Fatigue`: **0**
   - `Mata Uang`: 50 Silver Taels & 100 Copper Taels.
   - `Equipment`: Pakaian Baju Kain Biasa & Pedang/Pisau Besi Tua.
