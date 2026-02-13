
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Bandana ❤️</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif}

body{
  background:linear-gradient(135deg,#ff758c,#ff7eb3);
  height:100vh;
  overflow:hidden;
  color:#fff;
}

.slide{
  display:none;
  height:100vh;
  width:100vw;
  padding:30px;
  text-align:center;
  animation:fade 1s;
}

.slide.active{
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
}

h1{font-size:2.3rem;margin-bottom:15px}
p{font-size:1.15rem;max-width:750px;line-height:1.6}

img{width:220px;margin:20px 0}

button{
  margin-top:25px;
  padding:12px 35px;
  font-size:1.1rem;
  border:none;
  border-radius:30px;
  cursor:pointer;
}

.next{background:#fff;color:#ff4b6e}
#yes{background:#2ecc71;color:#fff}
#no{background:#e74c3c;color:#fff;position:absolute}

.gift{font-size:5rem;animation:bounce 1.5s infinite}

@keyframes fade{from{opacity:0}to{opacity:1}}
@keyframes bounce{
  0%,100%{transform:translateY(0)}
  50%{transform:translateY(-18px)}
}
</style>
</head>

<body>


<div class="slide active">
  <h1>Hey Bandana ❤️</h1>
  <p> This little card carries pieces of my heart…  
  Even if miles stand between us right now, my feelings for you have never felt closer.  
  Distance may test us, but it will never change what you mean to me❤️😭</p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>You Are My Safe Place 🌸</h1>
  <img src="panda.gif">
  <p>When the world feels heavy, you make everything lighter.
    No matter how loud the world becomes, my heart feels calm when I think of you.  
  Even from far away, you are still my comfort, my peace, my home.  
 loving you fills every empty space😭🫂❤️
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>Us, Always 🐻💕</h1>
  <img src="teddy.gif">
  <p>I don’t need perfect moments, I just need you.
   I wish we might  side by side right now, but we are still heart to heart.  
  Every memory we created, every laugh we shared, every quiet moment —  
  they remind me that what we have is real, strong, and worth holding onto❤️❤️
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>No Matter What 🌈</h1>
  <img src="couple.gif">
  <p>
     I know things aren’t easy.  
  Circumstances pulled us apart, but they never pulled my heart away from you.  
  Your overthinking, your tears, your dreams, your fears —  
  I don’t love you in parts… I love you completely😭💗
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>Some Gifts for You 🎁</h1>
  <div class="gift">🎁</div>
  <p>
     These aren’t things you can unwrap with your hands…  
  They’re pieces of reassurance, loyalty, and promises.  
  Because even when I can’t be there physically,  
  I still want you to feel chosen, valued, and deeply loved❤️</p>
  <button class="next">Open ➝</button>
</div>

<div class="slide">
  <h1>💌 A Letter</h1>
  <p>
    Dear Bandana,<br><br>
    Loving you is my favorite feeling.   
  Not just for your smile or your laugh —  
  but for your heart, your strength, and the way you care so deeply.  
  No situation, no distance, no misunderstanding  
  can erase what I feel for you❤️🫂
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>🤞 A Promise</h1>
  <p>
    I promise to listen when you overthink,  
    hold you when you cry,  
    and stand with you when life feels unfair. 
  I promise to be patience, to be understanding,  
  and to protect what we built together.  
  No matter how long it takes,  
  my heart still chooses you — every single day😭❤️
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>📸 Our Memories</h1>
  <p>
    Every late-night talk, every small argument we fixed,  
  every “I miss you” text — they all matter.  
  They remind me that what we have isn’t temporary.  
  It’s something real… something worth waiting for❤️😭
  </p>
  <button class="next">Next ➝</button>
</div>

<div class="slide">
  <h1>One Honest Question 😳❤️</h1>
  <p>Even with distance, even with circumstances,  
  even with everything life throws at us…  
  Will you still walk this journey with me?
    Bandana, will you be my Valentine?</p>
  <button id="yes">YES 💖</button>
  <button id="no">NO 😝</button>
</div>

<div class="slide">
  <h1>YAYYYY 💕</h1>
  <p>
     Thank you for choosing us.  
   nothing can separate our hearts.  
  I am yours — not just for today,  
  but for every tomorrow we are still fighting for. ❤️
  </p>
</div>

<script>
let slides=document.querySelectorAll('.slide');
let index=0;

document.querySelectorAll('.next').forEach(btn=>{
  btn.onclick=()=>{
    slides[index].classList.remove('active');
    index++;
    slides[index].classList.add('active');
  }
});

const noBtn=document.getElementById("no");
noBtn.addEventListener("mouseover",()=>{
  noBtn.style.left=Math.random()*80+"%";
  noBtn.style.top=Math.random()*80+"%";
});

document.getElementById("yes").onclick=()=>{
  slides[index].classList.remove('active');
  index++;
  slides[index].classList.add('active');
};
</script>

</body>
</html>
