# Latihan4webII
# Praktikum 4: CSS Layout (Box Element & Layout Sederhana) - Pemrograman Web
Repository ini dibuat untuk menyelesaikan tugas Praktikum 4 Pemrograman Web.

## Identitas Mahasiswa

| Keterangan      | Data                 |
| --------------- | -------------------- |
| **Nama**        | Lia Mulyati          |
| **Kelas**       | I251D                |
| **NIM**         | 312510167            |
| **Mata Kuliah** | Pemrograman Web      |
### Tujuan Praktikum

Mahasiswa mampu memahami konsep box element pada CSS (float dan clearfix).

Mahasiswa mampu membuat layout website sederhana menggunakan semantic element HTML5.

Mahasiswa mampu mengatur navigasi, hero panel, main content, sidebar, dan footer menggunakan CSS.

Mahasiswa mampu membuat halaman tambahan (About dan Kontak) dengan layout yang konsisten.

---

## Struktur Folder Proyek

```
Praktikum4/
├── Lab4_Layout/
│   ├── Lab4_Layout.html
│   ├── about.html
│   ├── kontak.html
│   └── style.css
├── Lab4web/
│   └── Lab4_box.html
└── README.md
```

<!-- Ganti dengan screenshot struktur folder -->

<img width="98" height="139" alt="image" src="https://github.com/user-attachments/assets/321a9f6a-0537-488b-b6c3-b2accb142d31" />


---

## Langkah-langkah Praktikum

### 1. Membuat Box Element (`Lab4_box.html`)

Langkah pertama adalah menyiapkan dokumen HTML dasar dengan nama `Lab4_box.html` yang berisi `<header>` dengan judul "Box Element".

<img width="481" height="117" alt="image" src="https://github.com/user-attachments/assets/32245100-a34e-4ad7-8de4-614a90ae4ee5" />



Kemudian di dalam `<body>` ditambahkan `<section>` yang berisi empat buah `<div>` dengan class `div1` sampai `div4`.

<img width="270" height="147" alt="image" src="https://github.com/user-attachments/assets/50791291-b8b2-4fc2-b798-3f0a1f052340" />



#### CSS Float Property

Pada bagian `<head>` ditambahkan CSS internal untuk membuat float element:

- Semua `div` diberi `float: left` dan `padding: 10px`.
- `.div1` berwarna merah, `.div2` kuning, `.div3` hijau.
- `.div4` berwarna biru dengan `clear: left` dan `float: none` (clearfix) agar tampil di baris baru.

<img width="190" height="331" alt="image" src="https://github.com/user-attachments/assets/d9631057-84e1-4488-b034-9d18187da72a" />


Hasil di browser: Div1, Div2, dan Div3 tampil sejajar ke samping, sedangkan Div4 berada di bawahnya dengan lebar penuh.

<img width="204" height="99" alt="image" src="https://github.com/user-attachments/assets/a738cb3d-a55c-47c2-9d03-b61d8d68b589" />



---

### 2. Membuat Layout Sederhana (`Lab4_Layout.html`)

Membuat kerangka layout menggunakan semantic element. Dokumen ini menghubungkan file `style.css` dan memiliki `<div id="container">` sebagai pembungkus utama.

<img width="490" height="122" alt="image" src="https://github.com/user-attachments/assets/23a295f1-6085-4ebe-9dbd-4b8fce1e94f3" />



Di dalam container ditambahkan elemen `<header>`, `<nav>` (Home, Artikel, About, Kontak), `<section id="hero">`, `<section id="wrapper">` (berisi `<section id="main">` dan `<aside id="sidebar">`), serta `<footer>`.

<img width="227" height="74" alt="image" src="https://github.com/user-attachments/assets/04854b66-847e-43d6-bdb5-a30c53794291" />

<img width="326" height="250" alt="image" src="https://github.com/user-attachments/assets/b898300a-4683-4dd0-8653-43a032bb9522" />



Hasil sebelum diberi CSS:

<img width="151" height="84" alt="Screenshot 2026-10-15 113832" src="https://github.com/user-attachments/assets/babdc9d2-69dc-470d-9231-45d63fefc382" />



---

### 3. Menambahkan CSS Layout (`style.css`)

CSS ditambahkan untuk membuat tampilan dasar layout, meliputi:

- `@import` Google Font **Open Sans** dan **Open Sans Condensed**.
- Reset CSS (`margin: 0; padding: 0`).
- Pengaturan `body` (font-size, font-family, warna teks).
- `#container` dengan lebar `980px`, rata tengah (`margin: 0 auto`), dan `box-shadow`.
- Pengaturan `header` dan `header h1`.

<img width="850" height="273" alt="image" src="https://github.com/user-attachments/assets/e0b0a241-b8a0-40e6-b39f-c202cc6fb65d" />



Hasil di browser:

<img width="186" height="79" alt="Screenshot 2026-10-15 121827" src="https://github.com/user-attachments/assets/42db1ac2-e177-476c-9eb4-779da3583a4b" />


---

### 4. Mengatur Navigasi

CSS navigasi dibuat dengan ketentuan:

- `nav` memiliki background biru (`#1f5faa`).
- Link `nav a` ditampilkan `inline-block`, berwarna putih, tebal, tanpa garis bawah.
- `nav a.active` dan `nav a:hover` memiliki background `#2b83ea`.

<img width="233" height="278" alt="image" src="https://github.com/user-attachments/assets/a82d3517-d157-4ceb-8e44-5313a8ba7cc9" />



<img width="959" height="109" alt="Screenshot 2026-10-15 122640" src="https://github.com/user-attachments/assets/24ad64e3-c924-4cab-b874-912f20a681ae" />


---

### 5. Membuat Hero Panel

Menambahkan kode HTML pada `<section id="hero">` berisi judul, paragraf, dan tombol "Learn more", lalu diberi style: background abu-abu (`#e4e4e5`), padding, serta pengaturan ukuran font `h1` dan `p`.

<img width="486" height="153" alt="image" src="https://github.com/user-attachments/assets/09dd1c61-fe86-4c57-9a35-ce6a7bbc28e0" />

<img width="214" height="253" alt="image" src="https://github.com/user-attachments/assets/34397c5d-11ad-414b-bf65-af13c8ee03b5" />



<img width="440" height="191" alt="image" src="https://github.com/user-attachments/assets/11eb068e-96db-4f53-bd3b-33dbfebaaf89" />



---

### 6. Menambahkan CSS Float untuk Main Content dan Sidebar

- `#main` dan `#sidebar` menggunakan `float: left`.
- Lebar `#main` = `640px`, lebar `#sidebar` = `260px`, keduanya dengan `padding: 20px`.
- Sidebar berisi dua `widget-box` (daftar link dan teks) yang diberi style border, title berwarna biru (`#428bca`), list tanpa bullet, dan efek hover.

<img width="556" height="257" alt="image" src="https://github.com/user-attachments/assets/ec8b71a0-3909-4d1e-add3-3bd4ef90e0a2" />



<img width="140" height="98" alt="image" src="https://github.com/user-attachments/assets/f9c44319-292d-4b2e-96a2-388893a31c2e" />


<img width="222" height="413" alt="image" src="https://github.com/user-attachments/assets/18e297c2-71ea-4a63-9c01-4c999b977d18" />

<img width="542" height="437" alt="Screenshot 2026-10-15 131902" src="https://github.com/user-attachments/assets/378b751f-6a7c-4ea6-a03e-58921d2debb4" />




---

### 7. Mengubah Tampilan Footer

Footer diberi style background gelap dengan teks putih agar terlihat berbeda dari konten utama.

<img width="319" height="41" alt="image" src="https://github.com/user-attachments/assets/19184954-817f-4ecf-8b42-269c36462afa" />


---

### 8. Menambahkan Elemen Lain pada Main Content

Menambahkan `div.row` yang berisi tiga `div.box`. Masing-masing box memiliki gambar, heading, paragraf, dan tombol "View detail". CSS yang digunakan:

- `.box` dengan `float: left`, `width: 33.333333%`, `box-sizing: border-box`, dan `text-align: center`.
- `.image-circle` dengan `border-radius: 50%` agar gambar berbentuk lingkaran.
- `.row` dengan margin negatif dan clearfix (`:before` dan `:after` dengan `display: table` dan `clear: both`).

<img width="595" height="289" alt="image" src="https://github.com/user-attachments/assets/8fc72df8-70b0-4432-b142-f443742e418a" />

<img width="214" height="371" alt="image" src="https://github.com/user-attachments/assets/d6f85bc4-29cc-40e5-b82a-7c1caa5f0cdf" />

<img width="219" height="317" alt="image" src="https://github.com/user-attachments/assets/b4c86e40-cdaf-4031-bf01-39077f13ae87" />

<img width="496" height="390" alt="Screenshot 2026-10-15 140851" src="https://github.com/user-attachments/assets/53eda04b-9f5d-4f28-aae2-15f5d9d1321c" />



---

### 9. Membuat Content Artikel

Menambahkan dua `<article class="entry">` yang dipisah dengan `<hr class="divider">`. Artikel pertama memiliki gambar di kiri, sedangkan artikel kedua memakai class `right-img` sehingga gambar berada di kanan.

CSS `.entry`:
- `margin: 15px 0`, `h2` dengan `margin-bottom: 20px`, dan `p` dengan `line-height: 25px`.
- `.entry img` menggunakan `float: left`, `border-radius: 5px`, dan `margin-right: 15px`.
- `.entry .right-img` menggunakan `float: right` dengan margin kiri `15px`.

<img width="793" height="218" alt="image" src="https://github.com/user-attachments/assets/409bb8c1-c207-40ef-a095-05878fd5f2c3" />



<img width="134" height="268" alt="image" src="https://github.com/user-attachments/assets/e642deb3-5b1e-4839-ab89-fb6c22058206" />


<img width="675" height="493" alt="image" src="https://github.com/user-attachments/assets/c949edd2-fd7c-4cd3-8bc3-acad7040cc72" />

---

## Pertanyaan dan Tugas

### 1. Menambahkan Menu About (`about.html`)

Membuat halaman About dengan layout yang sama (header, nav, hero, main, footer). Halaman ini berisi bagian **Tentang Saya** (hero), **Deskripsi Diri**, dan **Portfolio** (Website Layout Sederhana, Desain UI/UX, dan Project Pemrograman). Menu "About" diberi `class="active"`.

<img width="474" height="413" alt="image" src="https://github.com/user-attachments/assets/e2063a09-d3c2-4d47-b3a0-c3ddaab8597c" />
<img width="277" height="356" alt="image" src="https://github.com/user-attachments/assets/3c115075-2519-4fa8-b9d7-c7505730bfa3" />
<img width="308" height="316" alt="image" src="https://github.com/user-attachments/assets/1fd445e1-b4d8-4339-aa5e-7b2ad197b0f1" />
<img width="511" height="387" alt="image" src="https://github.com/user-attachments/assets/0be50a75-17de-4c60-a817-af739d6ea359" />
<img width="493" height="356" alt="image" src="https://github.com/user-attachments/assets/ae438a9d-3915-49bc-b45b-01b7b96c8e8e" />
<img width="354" height="242" alt="image" src="https://github.com/user-attachments/assets/5b1b7a43-668f-4fd2-9636-c5aa81c9d03c" />



hasilnya.
<img width="821" height="434" alt="image" src="https://github.com/user-attachments/assets/8ac9a363-4645-4ff2-aa16-60fe672904ea" />






### 2. Menambahkan Menu Kontak (`kontak.html`)

Membuat halaman Kontak yang berisi **Form Contact** dengan field Nama Lengkap, Email, Subjek, dan Pesan (textarea), serta tombol "Kirim Pesan". Semua field menggunakan atribut `required`, dan menu "Kontak" diberi `class="active"`.

<img width="469" height="391" alt="image" src="https://github.com/user-attachments/assets/65079961-1192-4987-a476-df1e78217425" />
<img width="260" height="337" alt="image" src="https://github.com/user-attachments/assets/2e5cdc39-69da-4676-b9e0-a05556dd6254" />
<img width="277" height="323" alt="image" src="https://github.com/user-attachments/assets/78c68c88-4e09-47e9-9ca7-a61b1aa590ba" />
<img width="338" height="374" alt="image" src="https://github.com/user-attachments/assets/c397a185-d4a9-4400-a10e-ac2d6ee08361" />
<img width="668" height="331" alt="image" src="https://github.com/user-attachments/assets/5358abe3-ca95-46ab-8e80-92c13b140caa" />
<img width="371" height="92" alt="image" src="https://github.com/user-attachments/assets/4bde679b-9176-4acb-9ec7-a718ea0f960f" />

hasilnya.
<img width="676" height="414" alt="image" src="https://github.com/user-attachments/assets/b09dd713-4481-435c-a584-21b3a4cc61a8" />



---

## Kesimpulan

Pada praktikum ini telah dipelajari cara membuat layout website dengan CSS menggunakan properti `float` dan `clear`, penggunaan semantic element HTML5, serta pembuatan komponen seperti navigasi, hero panel, sidebar widget, box, dan artikel. Selain itu juga dibuat halaman About dan Kontak dengan layout yang konsisten.
