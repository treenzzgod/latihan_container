# latihan_container :memo:
<hr>

![logo_Container](https://belajarflutter.com/wp-content/uploads/2020/08/penjelasan-container-widget-300x211.png)


## contoh struktur penggunaan container pada aplikasi flutter
<hr>

![logo_tree](https://belajarflutter.com/wp-content/uploads/2020/08/sample-flutter-layout-46c76f6ab08f94fa4204469dbcf6548a968052af102ae5a1ae3c78bc24e0d915.png)

Container adalah sebuah wadah dimana dapat menyimpan berbagai macam  attribute dan menampung berbagai macam fungsi objek yang membuat kotak container  bisa menampilkan berbagai macam efek dan hasil di dalamnya

## Penerapan Fungsi Property di Widget Container :memo:
<hr>

1. **Property child** :white_check_mark:

Seperti yang telah disampaikan sebelumnya bawah Container merupakan Single Child Widget. Ciri utama dari tipe tersebut yaitu memilik properti child. Pada properti ini digunakan untuk memuat anakan atau turunan dari Container, yang dapat memuat widget lainnya seperti Text, Column, ListView, dll.

Berikut contoh penerapan penggunaan property child dalam Widget Container Class.

``` dart
body: Container(
  child: Text(
    'Ayo Belajar Flutter',
  )
),

```
2. **Property Alignment** :white_check_mark:

Dengan container widget kita dapat mengatur posisi child widget menggunakan fungsi property Alignment diantaranya seperti :

- bottomCenter untuk memindahakan kebawah bagian tengah.
- bottomLeft untuk memindahkan ke bawah bagian Kiri.
- bottomRight untuk memindahkan ke bawah bagian Kanan.
- center untuk untuk memindahkan ke posisi tengah.
- centerLeft untuk memindahkan ke tengah bagian Kiri.
- centerRight untuk memindahkan ke tengah bagian Kanan.
- topCenter untuk memindahkan ke atas bagian Tengah.
- topLeft untuk memindahkan ke atas bagian Kiri.
- topRight untuk memindahkan ke atas bagian Kanan.

Contoh : 

``` dart 
body: Container(
  alignment: Alignment.bottomCenter,
  child: Text(
    'Ayo Belajar Flutter',
    style: TextStyle(
      fontSize: 20,
    ),
  )
),

```

![aligment](https://belajarflutter.com/wp-content/uploads/2020/08/penggunaan-container-alignment.png) 



3. **Property Color** :white_check_mark:

Penambahan property ini untuk membuat wadah / Container memiliki warna latar belakang

contoh : 

``` dart 
body: Container(
  alignment: Alignment.center,
  color: Colors.purple,
  child: Text(
    'Ayo Belajar Flutter',
    style: TextStyle(
      fontSize: 20,
      color: Colors.white
    ),
  )
),

```



![color](https://belajarflutter.com/wp-content/uploads/2020/08/Screen-Shot-2020-08-02-at-08.43.31-1024x798.png)


untuk pemilihan warna bisa menggunakan colors 
![colors](https://belajarflutter.com/wp-content/uploads/2020/08/pilihan-warna-materialDesign-flutter-1.gif)


4. **Property Height dan Weight** :white_check_mark:

karena secara default  ukuran container akan menyesuaikan  dengan body layar aplikasi maka layout bisa diatur dengan menambahkan properti height dan weight

![height_and_weight](https://belajarflutter.com/wp-content/uploads/2020/08/height-container-flutter.gif)

5.  **Property Margin** :white_check_mark:

margin digunakan untuk  membuat jarak diantara container dengan widget lainya sehingga container akan menjorok ke dalam

``` dart
body: Container(
  margin: EdgeInsets.all(20),
  height: 200,
  width: 200,
  alignment: Alignment.topLeft,
  color: Colors.purple,
  child: Text(
    'Ayo Belajar Flutter',
    style: TextStyle(
      fontSize: 20,
      color: Colors.white
    ),
  )
),
```

6. **Property Padding** :white_check_mark:

untuk menambahkan jarak container dengan widget yang ada didalamnya,sama dengan margin tetapi ini kalau margin itu container degan widget yang berada di luar nya 

``` dart
body: Container(
  padding: EdgeInsets.only(left:20),
  height: 200,
  width: 200,
  alignment: Alignment.topLeft,
  color: Colors.purple,
  child: Text(
    'Ayo Belajar Flutter',
    style: TextStyle(
      fontSize: 20,
      color: Colors.white
    ),
  )
),
```

7. **Property Transform** :white_check_mark:
 
 melakukan rotasi pada container atau perputaran sumbu x,y,z menggunakan fungsi Matrix4 untuk rotasinya

 contoh 

 ``` dart
Container(
  margin: EdgeInsets.all(20),
  transform: Matrix4.rotationZ(0.1),
  height: 200,
  width: 200,
  color: Colors.purple,
),
//rotasi pada sumbu z bisa diliat code rotationZ (0,1)
 ```

![rotasi](https://belajarflutter.com/wp-content/uploads/2020/08/Screen-Shot-2020-08-02-at-09.42.04-300x257.png)

8. **Property Decoration** :white_check_mark:

menghias container dengan berbagai macam efek dekor


contoh :

``` dart
Container(
  decoration: BoxDecoration(
    color: const Color(0xff7c94b6),
    image: const DecorationImage(
      image: NetworkImage('https://i.pinimg.com/originals/91/86/6b/91866b918c9cca0747f483a46943e926.jpg'),
      fit: BoxFit.cover,
    ),
    border: Border.all(
      color: Colors.black,
      width: 8,
    ),
    borderRadius: BorderRadius.circular(12),
  ),
  height: 280,
  width: 200,
  margin: EdgeInsets.all(20)
)

```

![dekor](https://belajarflutter.com/wp-content/uploads/2020/08/container-decoration-1.png)

menggunakan **networkImage** untuk mengambil gambar dari internet 










A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.dev/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.dev/docs/cookbook)

For help getting started with Flutter, view our
[online documentation](https://flutter.dev/docs), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
