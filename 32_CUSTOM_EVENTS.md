# 32 — CUSTOM EVENTS

## 1. Overview
Database dinamis untuk mencatat event khusus, krisis wilayah, festival, dan fenomena alam yang dipicu oleh perkembangan cerita roleplay di Qianyuan-World. Event dapat berjalan secara mandiri meskipun pemain tidak berada di lokasi kejadian.

---

## 2. Event Format Standard
Setiap event disatukan menggunakan struktur baku berikut:

* **Event ID**: Kode unik (Misal: `EVT-001`)
* **Title**: Nama Event
* **Trigger**: Syarat pemicu (Waktu, lokasi, aksi pemain, atau perkembangan politik)
* **Location**: Wilayah & lokasi spesifik
* **Participants**: Faksi/NPC yang terlibat
* **Public Objective**: Tujuan umum yang diketahui publik
* **Hidden Objective**: Agenda rahasia di balik event
* **Time Limit**: Batas waktu berlangsungnya event
* **Success Condition**: Syarat keberhasilan
* **Failure Condition**: Syarat kegagalan
* **World Consequence**: Dampak jangka panjang terhadap tatanan dunia/ekonomi/faksi

---

## 3. Registered Custom Events Sample

### EVT-001: Perekrutan Murid Baru Sekte Utama
* **Event ID**: `EVT-001`
* **Title**: Ujian Perekrutan Murid Baru Sepuluh Sekte Utama
* **Trigger**: Setiap awal tahun bulan ke-1.
* **Location**: Yuanjing & Ibu Kota Wilayah Utama.
* **Participants**: Pemuda dari seluruh benua, Penguji Sekte Utama.
* **Public Objective**: Lolos seleksi fisik, bakat meridian, dan ketahanan batin.
* **Hidden Objective**: Mengidentifikasi bakat berbakat dengan keturunan darah purba (*Ancient Bloodline*).
* **Time Limit**: 7 Hari.
* **Success Condition**: Mengumpulkan Token Seleksi di puncak ujian.
* **Failure Condition**: Tereliminasi atau gagal dalam pertarungan seleksi.
* **World Consequence**: Perubahan peta kekuatan murid muda antar-sekte.

---

## 4. GM Instructions
* Masukkan event baru hasil kreasi selama roleplay ke dalam modul ini agar menjadi rekaman histori dunia yang konsisten.
