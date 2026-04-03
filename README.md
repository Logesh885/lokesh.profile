<!DOCTYPE html>
<html>
<head>
<title>Cashback Reward</title>

<style>
body {
  margin:0;
  font-family: Arial;
  background:black;
  color:white;
  text-align:center;
  overflow:hidden;
}

#loader {
  position:absolute;
  width:100%;
  height:100%;
  background:black;
  display:flex;
  justify-content:center;
  align-items:center;
  font-size:24px;
}

#main {
  display:none;
  margin-top:100px;
}

button {
  padding:12px 25px;
  font-size:20px;
  background:#00c853;
  border:none;
  border-radius:10px;
  color:white;
}

#gorilla {
  position:fixed;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:black;
  display:none;
  justify-content:center;
  align-items:center;
}

#gorilla img {
  width:100%;
  height:100%;
  object-fit:cover;
}
</style>

</head>

<body>

<div id="loader">
⏳ Processing your ₹100 Cashback...
</div>

<div id="main">
<h1>🎉 Congrats! ₹100 Cashback Unlocked</h1>
<button onclick="showGorilla()">Claim Now</button>
</div>

<div id="gorilla">
<img src="https://i.imgur.com/6o5VQ0B.png">
<audio id="sound" src="https://www.myinstants.com/media_1.mp3/sounds"></audio>
</div>

<script>
setTimeout(()=>{
  document.getElementById("loader").style.display="none";
  document.getElementById("main").style.display="block";
}, 2500);

function showGorilla(){
  document.getElementById("gorilla").style.display="flex";
  document.getElementById("sound").play();
}
</script>

</body>
</html>
