# Praktikum 4 - Pemrograman Web
```
Maulana hasanudin
312010106
TI.20.D.1
Universitas Pelita Bangsa
```
# LANGKAH 1
## Membuat dokumen HTML dengan nama file lab4_box.html. Setelah itu buat struktur dasar HTML
~~~
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
~~~
<img width="1070" alt="1" src="https://user-images.githubusercontent.com/101716660/162386087-5b414734-be42-42f5-9cd2-772b36e89a31.png">


# LANGKAH 2
## Membuat box element dengan tag div
```
<section>
  <div class="div1">Div 1</div>
  <div class="div2">Div 2</div>
  <div class="div3">Div 3</div>
</section>
```
<img width="1070" alt="2" src="https://user-images.githubusercontent.com/101716660/162386182-6c94b4cc-7659-41d3-84de-e346090af371.png">

# LANGKAH 3
## Tambahkan deklarasi CSS pada head untuk membuat float element
~~~
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
~~~
<img width="1070" alt="3" src="https://user-images.githubusercontent.com/101716660/162386429-28d3364b-fc3f-4226-94a3-0c82d4c178a2.png">

# LANGKAH 4
## Mengatur Clearfix Element. Clearfix digunakan untuk mengatur element setelah float element
### Tambahkan element div lainnya seteleah div3
```
<section>
  <div class="div1">Div 1</div>
  <div class="div2">Div 2</div>
  <div class="div3">Div 3</div>
  <div class="div4">Div 4</div>
</section>
```
## Kemudian atur property clear pada CSS
```
.div4 {
  background-color: blue;
  clear: left;
  float: none;
}
```
<img width="1070" alt="4" src="https://user-images.githubusercontent.com/101716660/162387004-4d8f94b6-7537-4a83-abf1-b0ee0bed5169.png">

# Membuat Layout Sederhana
## LANGKAH 1
### Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama home.html, dan file css dengan nama style.css. folder layout sederhana

### Kemudian coding home.html
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
    </div>
</body>
</html>
```
### dan coding pada style.css
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
```
<img width="1070" alt="5" src="https://user-images.githubusercontent.com/101716660/162387978-13c96434-b1bd-4966-9555-fd265f8ef1a2.png">

# LANGKAH 2
## Mengatur Navigasi pada CSS
```
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
```
<img width="1070" alt="6" src="https://user-images.githubusercontent.com/101716660/162388340-8fd12125-c5f2-4bda-9eea-912544f3f06e.png">


# LANGKAH 2
## Membuat Hero Panel
### Tambahkan Coding pada home.html
```
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
Tambahkan Coding pada style.css
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
```
<img width="1070" alt="7" src="https://user-images.githubusercontent.com/101716660/162388613-078273b7-c80d-46bc-bd4b-ecfee39fab1e.png">

# LANGKAH 3
## Mengatur Layout Main dan Sidebar
### Tambahkan coding pada style.css

```/* main content */
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
<img width="1070" alt="8" src="https://user-images.githubusercontent.com/101716660/162388956-98c26de1-c4c6-42dd-96ac-aeefde9a0faf.png">

# LANGKAH 4
## Membuat Sidebar Widget
### Tambahkan Coding pada home.html
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
### Tambahkan Coding pada style.css
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
<img width="1070" alt="9" src="https://user-images.githubusercontent.com/101716660/162389184-15195d3a-36aa-4aba-a155-eb1a6c479b72.png">

<img width="1070" alt="hasil 9" src="https://user-images.githubusercontent.com/101716660/162389238-928939ab-f4c2-4508-8e7f-10a92cbeff72.png">

# LANGKAH 5
## Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer
```
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```
<img width="1070" alt="10" src="https://user-images.githubusercontent.com/101716660/162389359-3c9745fa-85fb-44ab-8836-d85ddb543c2c.png">


# LANGKAH 6
## Menambahkan Elemen lainnya pada Main Content
### Tambahkan Coding pada home.html
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
### Tambahkan Coding pada style.css
~~~
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
~~~
<img width="1070" alt="11" src="https://user-images.githubusercontent.com/101716660/162389516-8da330b4-447c-4089-b27b-6c2eaf4110ba.png">

<img width="1070" alt="11 hasil" src="https://user-images.githubusercontent.com/101716660/162389554-cbf54ee2-63fa-4e20-80e0-5da4403cae1c.png">

# LANGKAH 7
## Selanjutnya membuat content artikel
### Tambahkan Coding pada home.html
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
### Tambahkan Coding pada style.css
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
<img width="1070" alt="12" src="https://user-images.githubusercontent.com/101716660/162389730-f08ab14b-cce1-4bae-b697-a9b12ce241bb.png">

<img width="1070" alt="hasi 12" src="https://user-images.githubusercontent.com/101716660/162389763-244c581f-2a08-4814-bcae-7a3681ef93f8.png">

# TUGAS
## 1. Tambahkan Layout untuk menu About
## Buat file HTML baru dengan nama about.html, dan buat single layout yang berisi deskripsi, portfolio, dll
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About Me</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>About Me</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="about">
            <div class="row">
                <img src="Maulana.png" title="Maulana hasanudin" alt="Maulana hasanudin" class="image-circle" width="200" style="float: left; border: 2px solid black;">
                <h1>Maulana hasanudin</h1>
                <p>Nama saya Maulana hasanudin, Saya adalah seorang mahasiswa Universitas Pelita Bangsa Jurusan Teknik Informatika. Saya lahir di bekasi, 26 juni 1999, hobbi saya bermain futsal dan mendaki gunung.
                </p>
            </div>
        </section>
    </div>
</body>
</html>
```
### Tambahkan Coding pada style.css
```
/* About Panel */
#about{
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#about h1 {
    margin-bottom: 10px;
    font-size: 35px;
    position: relative;
    left: 15px;
}
#about p {
    margin-bottom: 20px;
    font-size: 18px;
    padding: 30px;
    line-height: 25px;
    position: relative;
    left: 15px;
}
```
<img width="1070" alt="ss tugas 1" src="https://user-images.githubusercontent.com/101716660/162390228-5380f787-7c7a-41be-ad74-5f9d173ddd3e.png">

<img width="1070" alt="hasil ss tugas 1" src="https://user-images.githubusercontent.com/101716660/162390267-b7ed8a69-c727-475f-9b8d-bbd0cc20e6d5.png">

# 2. Tambahkan layout untuk menu Contact
## Buat file HTML baru dengan nama kontak.html, dan buat form yang berisi: nama, email, message, dll
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
        <header>
            <h1>Contact Me</h1>
        </header>
        <nav>
            <a href="home.html" class="active">Home</a>
            <a href="artikel.html">Artikel</a>
            <a href="about.html">About</a>
            <a href="kontak.html">Kontak</a>
        </nav>
        <section id="kontak">
            <div class="login">
                <input type="text" placeholder="Your Name" class="input">
                <input type="text" placeholder="Your Email Address" class="input">
            </div>

            <div class="subject">
                <input type="text" placeholder="Subject" class="input">
            </div>

            <div class="msg">
                <textarea cols="35" rows="10" class="area" placeholder="Your Message" class="input"></textarea>
            </div>

            <button type="submit"> Send </button>

        </section>
    </div>
</body>
</html>
```
### Tambahkan Coding pada style.css
```
/* Kontak Panel */
#kontak{
    background-color: #e4e4e5;
    padding: 20px 20px;
    margin-bottom: 20px;
}
.input,
.msg, .area{
    width: 100%;
    padding: 10px;
    border: 2px solid white;
    box-sizing: border-box;
    font-size: 15px;
    margin-bottom: 20px;
}
button{
    font-size: 14px;
    background-color: #3f3f3f;
    color: white;
    border-radius: 5px;
    padding: 10px 20px;
    margin-top: 8x;
}
button :hover{
    opacity: 0,9;
}
```
<img width="1070" alt="ss tugas 2" src="https://user-images.githubusercontent.com/101716660/162390433-fae1ef96-d883-41f9-bd5a-274853fad4cf.png">

<img width="1070" alt="hasil ss tugas 2" src="https://user-images.githubusercontent.com/101716660/162390472-98d1a6e5-c6ca-4393-9c1d-fb555b03deff.png">
