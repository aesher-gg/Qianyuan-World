# 🎭 Qianyuan-World — Modul 32: Custom Events (Database Event Khusus & Krisis Wilayah)

> **Modul:** 32 — Custom Events
> **Fungsi:** Database dinamis untuk mencatat event khusus, krisis wilayah, festival, dan fenomena alam yang dipicu oleh perkembangan cerita roleplay di Qianyuan-World. Event dapat berjalan secara mandiri meskipun pemain tidak berada di lokasi kejadian.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.10 (prioritas konten kustom), `01`–`10` (lokasi kejadian), `11_CROSS_REGION_ORGANIZATIONS.md` (faksi yang terlibat)

---

## 📜 1. Overview & Format Standard Event

Setiap event baru yang muncul dari dinamika permainan atau aksi pemain wajib dicatat secara sistematis menggunakan struktur baku berikut:

```markdown
* **Event ID**: Kode unik (Misal: `EVT-001`)
* **Title**: Nama Resmi Event
* **Trigger**: Syarat pemicu (Waktu, lokasi, aksi pemain, atau perkembangan politik)
* **Location**: Wilayah & lokasi spesifik
* **Participants**: Faksi / NPC utama yang terlibat
* **Public Objective**: Tujuan umum yang diketahui publik
* **Hidden Objective**: Agenda rahasia di balik event
* **Time Limit**: Batas waktu berlangsungnya event (Jam / Hari / Bulan)
* **Success Condition**: Syarat keberhasilan event
* **Failure Condition**: Syarat kegagalan event
* **World Consequence**: Dampak jangka panjang terhadap tatanan dunia/ekonomi/faksi
```

---

## 🏛️ 2. Registered Custom Events (Database Event Terdaftar)

### 🏆 EVT-001: Ujian Perekrutan Murid Baru Sepuluh Sekte Utama
* **Event ID**: `EVT-001`
* **Title**: Ujian Perekrutan Murid Baru Sepuluh Sekte Utama Qianyuan
* **Trigger**: Setiap awal tahun bulan ke-1 tanggal 1.
* **Location**: Ibu Kota Yuanjing & Markas Utama 10 Sekte Regional.
* **Participants**: Pemuda dari seluruh benua, Penguji Sekte Utama, Pengawal Kekaisaran.
* **Public Objective**: Lolos seleksi fisik, tes ketahanan batin, dan kelayakan bakat meridian.
* **Hidden Objective**: Mengidentifikasi pemuda dengan potensi keturunan darah purba (*Ancient Bloodline*) untuk direkrut ke dalam faksi rahasia.
* **Time Limit**: 7 Hari.
* **Success Condition**: Mengumpulkan Token Seleksi di puncak ujian dan lulus duel kualifikasi.
* **Failure Condition**: Tereliminasi dalam ujian ketahanan atau kalah dalam pertarungan kualifikasi.
* **World Consequence**: Perubahan distribusi murid berbakat antar-sekte dan pergeseran reputasi faksi di Dao Registry.

---

### 🌿 EVT-002: Krisis Miasma Rawa Teratai Kelam
* **Event ID**: `EVT-002`
* **Title**: Miasma Beracun Rawa Teratai Kelam
* **Trigger**: Lonjakan fluktuasi *Water + Poison Qi* di perbatasan Nine-Reed Mire dan Vermilion River Basin.
* **Location**: Rawa Teratai Kelam (`02`) & Nine-Reed Mire (`05`).
* **Participants**: Golden Thread Medicine Hall, Mire Blood Orchid Sect, Warga Desa Bunga Embun.
* **Public Objective**: Membasmi wabah racun rawa dan mendistribusikan penawar miasma kepada warga terinfeksi.
* **Hidden Objective**: *Mire Blood Orchid Sect* memanfaatkan wabah untuk memanen darah kultivator terinfeksi demi ritual pemurnian racun darah.
* **Time Limit**: 14 Hari.
* **Success Condition**: Memusnahkan sumber spora racun di inti rawa dan mengamankan pasokan herba penawar.
* **Failure Condition**: Miasma meluas hingga mencemari pasokan air Pelabuhan Zhuque, memicu kerugian ekonomi masif.
* **World Consequence**: Harga ramuan penawar racun di bursa `13` naik +50%, dan reputasi Golden Thread Medicine Hall meningkat jika berhasil.

---

### ☀️ EVT-003: Badai Pasir Surya Agung & Penyingkapan Reruntuhan Sunken Sun
* **Event ID**: `EVT-003`
* **Title**: Penyingkapan Reruntuhan Istana Sunken Sun Saat Badai Pasir Agung
* **Trigger**: Badai pasir *Sunfire Qi* skala raksasa yang menyapu gurun Ashen Sun Expanse.
* **Location**: Reruntuhan Istana Sunken Sun (`04`).
* **Participants**: Red Sand Caravan, Pertapa Abu Gurun Master Chi, Dune-Scar Outlaws, Pemburu Harta Karun.
* **Public Objective**: Menjelajahi struktur istana kuno pra-bencana yang tersingkap untuk merebut *Sunfire Gem* Tier 6.
* **Hidden Objective**: Mengamankan inskripsi formasi surya purba sebelum jatuh ke tangan kelompok perampok *Dune-Scar Outlaws*.
* **Time Limit**: 3 Hari (sebelum gerbang istana tertimbun pasir kembali).
* **Success Condition**: Merebut *Sunfire Gem* dan membawa keluar inskripsi formasi kuno secara utuh.
* **Failure Condition**: Terjebak di dalam istana saat badai pasir meruntuhkan lorong gua bawah tanah.
* **World Consequence**: Munculnya artefak purba baru di bursa lelang Cincin 4 Yuanjing dan pertempuran berdarah di gurun barat.

---

### ❄️ EVT-004: Retakan Es Abadi Puncak Frostglass
* **Event ID**: `EVT-004`
* **Title**: Anomali Retakan Jiwa Es & Kemunculan Elemental Ice Dragon Fledgling
* **Trigger**: Penurunan suhu ekstrem yang memicu rekahnya Dinding Glacial Wall di Frostglass Crown.
* **Location**: Puncak Meditasi Frostglass Crown (`08`).
* **Participants**: Frost Edge School, Pemburu Naga Es Sanxiu, Utusan Imperial Court.
* **Public Objective**: Membendung serbuan elemental monster es dan mengamankan wilayah perbatasan dari pembekuan total.
* **Hidden Objective**: Memburu atau menjinakkan anak Naga Es (*Elemental Ice Dragon Fledgling* Tier 7) yang menetas dari retakan purba.
* **Time Limit**: 5 Hari.
* **Success Condition**: Menyegel kembali retakan menggunakan Formasi Penyegel Es atau menaklukkan anak naga es.
* **Failure Condition**: Badai salju abadi meluas ke Hollow Gale Corridor, menutup rute penerbangan Lingzhou.
* **World Consequence**: Kelangkaan kristal es spiritual di pasar dan terjadinya konflik antara Frost Edge School dan Imperial Court.

---

### 🌌 EVT-005: Konjungsi Rasi Bintang Pasang Pasifik
* **Event ID**: `EVT-005`
* **Title**: Pasang Bintang Sembilan & Kemunculan Mutiara Bintang Purba
* **Trigger**: Kesejajaran 9 rasi bintang di atas lautan Astral Tide Sea yang terjadi sekali setiap 3 tahun.
* **Location**: Palung Abyss & Perairan Pulau Coral (`06`).
* **Participants**: Star Compass School, Moonlit Abyss Sect, Kapten Bajak Laut Sea-Wolf, Nelayan Mutiara.
* **Public Objective**: Memanen *Astral Pearl Tier 5* yang memancar ke permukaan laut selama fenomena konjungsi.
* **Hidden Objective**: Membuka pilar segel bawah laut kuno yang menyimpan kitab pusaka *Astral Tide Compass Law*.
* **Time Limit**: 24 Jam (1 Hari).
* **Success Condition**: Mendapatkan *Astral Pearl* dan mempertahankan kapal dari serangan monster palung.
* **Failure Condition**: Pilar segel runtuh, membebaskan makhluk palung purba *Kraken Titan* ke perairan terbuka.
* **World Consequence**: Fluktuasi harga Mutiara Bintang di lelang Yuanjing dan pertempuran kapal maritim berskala besar.

---

## 🛠️ 3. GM Instructions & Propagasi Event

1. **Otonomi Event**: AI GM wajib mengabaikan atau mengalirkan perkembangan event secara berkala meskipun pemain tidak berada di lokasi kejadian.
2. **Pencatatan Baru**: Jika aksi pemain memicu krisis atau festival baru di dunia roleplay, AI GM wajib menambahkan data event tersebut ke dalam modul ini menggunakan format standard di atas.
3. **Eskalasi Dunia**: Kegagalan pemain dalam merespon event yang mengancam wilayah akan menghasilkan perubahan permanen pada kondisi peta regional (`01`–`10`) dan fluktuasi ekonomi (`13`).
