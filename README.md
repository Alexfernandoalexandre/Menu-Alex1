<!DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Alex Sumos Naturais & Lanches</title>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  background: #f5f5f5;
}

/* HEADER */
header {
  background: linear-gradient(red, #cc0000);
  color: white;
  text-align: center;
  padding: 25px;
  font-size: 22px;
  font-weight: bold;
}

/* BANNER */
.banner {
  background: url('banner.jpg') center/cover no-repeat;
  height: 150px;
}

/* SECTIONS */
.section {
  padding: 15px;
}

h2 {
  color: red;
  margin-bottom: 10px;
}

/* CARD */
.card {
  background: white;
  border-radius: 12px;
  padding: 10px;
  margin-bottom: 12px;
  display: flex;
  align-items: center;
  box-shadow: 0 3px 8px rgba(0,0,0,0.1);
  transition: 0.3s;
}

.card:hover {
  transform: scale(1.02);
}

.card img {
  width: 80px;
  height: 80px;
  border-radius: 10px;
  margin-right: 10px;
  object-fit: cover;
}

.info {
  flex: 1;
}

.price {
  font-weight: bold;
  color: red;
}

/* BOTÃO */
button {
  background: #25D366;
  color: white;
  border: none;
  padding: 8px 12px;
  border-radius: 6px;
  cursor: pointer;
}

/* BOTÃO FIXO WHATSAPP */
.whatsapp {
  position: fixed;
  bottom: 20px;
  right: 20px;
  background: #25D366;
  color: white;
  padding: 15px;
  border-radius: 50%;
  font-size: 20px;
  text-decoration: none;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 1000;
}
</style>

<script>
function pedir(item){
  let msg = "Olá, gostaria de pedir: " + item;
  let url = "https://wa.me/258846874780?text=" + encodeURIComponent(msg);
  window.open(url, "_blank");
}
</script>

</head>

<body>

<header>
Alex Sumos Naturais & Lanches 🍹  
<br><small>Sabor natural que refresca</small>
</header>

<div class="banner"></div>

<!-- REFEIÇÕES -->
<div class="section">
<h2>🍗 Refeições</h2>

<div class="card">
<img src="frango.jpg" alt="¼ de frango grelhado">
<div class="info">
<div>¼ de frango grelhado</div>
<div class="price">250 Mts</div>
</div>
<button onclick="pedir('¼ de frango grelhado')">Pedir</button>
</div>

<div class="card">
<img src="batata.jpg" alt="Dose de batata">
<div class="info">
<div>Dose de batata</div>
<div class="price">100 Mts</div>
</div>
<button onclick="pedir('Dose de batata')">Pedir</button>
</div>

</div>

<!-- SANDES -->
<div class="section">
<h2>🥪 Sandes</h2>

<div class="card">
<img src="sandes_simples.jpg" alt="Sandes simples">
<div class="info">
<div>Sandes simples</div>
<div class="price">40 Mts</div>
</div>
<button onclick="pedir('Sandes simples')">Pedir</button>
</div>

<div class="card">
<img src="sandes_mista.jpg" alt="Sandes mista">
<div class="info">
<div>Sandes mista</div>
<div class="price">75 Mts</div>
</div>
<button onclick="pedir('Sandes mista')">Pedir</button>
</div>

</div>

<!-- SOPAS -->
<div class="section">
<h2>🍲 Sopas</h2>

<div class="card">
<img src="sopa_feijao.jpg" alt="Sopa de feijão">
<div class="info">
<div>Sopa de feijão</div>
<div class="price">75 Mts</div>
</div>
<button onclick="pedir('Sopa de feijão')">Pedir</button>
</div>

<div class="card">
<img src="sopa_legumes.jpg" alt="Sopa de legumes">
<div class="info">
<div>Sopa de legumes</div>
<div class="price">100 Mts</div>
</div>
<button onclick="pedir('Sopa de legumes')">Pedir</button>
</div>

</div>

<!-- SUMOS -->
<div class="section">
<h2>🍹 Sumos Naturais</h2>

<div class="card">
<img src="manga.jpg" alt="Sumo de manga">
<div class="info">
<div>Sumo de manga</div>
<div class="price">50 Mts</div>
</div>
<button onclick="pedir('Sumo de manga')">Pedir</button>
</div>

<div class="card">
<img src="laranja.jpg" alt="Sumo de laranja">
<div class="info">
<div>Sumo de laranja</div>
<div class="price">50 Mts</div>
</div>
<button onclick="pedir('Sumo de laranja')">Pedir</button>
</div>

<div class="card">
<img src="ananas.jpg" alt="Sumo de ananás">
<div class="info">
<div>Sumo de ananás</div>
<div class="price">50 Mts</div>
</div>
<button onclick="pedir('Sumo de ananás')">Pedir</button>
</div>

<div class="card">
<img src="melancia.jpg" alt="Sumo de melancia">
<div class="info">
<div>Sumo de melancia</div>
<div class="price">75 Mts</div>
</div>
<button onclick="pedir('Sumo de melancia')">Pedir</button>
</div>

<div class="card">
<img src="maracuja.jpg" alt="Sumo de maracujá">
<div class="info">
<div>Sumo de maracujá</div>
<div class="price">50 Mts</div>
</div>
<button onclick="pedir('Sumo de maracujá')">Pedir</button>
</div>

<div class="card">
<img src="goiaba.jpg" alt="Sumo de goiaba">
<div class="info">
<div>Sumo de goiaba</div>
<div class="price">50 Mts</div>
</div>
<button onclick="pedir('Sumo de goiaba')">Pedir</button>
</div>

</div>

<!-- BOTÃO FIXO WHATSAPP -->
<a class="whatsapp" href="https://wa.me/258846874780" target="_blank">💬</a>

</body>
</html>
