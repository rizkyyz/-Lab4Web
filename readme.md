# Tugas LAB 3 Web
## Profil
| # | Biodata |
| -------- | --- |
| *Nama* | Muhammad rizky abdillah |
| *NIM* | 312010368 |
| *Kelas* | TI.20.A.2 |
| *Mata Kuliah* | Pemrograman Web |
## 1. Langkah Langkah Praktikum
* Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.

```
<!DOCTYPE html>
<html lang="en">
<head>
     <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
    <body>
        <header>
            <h1>Box Element</h1>
        </header>
    </body>
</html
```

* Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.

```
<section>
 <div class="div1">Div 1</div>
 <div class="div2">Div 2</div>
 <div class="div3">Div 3</div> 
</section>
```
* Membuat Bagian CSS

```
<style>
 div {
 float:left;
 padding: 10px; 
 }
 .div1 {
 background: red;
 }
 .div2 {
 background: yellow;
 }
 .div3 {
 background: green;
 }
</style>
```
* Kemudian Hasilnya adalah.
![internal](img/box.png)

## Mengatur Clearfix Element
* Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk 
mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut.

```
.div4 {
 background-color: blue;
 clear: left;
 float: none; }
```
* Maka Hasilnya Begini
![internal](img/box2.png)

## 2. Langkah Langkah Modul Praktikum 
## Layout Sederhana
* Kita akan membuat layout web sederhana seperti gambar berikut.
![internal](img/hasil_layout.png)

* Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama 
home.html, dan file css dengan nama style.css.

```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Layout Sederhana</title>
 <link rel="stylesheet" href="style.css">
</head>
<body>
 <div id="container">
 
 </div>
</body>
</html>
```

* Kemudian tulis kode berikut.
```
    <header>
 <h1>Layout Sederhana</h1>
    </header>
<nav>
    <a href="home.html" class="active">Home</a>
    <a href="artikel.html">Artikel</a>
    <a href="about.html">About</a>
    <a href="kontak.html">Kontak</a>
</nav>
<section id="hero"></section>
<section id="wrapper">
    <section id="main"></section>
    <aside id="sidebar"></aside>
</section>
<footer>
 <p>&copy; 2021 - Universitas Pelita Bangsa</p>
</footer>
```

* kemudian hasilnya 
![internal](img/layout1.png)

* kemudian berikan css nya untuk menambahkan style pada html nya 
```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
    margin: 0;
    padding: 0; }
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a; }
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc; }
/* header */
header {
    padding: 20px; }
header h1 {
    margin: 20px 10px;
    color: #b5b5b5; }
```
* kemudian hasilnya 
![internal](img/layout2.png)

# Selanjutnya Kita Mengatur Navigasi
* Kemudian selanjutnya mengatur navigasi Dibagian style.css.
```
/* navigasi */
nav {
    display: block;
    background-color: #1f5faa; }
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold; }
nav a.active,
nav a:hover {
    background-color: #2b83ea; }
```

# Selanjutnya Kita Membuat Isi Class HERO
* Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut
```
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
    elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
    pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
* Lalu Atur Css nya
```
/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px; }
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px; }
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px; }
```
* Maka hasilnya 
![internal](img/layout4.png)

## selanjutnya Mengatur Layout Main dan Sidebar
* Selanjutnya mengatur main content dan sidebar, tambahkan CSS float
```
/* main content */
#wrapper {
    margin: 0;
     }
#main {
    float: left;
    width: 640px;
    padding: 20px; 
    }
/* sidebar area */
#sidebar {
    float: left;
    width: 260px;
    padding: 20px;
    }
```
## Membuat Sidebar Widget
* Kemudian selanjutnya menambahkan element lain dalam sidebar.
```
<aside id="sidebar">
    <div class="widget-box">
    <h3 class="title">Widget Header</h3>
    <ul>
    <li><a href="#">Widget Link</a></li>
    <li><a href="#">Widget Link</a></li>
    <li><a href="#">Widget Link</a></li>
    <li><a href="#">Widget Link</a></li>
     <li><a href="#">Widget Link</a></li>
    </ul>
 </div>
    <div class="widget-box">
    <h3 class="title">Widget Text</h3>
    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt 
    arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer 
    pharetra est nunc, nec pretium nunc pretium ac.</p>
 </div>
</aside>
```
* Kemudian tambahkan CSS.
```
/* widget */
.widget-box {
    border:1px solid #eee;
    margin-bottom:20px;
    }
.widget-box .title {
    padding:10px 16px;
    background-color:#428bca;
    color:#fff; 
    }
.widget-box ul {
    list-style-type:none; 
    }
.widget-box li {
    border-bottom:1px solid #eee;
    }
```
* Selanjutnya Tambahkan 
```
}
.widget-box li a {
    padding:10px 16px;
    color:#333;
    display:block;
    text-decoration:none; 
    }
.widget-box li:hover a {
     background-color:#eee; 
     }
.widget-box p {
    padding:15px;
    line-height:25px; 
    }
```
* Maka Hasilnya 
![internal](img/layout5.png)

# Mengatur Footer
* Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer
```
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee; }
```

# Menambahkan Elemen lainnya pada Main Content
```
<section id="main">
    <div class="row">
    <div class="box">
    <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
class="image-circle">
    <h3>Heading</h3>
    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
    euismod.</p>
    <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
     <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
     class="image-circle">
 <h3>Heading</h3>
    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
    euismod.</p>
 <a href="#" class="btn btn-default">View detail</a>
 </div>
 <div class="box">
    <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
class="image-circle">
    <h3>Heading</h3>
    <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis 
    euismod.</p>
    <a href="#" class="btn btn-default">View detail</a>
 </div>
 </div>
</section>
```
* Kemudian Tambah CSS.
```
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
    padding:0 10px;
    text-align:center;
    }
.box h3 {
    margin: 15px 0; 
    }
.box p {
    line-height: 20px;
    font-size: 14px;
    margin-bottom: 15px; 
    }
box img {
     border: 0;
    vertical-align: middle; 
    }
.image-circle {
    border-radius: 50%; 
    }
.row {
     margin: 0 -10px;
    box-sizing: border-box;
    -moz-box-sizing: border-box;
    -webkit-box-sizing: border-box; 
    }
.row:after, .row:before,
.entry:after, .entry:before {
    content:'';
    display:table; 
    }
.row:after,
.entry:after {
    clear:both; 
    }
```
* Maka Hasilnya     
![internal](img/layout7.png)
# Menambahkan Content Artikel
Selanjutnya membuat content artikel. Tambahkan HTML berikut pada main content.
```
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
    elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
    pretium ac.</p>
</article>
<hr class="divider" />
<article class="entry">
    <h2>First featurette heading.</h2>
    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
class="right-img">
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem 
    elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, 
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc 
    pretium ac.</p>
</article>
```
* kemudian atur css nya.

```
.divider {
    border:0;
    border-top:1px solid #eeeeee;
    margin:40px 0; 
    }
/* entry */
.entry {
    margin: 15px 0;
     }
.entry h2 {
    margin-bottom: 20px;
    }
.entry p {
    line-height: 25px; }
.entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px; 
    }
.entry .right-img {
    float: right; 
    }
```
* Maka Hasil Akhir nya adalah
![internal](img/layout8.png)