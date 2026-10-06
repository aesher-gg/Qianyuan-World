# 🧭 Qianyuan-World — INDEX (Master Navigation Hub AI-GM)

> **Ini adalah SATU-SATUNYA link yang perlu ditempel pemain di setiap sesi.**
> Semua modul lain (aturan, wilayah, sistem, sekte, data karakter) dijangkau AI-GM secara otomatis dari sini lewat `read_file` / web fetch, sesuai kondisi yang sedang terjadi di roleplay.
>
> **Untuk AI Game Master (AI-GM):** baca seluruh file ini dulu sampai habis, lalu jalankan **Prosedur Bootstrap** di §0 SEBELUM menulis balasan apa pun ke pemain. Jangan menjawab dari ingatan/memori bebas — dunia ini hanya sah kalau datanya berasal dari modul-modul resmi yang ditautkan di sini.

---

## 0. Prosedur Bootstrap AI-GM (WAJIB, Urutan Ini Persis)

1. **Fetch `00_CORE_RULES_AI_GM.md`** (link di tabel §1) — WAJIB pertama, tanpa kecuali. File itu berisi aturan mutlak, anti-cheat, aturan Sesi Roleplay (Tanpa Batas), dan format respon wajib yang mengikat seluruh sesi. Jangan lanjut ke langkah berikutnya sebelum file ini selesai dibaca.
2. **Inisialisasi Indikator Step**:
   - Setiap balasan AI GM wajib mencantumkan header: `🕒 Waktu Qianyuan-World | 💬 Step: Tanpa Batas`.
   - Sesi berjalan tanpa batasan jumlah step, memberikan kebebasan penuh bagi pemain untuk terus bermain tanpa pembekuan sesi.
3. **Cek pesan pemain** untuk menentukan identitas & titik mulai karakter — ada 3 kemungkinan, jangan disamaratakan:
   - **(a) Karakter terdaftar, baru pertama kali dimainkan atau memulai sesi baru dari save repo** (nama cocok entri di `players.md`, TIDAK ada blok "Profil Karakter" yang ditempel/riwayat sebelumnya) ATAU **pemain menanyakan tentang karakter/player lain** → fetch `players.md` (link §1) atau langsung fetch file RAW karakter individual yang dituju di `players/<Nama_Karakter>.md` (misal: `https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Inggo.md`), muat data awalnya sebagai **titik mulai** narasi atau referensi informasi. `players.md` & folder `players/` dikelola oleh admin sebagai sumber save resmi.
   - **(b) Melanjutkan karakter yang sudah pernah dimainkan di dalam chat yang sama** (pemain menempel ulang blok "Profil Karakter" dari sesi sebelumnya, atau riwayatnya masih ada di chat yang sama) → pakai kondisi TERKINI itu sebagai starting state.
   - **(c) Karakter benar-benar baru** (nama tidak ada di `players.md` maupun riwayat manapun) → perlakukan sebagai karakter baru custom sesuai `00_CORE_RULES_AI_GM.md` §1.6, minta Nama + Lokasi Awal (pilih dari modul `02`–`10`).
4. **Tentukan lokasi karakter** (dari file karakter individual di `players/` atau dari input baru pemain), lalu fetch modul wilayah yang sesuai (`02`–`10`) dari tabel §1.
5. **Fetch `32_CUSTOM_EVENTS.md`** — cek apakah ada event aktif / krisis wilayah yang sedang berlangsung di dunia Qianyuan. Jika ada, pastikan event itu terasa dalam narasi (suasana, dialog NPC, kejadian acak).
6. **Mulai sesi** mengikuti format respon wajib di `00_CORE_RULES_AI_GM.md` dengan header `Step: Tanpa Batas`.
7. **Selama sesi berlangsung**, fetch modul tambahan secara dinamis begitu kondisinya muncul — lihat tabel pemicu di §2. Jangan fetch banyak file sekaligus di awal; itu boros token dan bertentangan dengan tujuan modularitas sistem ini.
8. Jika sebuah link gagal diakses (404/error), beri tahu pemain bahwa file itu mungkin belum ter-upload atau nama filenya salah — **jangan mengarang isinya**.

---

## 1. Direktori Lengkap Seluruh Modul Utama

| Kode | File Name | Link RAW (Klik / Fetch) | Isi Singkat & Fungsi |
|---|---|---|---|
| **00** | `00_CORE_RULES_AI_GM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/00_CORE_RULES_AI_GM.md | Aturan mutlak, anti-cheat, format respon wajib, cheat-sheet formula — **selalu difetch pertama** |
| 👤 | `players.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players.md | Katalog **data AWAL** karakter (statis, dikelola admin) — memuat link RAW ke file individual di `players/` |
| **01** | `01_WORLD_OVERVIEW_AND_CAPITAL.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/01_WORLD_OVERVIEW_AND_CAPITAL.md | Peta jarak benua Qianyuan, Nine Meridian Currents, Ibu Kota Yuanjing & 7 Cincin |
| **02** | `02_VERMILION_RIVER_BASIN.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/02_VERMILION_RIVER_BASIN.md | Vermilion River Basin: Pelabuhan Zhuque, Desa Bunga Embun, kota & NPC perairan |
| **03** | `03_BLACKSTONE_SKYREACH.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/03_BLACKSTONE_SKYREACH.md | Blackstone Skyreach: Benteng Skyreach, Lembah Anvil, Gua Tambang Besi Kuno |
| **04** | `04_ASHEN_SUN_EXPANSE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/04_ASHEN_SUN_EXPANSE.md | Ashen Sun Expanse: Kota Oasis Sunfire, Benteng Sandgate, Istana Sunken Sun |
| **05** | `05_NINE_REED_MIRE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/05_NINE_REED_MIRE.md | Nine-Reed Mire: Desa Panggung Mirewood, Pasar Kabut Kelam, Labirin Alang-Alang |
| **06** | `06_ASTRAL_TIDE_SEA.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/06_ASTRAL_TIDE_SEA.md | Astral Tide Sea: Pelabuhan Star-Compass, Benteng Pulau Coral, Palung Abyss |
| **07** | `07_WHISPERING_ROOT_FOREST.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/07_WHISPERING_ROOT_FOREST.md | Whispering Root Forest: Desa Root-Bound, Pondok Pemburu, World Tree Sanctuary |
| **08** | `08_FROSTGLASS_CROWN.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/08_FROSTGLASS_CROWN.md | Frostglass Crown: Benteng Salju Frost-Edge, Desa Gletser Bening, Puncak Meditasi |
| **09** | `09_HOLLOW_GALE_CORRIDOR.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/09_HOLLOW_GALE_CORRIDOR.md | Hollow Gale Corridor: Kota Wind-Gale, Pos Tebing Bisik, Lembah Gema |
| **10** | `10_FATE_SCARLANDS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/10_FATE_SCARLANDS.md | Fate Scarlands: Pos Perbatasan Scar-Watch, Kemah Penjelajah, Kota Terbalik |
| **11** | `11_CROSS_REGION_ORGANIZATIONS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/11_CROSS_REGION_ORGANIZATIONS.md | Imperial Court, Merchant Alliance, Beast Union, Courier, Dao Registry, Bounty Tribunal, Sanxiu, Demonic Outlaws |
| **12** | `12_CULTIVATION_RESONANCE_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/12_CULTIVATION_RESONANCE_SYSTEM.md | Inisiasi Mortal, 9 Major Realm, Formula QiCap, Law Origins, Nine Meridian Laws, Tribulasi, Karma |
| **13** | `13_ECONOMY_MARKET_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/13_ECONOMY_MARKET_SYSTEM.md | Mata uang resmi, Tier Base Values, Dynamic Price Formula, Harga Jasa/Aset, Haggling Rules |
| **14** | `14_VITALITY_BODY_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/14_VITALITY_BODY_SYSTEM.md | Formula HP Universal, Law HP Multiplier, Wound/Trauma, Satiety Decay, Fasting Multipliers (Bi Gu), Rest |
| **15** | `15_COMBAT_TACTICAL_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/15_COMBAT_TACTICAL_SYSTEM.md | Initiative, Action Economy (1 Main + 1 Minor), Hit Chance, Damage Resolution, Posture/Position States, Cooldowns |
| **16** | `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md | Alchemy, Forging, Formation Array, Talisman Inscription, Quality Grades, Success Rates & Risks |
| **17** | `17_ROLES_PROFESSIONS_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/17_ROLES_PROFESSIONS_SYSTEM.md | 10 Primary Combat Roles, 10 Secondary Professions (5 Tiers), Social Roles & Access Rights |
| **18** | `18_SPIRIT_GARDENING_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/18_SPIRIT_GARDENING_SYSTEM.md | Spirit Soil Grades 1–6, Growth Duration Formula, Spirit Water & Bee Pollination, Hybrid Crossbreeding, Plant Catalog |
| **19** | `19_BEAST_BOND_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/19_BEAST_BOND_SYSTEM.md | 3 Contract Types, Trust Metric (0–100), Taming Success Rate, Bloodline Awakening Evolution, Shared Telepathy |
| **20** | `20_BESTIARY_ECOLOGY.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/20_BESTIARY_ECOLOGY.md | MonsterHP & Attack formulas, Ambush Chance, Loot Drop Rates, Threat Levels, Common & Regional Monster Catalogs |
| **21–30** | *(10 file sekte/perguruan individual)* | — | Lihat **§1a** di bawah untuk daftar lengkap per-file — **JANGAN** fetch semuanya sekaligus, cari nama sekte yang relevan lalu fetch HANYA file itu |
| **31** | `31_SPIRIT_AIRSHIP_SYSTEM.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/31_SPIRIT_AIRSHIP_SYSTEM.md | Sistem Kapal Udara Lingzhou, rute penerbangan, dan pertempuran udara |
| **32** | `32_CUSTOM_EVENTS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/32_CUSTOM_EVENTS.md | **Event khusus & peristiwa dunia** — diisi Admin, AI wajib cek di awal sesi |
| **33** | `33_CUSTOM_LAWS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/33_CUSTOM_LAWS.md | **Hukum Kultivasi kustom** — buatan pemain/Admin, dicatat di sini agar resmi |
| **34** | `34_CUSTOM_SECTS.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/34_CUSTOM_SECTS.md | **Sekte/Dojo/Organisasi kustom** — buatan pemain/Admin, dicatat di sini agar resmi |
| **35** | `35_CUSTOM_TECHNIQUES.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/35_CUSTOM_TECHNIQUES.md | **Teknik & Jurus Kustom** — buatan pemain/Admin, dicatat di sini agar resmi |
| **Oracle** | `ECONOMY_ORACLE.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/ECONOMY_ORACLE.md | Cheat-sheet Referensi Harga Cepat GM |
| — | `README.md` | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/README.md | Dokumentasi setup untuk manusia (jarang perlu difetch AI) |

---

### 1a. Direktori Sekte & Perguruan Utama (10 File Individual)

> Setiap sekte/perguruan utama Qianyuan-World memiliki **file sendiri**, lengkap dengan hierarki, fasilitas, artefak/pusaka, kurikulum teknik bertingkat, Hukum kultivasi detail, relasi antar-faksi, dan rahasia internal. **Fetch HANYA** link file yang relevan dengan situasi saat ini — jangan fetch banyak sekaligus.

| Sekte / Perguruan Utama | Wilayah Dominan | Link RAW (Langsung Klik / Fetch AI) |
|---|---|---|
| **Moonlit Abyss Sect** | Astral Tide Sea (`06`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/21_MOONLIT_ABYSS_SECT.md |
| **River Lantern School** | Vermilion River Basin (`02`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/22_RIVER_LANTERN_SCHOOL.md |
| **Blackstone Vow Sect** | Blackstone Skyreach (`03`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/23_BLACKSTONE_VOW_SECT.md |
| **Red Sand Caravan** | Ashen Sun Expanse (`04`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/24_RED_SAND_CARAVAN.md |
| **Mire Blood Orchid Sect** | Nine-Reed Mire (`05`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/25_MIRE_BLOOD_ORCHID_SECT.md |
| **Star Compass School** | Astral Tide Sea (`06`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/26_STAR_COMPASS_SCHOOL.md |
| **Rootbound Covenant Sect** | Whispering Root Forest (`07`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/27_ROOTBOUND_COVENANT_SECT.md |
| **Frost Edge School** | Frostglass Crown (`08`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/28_FROST_EDGE_SCHOOL.md |
| **Hollow Wind Sect** | Hollow Gale Corridor (`09`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/29_HOLLOW_WIND_SECT.md |
| **Golden Thread Medicine Hall** | Ibu Kota Yuanjing (`01`) | https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/30_GOLDEN_THREAD_MEDICINE_HALL.md |

---

## 2. Alur Navigasi Otomatis AI-GM (Trigger → Modul yang Difetch)

| Trigger dalam Roleplay | Modul yang Difetch | Catatan Petunjuk AI-GM |
|---|---|---|
| **Awal sesi (selalu)** | `00_CORE_RULES_AI_GM.md` | Wajib pertama, lihat §0 |
| **Awal sesi (setelah Bootstrap selesai)** | `32_CUSTOM_EVENTS.md` | Cek apakah ada event/krisis aktif yang memengaruhi dunia |
| **Karakter terdaftar di `players.md`, baru pertama kali dimainkan OR pemain menanyakan informasi karakter lain** | `players.md` dan/atau `players/<Nama_Karakter>.md` | Muat/fetch data karakter dari link RAW individual sebagai titik mulai atau referensi |
| **Melanjutkan karakter yang sudah pernah dimainkan** | — | Pakai blok "Profil Karakter" terakhir yang ditempel/ada di riwayat chat — **jangan** fetch `players.md` / `players/` |
| **Karakter benar-benar baru (tidak ada di `players.md`)** | — | Ikuti `00` §1.6: minta Nama + Lokasi Awal (wilayah `02`–`10`) |
| **Karakter berada/menuju Vermilion River Basin** | `02_VERMILION_RIVER_BASIN.md` | Termasion Pelabuhan Zhuque & Desa Bunga Embun |
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
| **Inisiasi Mortal / Breakthrough Realm / Cek Law Origin / Tribulasi** | `12_CULTIVATION_RESONANCE_SYSTEM.md` | Formula QiCap, Law Origins, Nine Meridian Laws, Karma |
| **Pemain menyebut Hukum kultivasi kustom yang tidak ada di `12`** | `33_CUSTOM_LAWS.md` | Cek apakah Hukum kustom sudah dicatat Admin |
| **Transaksi, tawar-menawar, cek harga barang/jasa/aset** | `13_ECONOMY_MARKET_SYSTEM.md` | Dynamic Price Formula, Tier Base Values, Haggling Rules |
| **Perlu hitung detail HP, status luka/trauma, regenerasi, kelaparan/Bi Gu** | `14_VITALITY_BODY_SYSTEM.md` | Formula HP Universal, Law HP Multipliers, Fasting Decay |
| **Pertarungan resmi dimulai (Initiative, Aksi, Damage, Posture)** | `15_COMBAT_TACTICAL_SYSTEM.md` | Action Economy (1 Main + 1 Minor), Posture & Position |
| **Lawan monster/spirit beast liar, perjalanan lewat zona liar (ambush)** | `20_BESTIARY_ECOLOGY.md` | Dipakai bersamaan dengan `15` (Damage, Threat, Loot) |
| **Proses produksi (Alchemy, Forging, Formation, Talisman Inscription)** | `16_CRAFTING_ALCHEMY_ARRAY_SYSTEM.md` | Recipe Origin Log, Success Rate Formula, Risks |
| **Pemeriksaan bonus peran tempur, profesi sekunder, atau kedudukan sosial** | `17_ROLES_PROFESSIONS_SYSTEM.md` | 10 Primary Roles, 10 Secondary Professions, Social Roles |
| **Budidaya herba spiritual, pupuk, penyiraman, panen kebun** | `18_SPIRIT_GARDENING_SYSTEM.md` | Spirit Soil Grades 1–6, Growth Duration, Hybrid Plants |
| **Penjinakan spirit beast, peresmian kontrak, evolusi, serangan sinergi** | `19_BEAST_BOND_SYSTEM.md` | 3 Contract Types, Trust Metric (0–100), Taming Chance |
| **Karakter mau bergabung sekte, bertapa di fasilitas sekte, belajar jurus sekte** | Fetch langsung dari link RAW di §1a | Pilih HANYA satu file sekte yang relevan di §1a |
| **Pemain menyebut sekte kustom yang tidak ada di `21`–`30`** | `34_CUSTOM_SECTS.md` | Cek apakah sekte kustom sudah dicatat Admin |
| **Pemain menyebut/mengklaim teknik kustom yang baru diciptakan** | `35_CUSTOM_TECHNIQUES.md` | Cek apakah teknik kustom sudah dicatat Admin |
| **Bepergian menggunakan Kapal Udara Lingzhou** | `31_SPIRIT_AIRSHIP_SYSTEM.md` | Rute penerbangan Lingzhou & pertempuran udara |
| **Pemain minta bantuan setup GitHub / nanya cara pakai sistem ini** | `README.md` | Dokumentasi panduan manusia |

> 📌 **Efisiensi Token AI-GM**: Jika sebuah modul sudah difetch sebelumnya dalam percakapan yang sama dan kondisinya belum berubah (misal: karakter masih berada di wilayah yang sama), **tidak perlu fetch ulang** — gunakan data yang sudah ada di riwayat chat.

---

## 3. Cara Kerja `players.md` & Folder `players/` (Manajemen Save Data)

`players.md` dan file individual di folder `players/` berisi data karakter resmi pemain di core repository Qianyuan-World. File-file ini **hanya boleh diubah dan diperbarui oleh Admin (pemilik repo)** berdasarkan data Profil Karakter tersimpan yang dikirimkan oleh pemain.

**Alur Pemakaian & Sesi Baru:**
1. Pemain menyebutkan nama karakternya (misal: `Inggo`) saat membuka chat/sesi baru.
2. AI-GM memanggil file `players/<Nama_Karakter>.md` dari repository resmi.
3. Seluruh data di file karakter tersebut dimuat sebagai titik mulai sesi baru.
4. Selama sesi berlangsung, perkembangan karakter dilacak di dalam percakapan lewat blok Profil Karakter.
5. Pemain bebas menyalin blok Profil Karakter kapan saja dan mengirimkannya ke Admin untuk disimpan di core repo (`players/<Nama_Karakter>.md`).

---

## 4. Batasan Penting AI-GM

- **Tidak ada sistem auto-save otomatis ke repo GitHub.** Katalog `players.md` dan folder `players/` murni lembar data AWAL karakter yang statis — bukan file yang berubah otomatis saat AI mengetik.
- **Hanya Admin (pemilik repo) yang boleh mengubah file `.md` di repository.** AI-GM tidak bisa dan tidak akan menulis atau memperbarui file di repo secara langsung di akhir sesi.
- Perkembangan karakter selama roleplay (HP, Qi, item, breakthrough, lokasi, dll.) sepenuhnya hidup **di dalam riwayat percakapan** lewat blok Profil Karakter.
- **File `32_CUSTOM_EVENTS.md` s/d `35_CUSTOM_TECHNIQUES.md` dikelola oleh Admin.** AI-GM membaca dan menggunakan data yang sudah ada di dalamnya.
- Jika sebuah link 404/gagal fetch, beri tahu pemain bahwa file mungkin belum ter-push ke branch `main`.

---

## 5. Ringkasan Dunia Qianyuan-World

Xianxia · Wuxia · Kultivasi Hardcore Realism — 9 Wilayah Regional + 1 Zona Anomali Fate Scarlands, Ibu Kota Yuanjing, 9 Major Realm $\times$ 4 Stage, 9 Hukum Kultivasi Nine Meridian Currents, $\pm 310$ Juta Jiwa Populasi, Tanpa Plot Armor, Semua Mekanik Tunduk pada Formula Anti-Cheat Resmi di Modul `12`–`20`.
