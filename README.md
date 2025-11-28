<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Giới thiệu - Huỳnh Kim Khánh</title>
  <style>
    :root {
      --card: rgba(255, 255, 255, 0.95);
      --primary: #2563eb;
      --secondary: #1e40af;
      --text: #111827;
      --muted: #6b7280;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, Arial;
      background: url('https://raw.githubusercontent.com/daisubinta/Nhom4tin12anh.github.io/refs/heads/main/beach-wallpaper-3840x2160-sandy-shore-sunset-12590.jpg') no-repeat center center fixed;
      background-size: cover;
      color: var(--text);
      line-height: 1.6;
      min-height: 100vh;
      display: flex;
      flex-direction: column;
    }

    header {
      background: rgba(0,0,0,0.4);
      color: #fff;
      padding: 48px 20px;
      text-align: center;
      backdrop-filter: blur(4px);
    }

    header h1 { font-size: 36px; margin-bottom: 10px; }
    header p { font-size: 16px; opacity: 0.9; }

    .container {
      max-width: 960px;
      margin: 40px auto;
      padding: 20px;
      flex: 1;
    }

    .card {
      background: var(--card);
      border-radius: 16px;
      box-shadow: 0 12px 30px rgba(0,0,0,0.2);
      overflow: hidden;
      display: flex;
      flex-wrap: wrap;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 18px 40px rgba(0,0,0,0.3);
    }

    .left {
      flex: 1 1 280px;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 30px;
      background: rgba(255,255,255,0.1);
      backdrop-filter: blur(6px);
    }

    .avatar {
      width: 260px;
      height: 260px;
      border-radius: 14px;
      overflow: hidden;
      border: 5px solid rgba(255,255,255,0.6);
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
      transition: transform 0.3s ease;
    }

    .avatar img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .avatar:hover {
      transform: scale(1.05);
    }

    .right {
      flex: 2 1 320px;
      padding: 30px 40px;
      display: flex;
      flex-direction: column;
      justify-content: center;
    }

    .right h2 {
      margin-bottom: 8px;
      font-size: 26px;
    }

    .right .meta {
      color: var(--muted);
      margin-bottom: 16px;
    }

    .about {
      background: rgba(255,255,255,0.85);
      padding: 16px;
      border-radius: 12px;
      border: 1px solid rgba(0,0,0,0.05);
      min-height: 120px;
      box-shadow: inset 0 2px 6px rgba(0,0,0,0.05);
    }

    footer {
      text-align: center;
      padding: 20px 0;
      color: var(--muted);
      font-size: 14px;
      background: rgba(0,0,0,0.3);
      backdrop-filter: blur(4px);
    }

    @media(max-width: 720px){
      .right { padding: 20px; }
      header h1 { font-size: 28px; }
      .card { flex-direction: column; }
      .left, .right { flex: 1 1 100%; }
    }
  </style>
</head>

<body>
  <header>
    <h1>Giới thiệu bản thân</h1>
    <p>Trang cá nhân của Huỳnh Kim Khánh</p>
  </header>

  <div class="container">
    <div class="card">
      <div class="left">
        <div class="avatar">
          <img src="https://raw.githubusercontent.com/daisubinta/Nhom4tin12anh.github.io/refs/heads/main/golden-retriever-tongue-out.jpg" alt="Ảnh đại diện">
        </div>
      </div>

      <div class="right">
        <h2>Huỳnh Kim Khánh</h2>
        <div class="meta">Học sinh lớp 12A</div>

        <div class="about">
          <p>
            Xin chào! Mình là <strong>Huỳnh Kim Khánh</strong>, học sinh lớp 12A. Mình yêu thích học tập, tiếng Anh và những chuyến đi biển. Ngoài ra, mình cũng rất thích thú với công nghệ và các loài động vật dễ thương!
          </p>
        </div>
      </div>
    </div>
  </div>

  <footer>© 2025 — Trang cá nhân của Huỳnh Kim Khánh</footer>
</body>
</html>


<!-- FOOTER WITH HOME BUTTON -->
<footer>
  <a class="btn-home" href="javascript:history.back()">⬅️ Quay lại trang chính</a>
</footer>

</body>
</html>
