 <!DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Alex Sumos Naturais & Lanches</title>
<style>
body { margin:0; font-family: Arial, sans-serif; background:#f5f5f5; }
header { display:flex; align-items:center; padding:10px; position:fixed; top:0; left:0; width:100%; background:rgba(255,255,255,0.9); z-index:1000; box-shadow:0 2px 8px rgba(0,0,0,0.2); }
header img { height:50px; margin-right:10px; }
header h1 { font-size:18px; color:red; margin:0; }

.slide { max-width:500px; margin:80px auto 20px; display:none; animation:fade 1s; text-align:center; }
.slide img { width:100%; border-radius:12px; }
@keyframes fade { from {opacity:0} to {opacity:1} }

button#entrar { display:block; margin:20px auto; padding:12px 25px; font-size:16px; background:red; color:white; border:none; border-radius:8px; cursor:pointer; }

.price { font-weight:bold; color:red; margin-top:5px; }
</style>
<script>
let slideIndex = 0;
function showSlides() {
    let slides = document.getElementsByClassName("slide");
    for(let i=0;i<slides.length;i++) slides[i].style.display="none";
    slideIndex++;
    if(slideIndex>slides.length) slideIndex=1;
    slides[slideIndex-1].style.display="block";
    setTimeout(showSlides,3000);
}
window.onload = showSlides;
</script>
</head>
<body>

<header>
<img src="logo.png" alt="Alex Sumos Naturais & Lanches">
<h1>Alex Sumos Naturais & Lanches</h1>
</header>

<!-- SLIDES -->
<div class="slide">
<img src="frango.jpg" alt="¼ de frango grelhado">
<div class="price">250 MZN</div>
</div>
<div class="slide">
<img src="batata.jpg" alt="Dose de batata">
<div class="price">100 MZN</div>
</div>
<div class="slide">
<img src="sandes_simples.jpg" alt="Sandes simples">
<div class="price">40 MZN</div>
</div>
<div class="slide">
<img src="sandes_mista.jpg" alt="Sandes mista">
<div class="price">75 MZN</div>
</div>
<div class="slide">
<img src="manga.jpg" alt="Sumo de manga">
<div class="price">50 MZN</div>
</div>
<div class="slide">
<img src="laranja.jpg" alt="Sumo de laranja">
<div class="price">50 MZN</div>
</div>

<button id="entrar" onclick="window.location.href='menu.html'">Entrar no Menu</button>

</body>
</html> 
