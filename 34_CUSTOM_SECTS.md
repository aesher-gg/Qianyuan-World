# 🏯 Qianyuan-World — Modul 34: Custom Sects (Database Sekte & Dojo Baru)

> **Modul:** 34 — Custom Sects
> **Fungsi:** Database dinamis untuk mencatat sekte baru, dojo lokal, perkumpulan sanxiu, dan faksi baru yang didirikan oleh pemain atau didaftarkan di Dao Registry selama perkembangan cerita di Qianyuan-World.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.10 (legalitas Dao Registry), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (Cincin 3 Dao Registry), `11_CROSS_REGION_ORGANIZATIONS.md` (faksi benua)

---

## 📜 1. Overview & Format Standard Faksi Khusus

Setiap faksi, sekte, atau dojo baru yang didirikan oleh pemain atau dibentuk oleh kelompok NPC wajib dicatat secara resmi menggunakan struktur baku berikut:

```markdown
* **Faction ID**: Kode unik (Misal: `FCT-001`)
* **Name**: Nama Resmi Sekte / Dojo / Aliansi
* **Type**: Jenis faksi (Dojo Lokal / Sekte Orthodoks / Aliansi Sanxiu / Guild Dagang)
* **Region**: Wilayah domisili & lokasi markas utama
* **Origin**: Sejarah singkat pendirian faksi
* **Leadership**: Pemimpin / Pendiri resmi
* **Doctrine**: Ajaran utama / Prinsip filosofis
* **Techniques**: Kurikulum teknik khas yang diajarkan
* **Resources**: Aset lahan, bangunan, kebun spiritual, & sumber dana
* **Relations**: Sikap hubungan dengan faksi di sekitarnya
* **Political Position**: Status legalitas di Dao Registry (Terdaftar / Bebas / Ilegal)
* **Secrets**: Rahasia faksi / agenda internal tersembunyi
```

---

## 🏛️ 2. Registered Custom Sects (Sampel Terdaftar)

### 🎍 FCT-001: Dojo Bambu Hijau (Green Bamboo Dojo)
* **Faction ID**: `FCT-001`
* **Name**: Green Bamboo Dojo (Dojo Bambu Hijau)
* **Type**: Dojo Bela Diri Lokal
* **Region**: Vermilion River Basin (Tepi Dewflower Village — `02`).
* **Origin**: Didirikan oleh bekas prajurit veteran kekaisaran untuk melatih pemuda desa bertarung membela diri dari serangan pembajak sungai.
* **Leadership**: Guru Lin (Veteran Body Refining Realm Late Stage).
* **Doctrine**: *"Lentur Bagaikan Bambu, Teguh Menghadapi Badai."*
* **Techniques**: *Bamboo Pole Staff Art*, *Wind-Breeze Footwork*.
* **Resources**: Bangunan dojo kayu bambu, lapangan latihan, kebun obat herbal kecil.
* **Relations**: Bersahabat erat dengan warga Desa Bunga Embun dan River Lantern School (`22`).
* **Political Position**: Terdaftar resmi di *Dao Registry* Cabang Vermilion.
* **Secrets**: Menyimpan teknik staf bambu rahasia warisan jenderal kekaisaran yang mampu memutus pedang besi biasa.

---

### ⚒️ FCT-002: Perhimpunan Penambang Palu Besi (Iron Hammer Miners Guild)
* **Faction ID**: `FCT-002`
* **Name**: Iron Hammer Miners Guild
* **Type**: Serikat Kerja & Guild Penambang Independen
* **Region**: Blackstone Skyreach (Anvil Valley — `03`).
* **Origin**: Dibentuk oleh gabungan buruh tambang independen untuk melindungi hak galian mineral dari intimidasi perampok ngarai.
* **Leadership**: Master Miner Tie-Shan (Core Formation Early Stage).
* **Doctrine**: *"Keringat Mengalir di Batu, Kehormatan Ditempa di Api."*
* **Techniques**: *Heavy Hammer Strike*, *Rock-Solid Stance*.
* **Resources**: Bengkel tempa perkakas, hak galian Zona Iron Vein, pos persinggahan gua.
* **Relations**: Bermitra dengan Central Miners Union (`03`) dan Blackstone Vow Sect (`23`).
* **Political Position**: Terdaftar di *Dao Registry* Cincin 4 Yuanjing.
* **Secrets**: Menguasai peta celah rahasia di Zona Tengah tambang yang kaya akan urat *Deep Steel Ore*.

---

### 🏮 FCT-003: Kedai Informasi Teratai Malam (Night Lotus Information Lodge)
* **Faction ID**: `FCT-003`
* **Name**: Night Lotus Information Lodge
* **Type**: Jaringan Intelijen & Kedai Informasi
* **Region**: Astral Tide Sea (Pelabuhan Star-Compass — `06`).
* **Origin**: Didirikan oleh alumni murid luar Moonlit Abyss Sect sebagai pos penyamaran perdagangan berita rahasia maritim.
* **Leadership**: Nona Night-Lotus (Core Formation Early Stage).
* **Doctrine**: *"Cahaya Menyilaukan Mata, Bayangan Menyembunyikan Kebenaran."*
* **Techniques**: *Shadow Step*, *Silencing Voice Barrier*.
* **Resources**: Gedung kedai teh 3 lantai, jaringan burung pengintai malam, koleksi cermin perekam ingatan.
* **Relations**: Bersekutu secara rahasia dengan Moonlit Abyss Sect (`21`) dan bersaing netral dengan Feather Wind Guild (`11`).
* **Political Position**: Bebas / Penyamaran Bisnis Resmi.
* **Secrets**: Menyimpan dokumen daftar nama penyelundup artefak laut gelap yang melibatkan pejabat pelabuhan.

---

## 🛠️ 3. GM Instructions & Pendaftaran Faksi Baru

1. **Syarat Pendaftaran Pemain**: Pemain yang telah memiliki Realm minimal *Foundation Establishment Early Stage* dan dana modal 500 Tael Emas berhak mengajukan pendirian dojo/sekte baru ke *Dao Registry* (Cincin 3 Yuanjing).
2. **Pencatatan Baru**: AI GM wajib mencatatkan faksi baru yang berhasil didirikan ke dalam modul ini agar status politik, wilayah kekuasaan, dan hubungan diplomasi sekte terakumulasi secara permanen.
