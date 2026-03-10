<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Lilium Medica Library</title>

<style>

body{
font-family:Arial;
margin:0;

background-image: linear-gradient(
rgba(255,255,255,0.85),
rgba(255,255,255,0.85)
),
url("https://images.unsplash.com/photo-1586773860418-d37222d8fce3");

background-size:cover;
background-position:center;
background-attachment:fixed;
}

header{
background:#0b5394;
color:white;
text-align:center;
padding:20px;
}

nav ul{
list-style:none;
padding:0;
}

nav ul li{
display:inline;
margin:15px;
}

nav ul li a{
color:white;
text-decoration:none;
font-weight:bold;
}

section{
padding:40px;
}

.hero{
background:#e3f2fd;
text-align:center;
padding:60px;
}

.card-container{
display:flex;
gap:20px;
flex-wrap:wrap;
}

.card{
background:white;
padding:20px;
border-radius:10px;
box-shadow:0 2px 6px rgba(0,0,0,0.1);
width:220px;
}

button{
padding:10px 20px;
background:#0b5394;
color:white;
border:none;
cursor:pointer;
}

textarea{
width:300px;
height:80px;
display:block;
margin-top:10px;
}

.ulasan{
background:white;
padding:15px;
margin-top:10px;
border-radius:8px;
}

.reply{
margin-left:20px;
color:green;
}

footer{
background:#222;
color:white;
text-align:center;
padding:20px;
}

</style>

</head>

<body>

<header>

<h1>Lilium Medica Library</h1>
<p>Hospital Medical Library & Information Center</p>

<nav>
<ul>

<li><a href="#home">Home</a></li>
<li><a href="#koleksi">Koleksi</a></li>
<li><a href="#layanan">Layanan</a></li>
<li><a href="#login">Login</a></li>
<li><a href="#ulasan">Ulasan</a></li>
<li><a href="#kontak">Hubungi Kami</a></li>

</ul>
</nav>

</header>

<section id="home" class="hero">

<h2>Selamat Datang di Lilium Medica Library</h2>

<p>Pusat informasi kesehatan untuk dokter, perawat, peneliti, dan mahasiswa.</p>

</section>

<section id="koleksi">

<h2>Koleksi Perpustakaan</h2>

<div class="card-container">

<div class="card">
<h3>Buku Kedokteran</h3>
<p>Koleksi buku medis dari berbagai spesialisasi.</p>
</div>

<div class="card">
<h3>Jurnal Medis</h3>
<p>Akses jurnal nasional dan internasional.</p>
</div>

<div class="card">
<h3>E-Book</h3>
<p>Koleksi buku digital kesehatan.</p>
</div>

</div>

</section>

<section id="layanan">

<h2>Layanan Perpustakaan</h2>

<ul>

<li>Peminjaman Buku</li>
<li>Literature Search</li>
<li>Pelatihan Literasi Informasi</li>
<li>Bantuan Sitasi</li>

</ul>

</section>

<section id="login">

<h2>Login Pustakawan</h2>

<input type="text" id="username" placeholder="Username">
<br><br>

<input type="password" id="password" placeholder="Password">
<br><br>

<button onclick="login()">Login</button>

<p id="status"></p>

</section>

<section id="ulasan">

<h2>Ulasan Pengguna</h2>

<input type="text" id="nama" placeholder="Nama">
<br><br>

<textarea id="komentar" placeholder="Tulis ulasan"></textarea>

<br>

<button onclick="kirimUlasan()">Kirim Ulasan</button>

<div id="daftarUlasan"></div>

</section>

<section id="kontak">

<h2>Hubungi Kami</h2>

<p>WhatsApp / Telepon : <b>082172919084</b></p>

<p>Email : liliummedicalibrary@gmail.com</p>

</section>

<footer>

<p>© 2026 Lilium Medica Library</p>

</footer>

<script>

let adminLogin=false;

function login(){

let user=document.getElementById("username").value;
let pass=document.getElementById("password").value;

if(user=="admin" && pass=="library"){

adminLogin=true;

document.getElementById("status").innerHTML="Login berhasil sebagai pustakawan";

}else{

document.getElementById("status").innerHTML="Login gagal";

}

}

function kirimUlasan(){

let nama=document.getElementById("nama").value;
let komentar=document.getElementById("komentar").value;

let div=document.createElement("div");

div.className="ulasan";

div.innerHTML="<b>"+nama+"</b><p>"+komentar+"</p>";

if(adminLogin){

let tombol=document.createElement("button");

tombol.innerText="Balas";

tombol.onclick=function(){

let balasan=prompt("Tulis balasan pustakawan");

let p=document.createElement("p");

p.className="reply";

p.innerHTML="<b>Pustakawan:</b> "+balasan;

div.appendChild(p);

}

div.appendChild(tombol);

}

document.getElementById("daftarUlasan").appendChild(div);

}

</script>

</body>
</html>
