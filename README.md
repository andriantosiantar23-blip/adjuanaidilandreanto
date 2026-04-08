<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Lilium Medica Library</title>

<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<style>
body{
  background: linear-gradient(rgba(255,255,255,0.9), rgba(255,255,255,0.9)),
  url('https://images.unsplash.com/photo-1586773860418-d37222d8fce3');
  background-size: cover;
  background-attachment: fixed;
}
.reply{ color: green; margin-left: 15px; }
</style>
</head>

<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark bg-primary">
  <div class="container">
    <a class="navbar-brand" href="#">Lilium Medica</a>
    <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#menu">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="menu">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link" href="#home">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#koleksi">Koleksi</a></li>
        <li class="nav-item"><a class="nav-link" href="#layanan">Layanan</a></li>
        <li class="nav-item"><a class="nav-link" href="#login">Login</a></li>
        <li class="nav-item"><a class="nav-link" href="#event">Event</a></li>
        <li class="nav-item"><a class="nav-link" href="#ulasan">Ulasan</a></li>
        <li class="nav-item"><a class="nav-link" href="#kontak">Kontak</a></li>
      </ul>
    </div>
  </div>
</nav>

<!-- Hero -->
<section id="home" class="text-center py-5 bg-light">
  <div class="container">
    <h2>Selamat Datang di Lilium Medica Library</h2>
    <p>Pusat informasi kesehatan untuk tenaga medis dan mahasiswa</p>
  </div>
</section>

<!-- Koleksi -->
<section id="koleksi" class="py-5">
<div class="container">
<h2 class="text-center mb-4">Koleksi</h2>
<div class="row g-4">

<div class="col-md-4">
<div class="card shadow">
<div class="card-body">
<h5>Buku Kedokteran</h5>
<p>Koleksi berbagai spesialisasi medis</p>
</div>
</div>
</div>

<div class="col-md-4">
<div class="card shadow">
<div class="card-body">
<h5>Jurnal Medis</h5>
<p>Akses jurnal nasional & internasional</p>
</div>
</div>
</div>

<div class="col-md-4">
<div class="card shadow">
<div class="card-body">
<h5>E-Book</h5>
<p>Koleksi digital kesehatan</p>
</div>
</div>
</div>

</div>
</div>
</section>

<!-- Layanan -->
<section id="layanan" class="bg-light py-5">
<div class="container">
<h2 class="text-center">Layanan</h2>
<ul class="list-group mt-3">
<li class="list-group-item">Peminjaman Buku</li>
<li class="list-group-item">Literature Search</li>
<li class="list-group-item">Pelatihan Literasi Informasi</li>
<li class="list-group-item">Bantuan Sitasi</li>
</ul>
</div>
</section>

<!-- Login -->
<section id="login" class="py-5">
<div class="container text-center">
<h2>Login Pustakawan</h2>
<input class="form-control w-50 mx-auto mt-3" type="text" id="username" placeholder="Username">
<input class="form-control w-50 mx-auto mt-3" type="password" id="password" placeholder="Password">
<button class="btn btn-primary mt-3" onclick="login()">Login</button>
<p id="status" class="mt-2"></p>
</div>
</section>

<!-- Event -->
<section id="event" class="py-5">
<div class="container">
<h2 class="text-center mb-4">Event Perpustakaan</h2>
<div class="row g-4">

<div class="col-md-6">
<div class="card shadow h-100">
<div class="card-body">
<h5>Smart Health Literacy</h5>
<p><b>Waktu:</b> Setiap Rabu, 10.00 – 11.30 WIB</p>
<p><b>Lokasi:</b> Ruang Edukasi</p>
<p>Edukasi memahami informasi kesehatan dan membedakan hoaks.</p>
</div>
</div>
</div>

<div class="col-md-6">
<div class="card shadow h-100">
<div class="card-body">
<h5>Happy Story Time</h5>
<p><b>Waktu:</b> Jumat, 09.00 – 10.00 WIB</p>
<p><b>Lokasi:</b> Ruang Anak</p>
<p>Storytelling untuk meningkatkan semangat pasien anak.</p>
</div>
</div>
</div>

<div class="col-md-6">
<div class="card shadow h-100">
<div class="card-body">
<h5>Workshop Evidence-Based Practice</h5>
<p><b>Waktu:</b> 1x setiap bulan</p>
<p><b>Lokasi:</b> Ruang Seminar</p>
<p>Pelatihan literasi informasi untuk tenaga medis.</p>
</div>
</div>
</div>

<div class="col-md-6">
<div class="card shadow h-100">
<div class="card-body">
<h5>Creative Healing Corner</h5>
<p><b>Waktu:</b> Setiap hari</p>
<p><b>Lokasi:</b> Area Kreativitas</p>
<p>Kegiatan seni untuk mendukung proses penyembuhan pasien.</p>
</div>
</div>
</div>

<div class="col-12">
<div class="card shadow">
<div class="card-body">
<h5>Health Literacy Day</h5>
<p><b>Waktu:</b> 3 bulan sekali</p>
<p><b>Lokasi:</b> Aula RS</p>
<p>Talkshow, pameran buku, dan kuis kesehatan.</p>
</div>
</div>
</div>

</div>
</div>
</section>

<!-- Ulasan -->
<section id="ulasan" class="bg-light py-5">
<div class="container">
<h2 class="text-center">Ulasan</h2>

<input class="form-control mt-3" type="text" id="nama" placeholder="Nama">
<textarea class="form-control mt-2" id="komentar" placeholder="Tulis ulasan"></textarea>
<button class="btn btn-success mt-2" onclick="kirimUlasan()">Kirim</button>

<div id="daftarUlasan" class="mt-3"></div>
</div>
</section>

<!-- Kontak -->
<section id="kontak" class="py-5 text-center">
<div class="container">
<h2>Kontak</h2>
<p>082172919084</p>
<p>liliummedicalibrary@gmail.com</p>
</div>
</section>

<!-- Footer -->
<footer class="bg-dark text-white text-center p-3">
<p>© 2026 Lilium Medica Library</p>
</footer>

<!-- Bootstrap JS -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

<script>
let adminLogin=false;

function login(){
let user=document.getElementById("username").value;
let pass=document.getElementById("password").value;

if(user=="admin" && pass=="library"){
adminLogin=true;
document.getElementById("status").innerHTML="Login berhasil";
}else{
document.getElementById("status").innerHTML="Login gagal";
}
}

function kirimUlasan(){
let nama=document.getElementById("nama").value;
let komentar=document.getElementById("komentar").value;

let div=document.createElement("div");
div.className="card p-3 mt-2";
div.innerHTML="<b>"+nama+"</b><p>"+komentar+"</p>";

if(adminLogin){
let btn=document.createElement("button");
btn.className="btn btn-sm btn-primary";
btn.innerText="Balas";

btn.onclick=function(){
let balasan=prompt("Balas:");
let p=document.createElement("p");
p.className="reply";
p.innerHTML="<b>Pustakawan:</b> "+balasan;
div.appendChild(p);
}

div.appendChild(btn);
}

document.getElementById("daftarUlasan").appendChild(div);
}
</script>

</body>
</html>
