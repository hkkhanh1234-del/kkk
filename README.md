<!doctype html>
<html lang="vi">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Portfolio — Huỳnh Kim Khánh</title>

<meta property="og:title" content="Portfolio — Huỳnh Kim Khánh" />
<meta property="og:locale" content="vi_VN" />
<meta property="og:site_name" content="Huỳnh Kim Khánh Portfolio" />
<meta property="og:type" content="website" />
<meta name="twitter:card" content="summary" />
<meta property="twitter:title" content="Portfolio — Huỳnh Kim Khánh" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebSite","headline":"Portfolio — Huỳnh Kim Khánh","name":"Huỳnh Kim Khánh Portfolio"}
</script>

<style>
:root{
  --primary:#2563eb;
  --secondary:#1e40af;
}

/* Background and base */
body{
  margin:0;
  font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial;
  background: url("https://raw.githubusercontent.com/daisubinta/Nhom4tin12anh.github.io/refs/heads/main/beach-wallpaper-3840x2160-sandy-shore-sunset-12590.jpg") center/cover fixed no-repeat;
  color:#111827;
  overflow-x:hidden;
}

/* Header title styling (keeps previous look) */
header{ text-align:center; padding:110px 20px 50px; position:relative; overflow:hidden; }
.hero-title{
  font-size:68px; font-weight:900; margin:0; text-transform:uppercase;
  -webkit-text-stroke:2px #93c5fd;
  text-shadow:0 0 14px rgba(255,255,255,0.7), 0 6px 28px rgba(37,99,235,0.6), 0 12px 45px rgba(0,0,0,0.55);
  background:linear-gradient(to right,#ffffff,#bfdbfe,#60a5fa);
  -webkit-background-clip:text; -webkit-text-fill-color:transparent;
  animation: glowScale 2.5s infinite alternate ease-in-out; position:relative; display:inline-block;
}
.hero-title::after{ content:""; position:absolute; top:0; left:-120%; width:120%; height:100%; background:linear-gradient(90deg,transparent, rgba(255,255,255,0.4), transparent); transform:skewX(-22deg); animation: shine 3.5s ease-in-out infinite; }
@keyframes shine{ 0%{ left:-130%; } 100%{ left:130%; } }
@keyframes glowScale{ 0%{ opacity:0.95; transform:scale(1); } 100%{ opacity:1; transform:scale(1.06); } }

.hero-tagline{ font-size:22px; font-weight:600; color:#f0f9ff; margin-top:18px;
  background:rgba(0,0,0,0.32); display:inline-block; padding:10px 26px; border-radius:40px; backdrop-filter:blur(8px); box-shadow:0 4px 30px rgba(255,255,255,0.2);
}

/* Layout */
.container{ max-width:1000px; margin:10px auto 80px; padding:20px; }
.card{ display:flex; flex-wrap:wrap; border-radius:24px; background:rgba(255,255,255,0.78); backdrop-filter:blur(15px); box-shadow:0 15px 45px rgba(0,0,0,0.25); transition:0.5s; }
.card:hover{ transform: scale(1.02) rotate(-1deg); box-shadow:0 22px 58px rgba(37,99,235,0.35), 0 0 30px rgba(255,255,255,0.4); }

.left{ flex:1 1 260px; display:flex; justify-content:center; align-items:center; padding:40px 30px; }
.avatar{ width:260px; height:260px; border-radius:18px; overflow:hidden; border:6px solid rgba(255,255,255,0.65); box-shadow:0 8px 32px rgba(0,0,0,0.25); animation: avatarFloat 3s infinite alternate ease-in-out; }
.avatar img{ width:100%; height:100%; object-fit:cover; }
@keyframes avatarFloat{ from{transform: translateY(0);} to{transform: translateY(-10px);} }

.right{ flex:2 1 350px; padding:40px 45px; }
.meta{ font-size:16px; color:#1f2937; font-weight:600; opacity:0.9; margin-bottom:18px; }

/* Section card */
.section{ margin-top:24px; padding:18px 24px; border-radius:16px; background:rgba(255, 255, 255, 0.58); backdrop-filter:blur(6px); border-left:5px solid var(--primary); box-shadow: inset 0 2px 12px rgba(0,0,0,0.05); }
.section h3{ font-size:26px; font-weight:800; margin-bottom:10px; color: var(--secondary); text-shadow: 0 2px 6px rgba(37,99,235,0.4); }

/* ---- NEW: Humble intro styling with bold & effects ---- */
.humble-intro {
  font-size:16.5px;
  line-height:1.7;
  color:#0f172a;
  font-weight:500;
  background: linear-gradient(180deg, rgba(255,255,255,0.9), rgba(255,255,255,0.82));
  padding:16px;
  border-radius:12px;
  box-shadow: 0 8px 30px rgba(2,6,23,0.12);
  position: relative;
  overflow: hidden;
}

/* Emphasized (bold) words inside use <strong> — keep color & slight glow */
.humble-intro strong {
  font-weight:800;
  color: #0b1220;
  text-shadow: 0 2px 10px rgba(37,99,235,0.12);
}

/* Animated underline that grows from left when the section appears */
.humble-intro::after{
  content: "";
  position: absolute;
  left: 16px;
  right: 16px;
  bottom: 12px;
  height: 3px;
  border-radius: 4px;
  background: linear-gradient(90deg, rgba(37,99,235,0.9), rgba(96,165,250,0.9));
  transform: scaleX(0);
  transform-origin: left;
  animation: underlineGrow 1.4s cubic-bezier(.2,.9,.2,1) forwards 0.4s;
}
@keyframes underlineGrow {
  to { transform: scaleX(1); }
}

/* Subtle gentle glow behind the paragraph (gives focus) */
.humble-intro::before{
  content: "";
  position: absolute;
  top: -40px;
  right: -40px;
  width: 220px;
  height: 220px;
  background: radial-gradient(circle at center, rgba(96,165,250,0.25), transparent 40%);
  filter: blur(20px);
  opacity: 0.95;
  transform: rotate(12deg);
}

/* Button */
.btn-home{ display:inline-block; padding:14px 32px; font-size:18px; font-weight:700; color:white; border-radius:50px; background:linear-gradient(135deg,var(--primary),var(--secondary)); backdrop-filter:blur(6px); box-shadow:0 6px 30px rgba(37,99,235,0.4); transition:0.3s; text-decoration:none; }
.btn-home:hover{ transform:scale(1.08); box-shadow:0 0 40px rgba(255,255,255,0.6); }

/* Balloons (keeps previous effect but pastel) */
.balloon{ position:absolute; bottom:-140px; width:70px; height:90px; background:rgba(255,182,193,0.28); border-radius:50% 50% 45% 45%; opacity:0.8; animation:floatUp linear infinite; box-shadow: 0 0 18px rgba(255,255,255,0.4); }
.balloon:nth-child(2n){ background:rgba(147,197,253,0.28); }
.balloon:nth-child(3n){ background:rgba(167,243,208,0.28); }
@keyframes floatUp{ 0%{transform:translateY(0);} 100%{transform:translateY(-130vh);} }

/* Responsive small */
@media (max-width:720px){
  .hero-title{ font-size:40px; }
  .right{ padding:24px; }
  .avatar{ width:200px; height:200px; }
}
</style>
</head>

<body>

<header>
  <h1 class="hero-title">Huỳnh Kim Khánh</h1>
  <p class="hero-tagline">      • 📘 Language Explorer • 🌊 Ocean Lover</p>
</header>

<!-- Balloons -->
<script>
const balloonCount = 12;
for (let i = 0; i < balloonCount; i++) {
  const b = document.createElement("div");
  b.className = "balloon";
  const w = 50 + Math.random()*40;
  const h = 70 + Math.random()*50;
  b.style.width = w + "px";
  b.style.height = h + "px";
  b.style.left = Math.random()*100 + "vw";
  b.style.animationDuration = 6 + Math.random()*6 + "s";
  b.style.animationDelay = Math.random()*4 + "s";
  document.body.appendChild(b);
}
</script>

<div class="container">
  <div class="card">
    <div class="left">
      <div class="avatar">
        <img src="https://raw.githubusercontent.com/daisubinta/Nhom4tin12anh.github.io/refs/heads/main/golden-retriever-tongue-out.jpg" alt="Avatar" />
      </div>
    </div>

    <div class="right">
      <div class="meta">🎓 Học sinh lớp 12A • 🌅 Curious & Learning</div>

      <!-- HERE: humble intro (edited as you requested) -->
      <div class="section">
        <h3>🧠 About Me</h3>

        <p class="humble-intro">
          Mình là một học sinh cấp 3, đang trên hành trình khám phá bản thân và học hỏi những điều mới mỗi ngày. Mình đặc biệt thích <strong>viết lách</strong>, <strong>học ngôn ngữ</strong>, và <strong>yêu biển</strong> — nơi giúp mình cảm thấy thoải mái, bình yên, và là chính mình nhất. Trang web này là góc nhỏ để mìnhlưu lại sở thích, cảm hứng và
          <strong>những kỷ niệm trong hành trình trưởng thành</strong> của mình 🌿
        </p>
      </div>

      <!-- rest sections remain -->
      <div class="section"><h3>🗣 Language Journey</h3>
        <ul>
          <li>🇬🇧 English: advanced </li>
          <li>🇪🇸 Spanish: basic communication luyện nói</li>
          <li>🇨🇳 Chinese: HSK foundation đang học Nǐ hǎo</li>
        </ul>
      </div>

      <div class="section"><h3>🌊 Hobbies</h3>
        <ul>
          <li>🏊 Bơi lội</li>
          <li>🌅 Ngắm hoàng hôn biển</li>
          <li>📖 Đọc The Perfection Trap</li>
        </ul>
      </div>

      <div class="section"><h3>🚀 Future Goals</h3>
        <ul>
          <li>Xây portfolio freelance</li>
          <li>Xây dựng personal brand và sự nghiệp </li>
          <li>Học stocks, fintech, AI for marketing</li>
        </ul>
      </div>

    </div>
  </div>
</div>

<!-- FOOTER WITH HOME BUTTON -->
<footer>
  <a class="btn-home" href="javascript:history.back()">⬅️ Quay lại trang chính</a>
</footer>

</body>
</html>
