# 🏮 Qianyuan-World — World Bible (Modular Repository Edisi Qianyuan)

**Versi**: 2.0 (Reorganisasi & Modul Terstruktur)
**Genre**: Xianxia · Wuxia · Kultivasi · Hardcore Realism
**Tujuan**: Menjalankan roleplay kultivasi yang adil, mendalam, konsisten, taktis, dan realistis bersama AI Game Master (AI-GM) tanpa perlu menyalin satu dokumen tunggal yang raksasa — dioptimalkan agar AI-GM menjelajah secara otomatis lewat tautan modul yang jelas.

---

> 🧭 **Cara tercepat mulai bermain:** Tempelkan satu link saja — **link RAW `INDEX.md`** — lalu sebutkan nama karaktermu (atau tempel link RAW file karaktermu dari folder `players/`). AI-GM akan menjelajah sendiri ke modul lain sesuai kebutuhan cerita. Lihat bagian "💬 Cara Bermain" di bawah.

---

## 📂 Struktur Modul Repository

Repository Qianyuan-World diorganisasikan secara modular ke dalam file `.md` terstruktur sebagai berikut:

| Kode / Ikon | Nama File | Fungsi Utama & Isi Modul |
|---|---|---|
| 🧭 **INDEX** | `INDEX.md` | **Hub Navigasi Utama** — Seluruh link RAW modul & logika pemicu fetch AI-GM. *(Inilah yang ditempelkan ke AI)* |
| 📇 **PLAYERS** | `players.md` | Katalog data awal karakter & link file individual di folder `players/` *(Read-Only AI-GM)* |
| 👤 **PLAYERS/**| `players/*.md` | Folder berisi data awal karakter individual ringkas |
| 📖 **README** | `README.md` | Peta navigasi & dokumentasi panduan manusia ini |
| **00** | `00_CORE_RULES_AI_GM.md` | Aturan mutlak AI-GM, anti-cheat, format respon wajib, cheat-sheet formula |
| **01** | `01_WORLD_OVERVIEW_AND_CAPITAL.md` | Peta jarak benua, Nine Meridian Currents, Ibu Kota Yuanjing & Struktur 7 Cincin |
| **02–10** | `02`–`10_*.md` | Modul geografis, ekologi Qi, kota/desa, NPC, dan bahaya regional (9 Wilayah + 1 Scarlands) |
| **11** | `11_CROSS_REGION_ORGANIZATIONS.md` | Imperial Court, Merchant Alliance, Beast Union, Courier, Dao Registry, Bounty Tribunal, Sanxiu, Demonic Outlaws |
| **12** | `12_CULTIVATION_RESONANCE_SYSTEM.md` | Inisiasi Mortal, 9 Major Realm, Formula QiCap, Law Origins, Nine Meridian Laws, Tribulasi, Karma |
| **13** | `13_ECONOMY_MARKET_SYSTEM.md` | Mata uang resmi, Tier Base Values, Dynamic Price Formula, Harga Jasa/Aset, Haggling Rules |
| **14** | `14_VITALITY_BODY_SYSTEM.md` | Formula HP Universal, Law HP Multiplier, Wound/Trauma, Satiety Decay, Fasting Multipliers (Bi Gu), Rest |
| **15** | `15_COMBAT_TACTICAL_SYSTEM.md` | Initiative, Action Economy (1 Main + 1 Minor), Hit Chance, Damage Resolution, Posture/Position States |
| **16** | `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` | Alchemy, Forging, Formation Array, Talisman Inscription, Quality Grades, Success Rates & Risks |
| **17** | `17_ROLES_PROFESSIONS_SYSTEM.md` | 10 Primary Combat Roles, 10 Secondary Professions (5 Tiers), Social Roles & Access Rights |
| **18** | `18_SPIRIT_GARDENING_SYSTEM.md` | Spirit Soil Grades 1–6, Growth Duration Formula, Spirit Water & Bee Pollination, Hybrid Plants |
| **19** | `19_BEAST_BOND_SYSTEM.md` | 3 Contract Types, Trust Metric (0–100), Taming Success Rate, Bloodline Awakening Evolution |
| **20** | `20_BESTIARY_ECOLOGY.md` | MonsterHP & Attack formulas, Ambush Chance, Loot Drop Rates, Threat Levels, Monster Catalogs |
| **21–30** | `21`–`30_*.md` | 10 File Individual Sekte & Perguruan Utama (Hierarki, Fasilitas, Kurikulum Teknik, Rahasia) |
| **31** | `31_SPIRIT_AIRSHIP_SYSTEM.md` | Sistem Kapal Udara Lingzhou & Transportasi Udara |
| **32–35** | `32`–`35_*.md` | Database Konten Kustom (Event, Laws, Sects, Techniques) |
| 💰 **ORACLE** | `ECONOMY_ORACLE.md` | Cheat-sheet Referensi Harga Cepat GM |

---

## 🚀 Cara Setup di GitHub

1. Buat repository baru di GitHub — **wajib PUBLIC** agar RAW link dapat diakses AI-GM secara langsung.
2. Upload seluruh file `.md` ini ke root repo — termasuk `INDEX.md`, `players.md`, dan folder `players/`.
3. Format RAW link resmi GitHub:
   `https://raw.githubusercontent.com/USERNAME/REPO/main/NAMA_FILE.md?v=1`
4. Buka `INDEX.md` dan pastikan seluruh link RAW sudah cocok dengan username/repo GitHub-mu.
5. Selesai! Kamu hanya perlu menempelkan link RAW `INDEX.md` setiap kali membuka sesi permain baru.

---

## 💬 Cara Bermain — Metode Utama (Single Link / Direct Character Link)

Pilih salah satu template perintah di bawah sesuai situasimu:

### A. Mulai Karakter dari Katalog `players.md` (Pertama Kali Dimainkan)

```text
Analisis link berikut ini secara penuh dan pelajari dengan seksama untuk memulai permainan roleplay ini:

https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1 dan https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md?v=1

untuk Memulai permainan sebagai Inggo!
```
*(Ganti `Inggo.md` dan `Inggo` dengan nama karaktermu di katalog)*

### B. Karakter Custom Baru (Belum Terdaftar di Katalog)

```text
Kamu adalah AI Game Master untuk roleplay Qianyuan-World. Baca dan ikuti seluruh isi link berikut sebagai satu-satunya sumber kebenaran:

https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1

Data Karakter Baru Saya:
- Nama Karakter: [Nama Karaktermu]
- Wilayah Awal: [Pilih Wilayah: misal Vermilion River Basin]
- Identitas & Profesi: [Sebutkan Latar Belakang & Primary/Secondary Role]
```

### C. Melanjutkan Karakter di Sesi Baru (Save File Diperbarui)

```text
Analisis link berikut ini secara penuh dan pelajari dengan seksama untuk melanjutkan permainan roleplay ini:

https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1 dan https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md?v=1

untuk Melanjutkan permainan sebagai Inggo!
```

---

## ⏳ Aturan Sesi Roleplay & Sistem Save Data

1. **Sesi Roleplay Tanpa Batas Step**:
   - Sesi roleplay berjalan tanpa batasan jumlah step (`💬 Step: Tanpa Batas`).
   - Pemain bebas melanjutkan petualangan sesuka hati tanpa pembekuan sesi.
2. **Alur Save Karakter**:
   - Pemain bebas menyalin (*copy*) isi dari blok **Profil Karakter** di akhir respon AI-GM kapan saja.
   - Kirimkan data Profil Karakter tersebut kepada Admin (pemilik repo) untuk dimasukkan/diperbarui ke dalam file save resmi di `players/<Nama_Karakter>.md`.
   - Setelah Admin memperbarui file di repository, kamu dapat membuka sesi baru dan menempelkan link `INDEX.md` + link file karaktermu untuk memuat data terkini!

---

## 🎯 Metode Manual (Fallback, Jika AI Tidak Bisa Fetch Link)

Jika AI yang kamu gunakan tidak memiliki kemampuan membuka link/browse, kamu dapat menempelkan modul secara manual. Tempelkan modul sesuai kebutuhan berikut:

| Situasi Roleplay | Modul yang Ditempelkan Manual |
|---|---|
| **Selalu (Tiap Sesi Baru / Ganti Chat)** | `00_CORE_RULES_AI_GM.md` + Modul Wilayah lokasi karakter saat ini |
| **Mulai Karakter Pertama Kali** | Modul Wilayah + file karakter spesifik di `players/<Nama_Karakter>.md` |
| **Melanjutkan Sesi** | Tempel manual blok **Profil Karakter** terakhir dari percakapan sebelumnya |
| **Karakter Pindah Wilayah** | Ganti modul wilayah ke wilayah tujuan (`02`–`10`) |
| **Menerobos Realm / Klaim Teknik** | Tambahkan `12_CULTIVATION_RESONANCE_SYSTEM.md` |
| **Transaksi / Berdagang / Cek Harga** | Tambahkan `13_ECONOMY_MARKET_SYSTEM.md` |
| **Pertarungan Taktis / Melawan Monster** | Tambahkan `15_COMBAT_TACTICAL_SYSTEM.md` + `20_BESTIARY_ECOLOGY.md` |

---

## 🌏 Dunia Qianyuan dalam Angka

- **Luas Total**: $\pm 52$ Juta li² · **Populasi**: $\pm 310$ Juta Jiwa · **Kekayaan Total**: $\pm 4,5$ Miliar Tael Perak.
- **9 Wilayah Regional + 1 Scarlands**: Vermilion, Blackstone, Ashen Sun, Nine-Reed, Astral Tide, Whispering Root, Frostglass, Hollow Gale, Fate Scarlands, & Ibu Kota Yuanjing.
- **9 Major Realm $\times$ 4 Stage**: Body Refining hingga Tribulation Transcendence.
- **9 Hukum Kultivasi Utama**: Digerakkan oleh aliran gaib Nine Meridian Currents.
- **10 Sekte Utama & 10 Organisasi Lintas Wilayah**.

---

## ✅ Checklist Sebelum Bermain

- [ ] Repository GitHub sudah publik & seluruh file ter-upload (termasuk folder `players/`).
- [ ] Link RAW `INDEX.md` dan `players/Inggo.md` sudah dites dapat dibuka di browser.
- [ ] Tahu nama dan lokasi awal karaktermu.
