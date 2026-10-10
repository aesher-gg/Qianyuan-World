# ⚔️ Qianyuan-World — Modul 35: Custom Techniques (Database Jurus & Teknik Ciptaan)

> **Modul:** 35 — Custom Techniques
> **Fungsi:** Database dinamis untuk mencatat teknik bertarung, gerakan footwork, serangan mantra, dan jurus khusus (*Custom Techniques*) yang diciptakan, dikombinasikan, atau ditemukan oleh pemain dalam petualangan di Qianyuan-World.
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` §1.11 (validasi teknik baru), `12_CULTIVATION_RESONANCE_SYSTEM.md` §5 (kreasi teknik), `15_COMBAT_TACTICAL_SYSTEM.md` (klasifikasi combat)

---

## 📜 1. Overview & Format Standard Teknik Khusus

Setiap jurus, mantra, atau teknik gerakan baru yang berhasil dikembangkan oleh pemain melalui pengorbanan latihan, eksperimen Qi, atau panduan kitab kuno wajib dicatat menggunakan format baku berikut:

```markdown
* **Technique ID**: Kode unik (Misal: `TECH-001`)
* **Name**: Nama Resmi Jurus / Teknik
* **Type**: Kategori (Melee Attack / Ranged Spell / Footwork / Defense / Utility / Healing)
* **Element**: Elemen Qi utama (Water, Wood, Fire, Earth, Metal, Ice, Wind, Star, Fate)
* **Origin**: Pencipta / Kitab / Hasil Kombinasi
* **Requirements**: Realm minimal, Mastery statistik, atau kondisi senjata
* **Mastery**: Tingkat kemahiran saat ini (Basic / Proficient / Master / Perfection)
* **Qi Cost**: Konsumsi Qi per pemicuan
* **Stamina Cost**: Konsumsi Stamina per pemicuan
* **Effects**: Deskripsi efek serangan/pertahanan/status mekanis
* **Limitations**: Jarak jangkauan, cooldown, atau syarat penggunaan khusus
* **Risks**: Efek samping fisik/mental jika digunakan berlebihan
* **Known Users**: Tokoh / Pemain yang menguasai teknik ini
```

---

## 🏛️ 2. Registered Custom Techniques (Database Teknik Terdaftar)

### 🗡️ TECH-001: Tebasan Angin Pemotong Embun (Dew-Cutting Wind Slash)
* **Technique ID**: `TECH-001`
* **Name**: Dew-Cutting Wind Slash (Tebasan Angin Pemotong Embun)
* **Type**: Melee / Ranged Hybrid Attack
* **Element**: Wind Qi
* **Origin**: Hasil observasi gerakan angin sungai Vermilion oleh pengembara bebas.
* **Requirements**: Realm Qi Gathering Early Stage, Sword Mastery Proficient.
* **Mastery**: Proficient.
* **Qi Cost**: 15 Qi.
* **Stamina Cost**: 10 Stamina.
* **Effects**: Mengeluarkan tebasan angin tajam tembus pandang sejauh 10 langkah (Damage Physical + Wind 35 HP, efek Armor Piercing 15%).
* **Limitations**: Memerlukan senjata pedang tajam.
* **Risks**: Penggunaan 3 kali beruntun dalam 2 Jam memicu getaran kelelahan pada otot lengan (penalti Stamina Cost +5).
* **Known Users**: Karakter Pemain / Pengembara Bebas.

---

### 🛡️ TECH-002: Perisai Zirah Batu Hitam Purba (Blackstone Armor Shield)
* **Technique ID**: `TECH-002`
* **Name**: Blackstone Armor Shield (Perisai Zirah Batu Hitam)
* **Type**: Defense / Buff
* **Element**: Earth + Metal Qi
* **Origin**: Dikembangkan dari pengamatan struktur tebing Blackstone Skyreach.
* **Requirements**: Realm Foundation Establishment Early Stage, Body Refining Stage Peak.
* **Mastery**: Master.
* **Qi Cost**: 40 Qi.
* **Stamina Cost**: 20 Stamina.
* **Effects**: Membentuk zirah aura batu hitam tebal di permukaan kulit yang menahan 40% Physical Damage dan memberikan kekebalan pada efek terlempar (*Knockback Immune*, 2 Ronde).
* **Limitations**: Kecepatan gerak (*Movement Speed*) terkurangi -15% selama zirah aktif.
* **Risks**: Konsumsi Stamina ganda jika menahan serangan bertipe *Earth Core Impact* berat.
* **Known Users**: Murid Inti Blackstone Vow Sect (`23`).

---

### 🌌 TECH-003: Tombak Sinar Bintang Astral (Astral Ray Spear)
* **Technique ID**: `TECH-003`
* **Name**: Astral Ray Spear (Tombak Sinar Bintang)
* **Type**: Ranged Spell / Attack
* **Element**: Star Qi
* **Origin**: Diciptakan dari penelitian konjungsi rasi bintang di Astral Tide Sea.
* **Requirements**: Realm Core Formation Early Stage, Star Qi Law.
* **Mastery**: Proficient.
* **Qi Cost**: 65 Qi.
* **Stamina Cost**: 15 Stamina.
* **Effects**: Memanggil berkas cahaya bintang dari langit berbentuk tombak raksasa yang menembus perisai Qi musuh sejauh 25 langkah (Damage Star Qi 120 HP, memicu status *Blindness* 1 Ronde pada target).
* **Limitations**: Hanya dapat dipicu di bawah langit terbuka pada malam hari.
* **Risks**: Pemicuan di siang hari meningkatkan biaya Qi sebesar +50%.
* **Known Users**: Navigator Utama Star Compass School (`26`).

---

### 🌿 TECH-004: Tarian Lilitan Akar Kayu Purba (Ancient Wood Vine Bind)
* **Technique ID**: `TECH-004`
* **Name**: Ancient Wood Vine Bind (Tarian Lilitan Akar Kayu Purba)
* **Type**: Utility / Crowd Control
* **Element**: Wood + Life Qi
* **Origin**: Hasil perenungan di bawah World Tree Sanctuary Whispering Root Forest.
* **Requirements**: Realm Qi Gathering Mid Stage, Wood Affinity.
* **Mastery**: Proficient.
* **Qi Cost**: 25 Qi.
* **Stamina Cost**: 10 Stamina.
* **Effects**: Menyemburkan akar-akar kayu ber-Qi dari tanah yang melilit kaki target sejauh 15 langkah (Status *Rooted* selama 2 Ronde, menyerap 10 HP per ronde untuk memulihkan Stamina pengguna).
* **Limitations**: Tidak efektif pada target terbang di atas ketinggian 5 langkah.
* **Risks**: Penggunaan di tanah berbatu keras/tanpa unsur tanah meningkatkan konsumsi Qi +15.
* **Known Users**: Murid Perguruan Rootbound Covenant Sect (`27`).

---

### ❄️ TECH-005: Tebasan Es Jarum Embun Beku (Glacial Needle Blade)
* **Technique ID**: `TECH-005`
* **Name**: Glacial Needle Blade (Tebasan Es Jarum Embun Beku)
* **Type**: Melee / Piercing Attack
* **Element**: Ice Qi
* **Origin**: Diciptakan di Puncak Meditasi Frostglass Crown.
* **Requirements**: Realm Foundation Establishment Mid Stage, Sword Mastery Master.
* **Mastery**: Master.
* **Qi Cost**: 35 Qi.
* **Stamina Cost**: 15 Stamina.
* **Effects**: Memadatkan hawa dingin menjadi ribuan jarum es transparan di sepanjang mata pedang yang menusuk pertahanan musuh (Damage Piercing + Ice 65 HP, mengurangi *Movement Speed* target -25% selama 2 Ronde).
* **Limitations**: Memerlukan fokus pertarungan jarak dekat.
* **Risks**: Kegagalan pemicuan memicu *Frostbite* ringan pada telapak tangan pengguna (-5 HP).
* **Known Users**: Instruktur Frost Edge School (`28`).

---

## 🛠️ 3. GM Instructions & Validasi Kreasi Jurus

1. **Aturan Kreasi Jurus Pemain**: AI GM wajib memvalidasi bahwa teknik baru yang diciptakan pemain membutuhkan pengorbanan latihan yang pantas, biaya Qi/Stamina yang seimbang, serta risiko kegagalan/penyimpangan jika eksperimen dilakukan tanpa guru.
2. **Kenaikan Mastery**: Tingkat mastery (*Basic -> Proficient -> Master -> Perfection*) bertambah secara bertahap seiring frekuensi penggunaan jurus dalam pertempuran resmi.
3. **Pencatatan Permanen**: Setiap jurus baru yang dikonfirmasi oleh AI GM wajib dimasukkan ke dalam daftar di atas agar siap digunakan di sesi roleplay selanjutnya.
