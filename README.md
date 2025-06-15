
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>СПК «Хорошово-1» — Главная</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Официальный сайт СПК «Хорошово-1». Вся актуальная информация о кооперативе, правлении, документах, платежах и жизни сообщества.">
  <meta name="keywords" content="СПК, Хорошово-1, кооператив, председатель, правление, ревизионная комиссия, документы, взносы, форум, чат, карта, новости">
  <link rel="stylesheet" href="css/style.css">
  <link rel="icon" type="image/png" href="favicon.png">
  <style>
    :root {
      --main-color: #ff9900;
      --accent-color: #0077b6;
      --bg-gradient: linear-gradient(120deg, #e0f7fa 0%, #fffde4 100%);
      --header-bg: rgba(255,255,255,0.85);
      --nav-hover: #ffe0b2;
      --shadow: 0 2px 16px rgba(0,0,0,0.08);
    }
    html, body {
      margin: 0; padding: 0; min-height: 100vh;
      font-family: 'Segoe UI', 'Arial', sans-serif;
      background: var(--bg-gradient);
      color: #222;
      box-sizing: border-box;
    }
    header {
      background: var(--header-bg);
      box-shadow: var(--shadow);
      position: sticky; top: 0; z-index: 100;
      padding: 1rem 0 0.5rem 0;
      text-align: center;
    }
    .logo {
      max-width: 100px;
      border-radius: 50%;
      margin-bottom: 0.5rem;
      box-shadow: 0 2px 10px rgba(0,0,0,0.06);
    }
    .slogan {
      font-size: 1.2rem;
      color: var(--accent-color);
      margin: 0.2em 0 1em 0;
      font-style: italic;
    }
    nav {
      display: flex;
      justify-content: center;
      margin-bottom: 0.5rem;
    }
    nav ul {
      display: flex;
      flex-wrap: wrap;
      list-style: none;
      padding: 0; margin: 0;
      gap: 0.5rem;
    }
    nav li {
      margin: 0;
    }
    nav a {
      display: block;
      padding: 0.6em 1.1em;
      border-radius: 30px;
      color: #222;
      text-decoration: none;
      font-weight: 600;
      transition: background 0.20s, color 0.20s, box-shadow 0.2s;
      box-shadow: 0 1px 4px rgba(255,153,0,0.06);
    }
    nav a:hover, nav a:focus {
      background: var(--main-color);
      color: #fff;
      box-shadow: 0 2px 12px #ffb84d55;
    }
    main {
      max-width: 1100px;
      margin: 2rem auto 1rem auto;
      background: #fff;
      border-radius: 22px;
      box-shadow: var(--shadow);
      padding: 2rem;
    }
    h2 {
      color: var(--main-color);
      margin-top: 0;
    }
    .intro {
      text-align: center;
      margin-bottom: 2rem;
    }
    .highlight {
      background: #fffae6;
      border-left: 4px solid var(--main-color);
      padding: 1em;
      margin-bottom: 1.5rem;
      border-radius: 10px;
      font-size: 1.1em;
      color: #555;
    }
    .map {
      margin-bottom: 2rem;
    }
    .question-block {
      background: #f8f8ff;
      border-radius: 12px;
      padding: 1.2rem;
      box-shadow: 0 1px 8px #0077b61a;
      margin-bottom: 2rem;
    }
    .question-block form {
      display: flex;
      flex-direction: column;
      gap: 0.6em;
    }
    .question-block input, .question-block textarea {
      border: 1px solid #bbb;
      border-radius: 5px;
      padding: 0.7em;
      font-size: 1em;
      background: #fff;
    }
    .question-block button {
      background: var(--main-color);
      color: #fff;
      border: none;
      border-radius: 30px;
      padding: 0.6em 1.5em;
      font-size: 1em;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 2px 8px #ffb84d33;
      transition: background 0.2s;
    }
    .question-block button:hover {
      background: var(--accent-color);
    }
    .captcha {
      display: flex;
      align-items: center;
      gap: 1em;
    }
    .audio-controls { display: flex;
      justify-content: center;
      margin: 1.5em 0 0.5em 0;
    }
    .audio-controls button {
      padding: 0.7em 1.3em;
      font-size: 1em;
      border: none;
      border-radius: 30px;
      background: var(--main-color);
      color: #fff;
      font-weight: 600;
      cursor: pointer;
      box-shadow: 0 1px 6px #ffb84d55;
      transition: background 0.2s;
    }
    .audio-controls button:hover {
      background: var(--accent-color);
    }
    @media (max-width: 800px) {
      main { padding: 1em; }
      nav ul { gap: 0.3rem; }
      .logo { max-width: 70px; }
    }
    @media (max-width: 600px) {
      nav ul { flex-direction: column; gap: 0.07rem; }
      main { padding: 4vw 2vw; }
    }
    footer {
      text-align: center;
      margin: 2.5em 0 1em 0;
      color: #888;
      font-size: 0.95em;
    }
    footer a {
      margin-left: 1.5em;
      color: var(--accent-color);
      text-decoration: none;
      font-weight: 500;
    }
    .loading {
      position: fixed;
      top: 0; left: 0;
      width: 100vw; height: 100vh;
      background: #fff;
      display: flex; align-items: center; justify-content: center;
      font-size: 2.5em;
      color: var(--main-color);
      z-index: 9999;
      animation: fadeOut 2s 2s forwards;
    }
    @keyframes fadeOut {
      to { opacity: 0; visibility: hidden; }
    }
  </style>
</head>
<body>
<div class="loading" aria-hidden="true">Загрузка сайта...</div>
<header>
  <img src="logo.png" alt="Логотип СПК" class="logo">
  <h1>СПК «Хорошово-1»</h1>
  <p class="slogan">Гармония природы и комфорта</p>
  <nav aria-label="Главная навигация">
    <ul>
      <li><a href="index.html">Главная</a></li>
      <li><a href="pages/predsedatel.html">Председатель</a></li>
      <li><a href="pages/pravlenie.html">Правление</a></li>
      <li><a href="pages/revizion.html">Ревизионная комиссия</a></li>
      <li><a href="pages/vznosy.html">Взносы и платежи</a></li>
      <li><a href="pages/zadolzhennosti.html">Задолженности</a></li>
      <li><a href="pages/documents.html">Документы</a></li>
      <li><a href="gallery.html">Фотогалерея</a></li>
      <li><a href="pages/news.html">Новости</a></li>
      <li><a href="forum.html">Форум</a></li>
      <li><a href="chat.html">Чат</a></li>
      <li><a href="pages/faq.html">Задать вопрос</a></li>
      <li><a href="contact.html">Контакты</a></li>
      <li><a href="voting.html">Голосование</a></li>
      <li><a href="admin.html">Вход в кабинет</a></li>
      <li><a href="https://t.me/SPK_Khoroshovo_1" target="_blank">Telegram чат</a></li>
      <li><a href="https://t.me/SPK_Khoroshovo_Bot" target="_blank">Telegram-бот</a></li>
    </ul>
  </nav>
</header>
<main>
  <section class="intro">
    <h2>Добро пожаловать в СПК «Хорошово-1»!</h2>
    <div class="highlight">
      <strong>Вместе мы создаём комфортную, безопасную и гармоничную среду для жизни и отдыха!</strong>
      <br>
      Последние новости, документы, сервисы для садоводов, интерактивная карта, форум, чат и многое другое — всё на одном сайте.
    </div>
  </section>

  <section class="map">
    <h2>Интерактивная карта участков</h2>
    <iframe src="map.html" width="100%" height="450" frameborder="0" style="border-radius: 12px; box-shadow: 0 1px 8px #0077b61a;"></iframe>
  </section>

  <section class="question-block">
    <h2>Задать вопрос Правлению</h2>
    <form id="questionForm" action="send_question.php" method="POST" autocomplete="off">
      <input type="text" name="name" placeholder="Ваше имя" required>
      <input type="email" name="email" placeholder="Ваш Email" required>
      <textarea name="message" placeholder="Ваш вопрос" rows="4" required></textarea>
      <div class="captcha">
        <img src="captcha.php" alt="Капча">
        <input type="text" name="captcha" placeholder="Введите код" required>
      </div>
      <button type="submit">Отправить</button>
    </form>
  </section> <div class="audio-controls">
    <button id="audio-toggle" aria-pressed="false">Включить звуки природы</button>
  </div>
  <audio id="nature-audio" loop>
    <source src="nature-sounds.mp3" type="audio/mpeg">
    <source src="nature-sounds.ogg" type="audio/ogg">
    Ваш браузер не поддерживает аудио.
  </audio>
</main>

<footer>
  &copy; 2025 СПК «Хорошово-1». Все права защищены.
  <a href="rss.xml">RSS</a>
</footer>
<script>
  // Fade out loader
  document.addEventListener('DOMContentLoaded', function() {
      setTimeout(() => {
          document.querySelector('.loading').style.display = 'none';
      }, 3500);
  });

  // Аудио-контроль
  const audio = document.getElementById('nature-audio');
  const btn = document.getElementById('audio-toggle');
  let playing = false;
  btn.addEventListener('click', function () {
    if (!playing) {
      audio.play();
      btn.textContent = "Остановить звуки природы";
      playing = true;
    } else {
      audio.pause();
      btn.textContent = "Включить звуки природы";
      playing = false;
    }
    btn.setAttribute('aria-pressed', playing ? 'true' : 'false');
  });
</script>
</body>
</html> 
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>СПК «Хорошово-1» — Главная</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Официальный сайт СПК «Хорошово-1». Вся актуальная информация о кооперативе, правлении, документах, платежах и жизни сообщества.">
  <meta name="keywords" content="СПК, Хорошово-1, кооператив, председатель, правление, ревизионная комиссия, документы, взносы, форум, чат, карта, новости">
  <link rel="stylesheet" href="css/style.css">
  <link rel="icon" type="image/png" href="favicon.png">
  <style>
    /* ... ВСЕ ваши стили (из примера выше) ... */
  </style>
</head>
<body>
<div class="loading" aria-hidden="true">Загрузка сайта...</div>
<header>
  <img src="logo.png" alt="Логотип СПК" class="logo">
  <h1>СПК «Хорошово-1»</h1>
  <p class="slogan">Гармония природы и комфорта</p>
  <nav aria-label="Главная навигация">
    <ul>
      <li><a href="index.html">Главная</a></li>
      <li><a href="pages/predsedatel.html">Председатель</a></li>
      <li><a href="pages/pravlenie.html">Правление</a></li>
      <li><a href="pages/revizion.html">Ревизионная комиссия</a></li>
      <li><a href="pages/vznosy.html">Взносы и платежи</a></li>
      <li><a href="pages/zadolzhennosti.html">Задолженности</a></li>
      <li><a href="pages/documents.html">Документы</a></li>
      <li><a href="gallery.html">Фотогалерея</a></li>
      <li><a href="pages/news.html">Новости</a></li>
      <li><a href="forum.html">Форум</a></li>
      <li><a href="chat.html">Чат</a></li>
      <li><a href="pages/faq.html">Задать вопрос</a></li>
      <li><a href="contact.html">Контакты</a></li>
      <li><a href="voting.html">Голосование</a></li>
      <li><a href="admin.html">Вход в кабинет</a></li>
      <li><a href="https://t.me/SPK_Khoroshovo_1" target="_blank">Telegram чат</a></li>
      <li><a href="https://t.me/SPK_Khoroshovo_Bot" target="_blank">Telegram-бот</a></li>
    </ul>
  </nav>
</header>
<main>
  <section class="intro">
    <h2>Добро пожаловать в СПК «Хорошово-1»!</h2>
    <div class="highlight">
      <strong>Вместе мы создаём комфортную, безопасную и гармоничную среду для жизни и отдыха!</strong><br>
      Последние новости, документы, сервисы для садоводов, интерактивная карта, форум, чат и многое другое — всё на одном сайте.
    </div>
  </section>

  <section>
    <h2>Новости</h2>
    <div id="news-container"><em>Загрузка новостей...</em></div>
  </section>

  <section class="map">
    <h2>Интерактивная карта участков</h2>
    <iframe src="map.html" width="100%" height="450" frameborder="0" style="border-radius: 12px; box-shadow: 0 1px 8px #0077b61a;"></iframe>
  </section>

  <section>
    <h2>Документы</h2>
    <div id="docs-container"><em>Загрузка документов...</em></div>
  </section>

  <section class="question-block">
    <h2>Задать вопрос Правлению</h2>
    <form id="questionForm" action="send_question.php" method="POST" autocomplete="off">
      <input type="text" name="name" placeholder="Ваше имя" required>
      <input type="email" name="email" placeholder="Ваш Email" required>
      <textarea name="message" placeholder="Ваш вопрос" rows="4" required></textarea>
      <div class="captcha">
        <img src="captcha.php" alt="Капча">
        <input type="text" name="captcha" placeholder="Введите код" required>
      </div>
      <button type="submit">Отправить</button>
    </form>
  </section>

  <div class="audio-controls">
    <button id="audio-toggle" aria-pressed="false">Включить звуки природы</button>
  </div>
  <audio id="nature-audio" loop>
    <source src="nature-sounds.mp3" type="audio/mpeg">
    <source src="nature-sounds.ogg" type="audio/ogg">
    Ваш браузер не поддерживает аудио.
  </audio>
</main>

<footer>
  &copy; 2025 СПК «Хорошово-1». Все права защищены.
  <a href="rss.xml">RSS</a>
</footer>
<script>
  // Fade out loader
  document.addEventListener('DOMContentLoaded', function() {
      setTimeout(() => {
          document.querySelector('.loading').style.display = 'none';
      }, 3500);
  }); // Аудио-контроль
  const audio = document.getElementById('nature-audio');
  const btn = document.getElementById('audio-toggle');
  let playing = false;
  btn.addEventListener('click', function () {
    if (!playing) {
      audio.play();
      btn.textContent = "Остановить звуки природы";
      playing = true;
    } else {
      audio.pause();
      btn.textContent = "Включить звуки природы";
      playing = false;
    }
    btn.setAttribute('aria-pressed', playing ? 'true' : 'false');
  });

  // Динамическая загрузка новостей
  fetch('/api/news')
    .then(res => res.json())
    .then(data => {
      const container = document.getElementById('news-container');
      container.innerHTML = '';
      if (!data.length) {
        container.innerHTML = '<p>Новостей пока нет.</p>';
      } else {
        data.reverse().forEach(item => {
          const div = document.createElement('div');
          div.style.marginBottom = '20px';
          div.innerHTML = <h3>${item.title}</h3>
                           <small>${new Date(item.date).toLocaleString()}</small>
                           <p>${item.content}</p>;
          container.appendChild(div);
        });
      }
    })
    .catch(err => {
      document.getElementById('news-container').innerText = 'Ошибка загрузки новостей.';
    });

  // Динамическая загрузка документов
  fetch('/api/docs')
    .then(res => res.json())
    .then(data => {
      const container = document.getElementById('docs-container');
      container.innerHTML = '';
      if (!data.length) {
        container.innerHTML = '<p>Документов пока нет.</p>';
      } else {
        const ul = document.createElement('ul');
        data.forEach(doc => {
          const li = document.createElement('li');
          li.innerHTML = <a href="/docs/${doc.filename}" target="_blank">${doc.title}</a>;
          ul.appendChild(li);
        });
        container.appendChild(ul);
      }
    })
    .catch(err => {
      document.getElementById('docs-container').innerText = 'Ошибка загрузки документов.';
    });
</script>
</body>
</html> const express = require('express');
const session = require('express-session');
const bodyParser = require('body-parser');
const fs = require('fs');
const path = require('path');

const app = express();
const PORT = 3000;
app.use(express.static('public'));
app.use(bodyParser.urlencoded({ extended: true }));
app.use(bodyParser.json());

app.use(session({
  secret: 'secret-key',
  resave: false,
  saveUninitialized: true,
  cookie: { secure: false }
}));

const USERNAME = 'admin';
const PASSWORD = '1234';

function isAuthenticated(req, res, next) {
  if (req.session && req.session.user === USERNAME) return next();
  else res.redirect('/login.html');
}

// Авторизация
app.post('/login', (req, res) => {
  const { username, password } = req.body;
  if (username === USERNAME && password === PASSWORD) {
    req.session.user = username;
    res.redirect('/admin.html');
  } else {
    res.send('Неверный логин или пароль');
  }
});

// Защита admin.html
app.get('/admin.html', isAuthenticated, (req, res) => {
  res.sendFile(path.join(__dirname, 'public', 'admin.html'));
});

// API для новостей (для клиента)
app.get('/api/news', (req, res) => {
  const newsPath = path.join(__dirname, 'public', 'news.json');
  if (!fs.existsSync(newsPath)) fs.writeFileSync(newsPath, '[]');
  const news = JSON.parse(fs.readFileSync(newsPath, 'utf-8'));
  res.json(news);
});
// API для документов
app.get('/api/docs', (req, res) => {
  const docsPath = path.join(__dirname, 'public', 'docs.json');
  if (!fs.existsSync(docsPath)) fs.writeFileSync(docsPath, '[]');
  const docs = JSON.parse(fs.readFileSync(docsPath, 'utf8'));
  res.json(docs);
});
// Добавление новости (только из админки)
app.post('/api/admin/news', isAuthenticated, (req, res) => {
  const { title, content } = req.body;
  const newsPath = path.join(__dirname, 'public', 'news.json');
  if (!fs.existsSync(newsPath)) fs.writeFileSync(newsPath, '[]');
  const news = JSON.parse(fs.readFileSync(newsPath, 'utf-8'));
  news.push({ title, content, date: new Date().toISOString() });
  fs.writeFileSync(newsPath, JSON.stringify(news, null, 2));
  res.json({ status: 'success' });
});
app.listen(PORT, () => {
  console.log(Сервер запущен на http://localhost:${PORT});
}); <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Админ-панель</title>
  <script>
    function submitNews() {
      const title = document.getElementById('title').value;
      const content = document.getElementById('content').value;
      fetch('/api/admin/news', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ title, content })
      }).then(res => res.json())
        .then(data => alert('Новость добавлена!'))
        .catch(err => alert('Ошибка: ' + err));
    }
  </script>
</head>
<body>
  <h1>Админ-панель</h1>
  <input type="text" id="title" placeholder="Заголовок новости"><br>
  <textarea id="content" placeholder="Текст новости"></textarea><br>
  <button onclick="submitNews()">Добавить новость</button>
</body>
</html> <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Вход в админку</title>
</head>
<body>
  <h2>Авторизация</h2>
  <form action="/login" method="POST">
    <label>Логин: <input type="text" name="username"></label><br>
    <label>Пароль: <input type="password" name="password"></label><br>
    <button type="submit">Войти</button>
  </form>
</body>
</html> [ [] 
  {"filename": "ustav.pdf", "title": "Устав"},
  {"filename": "protokol1.pdf", "title": "Протокол №1"}
] /public
 ├── gallery/
 │    ├── photo1.jpg
 │    ├── photo2.jpg
 ├── gallery.html <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Фотогалерея СПК «Хорошово-1»</title>
  <style>
    body {
      font-family: sans-serif;
      padding: 20px;
    }
    h1 {
      margin-bottom: 20px;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
      gap: 15px;
    }
    .gallery img {
      width: 100%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
      transition: transform 0.2s;
    }
    .gallery img:hover {
      transform: scale(1.03);
    }
  </style>
</head>
<body>
  <h1>Фотогалерея СПК «Хорошово-1»</h1>
  <div class="gallery" id="gallery-container">Загрузка...</div>

  <script>
    fetch('/api/gallery')
      .then(res => res.json())
      .then(images => {
        const container = document.getElementById('gallery-container');
        container.innerHTML = '';
        if (images.length === 0) {
          container.innerHTML = '<p>Фотографий пока нет.</p>';
        } else {
          images.forEach(img => {
            const image = document.createElement('img');
            image.src = '/gallery/' + img;
            container.appendChild(image);
          });
        }
      })
      .catch(err => {
        console.error(err);
        document.getElementById('gallery-container').innerText = 'Ошибка загрузки фотографий.';
      });
  </script>
</body>
</html> app.get('/api/gallery', (req, res) => {
  const dirPath = path.join(__dirname, 'public', 'gallery');
  fs.readdir(dirPath, (err, files) => {
    if (err) {
      console.error(err);
      return res.json([]);
    }
    // Фильтрация только изображений
    const images = files.filter(f => /\.(jpg|jpeg|png|gif)$/i.test(f));
    res.json(images);
  });
}); <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Обратная связь — СПК «Хорошово-1»</title>
  <style>
    body { font-family: sans-serif; padding: 20px; }
    h1 { margin-bottom: 20px; }
    form { max-width: 500px; }
    input, textarea {
      width: 100%;
      margin-bottom: 10px;
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    button {
      padding: 10px 20px;
      background: #0077cc;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .success { color: green; margin-top: 10px; }
    .error { color: red; margin-top: 10px; }
  </style>
</head>
<body>
  <h1>Связаться с нами</h1>
  <form id="contact-form">
    <input type="text" name="name" placeholder="Ваше имя" required>
    <input type="email" name="email" placeholder="Ваш Email" required>
    <textarea name="message" placeholder="Ваше сообщение" rows="6" required></textarea>
    <button type="submit">Отправить</button>
    <div id="status"></div>
  </form>

  <script>
    document.getElementById('contact-form').addEventListener('submit', async (e) => {
      e.preventDefault();
      const form = e.target;
      const data = {
        name: form.name.value,
        email: form.email.value,
        message: form.message.value
      };
      const res = await fetch('/api/contact', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify(data)
      });
      const result = await res.json();
      const statusDiv = document.getElementById('status');
      if (res.ok) {
        statusDiv.className = 'success';
        statusDiv.textContent = 'Сообщение отправлено. Спасибо!';
        form.reset();
      } else {
        statusDiv.className = 'error';
        statusDiv.textContent = result.error || 'Ошибка при отправке.';
      }
    });
  </script>
</body>
</html> npm install nodemailer const nodemailer = require('nodemailer');

app.post('/api/contact', express.json(), async (req, res) => {
  const { name, email, message } = req.body;
  if (!name || !email || !message) {
    return res.status(400).json({ error: 'Все поля обязательны' });
  }

  try {
    const transporter = nodemailer.createTransport({
      service: 'gmail',
      auth: {
        user: 'your_email@gmail.com',
        pass: 'your_app_password'
      }
    });

    await transporter.sendMail({
      from: `"Сайт СПК" <your_email@gmail.com>`,
      to: 'recipient_email@gmail.com',
      subject: `Новое сообщение от ${name}`,
      text: `Email: ${email}\n\nСообщение:\n${message}`
    });

    res.json({ success: true });
  } catch (error) {
    console.error('Ошибка при отправке:', error);
    res.status(500).json({ error: 'Ошибка при отправке письма' });
  }
}); <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Голосование — СПК «Хорошово-1»</title>
  <style>
    body { font-family: sans-serif; padding: 20px; }
    h1 { margin-bottom: 10px; }
    .option {
      margin-bottom: 10px;
    }
    button {
      padding: 10px 20px;
      background: #0077cc;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    #result { margin-top: 20px; font-weight: bold; }
  </style>
</head>
<body>
  <h1>Поддерживаете ли вы установку видеонаблюдения?</h1>
  <form id="vote-form">
    <div class="option">
      <input type="radio" name="vote" value="yes" id="yes" required>
      <label for="yes">Да</label>
    </div>
    <div class="option">
      <input type="radio" name="vote" value="no" id="no">
      <label for="no">Нет</label>
    </div>
    <button type="submit">Проголосовать</button>
  </form>
  <div id="result"></div>

  <script>
    document.getElementById('vote-form').addEventListener('submit', async (e) => {
      e.preventDefault();
      const form = e.target;
      const vote = form.vote.value;
      const res = await fetch('/api/vote', {
        method: 'POST',
        headers: { 'Content-Type': 'application/json' },
        body: JSON.stringify({ vote })
      });
      const data = await res.json();
      document.getElementById('result').textContent = data.message;
      form.reset();
    });
  </script>
</body>
</html> const fs = require('fs');
const voteFile = './votes.json';

// Инициализируем файл, если не существует
if (!fs.existsSync(voteFile)) {
  fs.writeFileSync(voteFile, JSON.stringify({ yes: 0, no: 0 }));
}

app.post('/api/vote', express.json(), (req, res) => {
  const { vote } = req.body;
  if (!['yes', 'no'].includes(vote)) {
    return res.status(400).json({ message: 'Недопустимый голос' });
  }

  const votes = JSON.parse(fs.readFileSync(voteFile));
  votes[vote]++;
  fs.writeFileSync(voteFile, JSON.stringify(votes));

  res.json({ message: 'Спасибо, ваш голос учтён!' });
}); <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Результаты голосования</title>
</head>
<body>
  <h1>Результаты голосования</h1>
  <div id="results"></div>

  <script>
    fetch('/votes.json')
      .then(res => res.json())
      .then(data => {
        document.getElementById('results').innerHTML =
          `<p>Да: ${data.yes}</p><p>Нет: ${data.no}</p>`;
      });
  </script>
</body>
</html> public/
├── docs/
│   ├── ustav.pdf
│   ├── protokol-2024-05-01.pdf
│   └── otchet-audita.pdf <!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Документы СПК «Хорошово-1»</title>
  <style>
    body { font-family: sans-serif; padding: 20px; }
    h1 { margin-bottom: 10px; }
    ul { list-style: none; padding-left: 0; }
    li { margin-bottom: 10px; }
    a { color: #0077cc; text-decoration: none; }
    a:hover { text-decoration: underline; }
  </style>
</head>
<body>
  <h1>Официальные документы</h1>
  <ul>
    <li><a href="/docs/ustav.pdf" target="_blank">Устав СПК «Хорошово-1» (PDF)</a></li>
    <li><a href="/docs/protokol-2024-05-01.pdf" target="_blank">Протокол общего собрания от 1 мая 2024</a></li>
    <li><a href="/docs/otchet-audita.pdf" target="_blank">Отчет аудитора за 2024 г.</a></li>
  </ul>
</body>
</html> 
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <title>Карта сайта — СПК «Хорошово-1»</title>
  <style>
    body { font-family: sans-serif; padding: 20px; line-height: 1.6; }
    h1 { margin-bottom: 10px; }
    ul { padding-left: 20px; }
    a { color: #0077cc; text-decoration: none; }
    a:hover { text-decoration: underline; }
  </style>
</head>
<body>
  <h1>Карта сайта</h1>
  <ul>
    <li><a href="/index.html">Главная</a></li>
    <li><a href="/gallery.html">Фотогалерея</a></li>
    <li><a href="/docs.html">Документы</a></li>
    <li><a href="/vote.html">Голосование</a></li>
    <li><a href="/contact.html">Обратная связь</a></li>
  </ul>
</body>
</html> <p><a href="/sitemap.html">Карта сайта</a></p> <footer style="margin-top: 40px; border-top: 1px solid #ccc; padding-top: 10px;">
  <p>Мы в соцсетях:</p>
  <a href="https://vk.com/club228905465" target="_blank">ВКонтакте</a> |
  <a href="mailto:spk@example.com">E-mail</a>
</footer> <footer style="margin-top: 40px; border-top: 1px solid #ccc; padding-top: 10px;">
  <p>Мы в соцсетях:</p>
  <a href="https://vk.com/club228905465" target="_blank">ВКонтакте</a> |
  <a href="https://t.me/SPK_Khoroshovo_Bot" target="_blank">@SPK_Khoroshovo_Bot</a> |
  <a href="https://t.me/SPK_Khoroshovo_1" target="_blank">@SPK_Khoroshovo_1</a> |
  <a href="mailto:spk@example.com">E-mail</a>
</footer> <footer style="margin-top: 40px; border-top: 1px solid #ccc; padding-top: 10px;">
  <p>Мы в соцсетях:</p>
  <a href="https://vk.com/club228905465" target="_blank">ВКонтакте</a> |
  <a href="https://t.me/SPK_Khoroshovo_Bot" target="_blank">@SPK_Khoroshovo_Bot</a> |
  <a href="https://t.me/SPK_Khoroshovo_1" target="_blank">@SPK_Khoroshovo_1</a> |
  <a href="mailto:spk.horoshovo-1@yandex.ru">E-mail: spk.horoshovo-1@yandex.ru</a>
  </footer> 
