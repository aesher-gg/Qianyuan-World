# 📇 Qianyuan-World — Players (Katalog Data Karakter Awal)

> **Modul:** players — dirujuk lewat `INDEX.md` §3, HANYA dipakai saat karakter yang namanya terdaftar di sini dimainkan untuk **pertama kali**.
> **⚠️ SIFAT FILE & DIREKTORI: READ-ONLY MUTLAK BAGI AI.** Ini murni katalog & referensi **data awal** karakter — bukan sistem save, bukan checkpoint, bukan status terkini. AI tidak pernah menulis, mengedit, atau menyarankan perubahan pada file ini maupun file individual di folder `players/`. Hanya **admin (aesher-gg)** yang berhak mengubah isinya, langsung di GitHub, di luar sesi roleplay.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.6 & §1.9, `12_CULTIVATION_RESONANCE_SYSTEM.md` (Law Origin & QiCap), `13_ECONOMY_MARKET_SYSTEM.md` (Item Origin & mata uang)

---

## 0. Aturan Pemakaian (WAJIB DIPAHAMI AI GM)

1. File ini dan file individual di folder `players/` **hanya** berisi kondisi karakter **sebelum cerita dimulai**. Bukan status "terakhir dimainkan", bukan save slot, bukan progres yang sedang berjalan.
2. AI membaca file karakter **satu kali saja** — persis di momen karakter yang namanya ada di sini mulai dimainkan untuk **pertama kalinya**. Sejak saat itu, seluruh perkembangan karakter (HP berubah, Qi terpakai, item baru, breakthrough, pindah lokasi, dst.) **hanya** dicatat di dalam blok "Profil Karakter" pada percakapan yang sedang berjalan (format resmi ada di `00_CORE_RULES_AI_GM.md` §2) — **tidak pernah** ditulis balik ke file mana pun.
3. **Instruksi Fetch untuk AI GM:** Untuk mencegah batasan ekstraktor teks AI (misalnya limit 300 baris), data detail setiap karakter telah dipisahkan ke file individual di dalam folder `players/`. AI GM **WAJIB** mengambil/fetch file RAW karakter spesifik yang dimaksud (`players/<Nama_Karakter>.md`) melalui Link RAW pada tabel §1 di bawah saat:
   - Karakter tersebut dimainkan untuk **pertama kalinya**.
   - Pemain/Player bertanya atau menanyakan informasi/status/latar belakang mengenai karakter/player lain yang terdaftar di `players.md`.
4. AI **dilarang keras**: menulis ke file mana pun, menyarankan pemain "menyimpan"/"update" progres ke file ini, atau memperlakukan isi file karakter sebagai kondisi yang **terkini** setelah roleplay berjalan.
5. Untuk **melanjutkan** karakter yang sudah pernah dimainkan sebelumnya (bukan memulai baru), pemain menempelkan ulang blok "Profil Karakter" **terakhir** dari sesi sebelumnya di pesan pembuka. Folder `players/` **tidak dipakai** untuk kasus itu — isinya tetap/statis.

---

## 1. Daftar Katalog Karakter Terdaftar

> Klik atau fetch link RAW individual untuk memuat data awal lengkap karakter secara utuh tanpa terpotong limit ekstraktor teks AI.

| Nama Karakter | Lokasi Awal | Realm Awal | Sekte/Afiliasi Awal | File Detail & Link RAW |
|---|---|---|---|---|
| **Lin Feng** *(contoh)* | Kota Vermilion Port, Vermilion River Basin | Foundation Establishment, Early | River Lantern School (Murid Luar) | [`Lin_Feng.md`](https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Lin_Feng.md) |
| **Ye Chen** | Benteng Skyreach, Blackstone Skyreach | Body Refining, Early | Blackstone Vow Sect (Murid Magang) | [`Ye_Chen.md`](https://raw.githubusercontent.com/aesher-gg/Qianyuan-World/main/players/Ye_Chen.md) |

*(Admin menambah baris baru di sini dan membuat file di `players/` setiap kali mendaftarkan karakter baru.)*

---

## 2. Template Kosong (Untuk Admin — Salin untuk Mendaftarkan Karakter Baru di `players/[Nama_Karakter].md`)

```markdown
# 👤 [Nama Karakter]

> **Data Karakter Awal** — Statis, dikelola Admin. Bukan save-state.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.6 & §1.9, `01`–`10` (Regional Modules)

---

**Nama Karakter:** [Nama Karakter]
**Lokasi Awal:** [nama lokasi, sesuai modul 01–10]
**Realm & Stage Awal:** [Realm, Stage] — Qi Cap: [angka] *(kalkulasi: RealmBase × StageMultiplier per `12`)*
**Hukum Kultivasi Awal:** [nama Hukum, atau "Belum ada — akan ditentukan lewat roleplay"]
**Law Origin (jika sudah ada Hukum):** Jalur [Guru/Manual/Pencerahan] — [detail singkat]
**Sekte/Afiliasi Awal:** [nama sekte + peran, atau "Sanxiu"]

**Kondisi Awal:** HP X/Y · Qi X/Y · Stamina X/100 · Satiety X% · Kondisi Normal · Karma Netral

**Currency Awal:**
- Copper Taels × [jumlah]
- Silver Taels × [jumlah]
- Gold Taels × [jumlah]
- Spirit Stones Tier 1 × [jumlah]

**Equipment Awal (terpakai/digenggam):**
- Senjata: [nama item — Tier/Grade, asal singkat, atau "Tidak ada"]
- Zirah/Pelindung: [nama item, atau "Tidak ada"]
- Aksesoris: [nama item, atau "Tidak ada"]

**Inventory Awal (dibawa, tidak terpakai):**
- [Item 1 — Tier/Grade, asal singkat]
- [Item 2]

**Teknik Awal:**
- [teknik — sumber]

**Latar Belakang & Kepribadian:**
[1–2 paragraf: siapa dia, sifatnya, motivasinya, relasi penting dengan NPC kanon jika ada]
# 📇 Qianyuan-World — Players Database Index & Template Save Standar

> **Modul:** Players Index (`players.md`)
> **Fungsi:** Katalog direktori pemain aktif dan format baku template save karakter awal di dalam direktori `players/`.
> **Sifat Wajib:** READ-ONLY bagi AI GM selama roleplay berlangsung. AI GM memanggil file spesifik di `players/` HANYA saat karakter baru dimuat pertama kali (Jalur A di `00_CORE_RULES_AI_GM.md`).
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.6 (3 jalur input pemain), `12_CULTIVATION_RESONANCE_SYSTEM.md` (kalkulasi QiCap), `13_ECONOMY_MARKET_SYSTEM.md` (mata uang & item), `17_ROLES_PROFESSIONS_SYSTEM.md` (role & profesi)


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
