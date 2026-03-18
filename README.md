<!DOCTYPE html>
<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Alex Sumos Naturais & Lanches</title>

<style>
body {
  margin:0;
  font-family: Arial;
  text-align:center;
  background:black;
  color:white;
}

/* SLIDE */
.slide {
  position: fixed;
  width:100%;
  height:100%;
  background-size: cover;
  background-position:center;
  animation: slide 15s infinite;
}

@keyframes slide {
  0% {background-image:url('frango.jpg');}
  33% {background-image:url('sandes_mista.jpg');}
  66% {background-image:url('manga.jpg');}
  100% {background-image:url('frango.jpg');}
}

/* OVERLAY */
.overlay {
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background: rgba(0,0,0,0.6);
}

/* LOGO */
.logo {
  position:absolute;
  top:20px;
  left:20px;
  width:80px;
}

/* TEXTO */
.content {
  position:relative;
  top:40%;
}

h1 {
  color:#ff0000;
}

/* BOTÃO */
.btn {
  margin-top:20px;
  padding:15px 25px;
  background:red;
  color:white;
  border:none;
  border-radius:8px;
  font-size:18px;
}
</style>

</head>

<body>

<div class="slide"></div>
<div class="overlay"></div>

<img src="logo.png" class="logo">

<div class="content">
  <h1>Alex Sumos Naturais & Lanches</h1>
  <p>Sabor natural que refresca 🍹</p>

  <a href="menu.html">
    <button class="btn">Entrar no Menu</button>
  </a>
</div>

</body>
</html>
