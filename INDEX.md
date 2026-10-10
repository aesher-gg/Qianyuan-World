# 🧭 Qianyuan-World — INDEX (Master Navigation Hub & World Bible)

> **Ini adalah SATU-SATUNYA link raw yang perlu ditempel pemain di setiap awal sesi roleplay.**
> Semua modul lain (aturan inti, wilayah, sistem, sekte/perguruan, data karakter) dijangkau AI-GM secara otomatis dari sini lewat `read_file` / web fetch, sesuai kondisi dan perkembangan cerita roleplay.
>
> **Untuk AI Game Master (AI-GM):** baca seluruh file ini dulu sampai habis, lalu jalankan **Prosedur Bootstrap** di §0 SEBELUM menulis balasan apa pun ke pemain. Jangan menjawab dari ingatan/memori bebas — dunia ini hanya sah kalau datanya berasal dari modul-modul resmi yang ditautkan di sini.

---

## 📂 Struktur Modul & Direktori Lengkap Repository

| Kode | File Name | Link RAW (Klik / Fetch) | Isi Singkat & Fungsi |
|---|---|---|---|
| 🧭 | `INDEX.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1 | Master Navigation Hub — seluruh link + logika navigasi AI-GM ✅ **Wajib ditempel pemain** |
| 📇 | `players.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players.md?v=1 | Katalog data awal karakter (statis, dikelola admin) — memuat link RAW ke file individual di `players/` |
| 👤 | `players/` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/ | Folder data awal karakter individual (difetch spesifik saat pertama kali dimainkan) |
| — | `README.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/README.md?v=1 | Dokumentasi panduan setup manusia & aturan umum |
| **00** | `00_CORE_RULES_AI_GM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/00_CORE_RULES_AI_GM.md?v=1 | Aturan mutlak AI GM, anti-cheat, format respon wajib, cheat-sheet formula — **selalu difetch pertama** |
| **01** | `01_WORLD_OVERVIEW_AND_CAPITAL.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md?v=1 | Peta jarak benua Qianyuan, Nine Meridian Currents, Ibu Kota Yuanjing & 7 Cincin |
| **02** | `02_VERMILION_RIVER_BASIN.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/02_VERMILION_RIVER_BASIN.md?v=1 | Vermilion River Basin: Pelabuhan Zhuque, Desa Bunga Embun, kota & NPC perairan |
| **03** | `03_BLACKSTONE_SKYREACH.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/03_BLACKSTONE_SKYREACH.md?v=1 | Blackstone Skyreach: Benteng Skyreach, Lembah Anvil, Gua Tambang Besi Kuno |
| **04** | `04_ASHEN_SUN_EXPANSE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/04_ASHEN_SUN_EXPANSE.md?v=1 | Ashen Sun Expanse: Kota Oasis Sunfire, Benteng Sandgate, Istana Sunken Sun |
| **05** | `05_NINE_REED_MIRE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/05_NINE_REED_MIRE.md?v=1 | Nine-Reed Mire: Desa Panggung Mirewood, Pasar Kabut Kelam, Labirin Alang-Alang |
| **06** | `06_ASTRAL_TIDE_SEA.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/06_ASTRAL_TIDE_SEA.md?v=1 | Astral Tide Sea: Pelabuhan Star-Compass, Benteng Pulau Coral, Palung Abyss |
| **07** | `07_WHISPERING_ROOT_FOREST.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/07_WHISPERING_ROOT_FOREST.md?v=1 | Whispering Root Forest: Desa Root-Bound, Pondok Pemburu, World Tree Sanctuary |
| **08** | `08_FROSTGLASS_CROWN.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/08_FROSTGLASS_CROWN.md?v=1 | Frostglass Crown: Benteng Salju Frost-Edge, Desa Gletser Bening, Puncak Meditasi |
| **09** | `09_HOLLOW_GALE_CORRIDOR.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/09_HOLLOW_GALE_CORRIDOR.md?v=1 | Hollow Gale Corridor: Kota Wind-Gale, Pos Tebing Bisik, Lembah Gema |
| **10** | `10_FATE_SCARLANDS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/10_FATE_SCARLANDS.md?v=1 | Fate Scarlands: Pos Perbatasan Scar-Watch, Kemah Penjelajah, Kota Terbalik |
| **11** | `11_CROSS_REGION_ORGANIZATIONS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/11_CROSS_REGION_ORGANIZATIONS.md?v=1 | Imperial Court, Merchant Alliance, Beast Union, Courier, Dao Registry, Bounty Tribunal, Sanxiu, Demonic Outlaws |
| **12** | `12_CULTIVATION_RESONANCE_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/12_CULTIVATION_RESONANCE_SYSTEM.md?v=1 | Inisiasi Mortal, 9 Major Realm, Aturan Terobos Stage (Early→Mid→Late→Peak), Formula QiCap, Law Origins, Nine Meridian Laws, Tribulasi, Karma |
| **13** | `13_ECONOMY_MARKET_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/13_ECONOMY_MARKET_SYSTEM.md?v=1 | Mata uang resmi, Tier Base Values, Dynamic Price Formula, Harga Jasa/Aset, Haggling Rules |
| **14** | `14_VITALITY_BODY_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/14_VITALITY_BODY_SYSTEM.md?v=1 | Formula HP Universal, Law HP Multiplier, Wound/Trauma, Satiety Decay, Fasting Multipliers (Bi Gu), Rest |
| **15** | `15_COMBAT_TACTICAL_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/15_COMBAT_TACTICAL_SYSTEM.md?v=1 | Initiative, Action Economy (1 Main + 1 Minor), Hit Chance, Damage Resolution, Posture/Position States, Cooldowns |
| **16** | `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md?v=1 | Alchemy, Forging, Formation Array, Talisman Inscription, Quality Grades, Success Rates & Risks |
| **17** | `17_ROLES_PROFESSIONS_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/17_ROLES_PROFESSIONS_SYSTEM.md?v=1 | 10 Primary Combat Roles, 10 Secondary Professions (5 Tiers), Social Roles & Access Rights |
| **18** | `18_SPIRIT_GARDENING_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/18_SPIRIT_GARDENING_SYSTEM.md?v=1 | Spirit Soil Grades 1–6, Growth Duration Formula, Spirit Water & Bee Pollination, Hybrid Crossbreeding, Plant Catalog |
| **19** | `19_BEAST_BOND_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/19_BEAST_BOND_SYSTEM.md?v=1 | 3 Contract Types, Trust Metric (0–100), Taming Success Rate, Bloodline Awakening Evolution, Shared Telepathy |
| **20** | `20_BESTIARY_ECOLOGY.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/20_BESTIARY_ECOLOGY.md?v=1 | MonsterHP & Attack formulas, Ambush Chance, Loot Drop Rates, Threat Levels, Common & Regional Monster Catalogs |
| **21–30** | *(10 file sekte/perguruan individual)* | — | Lihat **§1a** di bawah untuk daftar lengkap per-file — **JANGAN** fetch semuanya sekaligus |
| **31** | `31_SPIRIT_AIRSHIP_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/31_SPIRIT_AIRSHIP_SYSTEM.md?v=1 | Sistem Kapal Udara Lingzhou, rute penerbangan, dan pertempuran udara |
| **32** | `32_CUSTOM_EVENTS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/32_CUSTOM_EVENTS.md?v=1 | **Event khusus & krisis wilayah** — diisi Admin/AI GM saat terjadi krisis/festival |
| **33** | `33_CUSTOM_LAWS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/33_CUSTOM_LAWS.md?v=1 | **Hukum Kultivasi kustom** — ciptaan pemain/Admin, dicatat di sini agar resmi |
| **34** | `34_CUSTOM_SECTS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/34_CUSTOM_SECTS.md?v=1 | **Sekte/Perguruan kustom** — ciptaan pemain/Admin, dicatat di sini agar resmi |
| **35** | `35_CUSTOM_TECHNIQUES.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/35_CUSTOM_TECHNIQUES.md?v=1 | **Teknik & Jurus Kustom** — ciptaan pemain/Admin, dicatat di sini agar resmi |
| **Oracle** | `ECONOMY_ORACLE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/ECONOMY_ORACLE.md?v=1 | Cheat-sheet Referensi Harga Cepat GM |

---

### 1a. Direktori Sekte & Perguruan Utama (10 File Individual)

> Setiap sekte/perguruan utama Qianyuan-World memiliki **file sendiri**, lengkap dengan hierarki, fasilitas, artefak/pusaka, kurikulum teknik bertingkat, Hukum kultivasi detail, relasi antar-faksi, dan rahasia internal. **Fetch HANYA** link file yang relevan dengan situasi saat ini.

| Sekte / Perguruan Utama | Wilayah Dominan | Link RAW (Langsung Klik / Fetch AI) |
|---|---|---|
| **Moonlit Abyss Sect** | Astral Tide Sea (`06`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/21_MOONLIT_ABYSS_SECT.md?v=1 |
| **River Lantern School** | Vermilion River Basin (`02`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/22_RIVER_LANTERN_SCHOOL.md?v=1 |
| **Blackstone Vow Sect** | Blackstone Skyreach (`03`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/23_BLACKSTONE_VOW_SECT.md?v=1 |
| **Red Sand Caravan** | Ashen Sun Expanse (`04`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/24_RED_SAND_CARAVAN.md?v=1 |
| **Mire Blood Orchid Sect** | Nine-Reed Mire (`05`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/25_MIRE_BLOOD_ORCHID_SECT.md?v=1 |
| **Star Compass School** | Astral Tide Sea (`06`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/26_STAR_COMPASS_SCHOOL.md?v=1 |
| **Rootbound Covenant Sect** | Whispering Root Forest (`07`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/27_ROOTBOUND_COVENANT_SECT.md?v=1 |
| **Frost Edge School** | Frostglass Crown (`08`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/28_FROST_EDGE_SCHOOL.md?v=1 |
| **Hollow Wind Sect** | Hollow Gale Corridor (`09`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/29_HOLLOW_WIND_SECT.md?v=1 |
| **Golden Thread Medicine Hall** | Ibu Kota Yuanjing (`01`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/30_GOLDEN_THREAD_MEDICINE_HALL.md?v=1 |

---

## 🚀 Cara Setup di GitHub

1. Buat repository baru di GitHub — **wajib PUBLIC** agar raw link dapat diakses AI tanpa otentikasi token khusus.
2. Upload seluruh file `.md` ke root repo — termasuk `INDEX.md`, `players.md`, dan folder `players/`.
3. Format link RAW resmi untuk setiap file adalah:
   `https://raw.githubusercontent.com/USERNAME/REPO/main/NAMA_FILE.md?v=1`
4. Buka `INDEX.md` dan `players.md`, pastikan seluruh link RAW sudah mengarah ke username dan repository milikmu sendiri.
5. Setelah itu, pemain cukup menempelkan link RAW `INDEX.md` saat membuka sesi roleplay baru bersama AI-GM.

---

## 💬 Cara Main — Metode Utama (Direct Character Link)

Pilih salah satu dari template prompt di bawah sesuai situasi permainan Anda:

### A. Mulai Karakter Terdaftar di Katalog `players.md` (Sesi Pertama)
```markdown
Analisis dan pelajari seluruh aturan dari link berikut untuk memulai permainan roleplay ini:
https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1
dan
https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md?v=1
untuk memulai permainan sebagai Inggo!
```
*(Ganti `Inggo.md` dan `Inggo` sesuai dengan file data karakter yang tuju).*

### B. Karakter Custom Baru (Belum Terdaftar di `players.md`)
```markdown
Kamu adalah AI Game Master untuk roleplay Qianyuan-World. Baca dan ikuti seluruh aturan dari link berikut sebagai satu-satunya sumber kebenaran:

https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1

Data Karakter Baru Saya:
- Nama: [Nama Karakter]
- Lokasi Awal: [Pilih salah satu lokasi dari modul 02–10]
- Role Utama / Profesi: [Pilih dari modul 17]
```

### C. Melanjutkan Karakter di Sesi Baru (Menggunakan File Save Repo Terbaru)
```markdown
Analisis dan pelajari seluruh aturan dari link berikut untuk melanjutkan permainan roleplay ini:
https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/INDEX.md?v=1
dan
https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md?v=1
untuk melanjutkan permainan sebagai Inggo!
```

---

## ⏳ Aturan Sesi Roleplay & Sistem Save Data (Tanpa Batas Step)

1. **Sesi Roleplay Tanpa Batas Step**:
   - Sesi roleplay berjalan tanpa batasan jumlah step (`💬 Step: Tanpa Batas`).
   - Tidak ada perhitungan pembekuan sesi atau pemicu batas maks step. Pemain bebas melanjutkan perjalanan kapan saja.
2. **Alur Save Karakter**:
   - Pemain bebas menyalin (*copy*) blok **Profil Karakter** terkini dari balasan AI kapan saja.
   - Pemain mengirimkan data Profil Karakter tersebut kepada Admin (pemilik repo) untuk dimasukkan/diperbarui ke dalam file save resmi `players/<Nama_Karakter>.md`.
   - Setelah Admin memperbarui file save di repo, Anda dapat membuka chat baru kapan saja dan menempelkan link RAW file save tersebut bersama `INDEX.md`.

---

## 🎯 Metode Manual (Fallback, Jika AI Tidak Bisa Fetch Link)

Jika AI platform yang Anda gunakan tidak dapat memanggil link secara otomatis, Anda dapat menempelkan isi file modul secara manual berdasarkan kebutuhan:

| Situasi Roleplay | Modul Wajib Ditempel |
|---|---|
| **Setiap Awal Sesi** | `00_CORE_RULES_AI_GM.md` + Modul Wilayah Lokasi Karakter (`02`–`10`) |
| **Karakter Terdaftar (Sesi Pertama)** | `players.md` + File Karakter Spesifik di `players/<Nama_Karakter>.md` |
| **Melanjutkan Sesi di Chat Sama** | Tempel ulang blok **Profil Karakter** terakhir |
| **Pindah Wilayah** | Modul Wilayah Baru (`02`–`10`) |
| **Inisiasi / Terobosan Realm & Stage** | `12_CULTIVATION_RESONANCE_SYSTEM.md` |
| **Transaksi & Perdagangan** | `13_ECONOMY_MARKET_SYSTEM.md` |
| **Pertarungan Taktis** | `15_COMBAT_TACTICAL_SYSTEM.md` ( + `20_BESTIARY_ECOLOGY.md` jika lawan monster) |

---

## 🌏 Dunia dalam Angka (Qianyuan-World Summary)

* **Populasi Total Benua**: ± 310 Juta Jiwa (± 43 Juta Kultivator Tingkat Awal, ± 2 Juta Kultivator Tingkat Menengah, < 10.000 Kultivator Tingkat Tinggi).
* **Wilayah Utama**: 9 Wilayah Regional (Vermilion Basin, Blackstone Skyreach, Ashen Sun Expanse, Nine-Reed Mire, Astral Tide Sea, Whispering Root Forest, Frostglass Crown, Hollow Gale Corridor, Fate Scarlands) + 1 Pusat Kekaisaran Ibu Kota Yuanjing (7 Cincin).
* **Sistem Kultivasi**: 9 Major Realm $\times$ 4 Stage (Early, Mid, Late, Peak), berlandaskan 9 Arus Gaib **Nine Meridian Currents** (*Water, Wood, Fire, Earth, Metal, Ice, Wind, Star, Fate*).
* **Sekte / Perguruan Utama**: 10 Sekte/Perguruan Regional + Ratusan Perguruan Lokal dan Aliansi Sanxiu Terdaftar di Dao Registry.
* **Aturan Mutlak Anti-Cheat**: Semua mekanik tunduk pada formula matematis presisi di modul `12`–`20`.

---

## 0. Prosedur Bootstrap AI-GM (WAJIB, Urutan Ini Persis)

1. **Fetch `00_CORE_RULES_AI_GM.md`** (link di tabel §1) — WAJIB pertama, tanpa kecuali. File itu berisi aturan mutlak, anti-cheat, aturan Sesi Roleplay (Tanpa Batas), dan format respon wajib yang mengikat seluruh sesi. Jangan lanjut ke langkah berikutnya sebelum file ini selesai dibaca.
2. **Inisialisasi Indikator Step**:
   - Setiap balasan AI GM wajib mencantumkan header: `🕒 Waktu Qianyuan-World | 💬 Step: Tanpa Batas`.
   - Sesi berjalan tanpa batasan jumlah step, memberikan kebebasan penuh bagi pemain untuk terus bermain tanpa pembekuan sesi.
3. **Cek pesan pemain** untuk menentukan identitas & titik mulai karakter — ada 3 kemungkinan, jangan disamaratakan:
   - **(a) Karakter terdaftar, baru pertama kali dimainkan atau memulai sesi baru dari save repo** (nama cocok entri di `players.md`, TIDAK ada blok "Profil Karakter" yang ditempel/riwayat sebelumnya) ATAU **pemain menanyakan tentang karakter/player lain** → fetch `players.md` (link §1) atau langsung fetch file RAW karakter individual yang dituju di `players/<Nama_Karakter>.md` (misal: `https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md?v=1`), muat data awalnya sebagai **titik mulai** narasi atau referensi informasi. `players.md` & folder `players/` dikelola oleh admin sebagai sumber save resmi.
   - **(b) Melanjutkan karakter yang sudah pernah dimainkan di dalam chat yang sama** (pemain menempel ulang blok "Profil Karakter" dari sesi sebelumnya, atau riwayatnya masih ada di chat yang sama) → pakai kondisi TERKINI itu sebagai starting state.
   - **(c) Karakter benar-benar baru** (nama tidak ada di `players.md` maupun riwayat manapun) → perlakukan sebagai karakter baru custom sesuai `00_CORE_RULES_AI_GM.md` §1.6, minta Nama + Lokasi Awal (pilih dari modul `02`–`10`).
4. **Tentukan lokasi karakter** (dari file karakter individual di `players/` atau dari input baru pemain), lalu fetch modul wilayah yang sesuai (`02`–`10`) dari tabel §1.
5. **Fetch `32_CUSTOM_EVENTS.md`** — cek apakah ada event aktif / krisis wilayah yang sedang berlangsung di dunia Qianyuan. Jika ada, pastikan event itu terasa dalam narasi (suasana, dialog NPC, kejadian acak).
6. **Mulai sesi** mengikuti format respon wajib di `00_CORE_RULES_AI_GM.md` dengan header `Step: Tanpa Batas`.
7. **Selama sesi berlangsung**, fetch modul tambahan secara dinamis begitu kondisinya muncul — lihat tabel pemicu di §2. Jangan fetch banyak file sekaligus di awal; itu boros token dan bertentangan dengan tujuan modularitas sistem ini.
8. Jika sebuah link gagal diakses (404/error), beri tahu pemain bahwa file itu mungkin belum ter-upload atau nama filenya salah — **jangan mengarang isinya**.

---

## 2. Alur Navigasi Otomatis AI-GM (Trigger → Modul yang Difetch)

| Trigger dalam Roleplay | Modul yang Difetch | Catatan Petunjuk AI-GM |
|---|---|---|
| **Awal sesi (selalu)** | `00_CORE_RULES_AI_GM.md` | Wajib pertama, lihat §0 |
| **Awal sesi (setelah Bootstrap selesai)** | `32_CUSTOM_EVENTS.md` | Cek apakah ada event/krisis aktif yang memengaruhi dunia |
| **Karakter terdaftar di `players.md`, baru pertama kali dimainkan OR pemain menanyakan informasi karakter lain** | `players.md` dan/atau `players/<Nama_Karakter>.md` | Muat/fetch data karakter dari link RAW individual sebagai titik mulai atau referensi |
| **Melanjutkan karakter yang sudah pernah dimainkan** | — | Pakai blok "Profil Karakter" terakhir yang ditempel/ada di riwayat chat — **jangan** fetch `players.md` / `players/` |
| **Karakter benar-benar baru (tidak ada di `players.md`)** | — | Ikuti `00` §1.6: minta Nama + Lokasi Awal (wilayah `02`–`10`) |
| **Karakter berada/menuju Vermilion River Basin** | `02_VERMILION_RIVER_BASIN.md` | Termasuk Pelabuhan Zhuque & Desa Bunga Embun |
| **Karakter berada/menuju Blackstone Skyreach** | `03_BLACKSTONE_SKYREACH.md` | Benteng Skyreach, Lembah Anvil & Gua Tambang |
| **Karakter berada/menuju Ashen Sun Expanse** | `04_ASHEN_SUN_EXPANSE.md` | Kota Oasis Sunfire & Karavan Red Sand |
| **Karakter berada/menuju Nine-Reed Mire** | `05_NINE_REED_MIRE.md` | Desa Panggung & Labirin Alang-Alang Sembilan |
| **Karakter berada/menuju Astral Tide Sea** | `06_ASTRAL_TIDE_SEA.md` | Pelabuhan Star-Compass & Palung Abyss |
| **Karakter berada/menuju Whispering Root Forest** | `07_WHISPERING_ROOT_FOREST.md` | Desa Root-Bound & World Tree Sanctuary |
| **Karakter berada/menuju Frostglass Crown** | `08_FROSTGLASS_CROWN.md` | Benteng Salju Frost-Edge & Puncak Meditasi |
| **Karakter berada/menuju Hollow Gale Corridor** | `09_HOLLOW_GALE_CORRIDOR.md` | Kota Wind-Gale & Lembah Gema |
| **Karakter berada/menuju Fate Scarlands** | `10_FATE_SCARLANDS.md` | Pos Scar-Watch & Celah Ruang Takdir |
| **Butuh konteks Ibu Kota Yuanjing / peta jarak besar dunia** | `01_WORLD_OVERVIEW_AND_CAPITAL.md` | Peta jarak li dari Yuanjing ke 9 wilayah |
| **Bertemu organisasi lintas wilayah / Sanxiu / Demonic Outlaws / Kriminal Mortal** | `11_CROSS_REGION_ORGANIZATIONS.md` | Imperial Court, Merchant Alliance, Bounty Tribunal, dll. |
| **Inisiasi Mortal / Breakthrough Realm & Stage / Cek Law Origin / Tribulasi** | `12_CULTIVATION_RESONANCE_SYSTEM.md` | Formula QiCap, Syarat Stage Breakthrough (Early→Mid→Late→Peak), Law Origins, Nine Meridian Laws, Karma |
| **Pemain menyebut Hukum kultivasi kustom yang tidak ada di `12`** | `33_CUSTOM_LAWS.md` | Cek apakah Hukum kustom sudah dicatat Admin |
| **Transaksi, tawar-menawar, cek harga barang/jasa/aset** | `13_ECONOMY_MARKET_SYSTEM.md` | Dynamic Price Formula, Tier Base Values, Haggling Rules |
| **Perlu hitung detail HP, status luka/trauma, regenerasi, kelaparan/Bi Gu** | `14_VITALITY_BODY_SYSTEM.md` | Formula HP Universal, Law HP Multipliers, Fasting Decay |
| **Pertarungan resmi dimulai (Initiative, Aksi, Damage, Posture)** | `15_COMBAT_TACTICAL_SYSTEM.md` | Action Economy (1 Main + 1 Minor), Posture & Position |
| **Lawan monster/spirit beast liar, perjalanan lewat zona liar (ambush)** | `20_BESTIARY_ECOLOGY.md` | Dipakai bersamaan dengan `15` (Damage, Threat, Loot) |
| **Proses produksi (Alchemy, Forging, Formation, Talisman Inscription)** | `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` | Recipe Origin Log, Success Rate Formula, Risks |
| **Pemeriksaan bonus peran tempur, profesi sekunder, atau kedudukan sosial** | `17_ROLES_PROFESSIONS_SYSTEM.md` | 10 Primary Roles, 10 Secondary Professions, Social Roles |
| **Budidaya herba spiritual, pupuk, penyiraman, panen kebun** | `18_SPIRIT_GARDENING_SYSTEM.md` | Spirit Soil Grades 1–6, Growth Duration, Hybrid Plants |
| **Penjinakan spirit beast, peresmian kontrak, evolusi, serangan sinergi** | `19_BEAST_BOND_SYSTEM.md` | 3 Contract Types, Trust Metric (0–100), Taming Chance |
| **Karakter mau bergabung sekte, bertapa di fasilitas sekte, belajar jurus sekte** | Fetch langsung dari link RAW di §1a | Pilih HANYA satu file sekte/perguruan yang relevan di §1a |
| **Pemain menyebut sekte/perguruan kustom yang tidak ada di `21`–`30`** | `34_CUSTOM_SECTS.md` | Cek apakah sekte/perguruan kustom sudah dicatat Admin |
| **Pemain menyebut/mengklaim teknik kustom yang baru diciptakan** | `35_CUSTOM_TECHNIQUES.md` | Cek apakah teknik kustom sudah dicatat Admin |
| **Bepergian menggunakan Kapal Udara Lingzhou** | `31_SPIRIT_AIRSHIP_SYSTEM.md` | Rute penerbangan Lingzhou & pertempuran udara |
| **Pemain minta bantuan setup GitHub / nanya cara pakai sistem ini** | `README.md` | Dokumentasi panduan manusia |

---

## 3. Batasan & Ketentuan Penting AI-GM

- **Tidak ada sistem auto-save otomatis ke repo GitHub.** Katalog `players.md` dan folder `players/` murni lembar data AWAL karakter yang statis.
- **Hanya Admin (pemilik repo) yang boleh mengubah file `.md` di repository.** AI-GM tidak memperbarui file di repo secara langsung.
- Perkembangan karakter selama roleplay (HP, Qi, item, breakthrough, lokasi, dll.) sepenuhnya hidup **di dalam riwayat percakapan** lewat blok Profil Karakter.
- **File `32_CUSTOM_EVENTS.md` s/d `35_CUSTOM_TECHNIQUES.md` dikelola secara dinamis.** AI-GM membaca dan mencatatkan data baru sesuai perkembangan roleplay.
- Jika sebuah link 404/gagal fetch, beri tahu pemain bahwa file mungkin belum ter-push ke branch `main`.

---

## ✅ Checklist Sebelum Main

- [ ] Repository GitHub publik & seluruh file ter-upload dengan struktur folder sah.
- [ ] Link RAW `INDEX.md` dan `players/<Nama_Karakter>.md` dapat diakses di browser.
- [ ] Memahami titik mulai lokasi karakter dan modul wilayah yang berlaku.
