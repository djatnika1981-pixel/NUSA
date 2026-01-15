# NusaGuard v2.2.0

NusaGuard adalah aplikasi keamanan Windows ringan untuk pemindaian file dan USB
secara **on-demand (manual)**. Dirancang sebagai **pendamping antivirus utama**,
bukan pengganti antivirus real-time.

Status: **Public Release (Stable)**

---

## Fitur Utama
- Pemindaian folder manual
- Pemindaian USB / removable drive
- Deteksi berbasis hash dan heuristik ringan
- Karantina file berisiko
- Pencatatan (log) hasil pemindaian secara lokal

---

## Batasan & Ruang Lingkup
- **BUKAN antivirus real-time**
- Tidak memonitor file, proses, atau memori secara terus-menerus
- Tidak berjalan otomatis di background
- Direkomendasikan sebagai **second-opinion / on-demand scanner**

---

## Persyaratan Sistem
- Windows 10 / 11 (64-bit)
- Tidak memerlukan .NET runtime tambahan
- Tidak memerlukan hak Administrator untuk pemindaian standar

> Catatan: Beberapa direktori sistem Windows mungkin tidak dapat dipindai tanpa
> hak akses yang sesuai.

---

## Cara Menggunakan
1. Jalankan `NusaGuard.exe` atau installer resmi
2. Pilih **SCAN FOLDER** atau **SCAN USB**
3. Tunggu hingga progress mencapai **100%**
4. Tinjau hasil pada jendela aplikasi dan file log

---

## Windows SmartScreen
Saat pertama kali dijalankan, Windows dapat menampilkan peringatan
**Microsoft Defender SmartScreen** karena aplikasi belum ditandatangani.

Disarankan untuk:
- Mengunduh aplikasi hanya dari **halaman Releases resmi**
- Memverifikasi checksum SHA256 sebelum menjalankan
- Menjalankan aplikasi hanya jika Anda memahami sumber dan risikonya

---

## Verifikasi Rilis
SHA256 checksum untuk setiap rilis disediakan di halaman **Releases**.
Pastikan checksum sesuai untuk menjamin integritas file.

---

## Lokasi Log & Karantina
Secara default, NusaGuard menyimpan data lokal di:

- Log:
  `%LOCALAPPDATA%\NusaGuard\logs\`
- Karantina:
  `%LOCALAPPDATA%\NusaGuard\quarantine\`

---

## Keamanan & Privasi
- Tidak menginstal driver kernel
- Tidak memodifikasi konfigurasi sistem Windows
- Tidak melakukan koneksi jaringan atau pengiriman data
- Tidak mengumpulkan atau mengirim data pribadi (PII)

Jika perilaku ini berubah di versi mendatang, dokumentasi akan diperbarui.

---

## Pelaporan Bug & Keamanan
- Bug dan masukan umum: gunakan **GitHub Issues**
- Laporan kerentanan keamanan: hubungi maintainer melalui GitHub Security Advisory

Sertakan:
- Versi aplikasi
- Sistem operasi
- Langkah reproduksi
- Potongan log yang relevan

---

## Lisensi
Lisensi: **MIT**  
Lihat file `LICENSE` untuk detail.

---

Versi: **2.2.0**  
Tanggal rilis: **15-01-2026**
