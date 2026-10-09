# DompetKu Android

Proyek Android berbasis WebView yang membungkus prototipe DompetKu. Fitur lokal meliputi pencatatan pemasukan/pengeluaran, ringkasan saldo, anggaran, target tabungan, pengingat tagihan, catatan utang, kalender, ekspor dan cadangan data.

## Cara mendapatkan APK tanpa Android Studio

APK belum dibangun di dalam paket ini. Gunakan GitHub Actions untuk membangunnya di cloud:

1. Masuk atau buat akun di https://github.com.
2. Buat repository baru, misalnya `DompetKuAndroid`.
3. Ekstrak ZIP ini, lalu unggah semua isi folder `DompetKuAndroid` ke repository tersebut (termasuk folder tersembunyi `.github/workflows`).
4. Buka tab **Actions** di repository dan pilih **Build DompetKu APK**.
5. Tekan **Run workflow** jika belum berjalan otomatis, lalu buka proses build yang selesai.
6. Di bagian **Artifacts**, unduh `DompetKu-debug-APK.zip`.
7. Ekstrak ZIP tersebut untuk mendapatkan `app-debug.apk`, lalu buka APK di HP Android untuk memasangnya. Android mungkin meminta izin memasang aplikasi dari sumber tersebut.

## Batasan penting

- Ini adalah APK debug setelah dibangun; bukan rilis Play Store.
- Login akun dan sinkronisasi cloud Supabase belum terhubung/aktif.
- Data prototipe disimpan secara lokal di WebView perangkat. Jangan anggap data sudah dicadangkan ke cloud.
- Jangan memasukkan informasi keuangan rahasia sampai autentikasi, keamanan, dan sinkronisasi online benar-benar diimplementasikan dan diuji.
