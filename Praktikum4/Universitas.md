# MODUL 3 DASAR BASIS DATA


# ✍ Langkah Pengerjaan ✍

<b>1. Mengunduh data universitas yang telah disediakan dan salin di Dbeaver.</b>
<br> Setelah menyalin kode SQL, jalankan menggunakan <i>"Execute SQL Script"</i> di DBeaver.
<br>Silahkan buka data universitas dengan mengklik tautan berikut : [[Kode SQL]](./Universitas.sql)

   
![Gambar](./ss/1.png)
![Gambar](./ss/2.png)

<b>2. Menampilkan Nama Mahasiswa dan Nama Departemen</b>
<br>Untuk menampilkan dapat menggunakan perintah SQL dibawah:

    SELECT s.name AS Nama_Mahasiswa, d.dept_name AS Departemen
    FROM student s
    LEFT JOIN department d ON s.dept_name = d.dept_name;

![Gambar](./ss/3.png)

<b>2. Menampilkan Nama Student dengan Total SKS Lebih dari 100.</b>
<br>Untuk menampilkan dapat menggunakan perintah SQL dibawah:

    SELECT s.name AS Nama_Mahasiswa, d.dept_name AS Departemen
    FROM student s
    INNER JOIN department d ON s.dept_name = d.dept_name
    WHERE s.tot_cred > 100;
![Gambar](./ss/6.png)

    
<b>3. Menampilkan Nama Mahasiswa dan Nama Departemen.</b>
<br>Untuk menampilkan dapat menggunakan perintah SQL dibawah:

    SELECT s.name AS Nama_Mahasiswa, i.name AS Nama_Instructor, s.dept_name AS Departemen
    FROM student s
    INNER JOIN instructor i ON s.dept_name = i.dept_name;

![Gambar](./ss/9.png)