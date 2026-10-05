# 13 — ECONOMY MARKET SYSTEM

## 1. Overview
Economy Market System mengatur sistem ekonomi dinamis, perdagangan komoditas spiritual, Fluktuasi harga, serta nilai mata uang di seluruh wilayah Qianyuan. Sistem ini memastikan tidak ada angka harga universal yang tidak didefinisikan canon.

---

## 2. Currency (Mata Uang Resmi)
Sistem mata uang terstandarisasi berdasarkan konversi resmi Kekaisaran Yuanjing:

* **1 Tael Emas (Gold Tael)** = 10 Tael Perak (Silver Tael)
* **1 Tael Perak (Silver Tael)** = 100 Tael Perunggu / Koin Tembaga (Copper Tael)
* **1 Spirit Stone (Tier 1 / Low Grade)** = 10 Tael Perak
* **1 Spirit Stone (Tier 2 / Mid Grade)** = 100 Spirit Stone Tier 1 (1,000 Tael Perak)
* **1 Spirit Stone (Tier 3 / High Grade)** = 100 Spirit Stone Tier 2 (100,000 Tael Perak)

---

## 3. Dynamic Price Formula
Setiap komoditas barang/jasa dihitung menggunakan rumus dinamis sebagai berikut:

$$\text{Final Price} = \text{Base Value} \times \text{Scarcity} \times \text{Regional Demand} \times \text{Quality Grade} \times \text{Season} \times \text{Market Conditions}$$

### Penjelasan Variabel:
* **Base Value**: Harga dasar standar barang di bursa Yuanjing.
* **Scarcity (Kelangkaan)**:
  * Melimpah: 0.7x - 0.9x
  * Normal: 1.0x
  * Langka: 1.5x - 2.5x
  * Sangat Langka / Terlarang: 3.0x - 5.0x
* **Regional Demand (Permintaan Wilayah)**:
  * Barang lokal diproduksi di wilayah sendiri: 0.8x
  * Barang impor dari wilayah jauh: 1.3x - 2.0x
* **Quality Grade**:
  * Low Grade / Defective: 0.5x - 0.8x
  * Normal / Standard Grade: 1.0x
  * High Grade / Superior: 1.5x - 2.0x
  * Flawless / Masterpiece: 3.0x+
* **Season (Musim / Arus Current)**:
  * Puncak panen/produksi: 0.8x
  * Musim paceklik/badai: 1.4x
* **Market Conditions (Reputasi / Gangguan)**:
  * Diskon Reputasi Pedagang: -10% s/d -25%
  * Perang / Blokade Rute: +50% s/d +100%

---

## 4. Regional Economic Differences
* **Vermilion River Basin**: Murah untuk herba & bahan pangan; Mahal untuk mineral logam keras.
* **Blackstone Skyreach**: Murah untuk bijih besi, zirah, & senjata tempa; Mahal untuk tanaman medis segar.
* **Ashen Sun Expanse**: Murah untuk rempah api & kristal api; Sangat Mahal untuk air murni & tanaman penyembuh.
* **Frostglass Crown**: Murah untuk kristal es & snow lotus; Sangat Mahal untuk bahan makanan segar & kayu.
* **Hollow Gale Corridor**: Murah untuk batu rekaman Echo Stone & jasa pengiriman; Sedang untuk barang umum.

---

## 5. GM Instructions
* Wajib menerapkan rumus kalkulasi harga saat terjadi transaksi jual beli antara pemain dan pedagang NPC.
* Rujuk `ECONOMY_ORACLE.md` untuk gambaran harga instan komoditas umum.
