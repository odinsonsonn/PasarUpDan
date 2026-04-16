# PasarUp

PasarUp adalah aplikasi marketplace mobile yang dirancang untuk mendigitalisasi pengalaman berbelanja di pasar tradisional. Aplikasi ini memungkinkan pengguna untuk mencari toko, melihat produk segar, dan melakukan pemesanan secara efisien melalui perangkat Android.

## Identitas Pembuat
- **Nama:** [NAMA ANDA]
- **NPM:** [NPM ANDA]

## Deskripsi Aplikasi
PasarUp bertujuan untuk menjembatani antara pedagang pasar tradisional dengan konsumen modern. Dengan antarmuka yang ramah pengguna, aplikasi ini menyediakan platform di mana kebutuhan pokok dapat dipesan dengan mudah, mendukung ekosistem ekonomi lokal melalui integrasi teknologi.

## Daftar Fitur
1. **Splash Screen**: Layar perkenalan saat aplikasi pertama kali dibuka.
2. **Autentikasi (Login & Register)**: Sistem masuk dan pendaftaran pengguna untuk keamanan dan personalisasi data.
3. **Beranda (Home)**: Menampilkan rekomendasi toko dan akses cepat ke berbagai menu navigasi.
4. **Pencarian (Search)**: Fitur untuk menemukan produk atau toko spesifik dengan cepat.
5. **Katalog Produk & Toko**: Halaman detail yang menampilkan daftar barang yang dijual oleh pedagang tertentu.
6. **Detail Produk**: Informasi lengkap mengenai harga, deskripsi, dan foto produk.
7. **Keranjang Belanja (Cart)**: Tempat penyimpanan sementara produk yang ingin dibeli sebelum proses checkout.
8. **Checkout**: Proses finalisasi pemesanan barang.
9. **Riwayat Pesanan**: Daftar transaksi yang telah dilakukan oleh pengguna untuk memantau status belanja.
10. **Profil Pengguna**: Informasi akun dan pengaturan pengguna.

## Deskripsi Fitur Teknis
- **Manajemen State**: Menggunakan fragment-based navigation untuk transisi layar yang ringan dan responsif.
- **Penyimpanan Lokal**: Menggunakan `SharedPreferences` untuk menyimpan data profil pengguna secara sederhana.
- **UI/UX**: Menggunakan `RecyclerView` dengan berbagai `Adapter` (seperti `TokoAdapter`, `produkadapter`, `OrderAdapter`) untuk menampilkan data dalam bentuk list atau grid secara dinamis.
