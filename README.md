# TugasPBPFlutter

## Tugas 7 

1. Apa perbedaan utama antara stateless dan stateful widget dalam konteks pengembangan aplikasi Flutter?<br>
    Jawab:
    - Stateful: widget dapat berubah saat ada interaksi dari user.<br>
    - Statless: widget tidak berubah saat ada interaksi dari user. Contoh(Icon, IconButton, Text).<br>
2. Sebutkan seluruh widget yang kamu gunakan untuk menyelesaikan tugas ini dan jelaskan fungsinya masing-masing.<br>
    Jawab:
    - Text: Menampilkan teks pada aplikasi<br>
    - Layout: Menyusun widget2 lain<br>
    - Assets: Icon gambar pada button<br>
3. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step (bukan hanya sekadar mengikuti tutorial)<br>
    Jawab:
    - Membuat proyek baru di folder<br>
    - Mengubah kode bawaan dari flutter dengan yang mirip seperti tutorial<br>
    - Agar bisa menampilkan tombol2 yang berbeda warna, saya membuat fungsi baru yang akan meng-increment setiap loop dan menyesuaikan warna tombol yang ada pada aplikasi

## Tugas 8

1. Jelaskan perbedaan antara Navigator.push() dan Navigator.pushReplacement(), disertai dengan contoh mengenai penggunaan kedua metode tersebut yang tepat!<br>
    Jawab:
    - Navigator.push() = Mengganti halaman dengan cara 'menumpuk' halaman selanjutnya dengan halaman sebelumnya.<br>
    - Navigator.pushReplacement() = Mengganti halaman dengan cara benar2 mengganti halaman sebelumnya dengan halaman selanjutnya<br>
    - Contoh Penerapan:<br>
        - .push() = Dari halaman login ke halaman main menu <br>
        - .pushreplacement() = Dari halaman fitur ke fitur2 lain<br>
2. Jelaskan masing-masing layout widget pada Flutter dan konteks penggunaannya masing-masing!<br>
    Jawab:
    - Row = Menempatkan berbagai widget atau elemen pada 1 baris (Kanan -> Kiri)<br>
    - Column = Menempatkan berbagai widget atau elemen pada 1 kolom (Atas -> Bawah)<br>
    - Wrap = Menyesuaikan penempatan widget atau elemen berdasarkan luas dari gadget masing2 user<br>
3. Sebutkan apa saja elemen input pada form yang kamu pakai pada tugas kali ini dan jelaskan mengapa kamu menggunakan elemen input tersebut!<br>
    Jawab:
    - TextField = Menerima value dari user berupa text.<br>
4. Bagaimana penerapan clean architecture pada aplikasi Flutter?<br>
    Jawab:
    - Clean Architecture merupakan prinsip desain perangkat lunak yang memisahkan berbagai "Separation Of Concern" dan mengutamakan pemisahan berbagai file sesuai kegunannya.<br>
5. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial)<br>
    Jawab:
    - Membuat beberapa file tambahan seprti shoplist_form.dart yang berisi form untuk menerima input dari user.<br>
    - Membuat variabel2 yang sesuai dengan input user seperti nama item, harga, jumlah item, dan deskripsi agar bisa digunakan untuk menyimpan input dari user.<br>
    - Menuliskan kode agar bisa menampilkan itempitem yang baru saja diinput dari user sesuai dengan data2 variabel.<br>
    - Melakukan refactoring file2 agar proyek flutter bisa menjadi lebih clean

## Tugas 9

1. Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu? Jika iya, apakah hal tersebut lebih baik daripada membuat model sebelum melakukan pengambilan data
JSON?<br>
   Jawab:
   - Ya, kita bisa melakukan pengambilan data JSON tanpa membuat model terlebih dahulu.<br>
   - Lebih baik atau tidaknya tergantung dengan penerapan dari aplikasi kita sendiri. Kekurangan dengan tidak membuat model terlebih dulu adalah data yang diambil akan menjadi kurang fleksibel jika ingin dimodifikasi kembali. Namun, prosesnya bisa cepat jika ingin sekedar mengambil data2nya.<br>
2. Jelaskan fungsi dari CookieRequest dan jelaskan mengapa instance CookieRequest perlu untuk dibagikan ke semua komponen di aplikasi Flutter.<br>
   Jawab:
   - Fungsi dari CookieRequest sendiri adalah agar data2 dari pengguna tidak langsung terhapus melainkan juga tersimpan pada perangkat keras pengguna.<br>
   - Instance CookieRequest perlu dibagikan ke semua komponen flutter agar data2 dari komponen yang berbeda dapat disimpan.<br>
3. Jelaskan mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter.<br>
   Jawab:
   - Mengambil data dari JSON<br>
        - Menggunakan paket HTTP untuk membuat permintaan htto ke server<br>
        - Mendapatkan respon dari server<br>
   - Deselerasi Data JSON
        - Mengubah dari dari JSON ke objek dart<br>
   - Model Dart Untuk Data = Membuat model data untuk digunakan pada dart<br>
   - Deselerasi JSON ke Objek Dart<br>
   - Menampilkan Data pada Flutter<br>
4. Jelaskan mekanisme autentikasi dari input data akun pada Flutter ke Django hingga selesainya proses autentikasi oleh Django dan tampilnya menu pada Flutter.<br>
    Jawab:
    - Login/Register Pada aplikasi Flutter<br>
    - Request data ke backend django<br>
    - Proses Autentikasi Django<br>
        - Django Memproses informasi login dan register yang diterima<br>
        - Jika login, django memeriksa apakah datanya valid<br>
        - Jika Register, django akan membuat data baru bagi user<br>
    - Token Authentication<br>
    - Penanganan Token di Flutter<br>
    - Pengiriman Token dalam setiap request<br>
    - Otentikasi dan otorisasi pada django<br>
    - Respon django ke flutter<br>
    - Menampilkan data di flutter<br>
5. Sebutkan seluruh widget yang kamu pakai pada tugas ini dan jelaskan fungsinya masing-masing.<br>
    Jawab:
    - Build<br>
    - InkWell<br>
    - Drawer<br>
6. Jelaskan bagaimana cara kamu mengimplementasikan checklist di atas secara step-by-step! (bukan hanya sekadar mengikuti tutorial).<br>
    Jawab:
    - Mencoba menjalankan hasil deployment projek django sebelumnya
    - Membuat halaman login pada flutter:
        - Menulis kode2 yang sesuai untuk menambahkan form agar user bisa menginput data2<br>
        - Membuat app authentication pada proyek django sebelumnya<br>
        - Membuat fungsi login pada views.py di app autehntication<br>
    - Meng-copy data2 JSON dari proyek django ke suatu web dan menggantinya menjadi kode dart lalu dimasukkan ke product.dart<br>
    - Menulis kode yang akan menampilkan semua item yang baru saja dimasukkan ke dalam list_product.dart<br>
