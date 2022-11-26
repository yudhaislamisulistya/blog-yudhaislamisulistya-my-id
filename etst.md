---
title: Test Debugging Python Code 2
tags: python, debug, beginners, debugging, vscode
cover: https://i.imgur.com/yE0BqvV.png
domain: blog.yudhaislamisulistya.my.id
---

*Debugging* merupakan istilah ~~yang~~ yang sering digunakan untuk mengidentifikasi atau melacak sebuah *bug*, error atau kesalahan pada baris kode. *Bug* inilah yang bisa saja sebuah program tidak dapat berjalan sesuai dengan perintah yang kita inginkan. Salah satu hal yang penting ketika kita melakukan *debug* adalah menjalankan baris demi baris kode sambil memeriksa setiap variabel menggunakan **breakpoint**. Hal ini lebih efisien ketimbang menggunakan pendekatan **Print()**

# Debugging di Visual Studio Code

Dalam aplikasi visual studio code atau VSCode, silahkan buat sebuah file dengan ekstensi **.py**. Setelah itu silahkan gunakan kode dibawah ini untuk tujuan demonstrasi

```python
x = 1
y = x + 2
z = [x for x in range(0, y+2)]

print(z)
```

#### 1. Buka Aplikasi Visual Studio Code

Hal pertama yang harus dilakukan ialah dengan menjalankan IDE VSCode lalu pindahkan kode program diatas kedalam IDE ini.
![001](https://i.imgur.com/dhexrwQ.png)

#### 2. Pilih Menu Debug Pada Sidebar

Pada bagian sisi kiri (sidebar) VSCode terdapat menu **Run and Debug**. Lalu pilih menu tersebut seperti tampilan berikut ini.
![002](https://i.imgur.com/UO4dWV8.png)

#### 3. Tentukan Breakpoint

**Breakpoint** secara sederhana merupakan lokasi dimana baris kode akan di hentikan secara sejenak melalui proses **debugging**. Silahkan pilih **breakpoint** pada baris kode pertama dengan tujuan untuk menjalankan baris demi baris mulai (baris 1-5)
![003](https://i.imgur.com/1ULj3Ut.png)

#### 4. Jalankan Debug

Pilih **Run and Debug Python File** untuk menjalankan proses *debugging* pada file ini. Setelah itu, silahkan perhatikan beberapa bagian sisi kiri

1. (*Container variables*) yang merupakan output dari setiap eksekusi baris per baris kode program
2. (*Watch*) yang berfungsi menampilkan sebuah value berdasarkan variabel
3. (*Breakpoint*) yang berfungsi sebagai titik atau lokasi dimana baris kode akan dihentikan secara sejenak

![004](https://i.imgur.com/DPMxKOh.png)

#### 5. Step Into Debugging

Pada bagian sisi kanan atas terdapat terdapat **step into** yang berfungsi untuk melakukan *debugging* pada baris kode selanjutnya. Setelah proses ini akan menghasilkan sebuah *variabel* dengan *value* dari baris kode yang telah di *debugging*
![005](https://i.imgur.com/xwmvpCH.png)
![006](https://i.imgur.com/OkVveEh.png)
Dapat kita lihat bahwa bagian *container variabel* telah memiliki variabel **x** dengan value **1** dan variabel **y** dengan value **3** serta kita juga dapat mengarahkan cursor pada variabel untuk melihat value pada variabel tersebut. Hal inilah yang dapat membuat lebih efisien ketimbang menggunakan pendekatan perintah **Print()**

#### 6. Hasil Debugging

Kode program demonstrasi sederhana ini yang terdiri dari 5 baris menghasilkan sebuah debugging sederhana pada **container variabel** disisi kiri.
![007](https://i.imgur.com/0oP2dl0.png)

#### 7. Bonus

![Full](https://i.imgur.com/YDnSCgH.gif)

# Kesimpulan

**Debugging** merupakan salah satu cara yang sangat efisien ketika kita ingin melakukan *debug* baris demi baris sambil memerika setiap variabel yang terdapat pada kode program tanpa menggunakan perintah **Print()**. Pada artikel ini, dapat kita lihat bahwa setelah melakukan *debug* variabel x, y, z secara proses bertahap akan sangat mudah dipahami.

## Repository

[Github](https://github.com/yudhaislamisulistya/blog-yudhaislamisulistya-my-id/tree/main/debugging-python-code)
