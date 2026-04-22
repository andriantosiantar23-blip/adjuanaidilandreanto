<?php include 'koneksi.php'; ?>
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Lilium Medica Library</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<style>
body{
background: linear-gradient(rgba(255,255,255,0.9), rgba(255,255,255,0.9)),
url('https://images.unsplash.com/photo-1586773860418-d37222d8fce3');
background-size:cover;
}

.card{border-radius:15px;}
</style>
</head>

<body>

<div class="container mt-4">

<h2 class="text-center text-primary mb-4">Lilium Medica Library</h2>

<!-- ================= LOOP ================= -->
<div class="card p-3 mb-4">
<h4>Belajar PHP</h4>
<?php
for($i=1;$i<=10;$i++){
echo "Hari ke-$i belajar PHP <br>";
}
?>
</div>

<!-- ================= KALKULATOR ================= -->
<div class="card p-3 mb-4">
<h4>Kalkulator</h4>

<form method="POST" class="row g-2">
<div class="col-md-3">
<input class="form-control" type="number" name="a" placeholder="Angka 1">
</div>

<div class="col-md-3">
<input class="form-control" type="number" name="b" placeholder="Angka 2">
</div>

<div class="col-md-3">
<select class="form-control" name="op">
<option value="+">+</option>
<option value="-">-</option>
<option value=""></option>
<option value="/">/</option>
</select>
</div>

<div class="col-md-3">
<button class="btn btn-primary w-100" name="hitung">Hitung</button>
</div>
</form>

<?php
if(isset($_POST['hitung'])){
$a=$_POST['a'];
$b=$_POST['b'];
$op=$_POST['op'];

if($op=="+") $h=$a+$b;
elseif($op=="-") $h=$a-$b;
elseif($op=="") $h=$a$b;
elseif($op=="/") $h=$b!=0 ? $a/$b : "Error";

echo "<div class='alert alert-success mt-3'>Hasil: $h</div>";
}
?>
</div>

<!-- ================= LOGIN ================= -->
<div class="card p-3 mb-4">
<h4>Login</h4>

<form method="POST" class="row g-2">
<div class="col-md-5">
<input class="form-control" name="user" placeholder="Username">
</div>

<div class="col-md-5">
<input class="form-control" type="password" name="pass" placeholder="Password">
</div>

<div class="col-md-2">
<button class="btn btn-success w-100" name="login">Login</button>
</div>
</form>

<?php
if(isset($_POST['login'])){
$u=$_POST['user'];
$p=$_POST['pass'];

if(empty($u) || empty($p)){
echo "<div class='alert alert-warning mt-3'>Input tidak lengkap!</div>";
}elseif($u=="admin" && $p=="123"){
echo "<div class='alert alert-success mt-3'>Login sukses</div>";
}else{
echo "<div class='alert alert-danger mt-3'>Login gagal</div>";
}
}
?>
</div>

<!-- ================= CRUD ================= -->
<div class="card p-3 mb-4">
<h4>Data Mahasiswa</h4>

<form method="POST" action="simpan.php" class="row g-2">
<div class="col-md-3">
<input class="form-control" name="nama" placeholder="Nama">
</div>
<div class="col-md-2">
<input class="form-control" name="nim" placeholder="NIM">
</div>
<div class="col-md-3">
<input class="form-control" name="jurusan" placeholder="Jurusan">
</div>
<div class="col-md-3">
<input class="form-control" name="alamat" placeholder="Alamat">
</div>
<div class="col-md-1">
<button class="btn btn-primary">+</button>
</div>
</form>

<hr>

<table class="table table-bordered table-striped">
<tr class="table-primary">
<th>No</th><th>Nama</th><th>NIM</th><th>Jurusan</th><th>Alamat</th><th>Aksi</th>
</tr>

<?php
$no=1;
$data=mysqli_query($conn,"SELECT * FROM mahasiswa");
while($d=mysqli_fetch_array($data)){
?>
<tr>
<td><?= $no++ ?></td>
<td><?= $d['nama'] ?></td>
<td><?= $d['nim'] ?></td>
<td><?= $d['jurusan'] ?></td>
<td><?= $d['alamat'] ?></td>
<td>
<a class="btn btn-danger btn-sm" href="hapus.php?id=<?= $d['id'] ?>">Hapus</a>
</td>
</tr>
<?php } ?>
</table>

</div>

</div>

</body>
</html>
