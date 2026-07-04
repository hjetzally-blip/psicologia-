 <!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Psicología - Olga Sarai Hernández Vázquez</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:Arial, Helvetica, sans-serif;
}

body{
    background-image:url("estrellas.jpg");
    background-size:cover;
    background-position:center;
    background-attachment:fixed;
    color:white;
    transition:.4s;
}

header{
    background:rgba(0,40,90,.8);
    text-align:center;
    padding:30px;
}

header h1{
    font-size:45px;
}

header h3{
    margin-top:10px;
    color:#b3e5fc;
}

nav{
    background:rgba(0,70,140,.8);
    padding:15px;
    text-align:center;
}

nav a{
    color:white;
    text-decoration:none;
    margin:15px;
    font-weight:bold;
    transition:.3s;
}

nav a:hover{
    color:#7dd3fc;
}

.botonModo{
    text-align:center;
    margin:20px;
}

button{
    background:#2196f3;
    color:white;
    border:none;
    padding:12px 20px;
    border-radius:8px;
    cursor:pointer;
    font-size:16px;
    transition:.3s;
}

button:hover{
    background:#1565c0;
}

section{
    width:85%;
    margin:30px auto;
    background:rgba(0,0,80,.65);
    padding:25px;
    border-radius:15px;
    box-shadow:0px 0px 15px #4fc3f7;
    opacity:0;
    transform:translateY(40px);
    animation:aparecer 1s forwards;
}

section:nth-of-type(1){
    animation-delay:.2s;
}

section:nth-of-type(2){
    animation-delay:.5s;
}

section:nth-of-type(3){
    animation-delay:.8s;
}

section:nth-of-type(4){
    animation-delay:1.1s;
}

h2{
    color:#7dd3fc;
    margin-bottom:15px;
}

ul{
    margin-left:20px;
}

li{
    margin:8px 0;
}

input,
textarea{
    width:100%;
    padding:10px;
    border:none;
    border-radius:8px;
    margin-top:8px;
}

.modoClaro{
    background:#eef7ff;
    color:black;
}

.modoClaro section{
    background:rgba(255,255,255,.9);
    color:black;
}

.modoClaro header,
.modoClaro nav,
.modoClaro footer{
    background:#64b5f6;
}

@keyframes aparecer{

from{
opacity:0;
transform:translateY(40px);
}

to{
opacity:1;
transform:translateY(0);
}

}

footer{
background:rgba(0,40,90,.8);
text-align:center;
padding:20px;
margin-top:40px;
}

</style>

</head>

<body>

<header>

<h1>PSICOLOGÍA</h1>

<h3>Olga Sarai Hernández Vázquez</h3>

<p>Conociendo la mente y el comportamiento humano.</p>

</header>

<nav>

<a href="#quees">¿Qué es?</a>

<a href="#ramas">Ramas</a>

<a href="#procesos">Procesos</a>

<a href="#contacto">Contacto</a>

</nav>

<div class="botonModo">

<button onclick="cambiarModo()">

🌙 Cambiar modo claro / oscuro

</button>

</div>
<section id="quees">

<h2>¿Qué es la Psicología?</h2>

<p>
La psicología es la ciencia que estudia el comportamiento humano,
las emociones, los pensamientos y los procesos mentales.
Su objetivo es comprender cómo las personas piensan, sienten y actúan
para mejorar su bienestar y calidad de vida.
</p>

</section>

<section id="ramas">

<h2>Temas Generales de la Psicología</h2>

<ul>

<li>Psicología Clínica.</li>

<li>Psicología Educativa.</li>

<li>Psicología Social.</li>

<li>Psicología Organizacional.</li>

<li>Psicología Infantil.</li>

<li>Psicología Forense.</li>

<li>Psicología Cognitiva.</li>

<li>Psicología del Desarrollo.</li>

<li>Psicología de la Salud.</li>

<li>Neuropsicología.</li>

</ul>

</section>

<section id="procesos">

<h2>Procesos Psicológicos Básicos</h2>

<ul>

<li>Percepción.</li>

<li>Memoria.</li>

<li>Apr
<footer>

<p>
© 2026 | Proyecto de Psicología
</p>

<p>
Elaborado por: Olga Sarai Hernández Vázquez
</p>

</footer>

<script>

const datos = [

"La psicología estudia tanto la conducta como los procesos mentales.",

"El cerebro humano posee aproximadamente 86 mil millones de neuronas.",

"Dormir entre 7 y 9 horas mejora la memoria y el aprendizaje.",

"La inteligencia emocional ayuda a comprender y controlar las emociones.",

"La autoestima influye en la forma en que enfrentamos los problemas.",

"Las emociones participan en la mayoría de nuestras decisiones.",

"La empatía fortalece las relaciones personales.",

"El aprendizaje ocurre durante toda la vida."

];

function mostrarDato(){

let numero = Math.floor(Math.random()*datos.length);

document.getElementById("dato").innerHTML = datos[numero];

}

function cambiarModo(){

document.body.classList.toggle("modoClaro");

}

</script>

</body>
</html>
