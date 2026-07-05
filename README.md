<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>For My Malkin ❤️</title>

<link rel="preconnect" href="https://fonts.googleapis.com">

<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Great+Vibes&display=swap" rel="stylesheet">

<link rel="stylesheet" href="style.css">

</head>

<body>

<div id="loading">

<div class="loader-heart">❤️</div>

<h2>Preparing Something Special...</h2>
<section id="<img width="1200" height="1600" alt="mis" src="https://github.com/user-attachments/assets/e81da00a-d454-43fa-a937-8feeea756e68" />
">

<div class="overlay"></div>

<img src="![Uploading mis.jpeg…]()
" class="hero-img">

<div class="hero-content">

<h1>For My Malkin Maishika ❤️</h1>

<p>

Before you decide anything...

Please give me just 2 minutes.

</p>

<button id="startBtn">

💌 Open My Heart

</button>

</div>

</section>
<section id="passwordPage">

<div class="glass">

<h2>

❤️ Unlock My Heart ❤️

</h2>

<p>

Enter Our Special Date

</p>

<input

type="password"

id="password"

placeholder="10-01-2022"

>

<button id="unlock">

Unlock ❤️

</button>

<p id="errorText"></p>

</div>

</section> 
<section id="envelopePage">

<div class="envelope">

<div class="lid"></div>

<div class="paper">

<h2>💌 To My Malkin Maishika Ji</h2>

<p id="typingText"></p>

</div>

</div>

</section>

<audio id="bgMusic">

<source src="assets/music.mp3" type="audio/mpeg">

</audio> 
#envelopePage{
display:none;
width:100%;
height:100vh;
background:linear-gradient(135deg,#ffd6e0,#ffeef4);
justify-content:center;
align-items:center;
overflow:hidden;
}

.envelope{
width:320px;
height:220px;
position:relative;
cursor:pointer;
transition:1s;
}

.paper{

position:absolute;

width:90%;

height:350px;

left:5%;

bottom:0;

background:white;

border-radius:15px;

padding:25px;

transform:translateY(170px);

transition:1.2s;

overflow:auto;

box-shadow:0 10px 40px rgba(0,0,0,.25);

}

.envelope.open .paper{

transform:translateY(-90px);

}

.lid{

position:absolute;

width:100%;

height:120px;

background:#ff4f81;

clip-path:polygon(0 0,100% 0,50% 100%);

transition:1s;

}

.envelope.open .lid{

transform:rotateX(180deg);

transform-origin:top;} 
const letter = `To my Malkin Maishika Ji 🙇🏻🙏🏽

I know you're really angry with me, and honestly, I don't blame you.

I'm so sorry for hurting you.

I don't expect you to forgive me immediately.

You mean the world to me.

Thank you for staying with me through every smile and every fight.

I love you.

Forever.

❤️

Your Paaipuu`;

document.querySelector(".envelope").onclick=function(){

this.classList.add("open");

document.getElementById("bgMusic").play();

setTimeout(typeLetter,900);

}

function typeLetter(){

let i=0;

const target=document.getElementById("typingText");

target.innerHTML="";

function typing(){

if(i<letter.length){

target.innerHTML+=letter.charAt(i);

i++;

setTimeout(typing,28);

}

}

typing();} 
<section id="memoryPage">

<div class="memory-overlay"></div>

<div class="memory-content">

<h1>❤️ Our Journey ❤️</h1>

<h2 id="loveCounter"></h2>

<img src="<img width="1200" height="1600" alt="mis" src="https://github.com/user-attachments/assets/2a762804-92ae-4e47-9013-958062f51ce4" />
" class="memoryPhoto">

<p>

Every smile.

Every fight.

Every hug.

Every memory.

Every moment.

I still choose you.

❤️

</p>

<button id="nextMemory">

Continue ❤️

</button>

</div>

</section>

<section id="finalPage">

<div class="final-overlay"></div>

<div class="glassCard">

<h1>🥺</h1>

<h2>Please Forgive Me</h2>

<p>

Maybe today you're angry...

Maybe tomorrow you'll forgive me...

But one thing will never change...

❤️

I will always love you.

</p>

<button id="forgive">

❤️ Forgive Me ❤️

</button>

</div>

</section>

<section id="endingPage">

<h1>❤️ Thank You ❤️</h1>

<img src="<img width="1200" height="1600" alt="mis" src="https://github.com/user-attachments/assets/324e6448-e0ec-434c-8435-106a0aa2dc65" />
" class="endingPhoto">

<h2>

Forever Yours

</h2>

<h3>

Your Naukar

Paaipuu 🙇🏻❤️

</h3>

<p>

No matter what happens...

You'll always have a special place in my heart.

</p>

</section> 
#memoryPage,
#finalPage,
#endingPage{

display:none;

width:100%;

height:100vh;

justify-content:center;

align-items:center;

flex-direction:column;

text-align:center;

background:linear-gradient(135deg,#ffe0ea,#fff7fa);

}

.memoryPhoto,
.endingPhoto{

width:220px;

height:220px;

border-radius:50%;

object-fit:cover;

border:8px solid white;

box-shadow:0 20px 50px rgba(0,0,0,.25);

margin:25px;

}

.glassCard{

background:rgba(255,255,255,.25);

backdrop-filter:blur(20px);

padding:40px;

border-radius:30px;

width:90%;

max-width:650px;

}

#forgive{

margin-top:25px;

padding:18px 45px;

border:none;

border-radius:40px;

font-size:22px;

background:#ff4f81;

color:white;

cursor:pointer;

box-shadow:0 0 35px #ff4f81;

transition:.4s;

}

#forgive:hover{

transform:scale(1.08);
// Relationship Counter

function updateLoveCounter(){

const start=new Date("2022-01-10");

const now=new Date();

let days=Math.floor((now-start)/(1000*60*60*24));

let years=Math.floor(days/365);

days%=365;

let months=Math.floor(days/30);

days%=30;

document.getElementById("loveCounter").innerHTML=

`${years} Years ❤️ ${months} Months ❤️ ${days} Days Together`;

}

updateLoveCounter();

document.getElementById("nextMemory").onclick=function(){

document.getElementById("memoryPage").style.display="none";

document.getElementById("finalPage").style.display="flex";

}

document.getElementById("forgive").onclick=function(){

document.getElementById("finalPage").style.display="none";

document.getElementById("endingPage").style.display="flex";
/* Rose Petals */

.petal{

position:fixed;

top:-10px;

width:18px;

height:18px;

background:#ff7aa2;

border-radius:60% 40% 60% 40%;

opacity:.8;

pointer-events:none;

animation:petalFall linear forwards;

}

@keyframes petalFall{

0%{

transform:translateY(-20px) rotate(0deg);

opacity:0;

}

20%{

opacity:1;

}

100%{

transform:translateY(110vh) translateX(120px) rotate(360deg);

opacity:0;

}

}

/* Floating Hearts */

.floatHeart{

position:fixed;

bottom:-20px;

font-size:22px;

pointer-events:none;

animation:heartFloat 6s linear forwards;

}

@keyframes heartFloat{

0%{

transform:translateY(0);

opacity:0;

}

20%{

opacity:1;

}

100%{

transform:translateY(-110vh);

opacity:0;

}

}

/* Smooth Fade */

.fadeIn{

animation:fadeIn 1s ease;

}

@keyframes fadeIn{

from{

opacity:0;

transform:translateY(30px);

}

to{

opacity:1;

transform:translateY(0);

}

}

/* Button Glow */

button{

transition:.35s;

}

button:hover{

transform:scale(1.05);

box-shadow:0 0 30px #ff4f81;

} 
/* Falling Petals */

setInterval(()=>{

const petal=document.createElement("div");

petal.className="petal";

petal.style.left=Math.random()*100+"vw";

petal.style.animationDuration=(5+Math.random()*4)+"s";

document.body.appendChild(petal);

setTimeout(()=>petal.remove(),9000);

},350);


/* Floating Hearts */

setInterval(()=>{

const heart=document.createElement("div");

heart.className="floatHeart";

heart.innerHTML="❤️";

heart.style.left=Math.random()*100+"vw";

heart.style.fontSize=(18+Math.random()*18)+"px";

heart.style.animationDuration=(4+Math.random()*3)+"s";

document.body.appendChild(heart);

setTimeout(()=>heart.remove(),7000);

},600);


/* Heart Explosion */

function heartExplosion(){

for(let i=0;i<120;i++){

const h=document.createElement("div");

h.innerHTML="❤️";

h.style.position="fixed";

h.style.left="50%";

h.style.top="50%";

h.style.fontSize=(15+Math.random()*30)+"px";

h.style.transition="2s";

document.body.appendChild(h);

setTimeout(()=>{

h.style.left=Math.random()*100+"vw";

h.style.top=Math.random()*100+"vh";

h.style.opacity="0";

},50);

setTimeout(()=>h.remove(),2200);

}

} document.getElementById("forgive").onclick=function(){

heartExplosion();

setTimeout(()=>{

document.getElementById("finalPage").style.display="none";

document.getElementById("endingPage").style.display="flex";

},1800);

} <h2 style="color:#ff4f81;">
Made With Love ❤️
</h2> 
