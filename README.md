<p align="center">
	PEMROGRAMAN WEB
</p>
<p align="center">
	TUGAS PRATIKUM 2
</p>
<p align="center">
	Dosen Pengampu : Agung Nugroho, M.Kom
</p>
<p align="center"> 
	<b>Tugas untuk memenuhi syarat penilain pada Pert-3</b>
</p>

<p align="center">
	<img src="Logo/logo.png" alt="UPB" width="350" height="350">
</p>

<p align="center">
                 Nama  : Jose Fisto
</p>
<p align="center">
                 NIM   : 312010119
</p>
<p align="center">
                 Kelas : TI.20 A.1
</p>

<br/>
<br/>

<p align="center">
	<b>UNIVERSITAS PELITA BANGSA</b>
</p>
<p align="center">
	<b>FAKULTAS TEKNIK</b>
</p>
<p align="center">
	<b>TEKNIK INFORMATIKA</b>
</p>
<p align="center">
	<b>TA 2021 / 2022</b>
</p>

<br></br>

<hr>
</hr>

<br></br>

# Laporan Praktikum 2

## 1. Membuat File Dokumen HTML
Pertama buat file dokumen HTML dan save as dengan format nama ``lab2_css_dasar.html``, selanjutnya isi dengan koding sebagai contoh berikut :

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
	<link rel = "icon" href ="pic/logo.png" type = "image/x-icon">
</head>
<body>
    <!-- CSS ID Selector -->
    <div id="intro">
        <div id="iintro">
            <header>
                <h1>CSS Internal dan <i>Inline CSS</i></h1>
            </header>
                <h1>Hello World</h1>
            <p>
                 Kami sedang belajar HTML dan CSS dasar, pada mata kuliah <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>. Pelajaran pertama yang kami dapat adalah membuat tampilan web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.
            </p>
            <nav>
                <a href="lab2_css_dasar.html">CSS Dasar</a>
                <a href="lab2_css_dasar_eksternal.html">CSS Eksternal</a>
                <a href="Lab1Web/Lab1_tag_dasar.html">HTML Dasar</a>
             </nav>
             <!-- CSS Class Selector -->
             <a class="button btn-primary" href="#intro">Informasi selengkapnya</a>
        </div>
    </div>
</body>
</html>
```

Selanjutnya Run untuk tampilkan output 

<p align="center">
	<img src="SS/output_doc_html.png" alt="UPB">
</p>

## 2. Mengdeklarasikan 3 Jenis CSS

Setelahnya sematkan CSS, terdapat 3 jenis CSS digunakan dalam website sampai saat ini, yaitu CSS Internal, inline, dan Eksternal.

### ● Penerapan CSS Internal dalam Web
Pertama mengdeklarasikan css internal dalam dokumen html, berikut merupakan koding css internal yang akan disematkan dalam kerangka head

```html
<head>
	...
	...
	...
</head>
```
Selanjutnya sematkan koding css pada kerangka head sebagai contoh berikut

```html
<head>
    <title>CSS Dasar</title>   
    <style>       
        h1 {
        font-size: 24px;
        color: #7a6340;
        text-align: center;
        padding: 20px 10px;
        }
        h1 i {
        color:#966596;
        }
        p b {
            color:#829752;
        }
        p i {
            color:#4a5697;
        }

		header {
			min-height: 80px;
			border-bottom:1px solid #852c2c;
		}

        body{
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #000000;
        }
    </style>
</head>
```
Lakukan refresh pada halaman web sebelumnya untuk perubahan pada tampilan web

<p align="center">
	<img src="SS/output_css_internal.png" alt="UPB">
</p>

Pada pernyataan tag css internal di atas dapat di jelaskan :

#### ⏵ Style Selektor Tag h1 (header 1)
Pada ``<style>`` tag ``<h1>`` untuk mendeklarasikan elemen style h1 atau desain pada elemen header 1 di dalam kerangka ``<body>...</body>``

```html  
    <style>       
        h1 {
        font-size: 24px;
        color: #7a6340;
        text-align: center;
        padding: 20px 10px;
        }
        h1 i {
        color:#966596;
        }
    </style>
	....
	<body>
                <h1>CSS Internal dan <i>Inline CSS</i></h1>
	</body>
```
Pernyataan di atas dapat di nyatakan :

Elemen Header 1 di sematkan dengan desain properti css yaitu, fungsi :
- ``font-size`` (mengatur ukuran besar kecilnya font tersebut),
- ``color`` (mengubah warna dari tulisan),
- ``text-align``(mengatur posisi teks), dan
- ``padding``(mengatur jarak elemen HTML dari dalam).

#### ⏵ Style Selektor Tag p (paragraf)
Pada ``<style>`` tag ``<p>`` untuk mendeklarasikan elemen style atau desain pada elemen paragraf di dalam kerangka ``<body>...</body>``

```html  
    <style>       
        }
        p b {
            color:#829752;
        }
        p i {
            color:#4a5697;
        }
    </style>
	....
	<body>
                <h1>CSS Internal dan <i>Inline CSS</i></h1>
	</body>			
```
Pernyataan di atas dapat di nyatakan :

Elemen ``<p>`` bold ``<b>`` dan italic ``<i>`` di sematkan dengan desain properti css yaitu, fungsi :
- ``color`` (mengubah warna dari tulisan).

#### ⏵ Style Selektor Tag header
Pada ``<style>`` tag ``<header>...</header>`` untuk mendeklarasikan elemen style atau desain pada elemen header di dalam kerangka ``<body>...</body>``

```html
	<style>       
        header {
			min-height: 80px;
			border-bottom:1px solid #852c2c;
		}
    </style>
	...
	<body>
            <header>
                ...
            </header>
	</body>
```
Pernyataan di atas dapat di nyatakan :

Elemen ``<header>`` di sematkan dengan desain properti css yaitu, fungsi :
- ``<min-height>``(mengatur minimal tinggi dari sebuah obyek), dan
- ``<border-bottom>``(membuat style garis pinggir bagian bawah).

#### ⏵ Style Selektor Tag body
Pada ``<style>`` tag ``<body>...</body>`` untuk mendeklarasikan elemen style pada kerangka ``<body>...</body>``

```html
	<style>       
        body{
            min-height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: #000000;
        }
    </style>
	...
	<body>
		...
		...
		...
	</body>
```
Pernyataan di atas dapat di nyatakan :

Elemen ``<body>`` di sematkan dengan desain properti css yaitu, fungsi :
- ``<min-height>``, mengatur minimal tinggi dari sebuah obyek, 
- ``<display>``mengatur tampilan pada elemen,
- ``<align-items>``menyalurkan item-item pada container flex yang diletakkan sepanjang garis tegak lurus pada sumbu utama (cross-axis),
- ``<justify-content>``, mensejajarkan item-item diantara flexbox agar container dari flexbox tersebut bisa mendistribusikan ruang kosong yang tersisa ketika item flex dalam satu baris tersebut tidak flexsibel atau meskipun flexsibel tapi sudah mencapai batas ukuran maksimum, dan
- ``<background-color>``, memberikan warna pada latar belakang suatu elemen .