# Catatan Minggu 04: Polymorphism

## Yang saya kerjakan
Pada minggu ini saya mempelajari penerapan polimorphism pada Java, khususnya penggunaan method hitungDenda() pada beberapa jenis aset. Setiap jenis aset memiliki perhitungan denda yang berbeda sesuai dengan aturan bisnis yang telah ditentukan.

## Keputusan desain
Saya menggunakan method overriding pada class Ruang, Laptop, dan AlatLab karena setiap jenis aset memiliki pengali denda yang berbeda.

## Kendala
Kendala yang saya alami adalah hasil perhitungan denda belum sesuai dengan hasil yang diharapkan pada pengujian. Pada class Ruang, tarif yang digunakan sebelumnya masih Rp20.000 per hari, sedangkan seharusnya mengikuti tarif dasar dengan pengali 1 kali. Pada class Laptop, saya juga belum menerapkan pengali 2 kali. Selain itu, terdapat kode UnsupportedOperationException yang masih tertinggal pada method validasiHariTerlambat() sehingga menyebabkan pengujian gagal. Saya mengatasinya dengan memperbaiki rumus perhitungan denda dan menghapus kode tersebut dari method validasi.

## Penggunaan AI
- Alat yang dipakai: Chat GPT
- Bagian yang dibantu AI: Class Aset, Ruang, Laptop, dan AlatLab, terutama method hitungDenda() dan validasiHariTerlambat().
- Prompt utama: "Bagaimana cara menerapkan perhitungan denda pada class Ruang, Laptop, dan AlatLab sesuai aturan bisnis","Mengapa hasil perhitungan denda pada class Ruang dan Laptop tidak sesuai dengan hasil pengujian?", dan "Apa fungsi method validasiHariTerlambat() dan bagaimana cara memperbaikinya?"
- Yang saya ubah atau tolak dari saran AI, dan alasannya: Saya menyesuaikan perhitungan denda berdasarkan aturan bisnis proyek. Saya tidak langsung menggunakan tarif yang ada pada kode awal karena tarif tersebut belum sesuai dengan pengali setiap jenis aset. Saya juga tetap memeriksa kode dan hasil pengujian sebelum menerapkan saran AI.
- Satu hal yang saya pahami lebih baik sekarang: Saya memahami bahwa validasi perlu dilakukan sebelum proses perhitungan agar data yang digunakan sesuai aturan.
