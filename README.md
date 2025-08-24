このコードは **React + Tailwind CSS** で作られているので、通常の「HTML + CSS」では少し構造が違います。React を使わずに、純粋な HTML と CSS で同じようなカフェサイトを作りたい場合は、次のように書けます👇

```html
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>カフェ Aroma</title>
  <style>
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      background: #fff;
      color: #333;
    }
    header {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      background: #f5f5f5;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }
    header h1 {
      font-size: 1.5rem;
    }
    nav a {
      margin: 0 1rem;
      text-decoration: none;
      color: #333;
    }
    nav a:hover {
      color: #d97706;
    }
    .hero {
      height: 80vh;
      background: url('https://images.unsplash.com/photo-1509042239860-f550ce710b93') center/cover;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      font-size: 3rem;
      font-weight: bold;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.5);
    }
    .menu, .gallery, .reservations {
      padding: 3rem 2rem;
      text-align: center;
    }
    .menu h2, .gallery h2, .reservations h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
    }
    .menu-list {
      max-width: 500px;
      margin: 0 auto;
      text-align: left;
    }
    .menu-item {
      display: flex;
      justify-content: space-between;
      padding: 0.5rem 0;
      border-bottom: 1px solid #ccc;
    }
    .gallery-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
      margin-top: 2rem;
    }
    .gallery-grid img {
      width: 100%;
      border-radius: 12px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    figcaption {
      margin-top: 0.5rem;
      font-size: 0.9rem;
      color: #666;
    }
    footer {
      text-align: center;
      padding: 1rem;
      background: #eee;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <!-- ヘッダー -->
  <header>
    <h1>カフェ Aroma</h1>
    <nav>
      <a href="#home">ホーム</a>
      <a href="#menu">メニュー</a>
      <a href="#gallery">ギャラリー</a>
      <a href="#reservations">予約</a>
    </nav>
  </header>

  <!-- ヒーロー -->
  <section id="home" class="hero">
    カフェ Aroma
  </section>

  <!-- メニュー -->
  <section id="menu" class="menu">
    <h2>メニュー</h2>
    <p>※価格はすべて税込表示です</p>
    <div class="menu-list">
      <div class="menu-item"><span>エスプレッソ</span><span>¥300（税込）</span></div>
      <div class="menu-item"><span>アメリカーノ</span><span>¥350（税込）</span></div>
      <div class="menu-item"><span>カプチーノ</span><span>¥400（税込）</span></div>
      <div class="menu-item"><span>ラテ</span><span>¥450（税込）</span></div>
      <div class="menu-item"><span>ドリンクセット（ケーキ付）</span><span>¥800（税込）</span></div>
    </div>
  </section>

  <!-- ギャラリー -->
  <section id="gallery" class="gallery">
    <h2>ギャラリー</h2>
    <div class="gallery-grid">
      <figure>
        <img src="https://images.unsplash.com/photo-1511920170033-f8396924c348" alt="クロワッサン">
        <figcaption>コーヒーとクロワッサンの朝食セット</figcaption>
      </figure>
      <figure>
        <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" alt="カフェ店内">
        <figcaption>落ち着いた店内の雰囲気</figcaption>
      </figure>
      <figure>
        <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085" alt="カプチーノ">
        <figcaption>泡がふわふわのカプチーノ</figcaption>
      </figure>
    </div>
  </section>

  <!-- 予約 -->
  <section id="reservations" class="reservations">
    <h2>予約</h2>
    <p>東京都新宿区カフェ通り123</p>
    <form>
      <input type="text" placeholder="お名前" required><br><br>
      <input type="email" placeholder="メールアドレス" required><br><br>
      <input type="date" required><br><br>
      <button type="submit">予約する</button>
    </form>
  </section>

  <!-- フッター -->
  <footer>
    <p>© 2025 カフェ Aroma - All rights reserved.</p>
  </footer>
</body>
</html>
```

---
こちらは **React なしで純粋な HTML + CSS** のコードです。ブラウザに保存して開けばそのままカフェサイトが表示されます ☕✨

👉 React のコードと HTML+CSS のどちらで進めたいですか？
