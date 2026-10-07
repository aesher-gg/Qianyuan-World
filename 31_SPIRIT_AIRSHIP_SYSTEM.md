# ☁️ Qianyuan-World — XXXII. Spirit Airship System (Sistem Kapal Udara Lingzhou & Armada Langit)

> **Modul:** 31 — Spirit Airship System
> **Genre:** Xianxia · Wuxia · Kultivasi · Hardcore Realism
> **Prinsip:** Anti-Cheat Enforced — Distance & Fuel Bound — Aerial Combat Enabled
> **Rujukan silang:** `00_CORE_RULES_AI_GM.md` (aturan mutlak), `01_WORLD_OVERVIEW_AND_CAPITAL.md` (peta jarak li dari Yuanjing), `11_CROSS_REGION_ORGANIZATIONS.md` (Merchant Alliance & Imperial Court), `13_ECONOMY_MARKET_SYSTEM.md` (harga sewa, bahan bakar, & aset), `15_COMBAT_TACTICAL_SYSTEM.md` (pertarungan udara & boarding)

---

## 🧭 0. Filosofi & Aturan Emas Anti-Cheat Lingzhou

Spirit Airship System (*Lingzhou / Kapal Udara Spiritual*) mengatur navigasi udara, transportasi logistik lintas benua, manajemen bahan bakar Spirit Stone (`13`), dan pertempuran armada langit (*Airship Combat*) di Qianyuan-World. Penerbangan Lingzhou bukan sekadar narasi "beberapa hari kemudian tiba", melainkan gameplay aktif yang terikat pada jarak peta (*Distance in Li*), konsumsi energi, ancaman monster langit, dan cuaca arus Qi.

### Aturan Emas Anti-Cheat Lingzhou (Mandatory Enforced Rules)
1. **Syarat Izin Terbang & Kepemilikan (Flight Permit Log)**: Penerbangan Lingzhou kelas menengah/besar wajib memiliki Surat Izin Terbang (*Imperial/Sect Flight Permit*) dari Imperial Court atau faksi penguasa wilayah (`11`).
2. **Larangan Penerbangan Instan**: Durasi penerbangan dihitung secara presisi berdasarkan jarak li peta (`01`) divided by kecepatan kelas Lingzhou. Pemain **TIDAK BISA** melakukan perjalanan instan tanpa alokasi waktu Jam dan bahan bakar.
3. **Manajemen Bahan Bakar Mutlak**: Setiap jam penerbangan mengonsumsi Spirit Stone (Tier 1 / Tier 2 / Tier 3) sesuai spesifikasi kelas kapal. Jika bahan bakar habis di udara, kapal akan jatuh (*Core Engine Shutdown & Crash Risk*).
4. **Batas Kapasitas Kargo & Penumpang**: Setiap kelas Lingzhou memiliki batas beban fisik dan penumpang. Overload memotong kecepatan sebesar `-30%` dan menaikkan konsumsi bahan bakar `+50%`.
5. **Akses Udara Terlarang (Restricted Airspace)**: Terbang langsung di atas Istana Imperial Sanctum Yuanjing atau zona inti *Fate Scarlands* tanpa izin khusus akan memicu serangan formasi pertahanan otomatis (*Automated Defense Array*).

---

## 🛥️ 1. Klasifikasi Kelas Kapal Udara (Vessel Classes & Specs)

Setiap kapal udara (*Lingzhou*) di benua Qianyuan dikategorikan ke dalam 4 kelas utama:

### 📊 Tabel Spesifikasi Teknis Kelas Lingzhou

| Kelas Kapal Udara | Kecepatan Terbang | Kapasitas Crew/Kargo | Durabilitas Hull (HP) | Perisai Qi Shield | Konsumsi Bahan Bakar |
|---|---|---|---|---|---|
| **Spirit Skiff (Perahu Udara Ringan)** | 75 li / Jam | 2–5 Orang / 500 kg | 500 HP | 300 Qi Shield | 0,5 Spirit Stone Tier 1 / Jam |
| **Cloud Cruiser (Kapal Jelajah)** | 50 li / Jam | 10–30 Orang / 5 Ton | 2.500 HP | 1.500 Qi Shield | 2,5 Spirit Stone Tier 1 / Jam |
| **Sect Airship (Kapal Perang Sekte)** | 40 li / Jam | 50–200 Murid / 25 Ton | 12.500 HP | 8.000 Qi Shield | 0,5 Spirit Stone Tier 2 / Jam |
| **Grand Spirit Ark (Bahtera Kekaisaran)** | 25 li / Jam | 500+ Orang / 100 Ton | 62.500 HP | 40.000 Qi Shield | 2,5 Spirit Stone Tier 2 / Jam |

---

## ⚙️ 2. Komponen Kritis Kapal Udara Lingzhou

Setiap Lingzhou disokong oleh 5 komponen utama yang dapat mengalami kerusakan fisik saat pertempuran:

1. **Lambung Kapal (Spirit Hull)**: Pelindung fisik utama yang terbuat dari kayu purba (*Mirewood/Ancient Wood*) atau pelat logam *Cold Steel*.
2. **Inti Energi (Spirit Core Engine)**: Kuali pendorong utama penampung Spirit Stone yang mengubah energi kristal menjadi aura daya dorong.
3. **Formasi Pendorong (Propulsion Formation Array)**: Array ukiran garis Qi pada baling-bahtera yang mengendalikan arah dan kecepatan.
4. **Formasi Navigasi Bintang (Navigation Array)**: Kompas spiritual penyeimbang posisi dan pemeta rasi bintang malam.
5. **Perisai Udara Pelindung (Defensive Qi Shield)**: Dome aura Qi yang menahan gesekan badai angin dan tembakan meriam musuh.

---

## ⏱️ 3. Formula Navigasi Udara & Konsumsi Bahan Bakar

Durasi penerbangan dan total biaya bahan bakar dihitung presisi sebelum Lingzhou lepas landas:

```
FlightDuration (Jam) = TotalDistance_li / AirshipSpeed_li_per_Jam
FuelCost = FlightDuration_Jam × ClassFuelRate × WeatherModifier
```

- `WeatherModifier`: Cuaca Cerah = `1.0` | Badai Angin Topan = `1.5` | Terbang Menembus Badai Gletser = `2.0`.

*Contoh Perhitungan Penerbangan:*
Perjalanan dari Yuanjing ke Pelabuhan Star-Compass Astral Tide Sea (1.500 li) menggunakan **Cloud Cruiser** (50 li / Jam):
- `FlightDuration` = 1.500 / 50 = **30 Jam**
- `FuelCost` = 30 Jam × 2,5 SS-T1 = **75 Spirit Stones Tier 1**

---

## ⚔️ 4. Mekanik Pertempuran Udara (Airship Combat & Boarding)

Pertempuran antar-kapal udara atau pertempuran melampaui monster langit mengikuti alur taktis berikut (`15`):

### 4.1 Tembakan Meriam Qi & Perisai Shield Overload
- **Meriam Meriam Qi (Qi Cannons)**: Menembakkan gumpalan energi berdaya hancur tinggi.
- **Mekanik Shield Overload**: Serangan meriam terlebih dahulu mengurangi *Perisai Qi Shield*. Jika Qi Shield mencapai 0, serangan selanjutnya langsung merusak *Hull HP*.

### 4.2 Sergap Seberang (Boarding Action)
- Ketika dua kapal berjarak dekat (*Close Range*), petarung dapat melompat menyeberang ke geladak musuh untuk melakukan pertempuran taktis jarak dekat (`15`).

### 4.3 Risiko Ledakan Spirit Core (Engine Explosion)
- Jika *Spirit Core Engine* menerima kerusakan tembus fisik di atas 50% HP-nya, akan terjadi **Ledakan Inti (*Engine Explosion*)** yang merusak 50% Hull HP kapal seketika dan melukai seluruh penumpang.

---

## 🦅 5. Bahaya Langit & Peluang Encounter (Sky Hazards)

Pemeriksaan *Sky Encounter* dilakukan oleh AI GM pada setiap 4 Jam penerbangan:

```
SkyEncounterChance = clamp(BaseChance × AirwayDangerMod × WeatherMod, 5%, 75%)
```

| Jenis Bahaya / Encounter Langit | Efek Mekanis & Dampak Pertempuran |
|---|---|
| **Serangan Spirit Beast Langit** | Serangan kawanan *Gale Falcon* (`09`), *Glacier Eagle* (`08`), atau *Astral Whale* (`06`). |
| **Pembajak Angin (Thorn Wing Sky Pirates)** | Penyadapan perahu udara oleh kelompok pembajak langit (`09` & `11`). |
| **Badai Angin Pemotong (*Void Gale Storm*)** | Memicu kerusakan Qi Shield -10% per Jam dan risiko disorientasi navigasi. |
| **Distorsi Ruang Anomali (Scar Rift)** | Terbang di perbatasan *Fate Scarlands* memicu teleportasi lokasi acak. |

---

## 🗺️ 6. Peta Rute Penerbangan Resmi Benua Qianyuan-World

*(Selaras dengan Peta Jarak Peta `01_WORLD_OVERVIEW_AND_CAPITAL.md`)*

1. **Rute Utama Yuanjing Hub**: Menghubungkan Cincin 7 Ibu Kota ke 9 pelabuhan udara utama regional.
2. **Rute Perairan Vermilion-Astral**: Rute kargo dagang dari Pelabuhan Zhuque (`02`) menuju Pelabuhan Star-Compass (`06`).
3. **Rute Ngarai Udara Hollow Gale**: Rute penerbangan kilat express melewati lorong angin Ngarai (`09`).
4. **Rute Terisolasi Frostglass-Scarlands**: Rute bernavigasi khusus dengan pengawalan militer Kekaisaran.

---

## 🛡️ 7. Checklist Validasi AI GM (Wajib Dicek Setiap Penerbangan)

- [ ] Izin terbang (*Flight Permit Log*) tervalidasi untuk kapal udara kelas menengah/besar?
- [ ] Durasi penerbangan dihitung jujur berdasarkan jarak li peta divided by kecepatan kapal?
- [ ] Persediaan bahan bakar Spirit Stone di inventory mencukupi untuk total Jam penerbangan?
- [ ] Pemeriksaan *Sky Encounter Chance* dilempar berkala setiap 4 Jam penerbangan?
- [ ] Kerusakan perisai Qi Shield dan Hull HP dicatat jujur saat terjadi pertempuran udara?

Jika **salah satu** poin di atas meragukan → Penerbangan Lingzhou **DITOLAK OTOMATIS** oleh AI GM.
