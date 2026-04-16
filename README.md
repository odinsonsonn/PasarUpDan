# PasarUp

PasarUp adalah aplikasi marketplace mobile yang dirancang untuk mendigitalisasi pengalaman berbelanja di pasar tradisional.

## Identitas Pembuat
- **Nama:** Dandra Jovan ALexi Tombokan
- **NPM:** 24082010180

## Deskripsi Aplikasi
PasarUp bertujuan untuk menjembatani antara pedagang pasar tradisional dengan konsumen modern. Aplikasi ini menyediakan platform di mana kebutuhan pokok dapat dipesan dengan mudah melalui perangkat Android.

## Daftar Fitur
1. **Splash Screen**: Layar perkenalan saat aplikasi dibuka.
2. **Autentikasi**: Login & Register menggunakan SharedPreferences.
3. **Beranda**: Menampilkan daftar toko menggunakan RecyclerView.
4. **Detail Toko & Produk**: Menampilkan list produk per toko dengan Grid layout.
5. **Keranjang Belanja**: Fitur tambah/kurang item secara real-time.
6. **Riwayat Pesanan**: Menyimpan list transaksi yang sudah checkout.
7. **Profil**: Menampilkan informasi akun pengguna.

## Implementasi Teknis & Data
Berikut adalah rincian penggunaan class dan manajemen data:

### 1. Manajemen Layar (Fragment)
Aplikasi menggunakan **Single Activity Architecture** (MainActivity) dengan Fragment untuk efisiensi memori dan navigasi yang mulus.
- **Class Utama:** `MainActivity.kt`, `BerandaFragment.kt`, `StoreDetailFragment.kt`.

### 2. Penyimpanan Data Akun (Permanen)
Menggunakan **SharedPreferences** untuk menyimpan sesi login dan nama user.
- **Class:** `LoginFragment.kt` (Simpan) & `ProfileFragment.kt` (Baca).

### 3. Manajemen Keranjang (Memory Storage)
Menggunakan **Object Singleton** agar data keranjang bisa diakses dari fragment mana pun tanpa hilang saat pindah halaman.
- **Class:** `CartManager` di dalam file `CartItem.kt`.

### 4. Pengiriman Data (Bundle)
Menggunakan **Bundle Arguments** untuk mengirim data spesifik dari satu fragment ke fragment lainnya.
- **Class:** `StoreDetailFragment.kt` (Mengambil data nama/foto toko yang diklik).

### 5. UI Dinamis (Adapter)
Menggunakan **RecyclerView Adapter** untuk mencetak list data secara otomatis dan efisien.
- **Class:** `TokoAdapter.kt`, `GridProductAdapter.kt`, `OrderAdapter.kt`.
