<!DOCTYPE html>
<html lang="kk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Марат Жыланбаев</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #000;
      color: #fff;
      overflow-x: hidden;
    }

    header {
      text-align: center;
      padding: 80px 20px;
      background: linear-gradient(180deg, #000, #111);
    }

    header h1 {
      font-size: 3rem;
      color: #00ff99;
      text-shadow: 0 0 15px #00ff99;
      animation: fadeInDown 1.2s ease forwards;
    }

    .video-btn {
      display: inline-block;
      background-color: #00ff99;
      color: #000;
      font-weight: bold;
      padding: 12px 24px;
      border-radius: 30px;
      text-decoration: none;
      margin-top: 30px;
      transition: all 0.3s ease;
      box-shadow: 0 0 15px #00ff99;
    }

    .video-btn:hover {
      background-color: #00cc77;
      box-shadow: 0 0 25px #00ff99;
      transform: scale(1.05);
    }

    section {
      max-width: 900px;
      margin: 80px auto;
      padding: 0 20px;
      opacity: 0;
      transform: translateY(40px);
      animation: fadeInUp 1.2s ease forwards;
    }

    section:nth-child(odd) {
      animation-delay: 0.5s;
    }

    h2 {
      color: #00ff99;
      text-shadow: 0 0 10px #00ff99;
      margin-bottom: 20px;
      font-size: 2rem;
    }

    p {
      line-height: 1.7;
      color: #ddd;
    }

    footer {
      text-align: center;
      padding: 30px;
      color: #888;
      background-color: #050505;
      border-top: 1px solid #111;
    }

    @keyframes fadeInUp {
      0% { opacity: 0; transform: translateY(40px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInDown {
      0% { opacity: 0; transform: translateY(-30px); }
      100% { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <header>
    <h1>Марат Жыланбаев</h1>
    <a href="https://www.youtube.com/results?search_query=Марат+Жыланбаев" target="_blank" class="video-btn">🎥 Ойнау бейне</a>
  </header>

  <section id="bio">
    <h2>Өмірбаяны</h2>
    <p>
      Марат Жыланбаев — қазақстандық марафоншы, ерекше төзімділігімен және жетістіктерімен танымал тұлға. Ол адам мүмкіндігінің шексіз екенін дәлелдеп, Африка, Аустралия және Еуразия құрлықтарында марафондар жүгірген. Оның аты әлемдік рекордтар кітабына енген.
    </p>
    <p>
      Ол мыңдаған шақырымды шөл мен далада еңсеріп, қазақстандық спорттың символына айналды. Мараттың рухы мен табандылығы жастарға үлгі болып қала береді.
    </p>
  </section>

  <section id="achievements">
    <h2>Жетістіктері</h2>
    <p>
      • Сахара шөлін жүгіріп өткен алғашқы адам.
      <br>• 13,000 км-ден астам қашықтықты тоқтаусыз бағындырған.
      <br>• Қазақстанның еңбек сіңірген спорт шебері.
      <br>• Халықаралық марафондар мен ультрамарафондардың жеңімпазы.
    </p>
  </section>

  <section id="inspiration">
    <h2>Мотивация және мұра</h2>
    <p>
      Марат Жыланбаев – тек спортшы ғана емес, ол күш-жігер мен мақсатқа адалдықтың символы. Оның өмірлік ұстанымы – «Тек алға!», көптеген жас спортшыларды шабыттандырады.
    </p>
  </section>

  <footer>
    © 2025. Барлық құқықтар қорғалған.
  </footer>

  <script>
    const sections = document.querySelectorAll('section');
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.style.opacity = '1';
          entry.target.style.transform = 'translateY(0)';
        }
      });
    }, { threshold: 0.2 });

    sections.forEach(section => observer.observe(section));
  </script>
</body>
</html>
