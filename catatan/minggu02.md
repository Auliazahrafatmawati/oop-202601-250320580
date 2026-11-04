# Catatan Minggu 02: Struktur OOP: Class, Object, Encapsulation

## Yang saya kerjakan
Pada minggu 2, saya mengerjakan class Aset dengan melengkapi atribut, konstruktor, getter, dan setter. Saya menerapkan enkapsulasi dengan menjadikan seluruh atribut memiliki akses private. Saya juga menambahkan validasi agar kode dan nama aset tidak boleh bernilai null, kosong, atau hanya berisi spasi. Selain itu, saya memastikan status awal aset adalah TERSEDIA dan kondisi awalnya adalah BAIK.

## Keputusan desain
Pada validasi String, saya memilih menggunakan trim().isEmpty() karena trim() menghapus spasi di awal dan akhir String, kemudian isEmpty() memeriksa apakah String tersebut menjadi kosong. Dengan demikian, input yang hanya berisi spasi juga dapat ditolak.

## Kendala
Kendala yang saya alami adalah memahami fungsi isEmpty() dan trim() dalam Java. Saya juga sempat mengalami kesalahan sintaks berupa kurung kurawal (}) yang berlebih saat mengubah kode.

## Penggunaan AI
- Alat yang dipakai: ChatGPT
- Bagian yang dibantu AI: Class Aset, khususnya konstruktor.
- Prompt utama: "isEmpty() gunanya untuk apa?", "kenapa pakenya isEmpty bukan isBlank?", "Di bagian mana saya harus menambahkan trim() pada kode Aset.java?".
- Yang saya ubah atau tolak dari saran AI, dan alasannya: Saya mengunakan trim().isEmpty(). Karena ingin memahami fungsi masing-masing method secara terpisah. Dengan menggunakan trim(), spasi di awal dan akhir String dihapus terlebih dahulu, kemudian isEmpty() digunakan untuk memeriksa apakah String sudah kosong. 
- Satu hal yang saya pahami lebih baik sekarang: Saya memahami bahwa validasi diperlukan agar data aset yang disimpan tetap sesuai dengan aturan sistem.