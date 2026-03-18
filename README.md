index.html   ← página inicial (slide + botão)
menu.html    ← menu completo
imagens...
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

.slide { max-width:500px; margin:80px auto 20px; display:none; animation:fade 2s; text-align:center; }
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
<a href="menu.html" style="text-decoration:none;">
  <button>Entrar no Menu</button>
</a>

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

<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Menu Alex Sumos Naturais & Lanches</title>
<style>
body { margin:0; font-family: Arial, sans-serif; background:#f5f5f5; }
header { display:flex; align-items:center; padding:10px; position:fixed; top:0; left:0; width:100%; background:rgba(255,255,255,0.9); z-index:1000; box-shadow:0 2px 8px rgba(0,0,0,0.2); }
header img { height:50px; margin-right:10px; }
header h1 { font-size:18px; color:red; margin:0; }
.section { max-width:500px; margin:80px auto 20px; }
h2 { color:red; margin-bottom:10px; }
.card { display:flex; align-items:center; background:white; border-radius:12px; padding:10px; margin-bottom:12px; box-shadow:0 3px 8px rgba(0,0,0,0.1); transition:0.3s; }
.card:hover { transform:scale(1.03); }
.card img { width:80px; height:80px; border-radius:10px; margin-right:10px; object-fit:cover; }
.info { flex:1; }
.price { font-weight:bold; color:red; }
button { background:#25D366; color:white; border:none; padding:8px 12px; border-radius:6px; cursor:pointer; }
.whatsapp { position:fixed; bottom:20px; right:20px; background:#25D366; color:white; padding:15px; border-radius:50%; font-size:22px; z-index:1000; display:flex; justify-content:center; align-items:center; text-decoration:none; }
</style>
<script>
function pedir(item){
  let msg = "Olá, gostaria de pedir: " + item;
  let url = "https://wa.me/258846874780?text=" + encodeURIComponent(msg);
  window.open(url,"_blank");
}
</script>
</head>
<body>

<header>
<img src="logo.png" alt="Alex Sumos Naturais & Lanches">
<h1>Alex Sumos Naturais & Lanches</h1>
</header>

<!-- SUMOS -->
<div class="section">
<h2>🍹 Sumos Naturais</h2>
<div class="card"><img src="manga.jpg"><div class="info">Sumo de manga<div class="price">50 MZN</div></div><button onclick="pedir('Sumo de manga')">Pedir</button></div>
<div class="card"><img src="laranja.jpg"><div class="info">Sumo de laranja<div class="price">50 MZN</div></div><button onclick="pedir('Sumo de laranja')">Pedir</button></div>
<div class="card"><img src="ananas.jpg"><div class="info">Sumo de ananás<div class="price">50 MZN</div></div><button onclick="pedir('Sumo de ananás')">Pedir</button></div>
<div class="card"><img src="melancia.jpg"><div class="info">Sumo de melancia<div class="price">75 MZN</div></div><button onclick="pedir('Sumo de melancia')">Pedir</button></div>
<div class="card"><img src="maracuja.jpg"><div class="info">Sumo de maracujá<div class="price">50 MZN</div></div><button onclick="pedir('Sumo de maracujá')">Pedir</button></div>
<div class="card"><img src="goiaba.jpg"><div class="info">Sumo de goiaba<div class="price">50 MZN</div></div><button onclick="pedir('Sumo de goiaba')">Pedir</button></div>
</div>

<!-- LANCHES -->
<div class="section">
<h2>🥪 Lanches</h2>
<div class="card"><img src="sandes_simples.jpg"><div class="info">Sandes simples<div class="price">40 MZN</div></div><button onclick="pedir('Sandes simples')">Pedir</button></div>
<div class="card"><img src="sandes_mista.jpg"><div class="info">Sandes mista<div class="price">75 MZN</div></div><button onclick="pedir('Sandes mista')">Pedir</button></div>
</div>

<!-- ALMOÇOS -->
<div class="section">
<h2>🍗 Almoços</h2>
<div class="card"><img src="frango.jpg"><div class="info">¼ de frango grelhado<div class="price">250 MZN</div></div><button onclick="pedir('¼ de frango grelhado')">Pedir</button></div>
<div class="card"><img src="batata.jpg"><div class="info">Dose de batata<div class="price">100 MZN</div></div><button onclick="pedir('Dose de batata')">Pedir</button></div>
</div>

<a class="whatsapp" href="https://wa.me/258846874780" ="_blank">💬</a>
frango.jpg
batata.jpg
sandes_simples.jpg
sandes_mista.jpg
sopa_feijao.jpg
sopa_legumes.jpg
manga.jpg
laranja.jpg
ananas.jpg
melancia.jpg
maracuja.jpg
goiaba.jpg
iogurte_malambe.jpg
logo.png
