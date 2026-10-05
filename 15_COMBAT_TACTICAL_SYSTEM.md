# 15 — COMBAT TACTICAL SYSTEM

## 1. Overview
Combat Tactical System mengatur mekanisme pertarungan taktis di Qianyuan-World. Pertarungan tidak ditentukan hanya oleh statistik/Realm murni, melainkan juga oleh taktik posisi (*Position*), postur bertarung (*Posture*), momentum, kondisi medan (*Terrain*), jarak (*Distance*), serta efisiensi penggunaan Qi dan Stamina.

---

## 2. Distance & Position

### 2.1 Distance (Jarak Tempur)
* **Close Range (Jarak Dekat / Melee)**: Jarak gulat, senjata pendek (pisau/belati), dan serangan telapak tangan.
* **Mid Range (Jarak Sedang)**: Jarak pedang, tombak, cambuk, dan serangan Qi jarak pendek.
* **Far Range (Jarak Jauh)**: Jarak busur panah, senjata lempar, dan serangan jarak jauh elemen Qi.

### 2.2 Position (Kondisi Posisi)
* **Ground Neutral**: Posisi berdiri biasa di tanah datar.
* **Elevated (Posisi Tinggi)**: Berada di atas tebing/pohon/atap. (Bonus Akurasi +15%, Bonus Damage Jarak Jauh +10%).
* **Concealed (Tersamar / Sembunyi)**: Berada di balik semak/kabut/bayangan. (Bonus Ambush / Surprise Attack +30%).
* **Cornered (Tersudut)**: Terjebak di dinding/tebing tanpa ruang gerak. (Penalti Evasive -25%).
* **Flanked / Surrounded (Dikeroyok)**: Diserang dari banyak sisi. (Penalti Defense -20%).

---

## 3. Posture States (Postur Tempur)
Setiap petarung berada pada salah satu status Posture yang menentukan efektivitas aksi:

1. **Neutral Posture**: Postur seimbang. Dapat melakukan ofensif/defensif tanpa bonus/penalti.
2. **Offensive Posture**: Fokus penuh pada serangan. (Bonus Damage +20%, Penalti Evasive/Defense -15%).
3. **Defensive Posture**: Fokus pada menangkis/bertahan dengan zirah atau Qi shield. (Bonus Block/Defense +30%, Penalti Damage -20%).
4. **Evasive Posture**: Fokus pada menghindar dan pergerakan cepat. (Bonus Evasive +30%, Penalti Hit Rate -15%).
5. **Charging Posture**: Mengumpulkan energi Qi untuk jurus berdaya rusak tinggi. (Rentan terhadap serangan sela / Counter Interrupt).
6. **Broken Posture**: Postur pertahanan hancur akibat parry/serangan berat. (Menerima Critical Damage +50% selama 1 turn).

---

## 4. Turn Flow & Tactical Execution
Satu turn pertarungan berlangsung mengikuti alur berikut:

1. **Inisiatif & Evaluasi Medan**: GM mengevaluasi Jarak, Posisi, Medan, dan Cuaca.
2. **Deklarasi Aksi Pemain**: Pemain memilih aksi (Menyerang, Bertahan, Menghindar, Menggunakan Jurus/Item).
3. **Kalkulasi Modifikator**:
   $$\text{Hit Rate} = \text{Base Accuracy} + \text{Position Mod} + \text{Posture Mod} - \text{Enemy Evasive Mod}$$
   $$\text{Final Damage} = (\text{Base Damage} + \text{Qi/Stamina Scale}) \times \text{Posture Mod} - \text{Enemy Armor/Qi Defense}$$
4. **Eksekusi & Konsumsi**: Pengurangan HP/Qi/Stamina serta penerapan status luka jika ada.

---

## 5. Environmental & Terrain Interactions
* **Mud / Swamp**: Penalti Speed & Evasive -20% (Kecuali pengguna teknik air/rawa).
* **High Wind**: Penalti Akurasi Senjata Panah -20%.
* **Extreme Heat / Cold**: Peningkatan konsumsi Stamina sebesar +25% per turn.

---

## 6. GM Instructions
* Evaluasi kondisi Posture dan Position sebelum menentukan hasil akhir damage pertarungan.
* Berikan deskripsi pertarungan yang mendalam dan taktis berdasarkan lokasi hit (kepala, dada, tangan, kaki).
