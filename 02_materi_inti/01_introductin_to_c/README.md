# Pengenalan Bahasa C

Pada bagian pertama modul ini, kita akan mengenal dasar-dasar pemrograman dalam bahasa C, yang dikenal dengan sintaks sederhana namun kuat. Bahasa C adalah bahasa pemrograman yang digunakan untuk berbagai aplikasi, mulai dari pengembangan sistem operasi hingga perangkat keras. Dalam bab ini, kita akan memulai dengan program pertama kita: **Hello, World!**.


### Tujuan Pembelajaran

Pada bab ini, kamu akan mempelajari dasar-dasar pemrograman dalam bahasa C. Setelah menyelesaikan bab ini, kamu akan memahami hal-hal berikut:

1. **Apa itu `printf`?**

   - **`printf`** adalah fungsi standar dalam bahasa C yang digunakan untuk mencetak atau menampilkan informasi ke layar. Fungsi ini memungkinkan kita untuk memberikan output berupa teks, angka, atau bahkan hasil perhitungan langsung di dalam program. Fungsi **`printf`** menerima argumen berupa string (teks) dan dapat berisi format untuk menampilkan data dalam berbagai bentuk.

   - **Contoh penggunaan `printf`:**

     ```c
     printf("Hello, World!\n");
     ```

     Pada contoh di atas, `printf` digunakan untuk menampilkan teks "Hello, World!" di layar. Teks ini adalah argumen pertama yang diberikan ke dalam fungsi **`printf`**.

   - **Format String di `printf`**:
     Fungsi **`printf`** dapat digunakan untuk menampilkan berbagai jenis data dengan menggunakan format tertentu. Contoh format yang sering digunakan antara lain:

     - **`%d`** untuk menampilkan angka bulat (integer).
     - **`%f`** untuk menampilkan angka desimal (float).
     - **`%s`** untuk menampilkan teks (string).

     Contoh:

     ```c
     int angka = 10;
     printf("Nilai angka: %d\n", angka);
     ```

     Outputnya:

     ```bash
     Nilai angka: 10
     ```

2. **Apa itu Fungsi `main`?**

   - **`main()`** adalah fungsi utama dalam program C. Fungsi ini adalah tempat eksekusi pertama kali dimulai saat program dijalankan. Tanpa adanya fungsi **`main`**, program C tidak dapat dijalankan. Di dalam **`main`**, kita menuliskan logika program yang ingin dijalankan.

   - **Struktur Fungsi `main`**:
     Fungsi `main` memiliki struktur seperti ini:

     ```c
     int main() {
         // Program dijalankan di sini
         return 0;
     }
     ```

     - **`int`**: Tipe data yang mengindikasikan bahwa fungsi `main` akan mengembalikan nilai berupa angka bulat (integer). Nilai ini biasanya digunakan untuk memberi tahu apakah program berhasil dijalankan (nilai 0 biasanya menunjukkan keberhasilan).
     - **`return 0;`**: Perintah ini memberi tahu sistem operasi bahwa program telah selesai dijalankan dengan sukses. Nilai **`0`** umumnya digunakan untuk menunjukkan bahwa program tidak mengalami kesalahan.

   - **Kenapa `main` sangat penting?**
     Fungsi **`main`** adalah titik awal dari eksekusi program. Semua program C yang valid harus memiliki fungsi **`main`**, karena tanpa fungsi ini, program tidak akan tahu di mana harus dimulai. Ketika kamu menjalankan program, sistem operasi akan mencari fungsi **`main`** untuk memulai eksekusi program.

### Struktur Program C

Program pertama yang akan kamu buat adalah program yang menampilkan pesan "Hello, World!" di layar. Program ini memperkenalkan beberapa elemen dasar dalam bahasa C, termasuk:

- **`#include <stdio.h>`**: Menyertakan library untuk input-output standar.
- **`main()`**: Fungsi utama dalam program C yang menjadi titik awal eksekusi.
- **`printf()`**: Fungsi untuk menampilkan teks ke layar.

Selanjutnya, mari kita lihat implementasi program pertama kita.

---

### Program 1: Hello, World!

Lihat file `hello_world.c` untuk implementasi kode.
