<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Adjuan Aidil Andreanto Library</title>

<style>
body {
    margin:0;
    font-family: 'Segoe UI', sans-serif;
    background: url('https://images.unsplash.com/photo-1524995997946-a1c2e315a42f') no-repeat center center fixed;
    background-size: cover;
    color:white;
}

.overlay{
    min-height:100vh;
    background: rgba(0,0,0,0.6);
    backdrop-filter: blur(4px);
    padding-bottom:40px;
}

/* NAVIGATION */
nav{
    background: rgba(0,0,0,0.7);
    backdrop-filter: blur(10px);
    padding:18px;
    display:flex;
    justify-content:space-between;
    align-items:center;
    position:sticky;
    top:0;
}

.nav-left{
    display:flex;
    gap:20px;
}

.nav-right{
    display:flex;
    flex-direction:column;
    align-items:flex-end;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
    letter-spacing:1px;
    transition:0.3s;
}

nav a:hover{
    color:#ffd700;
}

/* CONTAINER GLASS */
.container{
    padding:50px;
    max-width:900px;
    margin:40px auto;
    background: rgba(255,255,255,0.08);
    border-radius:20px;
    backdrop-filter: blur(15px);
    box-shadow: 0 8px 32px rgba(0,0,0,0.4);
}

/* SECTION CONTROL */
.section{
    display:none;
    animation: fade 0.5s ease-in-out;
}

.active{
    display:block;
}

@keyframes fade{
    from{opacity:0; transform:translateY(10px);}
    to{opacity:1; transform:translateY(0);}
}

h1,h2,h3{
    text-align:center;
}

p{
    text-align:center;
    font-size:18px;
}

.link-box{
    text-align:center;
    margin-top:25px;
}

.link-box a{
    display:inline-block;
    margin:10px;
    padding:12px 25px;
    background: linear-gradient(45deg, #ffd700, #ffae00);
    color:black;
    font-weight:bold;
    border-radius:30px;
    text-decoration:none;
    transition:0.3s;
}

.link-box a:hover{
    transform:scale(1.05);
}

ul{
    list-style:none;
    padding:0;
    text-align:center;
}

ul li{
    padding:10px;
    font-size:18px;
}

.video-box{
    text-align:center;
    margin-top:30px;
}

iframe{
    border-radius:15px;
    box-shadow:0 5px 20px rgba(0,0,0,0.5);
    max-width:100%;
}

/* FORM LOGIN */
form{
    max-width:400px;
    margin:auto;
    text-align:left;
}

form input{
    width:100%;
    padding:8px;
    margin-top:5px;
    border-radius:5px;
    border:none;
}

form button{
    margin-top:15px;
    width:100%;
    padding:10px;
    background:#ffd700;
    border:none;
    border-radius:20px;
    font-weight:bold;
    cursor:pointer;
}
</style>

<script>
function showMenu(menu){
    document.querySelectorAll('.section').forEach(sec=>{
        sec.classList.remove('active');
    });
    document.getElementById(menu).classList.add('active');
}
</script>

</head>

<body>
<div class="overlay">

<nav>
<div class="nav-left">
<a href="#" onclick="showMenu('dashboard')">Dashboard</a>
<a href="#" onclick="showMenu('katalog')">Katalog</a>
<a href="#" onclick="showMenu('kegiatan')">Kegiatan Literasi</a>
</div>

<div class="nav-right">
<a href="#" onclick="showMenu('login')">Login</a>
<a href="https://wa.me/6282172919084?text=Halo%20saya%20ingin%20bertanya%20tentang%20Adjuan%20Aidil%20Andreanto%20Library" target="_blank">
Hubungi Saya
</a>
</div>
</nav>

<div class="container">

<div id="dashboard" class="section active">
<h1>Adjuan Aidil Andreanto Library</h1>
<p>Selamat datang di perpustakaan pribadi Juan.</p>

<div class="link-box">
<a href="https://www.instagram.com/adjnaidlee_?igsh=MTd3cDB4NDhmYWFxbg==" target="_blank">
About Me
</a>

<a href="https://sites.google.com/view/adjuan/halaman-muka" target="_blank">
My Biodata
</a>
</div>

<div class="video-box">
<h3>Video Profil</h3>
<iframe width="560" height="315"
src="https://www.youtube.com/embed/3xPqfLkyKfg"
frameborder="0"
allowfullscreen>
</iframe>
</div>
</div>

<div id="katalog" class="section">
<h2>Daftar Buku</h2>
<ul>
<li>Manajemen</li>
<li>Sistem Informasi</li>
<li>Bibliometriks</li>
<li>Arsip</li>
</ul>
</div>

<div id="kegiatan" class="section">
<h2>Kegiatan Literasi</h2>
<ul>
<li>Program Pojok Literasi</li>
<li>Sosialisasi Digitalisasi Arsip</li>
<li>Diskusi Buku Mingguan</li>
</ul>
</div>

<div id="login" class="section">
<h2>Form Login Anggota</h2>

<form>
<label>Username</label>
<input type="text" placeholder="Masukkan username">

<label style="margin-top:15px;display:block;">Password</label>
<input type="password" placeholder="Masukkan password">

<button type="submit">Login</button>
</form>
</div>

</div>
</div>

</body>
</html>
