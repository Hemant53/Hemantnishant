
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Hemant & Nishant Friendship</title>

<style>

body{
    margin:0;
    font-family: Arial, sans-serif;
    text-align:center;
    background: linear-gradient(45deg,#ff7e5f,#feb47b);
    color:white;
}

header{
    padding:40px;
    font-size:35px;
    font-weight:bold;
}

.section{
    padding:40px;
}

.friend-box{
    background:rgba(255,255,255,0.2);
    padding:30px;
    margin:20px;
    border-radius:15px;
}

button{
    padding:12px 25px;
    font-size:18px;
    border:none;
    border-radius:10px;
    background:#ff0055;
    color:white;
    cursor:pointer;
}

button:hover{
    background:#ff2d6f;
}

footer{
    margin-top:50px;
    padding:20px;
    font-size:14px;
}

</style>
</head>

<body>

<header>
🤝 Hemant ❤️ Nishant 🤝
</header>

<div class="section">

<div class="friend-box">
<h2>Best Friends Forever</h2>
<p>
Dosti ka matlab sirf saath rehna nahi hota,
balki mushkil time me ek dusre ke saath khade rehna hota hai.
</p>

<p>
Hemant 🤝 Nishant  
Forever Friendship
</p>

</div>

<button onclick="playMusic()">Play Punjabi Music 🎵</button>

<br><br>

<audio id="music">
<source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
</audio>

</div>

<footer>
Made with ❤️ for Hemant & Nishant Friendship
</footer>

<script>

function playMusic(){
document.getElementById("music").play();
}

</script>

</body>
</html>
