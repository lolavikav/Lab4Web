# Lab4Web
## Membuat Layout Sederhana
## Membuat Box elemen
Kode ini menampilkan empat kotak berwarna untuk menunjukkan cara kerja box element dan properti float. Tiga kotak pertama diatur dengan `float: left;` sehingga tampil sejajar ke kiri, sedangkan kotak keempat menggunakan `clear: left;` agar turun ke bawah dan tidak sejajar dengan yang lain. Contoh ini menjelaskan bagaimana elemen HTML dapat diatur posisinya menggunakan float dan clear dalam membuat layout sederhana.
```html
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
</html>
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
    .div4 {
background-color: blue;
clear: left;
float: none;
}
</style>

<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
     <div class="div4">Div 4</div>
</section>
```
<img width="660" height="300" alt="Screenshot 2025-10-16 134751" src="https://github.com/user-attachments/assets/5458bac1-dde9-4d2b-9d25-054028883ded" />

## Membuat Layout Sederhana

Kode ini membentuk struktur halaman web dengan layout sederhana menggunakan elemen semantik HTML5. Bagian `<header>` menampilkan judul halaman, sedangkan `<nav>` berisi menu navigasi agar pengguna bisa berpindah antarhalaman seperti Home, Artikel, About, dan Kontak. Bagian `<section id="hero">` digunakan sebagai tampilan pembuka atau banner utama yang berisi teks dan tombol. Selanjutnya, area utama halaman dibungkus dalam `<section id="wrapper">` yang terdiri dari <main> untuk konten utama berisi kotak dan artikel, serta `<aside>` sebagai sidebar yang menampilkan widget link dan teks tambahan. Di bagian bawah, `<footer>` menampilkan informasi hak cipta. Semua elemen dibungkus dalam `<div id="container">` agar tata letaknya mudah diatur menggunakan CSS.
```html
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
        <header>
            <h1>Layout Sederhana</h1>
        </header>

        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>

        <section id="hero">
            <h1>Hello World!</h1>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis.</p>
            <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
        </section>

        <section id="wrapper">
            <section id="main">
                <div class="row">
                    <div class="box">
                        <img src="https://dummyimage.com/120/db7d25/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/3e73e6/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                    <div class="box">
                        <img src="https://dummyimage.com/120/71e6d4/fff.png" alt="" class="image-circle">
                        <h3>Heading</h3>
                        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
                        <a href="#" class="btn btn-default">View detail</a>
                    </div>
                </div>

                <hr class="divider">

                <article class="entry">
                    <h2>First featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla.</p>
                </article>

                <hr class="divider">

                <article class="entry">
                    <h2>Second featurette heading.</h2>
                    <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="" class="right-img">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu.</p>
                </article>
            </section>

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
                    <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla.</p>
                </div>
            </aside>
        </section>

        <footer>
            <p>&copy; 2021 - Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

## CSS Style
Kode CSS ini mengatur tampilan layout web agar terlihat rapi dan terstruktur. Font Open Sans diimpor dari Google Fonts, dan reset CSS digunakan untuk menghapus margin serta padding bawaan. Bagian `header` dan `nav` mengatur tampilan judul serta menu navigasi dengan warna biru dan efek hover. Elemen `#hero` digunakan sebagai banner utama dengan teks besar dan latar abu muda. Bagian `#main` dan `#sidebar` diatur sejajar menggunakan float untuk membentuk dua kolom. Widget di sidebar diberi border, warna biru pada judul, serta efek saat tautan diarahkan. Footer diberi latar hitam dan teks abu terang di bagian bawah halaman. Kelas `.box` membuat tiga kolom konten sejajar dengan gambar lingkaran, sedangkan `.entry` mengatur artikel agar rapi dengan garis pemisah di antaranya.
```
/* import google font */
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');
/* Reset CSS */
* {
    margin: 0;
    padding: 0;
}
body {
    line-height:1;
    font-size:100%;
    font-family:'Open Sans', sans-serif;
    color:#5a5a5a;
}
#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}
/* header */
header {
    padding: 20px;
}
header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
/* navigasi */
nav {
display: block;
background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}

/* Hero Panel */
#hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
}
#hero p {
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}

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

/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
/* box */
.box {
    display:block;
    float:left;
    width:33.333333%;
    box-sizing:border-box;
    -moz-box-sizing:border-box;
    -webkit-box-sizing:border-box;
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
    line-height: 25px; 
} 

.entry img { 
    float: left; 
    border-radius: 5px; 
    margin-right: 15px; 
} 

.entry .right-img { 
    float: right; 
}
```
<img width="680" height="462" alt="image" src="https://github.com/user-attachments/assets/d66f8fb8-058a-4745-8b00-400d73d11edc" />

<img width="717" height="503" alt="image" src="https://github.com/user-attachments/assets/1d74459a-40c6-4b2f-8623-1f0e2b35fee8" />




