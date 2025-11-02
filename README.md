# proposal
<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>For Manahil 💖</title>

<!-- optional background music -->
<audio id="bgmusic" autoplay loop>
  <source src="music.mp3" type="audio/mpeg" />
</audio>

<style>
  body{
    margin:0;
    height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    flex-direction:column;
    background:linear-gradient(135deg,#ffb6c1,#ff69b4,#ff5c8a);
    font-family:'Poppins',sans-serif;
    color:#fff;
    overflow:hidden;
    text-align:center;
  }
  .card{
    background:rgba(255,255,255,0.1);
    padding:40px 30px;
    border-radius:25px;
    backdrop-filter:blur(12px);
    box-shadow:0 4px 25px rgba(0,0,0,0.25);
    max-width:650px;
  }
  h1{margin:0 0 15px;font-size:2em;}
  p{font-size:1.2em;line-height:1.6;margin:10px 0;}
  button{
    margin-top:20px;
    background:#fff;
    color:#ff5c8a;
    border:0;
    padding:12px 28px;
    border-radius:30px;
    font-size:1em;
    font-weight:600;
    cursor:pointer;
    transition:0.3s;
  }
  button:hover{background:#ff5c8a;color:#fff;}
  .heart{font-size:3em;animation:pulse 1.4s infinite;}
  @keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.25)}}
  @keyframes fly{
    0%{transform:translateY(0) scale(1);opacity:1}
    100%{transform:translateY(-150px) scale(0.5);opacity:0}
  }
</style>
</head>

<body>
  <div class="card">
    <div class="heart">💖</div>
    <h1>Hey Manahil,</h1>
    <p>
      Jab se tu meri zindagi mein aayi hai, sab kuch badal gaya hai. <br>
      Har subah ka matlab ban gaya hai aur har shaam ek dua jaisi lagti hai. <br>
      Teri hansi meri favourite sound hai, teri aankhein meri peace ka address ❤️ <br>
      Main perfect nahi hoon, lekin tu saath ho to sab perfect lagta hai. <br>
      Main chahta hoon ki har kal ka pehla sooraj teri muskurahat se shuru ho ☀️ <br><br>
      <strong>So Manahil… kya tu meri life ka har chapter mere saath likhegi? 💍</strong>
    </p>
    <div style="display:flex;gap:15px;justify-content:center;">
      <button onclick="alert('She said YES ❤️ Forever & Always!')">Yes 💕</button>
      <button onclick="alert('Soch lo… lekin jawab wahi chahiye 😜')">Umm…</button>
    </div>
  </div>

<script>
  // Floating hearts on tap/click
  document.addEventListener('click', e=>{
    const heart=document.createElement('div');
    heart.textContent='💖';
    heart.style.position='fixed';
    heart.style.left=e.clientX+'px';
    heart.style.top=e.clientY+'px';
    heart.style.fontSize='1.8rem';
    heart.style.animation='fly 2s linear forwards';
    document.body.appendChild(heart);
    setTimeout(()=>heart.remove(),2000);
  });
</script>
</body>
</html>
