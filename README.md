# Arsitektur Multiple Prosesor dan Multiprosesor Symmetric

![Screenshot 2025-05-05 081554](https://github.com/user-attachments/assets/afda330b-4ee6-4799-8962-2ac11476649f)

### *1. Architecture Multiprocessor*
Pada sisi kiri gambar, arsitektur Multiprocessor digambarkan sebagai sistem dengan beberapa prosesor yang memiliki hierarki memori antara L1 Cache, L2 Cache, dan memori utama. Proses komunikasi antar prosesor dikelola menggunakan **System Bus/Interconnect* yang menghubungkan prosesor dengan memori utama.

#### *Karakteristik Utama*:
1. *L1 Cache dan L2 Cache*:
   - Setiap CPU memiliki *L1 Cache* (cache tingkat pertama) untuk akses cepat ke data yang sering digunakan.
   - *L2 Cache* berfungsi sebagai cache tingkat kedua yang mungkin berbagi data antara beberapa prosesor.

2. *System Controller*:
   - Bertindak sebagai pengatur komunikasi antara memori utama, I/O, dan prosesor.

3. *Independensi Prosesor*:
   - Setiap prosesor bekerja secara relatif independen dengan memori lokal (local cache), namun komunikasi tetap dikoordinasikan melalui *System Bus*.

---

### *2. Architecture Multiprocessor Symmetric (SMP)*
Pada sisi kanan gambar, arsitektur SMP ditunjukkan sebagai sistem dengan *System Bus* sebagai penghubung langsung antara semua prosesor dan memori utama. Dalam sistem ini, semua prosesor memiliki akses simetris terhadap memori bersama.

#### *Karakteristik Utama*:
1. *System Bus*:
   - Semua prosesor terhubung langsung ke memori dan perangkat I/O melalui *System Bus*, sehingga memungkinkan komunikasi yang cepat dan efisien.

2. *Cache Bersama*:
   - Data dari memori utama dapat di-cache untuk mempercepat akses oleh masing-masing prosesor.

3. *I/O Controller*:
   - Mengatur komunikasi antara perangkat input/output dengan prosesor.

4. *Akses Simetris*:
   - Semua prosesor memiliki akses yang sama terhadap memori utama dan perangkat I/O, sehingga tidak ada hierarki di antara prosesor.
