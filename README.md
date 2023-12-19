# JS1-Hello-World-Muhamad-Fathur-Rahman

1. Import Modul HTTP:
   const http = require('http');

   Mengimpor modul http dari Node.js, yang memungkinkan Anda membuat server HTTP.

2. Atur Hostname dan Port:
   const hostname = '127.0.0.1';
   const port = 3000;

   Menetapkan nilai hostname ke '127.0.0.1' (localhost) dan port ke 3000.

3. Buat Server HTTP, dan Atur Respon Server::
   const server = http.createServer((req, res) => {
    res.statusCode = 200;
    res.setHeader('Content-Type', 'text/plain');
    res.end('Hello World Gue Patot');
   });

   Membuat server HTTP dengan menggunakan fungsi createServer dari modul http. Fungsi ini menerima callback yang akan dipanggil setiap kali ada permintaan HTTP.
   Di dalam callback server, Anda mengatur status code respon menjadi 200 (OK), mengatur header konten menjadi 'text/plain', dan mengirimkan pesan 'Hello World Gue Patot' sebagai
   isi respon.

5. Mulai Mendengarkan Server:
   server.listen(port, hostname, () => {
    console.log(`Server running at http://${hostname}:${port}/`);
   });

6. Cek Output:
   Buka browser dan akses http://127.0.0.1:3000/. Anda seharusnya melihat pesan "Hello World Gue Patot" sebagai respon dari server Anda.

   Memulai server untuk mendengarkan permintaan pada hostname dan port yang telah ditentukan sebelumnya. Ketika server siap mendengarkan, fungsi callback dijalankan, dan
   pesan log dicetak ke konsol.

8. Menjalankan Aplikasi:
   Setelah menulis semua kode di atas, Kita dapat menjalankan aplikasi melalui terminal dengan perintah:
   node hello-world.js
