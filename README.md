# Praktikum 3: Membuat List, Table dan Form
# Mata Kuliah Pemrograman WEB
```
Nama  : Abdul Majid
NIM   : 311810693
Kelas : TI.19.C.1
Universitas Pelita Bangsa
```
## Persiapan
Buka VSCode dan Browser lalu buat file HTML baru dengan nama lab3_list.html

## 1. Membuat Ordered List
Buatlah dokumen HTML dan tambahkan Ordered List seperti berikut.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
    <section id="order-list">
        <h2>Ordered List</h2>
        <ol>
            <li>Pemrograman Web</li>
            <li>Sistem Informasi</li>
            <li>Basis Data 2</li>
        </ol>
    </section>
</body>
</html>
```
![1-Ordered-List](https://user-images.githubusercontent.com/81838946/114571355-cf352880-9ca0-11eb-9cb2-39ac056de464.PNG)

## 2. Membuat Unordered List
Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada section unordered-list, seperti berikut.
```html
    <section id="unorder-list">
        <h2>Unordered List</h2>
        <ul type="square">
            <li>Jaringan Komputer</li>
            <li>Struktur Data</li>
            <li>Algoritma &amp; Pemrograman</li>
        </ul>
    </section>
```
![2-Unordered-List](https://user-images.githubusercontent.com/81838946/114572207-7e71ff80-9ca1-11eb-8863-4469a1402fd3.PNG)

## 3. Membuat Description List
Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.
```html
    <section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industri</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntansi</dd>
            <dd>Manajemen</dd>
            <dd>Bisnis Digital</dd>
        </dl>
    </section>
 ```
![3-Description-List](https://user-images.githubusercontent.com/81838946/114573091-44edc400-9ca2-11eb-88dc-d65c2ab1800e.PNG)

 ## 4. Membuat Tabel
Buat file baru dengan nama lab3_tabel.html seperti berikut.
 ```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
</body>
</html>
 ```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```html
    <table border="1" cellpadding="4" cellspacing="0">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td>Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
```
![4-Tabel](https://user-images.githubusercontent.com/81838946/114574502-829f1c80-9ca3-11eb-8fd4-e89b57967e58.PNG)

## 5. Mengatur Margin dan Padding
Untuk mengatur margin dan padding pada cel data, tambahkan atribut cellpadding dan cellspacing pada tag table.
```html
<table border="1" cellpadding="4" cellspacing="0">
```
![5-Margin-Padding](https://user-images.githubusercontent.com/81838946/114575073-0953f980-9ca4-11eb-8999-87c00d733c8f.PNG)

## 6. Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara horizontal).
```html
    <table border="1" cellpadding="6" cellspacing="0">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td rowspan="3">Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
```
![6-Menggabungkan-Sel-data](https://user-images.githubusercontent.com/81838946/114575783-b6c70d00-9ca4-11eb-8677-ce08ed5a7510.PNG)

## 7. Membuat Form
Buat file baru dengan nama lab3_form.html seperti berikut.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
</body>
</html>
```
Kemudian selanjutnya tambahkan kode untuk membuat tabel sederhana seperti berikut:
```html
    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Pelanggan</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P" /><label for="jk_p">Perempuan</label>
            </p>
            <p><input type="submit" value="Login"></p>
        </fieldset>
    </form>
```
![7-Membuat-form](https://user-images.githubusercontent.com/81838946/114577367-24276d80-9ca6-11eb-977e-cd9412a5cbf9.PNG)

## 8. Menambahkan Style pada Form
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```html
    <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
```
![8-Menambahkan-Style](https://user-images.githubusercontent.com/81838946/114577925-a4e66980-9ca6-11eb-97da-08438d854e73.PNG)

## Jawab Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
```
Untuk menjawab pertanyaan tugas ini, saya membuat file tugas_form_no1.html yang berisi kode html sebagai berikut.
```
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
    <style>
        form p > label {
            display: inline-block;
            width: 100px;
        }
        form input[type="text"], form textarea {
            border: 1px solid #197a43;
        }
        form input[type="submit"] {
            border: 1px solid #197a43;
            background-color: #197a43;
            color: #ffffff;
            font-weight: bold;
            padding: 5px 15px;
        }
    </style>
</head>
<body>
    <header>
        <h1>Membuat Form (Dropdown & Listbox)</h1>
    </header>
    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Mahasiswa</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="kelas">Kelas</label>
                <input type="text" id="kelas" name="kelas">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label for="fakultas">Fakultas</label>
                <select name="fakultas">
                    <option value="teknik">Teknik</option>
                    <option value="ekonomi_dan_bisnis">Ekonomi dan Bisnis</option>
                </select>
            </p>
            <p>
                <label for="program-studi">Program Studi</label>
                <select name="program-studi" multiple="multiple" size="6">
                    <optgroup label="Teknik">
                        <option value="teknik-industri">Teknik Industri</option>
                        <option value="teknik-informatika">Teknik Informatika</option>
                        <option value="teknik-lingkungan">Teknik Lingkungan</option>
                    <optgroup label="Ekonomi dan Bisnis">
                        <option value="akuntansi">Akuntansi</option>
                        <option value="manajemen">Manajemen</option>
                        <option value="bisnis-digital">Bisnis Digital</option>
                </select>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L" /><label for="jk_l">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P" /><label for="jk_p">Perempuan</label>
            </p>
            <p><input type="submit" value="Simpan"></p>
        </fieldset>
    </form>
</body>
</html>
```
![jawabno1](https://user-images.githubusercontent.com/81838946/114584570-03aee180-9cad-11eb-8090-3721825e5ce2.PNG)
