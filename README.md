<h1 <p align="center"><b>Praktikum 4</b></p></h1> 

**Nama: Rini Ariza**

**NIM: 312210337**

**Kelas: TI.22.A3**

---

## Membuat Dokumen HTML
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.

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
```

## Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.

```html
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
</section>
```

## CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.

```html
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

Kemudian buka browser untuk melihat hasilnya.

![Screenshot (309)](https://github.com/rniarzz/Lab4Web/assets/115542704/e374234a-745b-4442-9795-a10d2bdc9b23)

## Mengatur Clearfix Element
**Clearfix** digunakan untuk mengatur element setelah float element. Property clear digunakan untuk
mengaturnya.

Tambahkan element div lainnya seteleah div3 seperti berikut.

```html
<section>
    <div class="div1">Div 1</div>
    <div class="div2">Div 2</div>
    <div class="div3">Div 3</div>
    <div class="div4">Div 4</div>
</section>
```
Kemudian atur property clear pada CSS, seperti berikut.

```html
.div4 {
    background-color: blue;
    clear: left;
    float: none;
}
```
Selanjutnya buka browser dan refresh kembali.

![Screenshot (310)](https://github.com/rniarzz/Lab4Web/assets/115542704/1d634f65-7eda-44bd-9fdf-c4022d95fe4f)

## Membuat Layout Sederhana
Kita akan membuat layout web sederhana seperti gambar berikut.

![Screenshot (319)](https://github.com/rniarzz/Lab4Web/assets/115542704/a82ce2fa-2609-4679-93e2-a49970d7f3d9)
![Screenshot (320)](https://github.com/rniarzz/Lab4Web/assets/115542704/7cc4430c-ee3f-49e0-b11f-ef1c3f8c8de9)

Kemudian tulis kode berikut.

```html
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

Kemudian buka browser dan lihat hasilnya.

![Screenshot (311)](https://github.com/rniarzz/Lab4Web/assets/115542704/fdf7b542-bb89-4620-916b-d3047a00dd7c)

Kemudian tambahkan kode CSS untuk membuat layoutnya.

```html
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
Kemudian lihat hasilnya pada browser.

![Screenshot (313)](https://github.com/rniarzz/Lab4Web/assets/115542704/eb5e6c84-5e87-495a-9b93-a04626967f05)

## Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.

```html
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
Kemudian lihat hasilnya.

![Screenshot (314)](https://github.com/rniarzz/Lab4Web/assets/115542704/5da97a5f-d0f5-45d2-81e7-f787c427219e)

## Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.

```html
<section id="hero">
    <h1>Hello World!</h1>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
pretium ac.</p>
    <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
</section>
```
```html/* Hero Panel */
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

 ![Screenshot (315)](https://github.com/rniarzz/Lab4Web/assets/115542704/e7e05ae1-8f64-49dc-b62d-188ce72e036a)

## Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.

```html
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
Kemudian selanjutnya menambahkan element lain dalam sidebar.

```html
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
Kemudian tambahkan CSS.

```html
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

![Screenshot (316)](https://github.com/rniarzz/Lab4Web/assets/115542704/9f447bdd-d8c9-4831-a43d-328c1536bd75)

```html
/* footer */
footer {
    clear:both;
    background-color:#1d1d1d;
    padding:20px;
    color:#eee;
}
```

![Screenshot (318)](https://github.com/rniarzz/Lab4Web/assets/115542704/72215e3f-e4b3-4b87-981c-13a4992bab0e)

## Modul Praktikum Pemrograman Web

