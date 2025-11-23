hope atleast you understand me 🤧


stay with me 🥲

<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1.0,maximum-scale=1.0,user-scalable=no" />
  <title>For My Love — Photo Notes</title>
  <style>
    :root{--bg:#fff5fb;--paper:#fffefc;--accent:#ff6f9a}
    html,body{height:100%;margin:0;font-family:Inter, Poppins, system-ui, -apple-system, sans-serif;background:linear-gradient(180deg,var(--bg),#fff);}
    .doodle-bg{position:fixed;inset:0;z-index:0;pointer-events:none}/* Intro */
.intro{position:fixed;inset:0;display:flex;align-items:center;justify-content:center;z-index:60}
.hello-card{background:linear-gradient(135deg,#ffdbe9,#ffeef6);padding:26px 28px;border-radius:18px;box-shadow:0 18px 48px rgba(16,6,20,0.12);text-align:center}
.hello-card h1{margin:0;font-size:34px;color:#ad1d5b}
.hello-card p{margin:8px 0 0;color:#6a2c47}
.hello-card button{margin-top:14px;padding:12px 20px;border-radius:999px;border:0;background:#ff4d8f;color:#fff;font-weight:700;cursor:pointer}

/* Stage */
.stage{position:relative;z-index:10;padding:120px 20px 80px;min-height:120vh}
.container{max-width:1100px;margin:0 auto}
.top-title{text-align:center;font-weight:800;color:#c62c68;margin-bottom:18px}

/* board layout */
.board{display:grid;grid-template-columns:repeat(3,1fr);gap:28px;align-items:start}
@media(max-width:980px){.board{grid-template-columns:repeat(2,1fr)}}
@media(max-width:640px){.board{grid-template-columns:1fr}}

/* polaroid / sticky note look */
.card{background:var(--paper);border-radius:12px;padding:12px;box-shadow:0 18px 36px rgba(20,10,20,0.12);transform-origin:center;transition:transform .45s,box-shadow .35s;overflow:visible;position:relative}
.photo-wrap{width:100%;height:220px;border-radius:8px;overflow:hidden;box-shadow:inset 0 -6px 18px rgba(0,0,0,0.06)}
.photo{width:100%;height:100%;object-fit:cover;display:block}
.caption{padding:10px 6px 12px}
.headline{display:inline-block;padding:6px 8px;border-radius:8px;background:linear-gradient(90deg, rgba(255,127,177,0.12), rgba(255,200,210,0.06));font-weight:700;color:#8a1f4b}
.body{margin-top:8px;color:#4b3742;line-height:1.45}

/* scattered 3D vibe */
.card[data-rot] { transform: rotate(var(--rot)); }
.card:hover{transform:translateY(-10px) scale(1.01);box-shadow:0 36px 60px rgba(20,8,30,0.18)}

/* polaroid small label */
.polab{position:absolute;left:14px;top:-12px;background:#fff;padding:6px 8px;border-radius:8px;font-size:12px;box-shadow:0 8px 18px rgba(0,0,0,0.06)}

/* footer */
footer{text-align:center;padding:24px 8px;color:#7a4a5a}

  </style>
</head>
<body>  <!-- decorative doodle background (keeps page full) -->  <div class="doodle-bg" aria-hidden>
    <svg width="100%" height="100%" viewBox="0 0 1400 900" preserveAspectRatio="xMidYMid slice">
      <defs>
        <linearGradient id="g" x1="0" x2="1"><stop offset="0" stop-color="#fff1f7"/><stop offset="1" stop-color="#fff8f2"/></linearGradient>
      </defs>
      <rect width="100%" height="100%" fill="url(#g)"/>
      <g fill="none" stroke="#fcd8e9" stroke-width="2" opacity="0.7">
        <path d="M120 160 C320 40, 520 40, 720 160"/>
        <path d="M80 260 C260 140, 460 140, 660 260"/>
      </g>
    </svg>
  </div>  <div class="intro" id="intro">
    <div class="hello-card" role="button" id="enterBtn">
      <h1>Hello my love 💕</h1>
      <p>Tap to open — a little gallery of reasons and memories.</p>
      <button>Tap to Enter</button>
    </div>
  </div>  <section class="stage" id="stage" aria-hidden>
    <div class="container">
      <div class="top-title">A collection of small notes — made for you</div>
      <div id="board" class="board"></div>
      <footer>Made with ❤️ — just for you</footer>
    </div>
  </section>  <!-- Embedded audio so no extra upload required --><audio id="bgMusic" loop preload="auto" src="data:audio/mp3;base64,SUQzBAAAAAAAI1RTU0UAAAAPAAADTGF2ZjU2LjM2LjEwNAAAAAAAAAAAAAAA//tQxAADBQBCgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgP/7UMQAFgUBQoICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAA//sQxAAMBAEKAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgP/7EMQADQUhAoICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAg/9k="></audio>

<script>
// --- IMPORTANT ---
// To show the photos you just uploaded here in chat, name them exactly as below and place them
// in the same folder as this `index.html` on GitHub. (Or put them in an `images/` folder and update the paths.)
// Filenames to use (in repo root):
// photo1.jpg, photo2.jpg, photo3.jpg, photo4.jpg, photo5.jpg, photo6.jpg, photo7.jpg

const gallery = [
  {file:'photo1.jpg', headline:'You smiling', body:'A small curve that feels like home.'},
  {file:'photo2.jpg', headline:'Close-up', body:'Your eyes say more than words ever could.'},
  {file:'photo3.jpg', headline:'Daydream', body:'Lost in a thought, priceless simply being you.'},
  {file:'photo4.jpg', headline:'Soft light', body:'Every light paints you more beautiful.'},
  {file:'photo5.jpg', headline:'Golden moment', body:'A little golden memory I keep.'},
  {file:'photo6.jpg', headline:'Quiet smile', body:'The calm that stays with me.'},
  {file:'photo7.jpg', headline:'Lovely', body:'Just you — lovely in every way.'}
];

const board = document.getElementById('board');

// create polaroid-style cards
gallery.forEach((g, i)=>{
  const card = document.createElement('article');
  card.className='card';
  const rot = (Math.random()*14 - 7).toFixed(2) + 'deg';
  card.style.setProperty('--rot', rot);
  card.setAttribute('data-rot', rot);

  card.innerHTML = `
    <div class="polab">Note ${i+1}</div>
    <div class="photo-wrap"><img class="photo" src="${g.file}" alt="photo ${i+1}" onerror="this.style.opacity=0.05;this.style.filter='grayscale(70%)';"/></div>
    <div class="caption">
      <div class="headline">${g.headline}</div>
      <div class="body">${g.body}</div>
    </div>
  `;
  board.appendChild(card);
});

// reveal action: play audio + show stage
const enterBtn = document.getElementById('enterBtn');
const intro = document.getElementById('intro');
const stage = document.getElementById('stage');
const bgMusic = document.getElementById('bgMusic');
enterBtn.addEventListener('click', ()=>{
  intro.style.display='none';
  stage.removeAttribute('aria-hidden');
  bgMusic.play().catch(()=>{});
  // subtle staggered appear
  const cards = document.querySelectorAll('.card');
  cards.forEach((c,idx)=>{ c.style.opacity=0; setTimeout(()=>{ c.style.opacity=1; c.style.transform += ' translateZ(12px)'; }, idx*170); });
});

</script></body>
</html>
