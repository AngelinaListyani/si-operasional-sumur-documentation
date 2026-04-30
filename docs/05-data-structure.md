# Data Structure 

## 1. User
   Entitas ini digunakan untuk menyimpan data pengguna yang memiliki akses ke sistem.
   **Field:**
   * id
   * username
   * password
   * email
---
## 2. Master Sumur 
   Entitas ini berisi data referensi jenis - jenis sumur yang digunakan dalam operasional.
   **Field:**
   * id
   * name
   * code
---
## 3. Data Operasional Sumur 
   Entitas ini berisi data utama yang menyimpan hasil operasional sumur setiap periode 
   **Field:**
   * id
   * master_bagan (relasi ke master sumur)
   * code
   * type
   * date
   * debit
   * kadar
   * jam kerja
   * jumlah air
---
## Relasi Antar Entitas
   * Setiap data operasional sumur terhubung dengan satu jenis sumur pada tabel master sumur
   * Satu user dapat mengelola banyak data operasional sumur
