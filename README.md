<!DOCTYPE html>  <html lang="en">  
<head>  
<meta charset="UTF-8" />  
<meta name="viewport" content="width=device-width, initial-scale=1.0" />  
<title>For Karan</title>  
<style>  
body {  
    background: linear-gradient(135deg, #ffd6e8, #d4e8ff);  
    font-family: 'Poppins', sans-serif;  
    text-align:center;  
    padding:20px;  
    margin:0;  
}  
.card, .letter {  
    background:white;  
    padding:20px;  
    margin:18px auto;  
    width:90%;  
    max-width:420px;  
    border-radius:18px;  
    box-shadow:0 6px 20px rgba(0,0,0,0.12);  
}  
button {  
    padding:10px 18px;  
    border:none;  
    border-radius:12px;  
    font-size:16px;  
    cursor:pointer;  
    background:#ff8eb3;  
    color:white;  
}  
.hidden { display:none; }  
.envelope { font-size:3.5rem; cursor:pointer; margin-top:40px; }  
.card-box { background:#fff0f6; padding:12px; border-radius:12px; margin:12px 0; cursor:pointer; }  
.card-box:hover { background:#ffd6e8; }  
.heart-shape { position:fixed; bottom:-20px; font-size:1.4rem; color:#ff4f8b; animation:floatUp 6s linear infinite; }  
.heart-shape:nth-child(1) { left:15%; animation-duration:7s; }  
.heart-shape:nth-child(2) { left:50%; animation-duration:5.5s; }  
.heart-shape:nth-child(3) { left:85%; animation-duration:6.5s; }  
@keyframes floatUp { 0%{transform:translateY(0);opacity:1} 100%{transform:translateY(-120vh);opacity:0} }  
</style>  
</head>  
<body>  <div class="envelope" id="envelope" onclick="openLetter()">✉️</div>  <div id="letter" class="letter" style="display:none;">  
  <div class="card">  
    <h2 style="font-family:'Playfair Display', serif;">Hey Karan (Mendak) :)</h2>  
    <p style="font-family:'Playfair Display', serif;">Karan… you tease me so much that I should be annoyed, but instead I end up liking you a little more every day. So I made this for you… hope you feel it the way I do.</p>  <p style="font-family:'Playfair Display', serif;">I know I confessed once and you weren’t ready… and I respected that.</p>  
<p style="font-family:'Playfair Display', serif;">But these 5 months with you—laughing with you, getting teased by you—have become my favourite part of everything.</p>  
<p style="font-family:'Playfair Display', serif;">You don’t share everything with me, and that’s okay. But the way you check on me when I’m sad… it means more than you think.</p>  
<p style="font-family:'Playfair Display', serif;">Whenever I see you smiling with your sparkling eyes, I fall for you again and again, Mendak. 🐸💗</p>  

<h3 style="margin-top:14px;">Tap the cards ↓</h3>  

<div class="card-box" onclick="toggleCard(1)">Card 1 ✨ — You're so good at games</div>  
<div id="c1" class="hidden" style="padding:10px 12px; text-align:left;">I love how effortlessly you win… watching you play makes me smile 🎮💗</div>  

<div class="card-box" onclick="toggleCard(2)">Card 2 ✨ — Your sparkling eyes</div>  
<div id="c2" class="hidden" style="padding:10px 12px; text-align:left;">Your eyes when you smile are my favourite — they sparkle and make my day ✨</div>  

<div style="margin-top:16px;">  
  <h4 style="margin-bottom:6px;">Playlist 🎧</h4>  
  <p style="margin:0;">Dhoonde Akhiyaan • Shayrana • Saiyaara</p>  
</div>

  </div>  
</div>  <!-- floating hearts -->  <div class="heart-shape">❤</div>  
<div class="heart-shape">❤</div>  
<div class="heart-shape">❤</div>  <!-- bottom yes/no -->  <div style="margin-top:28px; padding-bottom:60px;">  
  <div class="card" style="max-width:420px; margin:auto;">  
    <p style="font-weight:600;">Do you like me even a little? 💗</p>  
    <button onclick="answerYes()">Yes</button>  
    <button id="noBtn" onmouseover="moveNo()" onclick="answerNo()" style="margin-left:8px;background:#cccccc;">No</button>  
    <p id="resp" style="margin-top:12px;font-weight:600;color:#444;"></p>  
  </div>  
</div>  <audio autoplay loop>  
  <source src="https://aac.saavncdn.com/961/801ba464f562ba419748d6ddfb669143_320.mp4" type="audio/mp4">  
</audio>  <script>  
function openLetter(){ document.getElementById('envelope').style.display='none'; document.getElementById('letter').style.display='block'; }  
function toggleCard(n){ const el=document.getElementById('c'+n); el.style.display = (el.style.display==='block')?'none':'block'; }  
function moveNo(){ const btn=document.getElementById('noBtn'); const x=(Math.random()*200)-100; const y=(Math.random()*200)-100; btn.style.transform = `translate(${x}px,${y}px)`; }  
let noCount=0;  
function answerYes(){ document.getElementById('resp').innerText='I knew it… 💗'; }  
function answerNo(){ noCount++; if(noCount==1) document.getElementById('resp').innerText='Think again 😭💗'; else if(noCount==2) document.getElementById('resp').innerText='You really don\\'t like me?? 😭'; else document.getElementById('resp').innerText='Okay… but I still like you Mendak 💗'; }  
</script>  </body>  
</html>
