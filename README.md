<!DOCTYPE html>

<html>
<head>
    <link rel="stylesheet" href="vahelehed.css">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Miisu</title>

</head>
<body>
<!-- Tabel piltidega -->
<div class="row">
    <img src='pildid/miisu5.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu2.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu3.jpg' alt='Miisu' class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu4.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu6.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu7.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu8.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu9.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu10.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
    <img src='pildid/miisu4.jpg' alt="Miisu" class='pilt' onclick="myFunction(this);">
</div>

<!-- Piltide galerii idee ja JavaScript pärineb: https://www.w3schools.com/howto/howto_js_tab_img_gallery.asp -->
<!-- Suurendatud pildi osa-->
<div class="container">
  <!-- Pildi sulgemine -->
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>
  <!-- Suurendatud pilt -->
  <img id="expandedImg_vertikaalne" alt='Suurendatud pilt' style="width:100%">
  <!-- Pildi tekst -->
  <div id="imgtext"></div>
</div>

<!-- Nupp, millega saab tagasi avalehele -->
<div>
    <a href='avaleht.html'><img src='pildid/tagasinupp.png' alt='Tagasi' class='tagasinupp'></a>
</div>
<!-- JS -->
<script>
<!-- JS -->
function myFunction(imgs) {
  // Võtab suurendatud pildi
  var expandImg = document.getElementById("expandedImg_vertikaalne");
  // Võtab pildi teksti
  var imgText = document.getElementById("imgtext");
  // Kasutab sama src, mis on klõpsatul pildil 
  expandImg.src = imgs.src;
  // Kasutab alt väärtust tekstina suurendatud pildile
  imgText.innerHTML = imgs.alt;
  // Näitab pilti 
  expandImg.parentElement.style.display = "block";
}
</script>
</body>
</html>
