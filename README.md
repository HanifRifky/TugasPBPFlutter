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
