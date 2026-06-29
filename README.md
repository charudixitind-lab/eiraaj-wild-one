<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Eiraaj's Wild One</title>

<link href="https://fonts.googleapis.com/css2?family=Fredoka:wght@400;600&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Fredoka',sans-serif;
}

body{

background:linear-gradient(#0d4f2d,#1d7a44,#6bc66b);

overflow-x:hidden;

color:white;

text-align:center;

}

.hero{

height:100vh;

display:flex;

flex-direction:column;

justify-content:center;

align-items:center;

position:relative;

overflow:hidden;

}

h1{

font-size:60px;

margin-bottom:10px;

animation:pop 1s ease;

}

h2{

font-size:28px;

font-weight:400;

}

.photo{

width:180px;

height:180px;

border-radius:50%;

border:8px solid #FFD54F;

overflow:hidden;

margin:30px 0;

box-shadow:0 0 30px rgba(255,255,255,.4);

animation:float 3s infinite ease-in-out;

}

.photo img{

width:100%;

height:100%;

object-fit:cover;

}

.button{

background:#FFD54F;

padding:18px 35px;

border-radius:50px;

margin-top:30px;

font-size:22px;

color:#235d25;

text-decoration:none;

font-weight:bold;

transition:.3s;

}

.button:hover{

transform:scale(1.1);

}

.leaf{

position:absolute;

font-size:42px;

animation:fall linear infinite;

}

@keyframes float{

0%,100%{transform:translateY(0)}

50%{transform:translateY(-12px)}

}

@keyframes pop{

0%{transform:scale(.3)}

100%{transform:scale(1)}

}

@keyframes fall{

0%{

transform:translateY(-100px) rotate(0deg);

}

100%{

transform:translateY(110vh) rotate(360deg);

}

}

</style>

</head>

<body>

<div class="hero">

<h2>🌿 Welcome to 🌿</h2>

<h1>🦁 Eiraaj's Wild One 🦁</h1>

<div class="photo">

<img src="https://picsum.photos/400">

</div>

<h2>25 July 2026 • 3:30 PM</h2>

<a class="button" href="#details">

Enter The Jungle 🐒

</a>

</div>

<script>

for(let i=0;i<30;i++){

const leaf=document.createElement("div");

leaf.className="leaf";

leaf.innerHTML=Math.random()>.5?"🍃":"🌿";

leaf.style.left=Math.random()*100+"vw";

leaf.style.animationDuration=(6+Math.random()*6)+"s";

leaf.style.animationDelay=Math.random()*6+"s";

document.body.appendChild(leaf);

}

</script>

</body>

</html>
