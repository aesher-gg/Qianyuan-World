# ECONOMY ORACLE

## 1. Overview
Dokumen ini berfungsi sebagai patokan referensi cepat (Oracle/Cheat-sheet) bagi AI-GM untuk menentukan harga standar komoditas, biaya jasa, kelangkaan bahan, serta fluktuasi pasar secara instan di benua Qianyuan.

> **Catatan Penting**: Dokumen ini bersifat referensi pendukung dan wajib tunduk pada kalkulasi rumus dinamis di `13_ECONOMY_MARKET_SYSTEM.md`.

---

## 2. Base Commodity Price Index (Harga Dasar Standard)

### 2.1 Bahan Pangan & Kebutuhan Harian
* **Ransum Makanan Biasa (1 Hari)**: 5 Copper Tael
* **Daging Spiritual Tier 1 (1 Porsi)**: 2 Silver Tael
* **Air Murni Gurun (1 Pelepah/Botol)**: 1 Silver Tael (di Oasis) / 10 Silver Tael (di Tengah Gurun)
* **Penginapan Kedai Biasa (1 Malam)**: 2 Silver Tael
* **Penginapan Kamar Ber-Qi / Meditasi**: 1 Spirit Stone Tier 1

### 2.2 Material & Bijih Mineral
* **Iron Ore (1 Jin/0.5kg)**: 1 Silver Tael
* **Blackstone Ore (1 Jin)**: 5 Silver Tael
* **Cold Steel Ore (1 Jin)**: 2 Spirit Stones Tier 1
* **Star Coral (1 Biji)**: 5 Spirit Stones Tier 1

### 2.3 Standar Harga Herba Spiritual Menurut Tier (Segar & Benih)

| Tier Herba | Harga Herba Segar (Base Market) | Harga Benih Spiritual (*Spirit Seeds*) |
|---|---|---|
| **Tier 1** | 5 – 10 Silver Taels | 1 – 2 Silver Taels |
| **Tier 2** | 1 – 3 Spirit Stones Tier 1 | 5 – 10 Silver Taels |
| **Tier 3** | 8 – 15 Spirit Stones Tier 1 | 2 – 4 Spirit Stones Tier 1 |
| **Tier 4** | 30 – 50 Spirit Stones Tier 1 | 8 – 12 Spirit Stones Tier 1 |
| **Tier 5** | 1 – 2 Spirit Stones Tier 2 (100–200 SS T1) | 25 – 40 Spirit Stones Tier 1 |
| **Tier 6** | 5 – 8 Spirit Stones Tier 2 | 1 – 2 Spirit Stones Tier 2 |
| **Tier 7** | 20 – 35 Spirit Stones Tier 2 | 5 – 8 Spirit Stones Tier 2 |
| **Tier 8** | 1 – 2 Spirit Stones Tier 3 (100–200 SS T2) | 20 – 35 Spirit Stones Tier 2 |
| **Tier 9** | 5 – 10 Spirit Stones Tier 3 | 1 – 2 Spirit Stones Tier 3 |

### 2.4 Cairan Nutrisi Alkimia Kebun (Nutrient Liquids — `18`)
* **Basic Spirit Nutrient Liquid (Grade 1)**: 5 Silver Taels
* **Wood-Vitality Nutrient Essence (Grade 2)**: 1 Spirit Stone Tier 1
* **Elemental Harmony Liquid (Grade 3)**: 5 Spirit Stones Tier 1
* **Life-Surge Nutrient Elixir (Grade 4)**: 20 Spirit Stones Tier 1
* **Grand Dao Spirit Catalytic Dew (Grade 5)**: 1 Spirit Stone Tier 2 (100 SS T1)

### 2.5 Pil Alkimia (Dan-Pill)
* **Qi Replenishing Pill (Basic)**: 2 Spirit Stones Tier 1
* **Healing Wound Pill (Basic)**: 3 Spirit Stones Tier 1
* **Foundation Breakthrough Pill**: 5 Spirit Stones Tier 2
* **Golden Core Creation Pill**: 10 Spirit Stones Tier 3

### 2.5 Senjata, Zirah & Artefak
* **Pedang Besi Biasa (Common Grade)**: 5 Silver Tael
* **Pedang Cold Steel (Superior Grade)**: 15 Spirit Stones Tier 1
* **Zirah Heavy Iron (Blackstone Skyreach)**: 25 Spirit Stones Tier 1
* **Jimat Serang Kertas (Talisman Basic)**: 1 Spirit Stone Tier 1 per 3 Lembar

---

## 3. Biaya Jasa & Transportasi
* **Sewa Perahu Sungai (Vermilion Basin / Hari)**: 1 Silver Tael
* **Kargo Kapal Udara Lingzhou (Per 100 Li)**: 2 Spirit Stones Tier 1
* **Pengiriman Surat Kilat Grand Courier Network**: 5 Silver Tael
* **Jasa Penjinakan Beast (Spirit Beast Union)**: 10 - 50 Spirit Stones Tier 1 (Tergantung Tier Beast)
* **Jasa Pengobatan Tabib (Golden Thread Medicine Hall)**: 3 - 20 Silver Tael (Luka Ringan/Sedang)

---

## 4. GM Oracle Usage
* Gunakan daftar harga ini sebagai titik awal (*Base Value*) sebelum mengalikan dengan modifikator wilayah, kelangkaan, dan musim.
