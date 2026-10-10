# 📜 Qianyuan-World — Modul 33: Custom Laws (Database Hukum Kultivasi Khusus)

> **Modul:** 33 — Custom Laws
> **Fungsi:** Database dinamis untuk mencatat hukum kultivasi khusus (*Custom Cultivation Laws*), kitab mantra kuno, dan teknik hukum alam unik yang tidak termasuk dalam sistem umum atau ditemukan selama petualangan di Qianyuan-World.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.10 (prioritas override), `12_CULTIVATION_RESONANCE_SYSTEM.md` §4 (Hukum & QiCap), `35_CUSTOM_TECHNIQUES.md` (jurus turunan)

---

## 📜 1. Overview & Format Standard Hukum Khusus

Setiap Hukum Kultivasi Khusus atau Kitab Mantra Purba baru yang dipelajari atau ditemukan wajib dicatat menggunakan format baku sebagai berikut:

```markdown
* **Law ID**: Kode unik (Misal: `LAW-001`)
* **Name**: Nama Resmi Hukum / Kitab Kultivasi
* **Element**: Elemen Qi utama (Water, Wood, Fire, Earth, Metal, Ice, Wind, Star, Fate)
* **Origin**: Asal-usul penciptaan / lokasi ditemukannya kitab
* **Requirements**: Syarat Realm, kualitas meridian, atau ketahanan batin minimal
* **Stages**: Tingkatan penguasaan hukum (Entry / Proficient / Master / Ancestor)
* **Abilities**: Kemampuan pasif & aktif yang diperoleh di setiap tingkat
* **Risks**: Risiko penyimpangan kultivasi / backlash fisik & mental
* **Restrictions**: Batasan elemen bertentangan / pantangan moral
* **Known Users**: Tokoh / NPC / Pemain yang menguasai hukum ini
* **Hidden Effects**: Efek rahasia saat mencapai pemahaman puncak (*Peak Insight*)
```

---

## 🏛️ 2. Registered Custom Laws (Database Hukum Terdaftar)

### ❄️ LAW-001: Hukum Es Keheningan Abadi (Eternal Stillness Ice Law)
* **Law ID**: `LAW-001`
* **Name**: Eternal Stillness Ice Law (Hukum Es Keheningan Abadi)
* **Element**: Ice + Stillness Qi
* **Origin**: Frostglass Crown (Reruntuhan Menara Pedang Beku — `08`).
* **Requirements**: Realm Foundation Establishment Early Stage, Cold Resistance > 40%, Spirit Qi Capacity ≥ 1,250.
* **Stages**: 3 Stage (Entry: *Frost Body* -> Master: *Glacial Mind* -> Ancestor: *Absolute Zero Domain*).
* **Abilities**: Kebal penuh terhadap provokasi emosi/mentalis, bonus damage teknik pedang es +30%, membekukan aliran Qi musuh sebesar -15% saat kontak fisik.
* **Risks**: Emosi fisik menumpul secara perlahan; risiko hipotermia batin jika terburu-buru melakukan breakthrough.
* **Restrictions**: Dilarang mengombinasikan dengan teknik pemurni *Fire Qi* berintensitas tinggi (memicu benturan Dantian).
* **Known Users**: Master Perguruan Han Bing-Fei (`28`), Pendekar Leng-Yue.
* **Hidden Effects**: Mampu membekukan aliran waktu lokal di dalam radius 3 langkah selama 1 detik pada pemahaman puncak (*Peak Insight*).

---

### 🌿 LAW-002: Hukum Perjanjian Akar Kayu Purba (Ancient Rootbound Life Law)
* **Law ID**: `LAW-002`
* **Name**: Ancient Rootbound Life Law (Hukum Perjanjian Akar Kayu Purba)
* **Element**: Wood + Life Qi
* **Origin**: Whispering Root Forest (Ancient Tree Sanctuary — `07`).
* **Requirements**: Realm Qi Gathering Late Stage, Wood Affinity, Spirit Qi Capacity ≥ 100.
* **Stages**: 3 Stage (Entry: *Sprout Resonance* -> Master: *Bark Resilience* -> Ancestor: *World Tree Sanctum*).
* **Abilities**: Meningkatkan kecepatan pemulihan HP & Stamina alami sebesar +35% di area hutan, memicu refleks penyerapan racun miasma alami, serta meningkatkan keberhasilan taming spirit beast sebesar +20% (`19`).
* **Risks**: Konsumsi Qi meningkat +30% saat berada di area padang pasir/tanah tandus tanpa vegetasi.
* **Restrictions**: Dilarang membantai binatang spiritual yang dalam keadaan menyerah atau mengasuh anak.
* **Known Users**: Master Root-Covenant (`27`), Elder Beast-Master.
* **Hidden Effects**: Mampu memanggil getah vitalitas purba untuk menyembuhkan keretakan Inti Dantian pada pemahaman puncak.

---

### 🧭 LAW-003: Hukum Rasi Bintang Laut Pasang (Astral Tide Compass Law)
* **Law ID**: `LAW-003`
* **Name**: Astral Tide Compass Law (Hukum Rasi Bintang Laut Pasang)
* **Element**: Water + Star Qi
* **Origin**: Astral Tide Sea (Observatorium Bintang — `06`).
* **Requirements**: Realm Foundation Establishment Early Stage, Navigation Mastery Proficient.
* **Stages**: 3 Stage (Entry: *Star Chart Reader* -> Master: *Tidal Flow Master* -> Ancestor: *Nine Stars Projector*).
* **Abilities**: Memberikan kebal terhadap ilusi laut/kabut, meningkatkan jangkauan serangan formasi maritim sebesar +20% di bawah langit malam berbintang, serta navigasi instingtif tanpa tersesat.
* **Risks**: Di dalam ruangan tertutup rapat tanpa pemandangan langit malam, kecepatan regenerasi Qi berkurang -20%.
* **Restrictions**: Memerlukan kompas formasi bintang untuk pemicuan teknik ultimate.
* **Known Users**: Master Star-Navigator (`26`), Captain Hai-Yue.
* **Hidden Effects**: Mampu memanggil proyeksi jarum cahaya bintang sembilan yang menyegel aliran Qi Dantian musuh pada pemahaman puncak.

---

### 🔥 LAW-004: Hukum Nyala Api Pasir Ashen (Ashen Fire Sun Law)
* **Law ID**: `LAW-004`
* **Name**: Ashen Fire Sun Law (Hukum Nyala Api Pasir Ashen)
* **Element**: Fire + Sun Qi
* **Origin**: Ashen Sun Expanse (Kuil Matahari Tenggelam — `04`).
* **Requirements**: Realm Foundation Establishment Early Stage, Fire Affinity, Heat Resistance > 50%.
* **Stages**: 3 Stage (Entry: *Sunfire Ember* -> Master: *Solar Flare Core* -> Ancestor: *Ashen Sun Domain*).
* **Abilities**: Mengubah aura Qi menjadi gelombang panas yang membakar perisai Qi lawan (Damage Fire +25%), serta kebal terhadap efek dehidrasi gurun.
* **Risks**: Pengeluaran Stamina melonjak +20% dalam pertempuran panjang di lingkungan bersuhu dingin.
* **Restrictions**: Pantang dikombinasikan dengan teknik berbasis *Water Qi* murni.
* **Known Users**: Tetua Red Sand Caravan (`24`), Pengawal Istana Sunfire.
* **Hidden Effects**: Mampu menciptakan percikan *Sunfire Explosion* yang melelehkan senjata besi biasa saat memangkas tebasan lawan.

---

### 🌪️ LAW-005: Hukum Gema Angin Topan Ngarai (Hollow Gale Resonance Law)
* **Law ID**: `LAW-005`
* **Name**: Hollow Gale Resonance Law (Hukum Gema Angin Topan Ngarai)
* **Element**: Wind + Sound Qi
* **Origin**: Hollow Gale Corridor (Lembah Bisik — `09`).
* **Requirements**: Realm Qi Gathering Late Stage, Movement Speed Modifier ≥ +10%.
* **Stages**: 3 Stage (Entry: *Wind Echo* -> Master: *Sonic Tempest* -> Ancestor: *Void Voice Domain*).
* **Abilities**: Meningkatkan kecepatan bergerak (*Movement Speed*) sebesar +30%, memancarkan gelombang sonik pemecah konsentrasi mantra musuh, serta melacak suara dalam radius 1 li.
* **Risks**: Rentan mengalami getaran gendang telinga jika diserang gelombang gema yang dipantulkan.
* **Restrictions**: Efektivitas berlipat di ngarai/gua, namun menurun -15% di padang terbuka tanpa gema.
* **Known Users**: Utusan Hollow Wind Sect (`29`), Kurir Wind-Gale.
* **Hidden Effects**: Mampu memancarkan tebasan bisikan gema kedap suara yang menembus pertahanan aura fisik target.

---

## 🛠️ 3. GM Instructions & Override Rule

1. **Aturan Override**: Jika ada kitab hukum khusus yang tercatat di modul ini dan berbenturan dengan aturan umum modul `12`, maka **data di modul kustom ini yang berlaku (override)** khusus untuk praktisi hukum tersebut.
2. **Pencatatan Baru**: AI GM wajib memasukkan kitab hukum atau ajaran kuno baru yang dipelajari pemain ke dalam daftar di atas agar konsistensi status dan efek pasif tetap terjaga di sesi berikutnya.
