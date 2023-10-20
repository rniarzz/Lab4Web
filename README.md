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
