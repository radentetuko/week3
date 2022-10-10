# Materi Week 3

## 1. JavaSripct Array

- ### Apa itu Array ?
  Array merupakan struktur data yang digunakan untuk menyimpan sekumpulan data dalam satu tempat. Setiap data dalam Array memiliki indeks, sehingga kita akan mudah memprosesnya. Indeks array selalu dimulai dari angka nol ( 0 ).
- ### Array methods

  Untuk mempermudah penggunaan array, JavaScript menyediakan beberapa fungsi yang melekat pada setiap variabel array (atau lebih tepat disebut dengan method). Berikut adalah method objek array di dalam JavaScript.

  - push() -> menambahkan array pada index terakhir
  - pop() -> Menghapus array pada index terakhir
  - shift() -> Menghapus array pada index pertama
  - unshift() -> Menambahkan array pada index pertama
  - sort() -> Mengurutkan array secara ascending maupun descending

- ### Looping Array

  Untuk looping array kita bisa menggunakan forEach() dan map().

  Di dalam JavaScript Fungsi forEach melakukan iterasi dalam array yang kita pakai dan melakukan perubahan secara langsung dalam element array tersebut. Sedangkan fungsi map dalam JavaScript melakukan iterasi terhadap array dan nge return array baru yang telah dimodifikasi dalam operasi yang kita lakukan.

- ### Array Multidimensi
  Array Multidimensi adalah sebuah Array yang memiliki lebih dari satu subskrip. Atau bisa dianalogikan dengan array of array. Artinya array di dalam sebuah array.

## 2. Rekursif

- ### Apa itu Rekursif ?
  Fungsi rekursif adalah fungsi yang memanggil dirinya sendiri. Biasanya digunakan untuk kasus yang melibatkan operasi matematika di dalamnya. Adapun ciri-ciri dari rekursif adalah selalu memiliki kondisi yang menyatakan kapan fungsi tersebut akan berhenti. Tujuan utama dari rekursif adalah memecahkan masalah dengan mengurangi masalah tersebut menjadi masalah-masalah kecil.

## 3. Modules

- ### Apa itu Modules ?

  Module adalah file Javascript yang di dalamnya terdapat value dari objects, functions, dan variables. Kemudian file tersebut dapat diexport dan diimport oleh file lain. Yang mana file lain yang mengimportnya dapat menggunakan values yang ada di file tersebut.

  Ada beberapa tindakan yang ada di dalam modules.

  - Export
  - Import
  - Export as
  - Import as
  - Export Default

## 4. Object

- ### Apa itu Object ?

  Object JavaScript adalah wadah untuk nilai atau value yang diberi nama atau biasa disebut properti atau method.Objek pada javascript, dapat dibuat dengan tanda kurung kurawal dengan isi berupa key dan value.

  Contoh :

  ```javascript
  var car = {
    type: "Fiat",
    model: "500",
    color: "white",
  };
  ```

  Penjelasan :

  - type, model, dan color disebut _key_
  - fiat, 500, white disebut _value_

## 5. OOP (Object Oriented Programming)

- ### Apa itu OOP (Object Oriented Programming) ?

  Object Oriented Programing adalah salah satu paradigma atau teknik atau cara dalam menulis program yang berorientasikan pada objek.

- ### Kenapa perlu OOP ?

  Tujuan dari OOP diciptakan yaitu untuk mempermudah dalam pengembangan program, karena aplikasi yang dibuat semakin lama akan semakin besar dan baris kodenya pun semakin lama akan semakin banyak. Maka dari itu, kamu membutuhkan teknik baru untuk dapat mengatur manajemen kode yang kamu punya sehingga akan lebih mudah dikembangkan dan dilakukan update.

  OOP memiliki 4 pilar utama yaitu:

  - Inheritance
  - Polymorphism
  - Encapsulation
  - Abstraction

## 6. Web Storage

- ### Apa itu Web Storage?

  Web storage adalah salah satu Web API yang dapat menyimpan data secara lokal pada sisi client. Berbeda dengan objek atau array, data yang disimpan pada objek atau array JavaScript bersifat sementara, dan akan hilang jika terjadi reload atau pergantian URL pada browser. Sedangkan data yang disimpan pada Web Storage akan bertahan lebih lama karena data akan disimpan pada storage browser.

- ### Perbedaan Local Storage dan Session Storage

  Web Storage itu ada dua jenisnya yaitu localStorage dan sessionStorage. LocalStorage digunakan untuk menyimpan data pada browser dan data akan tetap tersimpan walaupun browser ditutup atau komputer dimatikan sekalipun. Sedangkan sessionStorage digunakan untuk menyimpan data pada browser hanya pada satu sesi dan data akan dihapus ketika browser ditutup.

  roperty dan method yang digunakan pada localStorage dan sessionStorage yaitu:

  - key(n) Mendapatkan nama key atau nama data urutan ke-n pada penyimpanan dimulai dari 0.
  - length Mendapatkan jumlah item data yang disimpan pada storage
  - getItem(nama_key) Mendapatkan data dari storage dengan nama yang disebutkan
  - setItem(nama_key, data_disimpan) Menyimpan data ke storage
  - removeItem(nama_key) Menghapus data pada storage dengan nama yang disebutkan
  - clear() Mengosongkan semua data tersimpan pada storage

## Asynchronous

- ### Perbedaan Synchronous dan asynchronous

  Synchronous adalah yang paling umum dan mudah di mengerti. Setiap perintah di eksekusi satu persatu sesuai urutan kode yang kita tuliskan. Sedangkan Asynchronous hasil eksekusi atau output tidak selalu berdasarkan urutan kode, tetapi berdasarkan waktu proses. Eksekusi dengan asynchronous tidak akan membloking atau menunggu suatu perintah sampai selesai. Daripada menunggu, asynchronous akan mengeksekusi perintah selanjutnya.

- ### Cara menjalankan Asynchronous

  Ada beberapa cara untuk membuat proses asynchronous. Kami membatasi hanya memberikan 2 cara ini:

  - _setTimeout(function, milliseconds)_ digunakan untuk simulasi pemanggilan kembali proses asynchronous yang sedang/sudah selesai dijalankan. Pemanggilan hanya dilakukan 1 kali.
  - _setInterval(function, milliseconds)_ digunakan untuk simulasi pemanggilan proses asynchronous yang sedang/sudah dijalankan dalam interval waktu tertentu. Pemanggilan dilakukan berkali-kali sesuai interval waktu yang ditentukan.

- ### kelemahan Asynchronous

  Asynchronous memiliki kelemahan yaitu ada satu perintah yang bergantung pada output eksekusi proses sebelumnya. Dengan kata lain fungsi akan berjalan secara kejar-kejaran, sehingga datang yang diinginkan akan menjadi kosong. Untuk mengatasinya kita dapat menggunakan cara dibawah ini:

  - Callback
  - Promise
  - Async/await
  - Fetch
