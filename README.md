<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Klasifikasi Sampah & Edukasi</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
  <h1>♻️ Klasifikasi Sampah Berbasis AI</h1>
  <p>Edukasi Daur Ulang untuk Lingkungan Bersih</p>
</header>

<section class="upload-box">
  <h3>Unggah Gambar Sampah</h3>
  <input type="file" accept="image/*" onchange="previewImage(event)">
  <img id="preview" />
</section>

<section class="result-box">
  <h3>Hasil Klasifikasi (Simulasi AI)</h3>
  <p id="classification">Belum ada gambar</p>
  <p id="education"></p>
</section>

<section class="sample">
  <h3>Contoh Sampah</h3>
  <img src="https://images.unsplash.com/photo-1581578017420-2f26cbd35b5d" alt="Sampah Plastik">
  <img src="https://images.unsplash.com/photo-1605600659873-d808a13e4d2f" alt="Sampah Organik">
</section>

<script src="script.js"></script>
</body>
</html>
