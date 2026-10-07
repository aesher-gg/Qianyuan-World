# 🐾 Qianyuan-World — XX. Beast Bond System (Sistem Penjinakan, Kontrak, & Evolusi Spirit Beast)

> **Modul:** 19 — Beast Bond System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Contract-Validated — Bloodline & Trust Driven
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `11_CROSS_REGION_ORGANIZATIONS.md` (Spirit Beast Union), `12_CULTIVATION_RESONANCE_SYSTEM.md` (QiCap & breakthrough beast), `14_VITALITY_BODY_SYSTEM.md` (HP & pemicuan trauma), `15_COMBAT_TACTICAL_SYSTEM.md` (pertempuran sinergi beast), `20_BESTIARY_ECOLOGY.md` (database monster & threat level)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Beast Bond

Beast Bond System di Qianyuan-World mengatur ikatan, penjinakan (*Taming*), peresmian kontrak (*Contract*), serta perkembangan hubungan dan evolusi garis keturunan (*Bloodline Awakening*) antara kultivator dan binatang spiritual (*Spirit Beast*). Berbeda dengan `20_BESTIARY_ECOLOGY.md` yang berfokus pada ekologi monster liar, modul ini mengatur mekanisme interaksi, kontrak, dan pertarungan sinergi pasangan kultivator-beast.

### Aturan Emas Anti-Cheat Beast Bond (Mandatory Enforced Rules)
1. **Syarat Riwayat Kontrak (Contract Origin Log)**: Binatang spiritual binaan (**Tier 3+ / Spirit Beast Langka**) wajib memiliki catatan riwayat kontrak (*Contract Origin Log*) dari proses penjinakan naratif, pendaftaran di Spirit Beast Union (`11`), atau penetasan telur purba.
2. **Larangan Penjinakan Instan**: Pemain **TIDAK BISA** menjinakkan monster liar secara instan di tengah pertempuran tanpa proses penurunan ketahanan batin (*Willpower Depletion*), pemberian pakan spiritual, atau penggunaan segel jimat taming tervalidasi.
3. **Batasan Realm Kultivator vs Beast**: Menjinakkan Spirit Beast dengan Realm/Tier yang lebih tinggi dari kultivator memicu risiko **Soul Backlash** (penalti Max Qi -30% dan status *Dantian Shock Trauma*).
4. **Indikator Kepercayaan Berkelanjutan (Trust Metric)**: Kepatuhan beast binaan dalam pertempuran terikat pada skala *Trust Metric* ($0 \text{ s/d } 100$). Kebencian atau siksaan fisik menurunkan Trust dan memicu pemberontakan.
5. **Evolusi Terikat Bahan & Waktu**: Evolusi garis keturunan (*Bloodline Awakening*) memerlukan konsumsi Inti Monster (*Spirit Core*), herba spiritual (`18`), dan latihan di daerah *Qi Density Modifier* yang sesuai.

---

## 📜 1. Tiga Jenis Kontrak Jiwa (Contract Types & Requirements)

Kultivator dapat mengikat binatang spiritual melalui salah satu dari 3 jenis kontrak resmi:

| Jenis Kontrak | Syarat Minimum Realm | Kelebihan Mekanis | Kekurangan & Risiko Utama |
|---|---|---|---|
| **Master-Servant Contract (Kontrak Tuan-Pelayan)** | Body Refining Early (`12`) | Kepatuhan mutlak pada perintah tempur dasar, tidak dapat menolak serangan. | Membatasi perkembangan kecerdasan beast, potensi pemberontakan jika Trust < 30. |
| **Equal Companion Contract (Kontrak Mitra Sejajar)** | Qi Gathering Early (`12`) | Beast bertarung dengan kecerdasan alami penuh, bonus peluang evolusi +25%, persepsi pikiran (*Telepathy*). | Beast dapat menolak perintah yang bertentangan dengan keadilan/temperamen dasarnya. |
| **Symbiotic Life Bond (Kontrak Simbiosis Jiwa)** | Foundation Est. Mid (`12`) | Penyatuan energi Qi & HP (dapat saling menyalurkan HP/Qi), bonus status tempur +20%. | **Sangat Berbahaya!** Kematian salah satu pihak memicu kerusakan Dantian parah atau kematian pihak lainnya. |

---

## ❤️ 2. Indikator Kepercayaan & Loyalitas (Trust Metric 0–100)

Tingkat hubungan batin antara kultivator dan binatang spiritual binaan dicatat dalam skala **Trust Metric ($0 \text{ s/d } 100$)**:

### 📊 Tabel Tingkatan Trust & Efek Perilaku Tempur

| Skala Trust | Status Hubungan | Efek Perilaku & Performa Tempur (`15`) |
|---|---|---|
| **0 s/d 29** | **Hostile / Memberontak** | Penalti Accuracy -30%, berisiko kabur atau menyerang pemiliknya saat pertempuran sengit. |
| **30 s/d 69** | **Obedient / Patuh** | Mematuhi perintah tempur standar, melakukan pergerakan taktis biasa. |
| **70 s/d 89** | **Loyal / Setia** | Bonus Damage Sinergi +15%, siap menahan serangan demi melindungi pemiliknya. |
| **90 s/d 100** | **Soulbound / Sejiwa** | Bonus Damage Sinergi +30%, kebal terhadap intimidasi mental, siap mengorbankan nyawa. |

---

## 🎲 3. Formula Peluang Penjinakan (Taming Success Rate)

Proses penjinakan binatang spiritual liar memerlukan pelemparan peluang sukses oleh AI GM:

```
TamingChance = clamp(TamingSkill + BeastTrustMod + BaitBonus − BeastWillpower − RealmDiffPenalty, 10%, 90%)
```

- `TamingSkill`: Nilai kemahiran profesi Pawang / Beast Tamer (10 s/d 100).
- `BeastTrustMod`: Bonus dari pemberian pakan spiritual / obat penyembuh luka (+10% s/d +30%).
- `BaitBonus`: Bonus penggunaan pakan kesukaan beast (+15%).
- `BeastWillpower`: Ketahanan batin beast (20 s/d 80, berkurang saat HP beast di bawah 30%).
- `RealmDiffPenalty`: Penalti jika Realm Beast > Realm Kultivator (20% × Selisih Realm).

### ⚠️ Risiko Kegagalan Penjinakan (Taming Backlash)
Jika lemparan penjinakan **GAGAL** dengan selisih ≥ 20%, binatang spiritual akan mengalami *Rage Frenzy* (bonus Damage +30%) dan menyerang kultivator secara ganas.

---

## 🐉 4. Perkembangan & Evolusi Garis Keturunan (Bloodline Awakening)

Binatang spiritual binaan dapat ditingkatkan kekuatannya dan memicu evolusi bentuk fisik (*Evolution*) melalui 3 metode:

1. **Konsumsi Inti Monster & Herba Spiritual (`16` & `18`)**:
   - Memberikan pakan *Spirit Core* dan herba obat elemen selaras meningkatkan akumulasi Qi Cap beast.
2. **Bertapa di Daerah Qi Density Tinggi (`02`–`10`)**:
   - Melatih beast di lingkungan ber-Qi padat (misal: Emerald Panther di *Whispering Root Forest* $\times 1.5$ Wood Qi) mempercepat pemurnian aura.
3. **Pemurnian Garis Keturunan Purba (Bloodline Awakening Ritual)**:
   - Menggunakan ramuan alkimia *Bloodline Awakening Pill* (Tier 4+) untuk membangkitkan wujud binatang purba kuno (misal: Emerald Panther → **Ancient Jade Tiger**).

---

## 🔗 5. Teknik Sinergi & Komunikasi Pikiran (Shared Arts & Telepathy)

Kultivator dan Spirit Beast binaan dengan *Equal Companion* atau *Symbiotic Bond* dapat menggunakan teknik sinergi:

- **Persepsi Pikiran (Telepathic Link)**: Saling berkomunikasi suara batin dan berbagi penglihatan/penciuman dalam jarak 500 li.
- **Penglihatan Malam Bersama (Shared Vision)**: Kultivator meminjam kemampuan penglihatan malam atau pendengaran gema beast.
- **Serangan Sinergi Elemen (Elemental Fusion Strike)**: Mengombinasikan serangan Qi kultivator dan elemen alami beast untuk meningkatkan *TechniqueTierBonus* menjadi $\times 2.0$ (`15`).

---

## 🐺 6. Katalog 10 Spirit Beast Binaan Khas Qianyuan-World

*(Selaras dengan Database Bestiarium Modul `20_BESTIARY_ECOLOGY.md`)*

| # | Nama Spirit Beast | Tier / Threat | Habitat Utama | Elemen Qi | Teknik Sinergi Tempur Utama (`15`) |
|---|---|---|---|---|---|
| 1 | **Emerald Panther** | Tier 2 / Medium | Whispering Root Forest (`07`) | Wood Qi | *Cakar Sergap Serat Kayu* — serangan stealth berkecepatan tinggi. |
| 2 | **Gale Falcon** | Tier 2 / Medium | Hollow Gale Corridor (`09`) | Wind Qi | *Tebasan Sayap Angin Topan* — serangan udara pemotong zirah. |
| 3 | **Ice-Crystal Wolf** | Tier 3 / Dangerous | Frostglass Crown (`08`) | Ice Qi | *Hembusan Nafas Es Abadi* — membekukan pergerakan musuh (*Immobilized*). |
| 4 | **Miasma Python** | Tier 3 / Dangerous | Nine-Reed Mire (`05`) | Poison Qi | *Lilitan Racun Pembusuk Dantian* — racun penyerap Qi bertahap. |
| 5 | **Ironclad Bear** | Tier 4 / High | Blackstone Skyreach (`03`) | Earth + Metal | *Perisai Zirah Batu Hitam* — benteng aura penahan serangan fisik. |
| 6 | **Sandstorm Scorpion**| Tier 3 / Dangerous | Ashen Sun Expanse (`04`) | Fire + Sun | *Sengatan Racun Api Gurun* — membakar HP & Dantian lawan. |
| 7 | **Wood-Deer** | Tier 1 / Low | Whispering Root Forest (`07`) | Life Qi | *Aroma Embun Penyembuh* — memulihkan HP & Stamina secara alami. |
| 8 | **Sea Serpent** | Tier 4 / High | Astral Tide Sea (`06`) | Water + Star | *Gelombang Pasang Bintang* — pemicuan pusaran air penenggelam. |
| 9 | **Echo Bat** | Tier 2 / Medium | Hollow Gale Corridor (`09`) | Sound Qi | *Raungan Gelombang Suara* — merusak Qi & pendengaran musuh. |
| 10| **Chrono-Beast** | Tier 7 / Extreme | Fate Scarlands (`10`) | Fate Qi | *Hentakan Waktu Stasis* — menghentikan giliran musuh selama 1 turn. |

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Dicek Setiap Interaksi Beast)

- [ ] Spirit Beast Tier 3+ memiliki riwayat kontrak yang sah (*Contract Origin Log*)?
- [ ] Jenis kontrak (*Master-Servant, Equal Companion, Symbiotic*) ditaati syarat Realm-nya?
- [ ] Kepatuhan beast dalam pertarungan dihitung jujur berdasarkan skala *Trust Metric* (0 s/d 100)?
- [ ] Penjinakan beast liar dilakukan melalui pelemparan formula `TamingChance` resmi?
- [ ] Kematian atau pembatalan paksa *Symbiotic Bond* menerapkan penalti *Soul Backlash* secara jujur?

Jika **salah satu** poin di atas meragukan → Status Ikhtisar Beast **DIKOREKSI OTOMATIS** oleh AI GM.
