<html lang="en">
<head>
<meta charset="UTF-8">
<title>Hemant ❤️ Nishant</title>

<style>

body{
margin:0;
font-family:Arial;
background:black;
color:white;
text-align:center;
overflow:hidden;
}

/* Stylish Name */

.name{
font-size:70px;
margin-top:60px;
background:linear-gradient(45deg,#ff0066,#ffcc00);
-webkit-background-clip:text;
color:transparent;
animation:shine 3s infinite;
}

@keyframes shine{
0%{filter:brightness(1)}
50%{filter:brightness(2)}
100%{filter:brightness(1)}
}

/* Hearts Animation */

.heart{
position:absolute;
color:red;
font-size:25px;
animation:float 6s infinite;
}

@keyframes float{
0%{transform:translateY(100vh);opacity:1}
100%{transform:translateY(-10vh);opacity:0}
}

/* Music Graph */

.graph{
display:flex;
justify-content:center;
align-items:flex-end;
height:120px;
gap:6px;
margin-top:40px;
}

.bar{
width:10px;
background:#00ffcc;
animation:beat 1s infinite;
}

.bar:nth-child(2){animation-delay:.2s}
.bar:nth-child(3){animation-delay:.4s}
.bar:nth-child(4){animation-delay:.6s}
.bar:nth-child(5){animation-delay:.8s}

@keyframes beat{
0%{height:20px}
50%{height:100px}
100%{height:30px}
}

/* Button */

button{
padding:15px 30px;
font-size:20px;
border:none;
border-radius:20px;
background:#ff0066;
color:white;
cursor:pointer;
}

button:hover{
background:#ff3399;
}

</style>
</head>

<body>

<h1 class="name">Hemant ❤️ Nishant</h1>

<p>Best Friendship Forever 🤝</p>

<button onclick="playMusic()">Play Punjabi Song 🎵</button>

<audio id="music">
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-2.mp3">
</audio>

<div class="graph">
<div class="bar"></div>
<div class="bar"></div>
<div class="bar"></div>
<div class="bar"></div>
<div class="bar"></div>
</div>

<script>

/* Play Music */

function playMusic(){
document.getElementById("music").play();
}

/* Floating Hearts */

function createHeart(){

let heart=document.createElement("div")
heart.className="heart"
heart.innerHTML="❤️"

heart.style.left=Math.random()*100+"vw"

document.body.appendChild(heart)

setTimeout(()=>{
heart.remove()
},6000)

}

setInterval(createHeart,500)

</script>

</body>
</html>
