
# Struktur Kontrol dalam Bahasa C

Hai, teman-teman! 🌟  
Pernahkah kalian merasa bingung bagaimana membuat program yang bisa **berpikir** dan **memilih** jalan ceritanya sendiri? Atau mungkin pernah terbayang, bagaimana caranya supaya program kita enggak jalan terus secara linear tanpa bisa memilih apa yang harus dilakukan?

Di bab ini, kita bakal bahas tentang **Struktur Kontrol** dalam bahasa C! Yap, struktur kontrol adalah bagian penting dalam pemrograman yang memungkinkan kita untuk membuat **keputusan** dalam program, seperti memilih mana yang harus dijalankan berdasarkan kondisi tertentu. Selain itu, kalian juga bakal belajar cara membuat program yang **mengulang** tindakan tertentu tanpa harus menulis kode berulang-ulang. Seru kan?

### Kenapa Kamu Harus Tahu Ini?

Tanpa struktur kontrol yang tepat, program yang kamu buat bisa jadi **kaku** dan **boring**. Contohnya, coba bayangkan program yang harus melakukan sesuatu berulang-ulang (misalnya, mencetak angka atau menghitung total uang), tetapi kita harus menulis kode yang sama berulang kali. Kalau begitu, programmer bakal kelihatan seperti orang yang mengulang-ulang pekerjaan tanpa alasan, kan? 😅

Nah, di bab ini kamu akan belajar cara menggunakan **percabangan** dan **perulangan** di bahasa C, yang membuat program kamu bisa **mengambil keputusan** dan **mengulang** langkah-langkah dengan lebih cerdas dan efisien.

**Gak usah khawatir**, semua penjelasan disajikan dengan cara yang **simple**, **penuh contoh**, dan pastinya bisa langsung kalian coba dalam program yang nyata! Dengan menguasai struktur kontrol, kalian bisa bikin program yang **lebih fleksibel**, **dinamis**, dan tentunya **lebih powerful**!

Ayo, siap-siap untuk jadi pro dalam menggunakan struktur kontrol! 🚀

---

### **Tujuan Pembelajaran: Struktur Kontrol dalam Pemrograman C**

Yuk, kita mulai perjalanan kita untuk memahami **Struktur Kontrol** dalam bahasa C! Setelah mempelajari bab ini, kalian diharapkan bisa:

1. **Paham dan Bisa Gunakan `if` dan `else` dengan Pede**  
   Di dunia pemrograman, kita akan sering dihadapkan dengan masalah membuat keputusan berdasarkan kondisi tertentu. Misalnya, program bisa menampilkan pesan yang berbeda tergantung apakah angka yang dimasukkan lebih besar atau lebih kecil dari angka tertentu. Dengan menggunakan **`if`**, **`else`**, dan **`else if`**, kalian bisa membuat program yang **berpikir** dan **beradaptasi** dengan berbagai kondisi. Gampang kan?

2. **Menguasai Perulangan: `for`, `while`, dan `do-while`**  
   Terkadang kita perlu melakukan hal yang sama berulang kali, entah itu menghitung jumlah angka atau mencetak data. Nah, di sini lah perulangan datang untuk menyelamatkan kalian! Dengan **`for`**, **`while`**, dan **`do-while`**, kalian bisa membuat program yang **lebih efisien** dan **lebih ringkas**. Misalnya, kalian bisa mencetak angka dari 1 sampai 100 tanpa menulis kode berulang-ulang. 

3. **Bisa Menggabungkan Semua yang Dipelajari ke dalam Program Sederhana**  
   Setelah paham cara kerjanya, saatnya kalian praktek! Kami siapkan latihan-latihan seru di akhir pembelajaran ini, supaya kalian bisa langsung implementasikan **percabangan** dan **perulangan** dalam program nyata. Semakin sering berlatih, semakin jago!

---

### **Kenapa Struktur Kontrol Itu Penting?**

Bayangkan kalau program yang kalian buat berjalan tanpa ada kemampuan untuk memilih atau mengulang sesuatu. Programnya jadi kaku dan enggak bisa beradaptasi dengan situasi yang berubah, kan? Struktur kontrol adalah **otak** dari program kalian:  
- **Percabangan** itu seperti kalian memilih jalan hidup, memilih mana yang harus dilakukan berdasarkan situasi. Misalnya, apakah nilai ujian kalian lulus atau tidak?  
- **Perulangan** itu seperti kalian ngulang kegiatan yang sama, seperti ngitung uang kembalian, tapi enggak perlu tulis kode berulang-ulang. Gampang banget!

Struktur kontrol bikin program kalian **lebih fleksibel**, **lebih dinamis**, dan tentunya **lebih powerful**.

---

## **Struktur Kontrol dalam Pemrograman C**

### **1. Percabangan (Conditional Statements)**

Di dunia nyata, kita sering dihadapkan pada keputusan yang bergantung pada situasi atau kondisi tertentu. Begitu juga dalam pemrograman, kita perlu **memilih jalur mana** yang akan diambil program kita berdasarkan kondisi yang ada. Nah, di sinilah struktur percabangan berperan penting!

**Percabangan** memungkinkan kita untuk mengeksekusi bagian kode tertentu hanya jika kondisi yang ditentukan **benar**. Di C, struktur percabangan yang paling sering digunakan adalah **`if`**, **`else`**, dan **`else if`**.

#### **`if` Statement**
Struktur percabangan pertama yang harus kalian kenal adalah **`if`**. Fungsi utamanya adalah untuk menjalankan blok kode hanya jika **kondisi** yang diberikan **benar**.

**Sintaks:**
```c
if (kondisi) {
    // Blok kode yang dijalankan jika kondisi benar
}
```

**Contoh:**
```c
int angka = 10;
if (angka > 5) {
    printf("Angka lebih besar dari 5.\n");
}
```
Pada contoh di atas, program akan menampilkan "Angka lebih besar dari 5" karena kondisi `angka > 5` adalah benar.

#### **`if-else` Statement**
Selain **`if`**, ada juga **`else`** yang memungkinkan kita menjalankan kode lain jika kondisi **salah**. Jadi, program bisa memilih antara dua jalur, yaitu jika kondisi benar atau salah.

**Sintaks:**
```c
if (kondisi) {
    // Blok kode jika kondisi benar
} else {
    // Blok kode jika kondisi salah
}
```

**Contoh:**
```c
int angka = 3;
if (angka > 5) {
    printf("Angka lebih besar dari 5.\n");
} else {
    printf("Angka tidak lebih besar dari 5.\n");
}
```
Pada contoh ini, karena `angka` tidak lebih besar dari 5, maka program akan mencetak "Angka tidak lebih besar dari 5".

#### **`else if` Statement**
Kadang-kadang kita perlu memeriksa lebih dari satu kondisi. Di sinilah **`else if`** masuk. Ini memungkinkan kita untuk memeriksa kondisi tambahan jika kondisi pertama salah.

**Sintaks:**
```c
if (kondisi1) {
    // Blok kode jika kondisi1 benar
} else if (kondisi2) {
    // Blok kode jika kondisi2 benar
} else {
    // Blok kode jika semua kondisi salah
}
```

**Contoh:**
```c
int nilai = 75;
if (nilai >= 90) {
    printf("Grade: A\n");
} else if (nilai >= 75) {
    printf("Grade: B\n");
} else {
    printf("Grade: C\n");
}
```
Di sini, program akan mengecek kondisi satu per satu dan memberikan hasil grade yang sesuai dengan nilai yang dimasukkan.

---

### **2. Perulangan (Loops)**

Kadang dalam pemrograman kita perlu mengulang eksekusi blok kode yang sama beberapa kali. Misalnya, mencetak angka 1 hingga 10, atau memproses setiap elemen dalam array. Di sinilah **perulangan** menjadi sangat berguna!

Ada beberapa jenis perulangan yang sering digunakan dalam bahasa C: **`for`**, **`while`**, dan **`do-while`**.

#### **`for` Loop**
Perulangan **`for`** digunakan ketika kita mengetahui **jumlah iterasi** yang ingin dilakukan. Biasanya digunakan untuk perulangan yang memiliki batasan yang jelas.

**Sintaks:**
```c
for (inisialisasi; kondisi; perubahan) {
    // Blok kode yang akan diulang
}
```

**Contoh:**
```c
for (int i = 1; i <= 5; i++) {
    printf("Perulangan ke-%d\n", i);
}
```
Di sini, perulangan **`for`** akan mencetak angka 1 hingga 5.

#### **`while` Loop**
Jika kalian tidak tahu seberapa banyak iterasi yang diperlukan, **`while`** bisa jadi pilihan. **`while`** akan terus mengulang selama kondisi yang diberikan bernilai **benar**.

**Sintaks:**
```c
while (kondisi) {
    // Blok kode yang akan diulang
}
```

**Contoh:**
```c
int i = 1;
while (i <= 5) {
    printf("Perulangan ke-%d\n", i);
    i++;
}
```
Pada contoh ini, selama nilai **`i`** masih kurang dari atau sama dengan 5, perulangan akan terus terjadi.

#### **`do-while` Loop**
Berbeda dengan **`while`**, **`do-while`** akan selalu menjalankan blok kode setidaknya sekali, **terlepas dari apakah kondisi bernilai benar atau salah**. Setelah itu, baru mengecek kondisi.

**Sintaks:**
```c
do {
    // Blok kode yang akan diulang
} while (kondisi);
```

**Contoh:**
```c
int i = 1;
do {
    printf("Perulangan ke-%d\n", i);
    i++;
} while (i <= 5);
```
Walaupun kondisi awal `i` adalah 1, perulangan **`do-while`** tetap akan dieksekusi setidaknya satu kali sebelum memeriksa kondisi.

---

Dengan penjelasan ini, kalian sudah lebih siap untuk menggunakan **percabangan** dan **perulangan** dalam program kalian. Percabangan untuk membuat keputusan, dan perulangan untuk mengulang bagian kode tanpa perlu menulisnya berulang kali. Pahami konsep ini dengan baik, dan kalian akan lebih siap untuk menulis program-program yang lebih kompleks! 🚀

Semoga setelah mempelajari bab ini, kalian jadi lebih ngerti dan semakin percaya diri dalam menulis kode. Struktur kontrol ini adalah dasar yang harus dikuasai untuk bisa bikin program-program yang lebih seru dan kompleks. Ayo, jangan ragu untuk eksplorasi dan coba latihan-latihan serunya!