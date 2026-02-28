<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Lilium Medica Center</title>

<style>
body{
    margin:0;
    font-family:'Segoe UI', sans-serif;
    color:white;
    scroll-behavior:smooth;
}

/* NAVIGATION */
nav{
    position:absolute;
    top:0;
    right:0;
    padding:20px 40px;
    z-index:2;
}

nav a{
    text-decoration:none;
    color:white;
    margin-left:20px;
    font-weight:bold;
    padding:8px 18px;
    border-radius:20px;
    border:2px solid #ffd700;
    transition:0.3s;
}

nav a:hover{
    background:#ffd700;
    color:black;
}

/* HERO */
.hero{
    min-height:100vh;
    background:url('https://images.unsplash.com/photo-1586773860418-d37222d8fce3') no-repeat center center/cover;
    position:relative;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:80px 20px;
}

.hero::before{
    content:"";
    position:absolute;
    inset:0;
    background:rgba(0,0,0,0.65);
}

.hero-content{
    position:relative;
    z-index:1;
    max-width:1000px;
}

.hero h2{
    letter-spacing:3px;
    color:#ffd700;
}

.hero h1{
    font-size:50px;
    color:#ff4d6d;
    margin:10px 0;
}

.hero p{
    font-style:italic;
}

.btn-main{
    margin-top:25px;
    display:inline-block;
    padding:15px 40px;
    background:#e60039;
    border-radius:40px;
    text-decoration:none;
    color:white;
    font-weight:bold;
    font-size:18px;
    border:3px solid #ffd700;
    transition:0.3s;
}

.btn-main:hover{
    background:#ffd700;
    color:black;
}

/* FOTO SECTION */
.hero-image{
    margin-top:40px;
}

.hero-image img{
    width:100%;
    max-width:850px;
    border-radius:20px;
    box-shadow:0 15px 40px rgba(0,0,0,0.6);
}

/* VISI MISI */
.visi-misi{
    padding:80px 20px;
    background:#111;
    text-align:center;
}

.visi-misi h2{
    color:#ffd700;
}

.card{
    max-width:800px;
    margin:20px auto;
    padding:30px;
    background:rgba(255,255,255,0.05);
    border-radius:20px;
}

.card h3{
    color:#ff4d6d;
}

.card ul{
    list-style:none;
    padding:0;
}

.card ul li{
    padding:8px 0;
}

/* LOGIN POPUP */
.login-box{
    display:none;
    position:fixed;
    inset:0;
    background:rgba(0,0,0,0.7);
    justify-content:center;
    align-items:center;
}

.login-content{
    background:white;
    color:black;
    padding:30px;
    border-radius:20px;
    width:300px;
}

.login-content input{
    width:100%;
    padding:8px;
    margin:8px 0;
}

.login-content button{
    width:100%;
    padding:10px;
    background:#e60039;
    color:white;
    border:none;
    border-radius:10px;
    cursor:pointer;
}

@media(max-width:768px){
    .hero h1{
        font-size:35px;
    }
}
</style>

<script>
function openLogin(){
    document.getElementById("loginBox").style.display="flex";
}
function closeLogin(){
    document.getElementById("loginBox").style.display="none";
}
</script>

</head>

<body>

<!-- NAVIGATION -->
<nav>
    <a href="javascript:void(0)" onclick="openLogin()">Login</a>
    <a href="https://wa.me/6282172919084" target="_blank">Hubungi Saya</a>
</nav>

<!-- HERO -->
<section class="hero">
    <div class="hero-content">
        <h2>Selamat Datang di</h2>
        <h1>Lilium Medica Center</h1>
        <p>"Knowledge for Healing, Science for Life"</p>

        <a href="#visi" class="btn-main">
            Jelajahi Informasi Medis
        </a>

        <!-- FOTO YANG KAMU KIRIM -->
        <div class="hero-image">
            <img src="/mnt/data/7979.jpg" alt="Perpustakaan Lilium Medica Center">
        </div>

    </div>
</section>

<!-- VISI MISI -->
<section class="visi-misi" id="visi">
    <h2>Visi & Misi</h2>

    <div class="card">
        <h3>Visi</h3>
        <p>
        Menjadi pusat informasi kesehatan terpercaya yang mendukung pelayanan medis berbasis bukti dan inovasi ilmiah.
        </p>
    </div>

    <div class="card">
        <h3>Misi</h3>
        <ul>
            <li>Menyediakan literatur medis terkini.</li>
            <li>Mendukung penelitian tenaga kesehatan.</li>
            <li>Menyediakan layanan penelusuran klinis.</li>
            <li>Mengembangkan repository digital medis.</li>
            <li>Meningkatkan mutu layanan rumah sakit.</li>
        </ul>
    </div>
</section>

<!-- LOGIN POPUP -->
<div class="login-box" id="loginBox" onclick="closeLogin()">
    <div class="login-content" onclick="event.stopPropagation()">
        <h3>Login Anggota</h3>
        <input type="text" placeholder="Username">
        <input type="password" placeholder="Password">
        <button>Login</button>
    </div>
</div>

</body>
</html>
