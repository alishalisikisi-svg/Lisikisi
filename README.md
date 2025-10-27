<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Alina Web Studio — Создание современных сайтов</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');
  * { margin: 0; padding: 0; box-sizing: border-box; }
  body {
    font-family: 'Inter', sans-serif;
    color: #222;
    background: #f9f9fb;
    overflow-x: hidden;
    scroll-behavior: smooth;
  }
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 60px;
    background: white;
    box-shadow: 0 2px 10px rgba(0,0,0,0.05);
    position: sticky;
    top: 0;
    z-index: 10;
  }
  header h1 {
    font-size: 1.5rem;
    font-weight: 700;
    color: #0078ff;
  }
  nav a {
    margin-left: 30px;
    text-decoration: none;
    color: #333;
    font-weight: 500;
    transition: color 0.3s;
  }
  nav a:hover { color: #0078ff; }
  section {
    padding: 100px 60px;
    max-width: 1100px;
    margin: 0 auto;
  }
  #hero {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    background: linear-gradient(135deg, #0078ff, #00c6ff);
    color: white;
    border-radius: 0 0 60px 60px;
    padding: 140px 20px;
  }
  #hero h2 { font-size: 2.8rem; margin-bottom: 20px; }
  #hero p { font-size: 1.2rem; max-width: 600px; opacity: 0.9; }
  #about {
    background: white;
    border-radius: 20px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.05);
    text-align: center;
  }
  #about h3 { font-size: 2rem; margin-bottom: 20px; color: #0078ff; }
  #about p { font-size: 1.1rem; line-height: 1.6; }
  #services h3, #portfolio h3, #contact h3 {
    font-size: 2rem;
    text-align: center;
    color: #0078ff;
    margin-bottom: 40px;
  }
  .service-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 30px;
  }
  .service {
    background: white;
    border-radius: 20px;
    box-shadow: 0 4px 15px rgba(0,0,0,0.05);
    padding: 30px;
    transition: transform 0.3s;
  }
  .service:hover { transform: translateY(-8px); }
  .service h4 { margin-bottom: 10px; color: #222; }
  .service p { font-size: 0.95rem; color: #555; }

  /* Portfolio */
  .portfolio-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 25px;
  }
  .portfolio-item {
    background: white;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 4px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s;
  }
  .portfolio-item:hover { transform: scale(1.03); }
  .portfolio-item img {
    width: 100%;
    height: 200px;
    object-fit: cover;
  }
  .portfolio-content {
    padding: 20px;
  }
  .portfolio-content h4 {
    color: #0078ff;
    margin-bottom: 10px;
  }
  .portfolio-content p {
    font-size: 0.95rem;
    color: #555;
  }

  /* Contact */
  #contact form {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 15px;
    max-width: 500px;
    margin: 0 auto;
  }
  input, textarea {
    width: 100%;
    padding: 12px 15px;
    border: 1px solid #ccc;
    border-radius: 8px;
    font-size: 1rem;
    font-family: inherit;
  }
  button {
    background: #0078ff;
    color: white;
    border: none;
    padding: 12px 25px;
    border-radius: 8px;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.3s;
  }
  button:hover { background: #005fcc; }
  footer {
    text-align: center;
    padding: 30px;
    font-size: 0.9rem;
    color: #666;
  }
  @media (max-width: 768px) {
    header { flex-direction: column; padding: 15px 20px; }
    nav a { margin: 10px; display: inline-block; }
    section { padding: 80px 20px; }
    #hero h2 { font-size: 2.2rem; }
  }
</style>
</head>
<body>
  <header>
    <h1>Alina Web Studio</h1>
    <nav>
      <a href="#hero">Главная</a>
      <a href="#about">Обо мне</a>
      <a href="#services">Услуги</a>
      <a href="#portfolio">Портфолио</a>
      <a href="#contact">Контакты</a>
    </nav>
  </header>

  <section id="hero">
    <h2>Создаю современные и стильные сайты</h2>
    <p>Помогаю бизнесам и личным брендам заявить о себе в интернете с помощью дизайна, структуры и функционала, которые действительно работают.</p>
  </section>

  <section id="about">
    <h3>Обо мне</h3>
    <p>Привет! Меня зовут <strong>Алина</strong>.  
    Я — веб-разработчик, создаю сайты «под ключ»: от идеи и дизайна до адаптации под телефон и публикации в интернете.  
    Мне важно, чтобы каждый сайт был не просто красивым, а удобным, понятным и работающим на результат.</p>
  </section>

  <section id="services">
    <h3>Мои услуги</h3>
    <div class="service-list">
      <div class="service">
        <h4>Сайт-визитка</h4>
        <p>Идеален для личного бренда, специалиста или малого бизнеса. Лаконичный, современный и быстрый сайт.</p>
      </div>
      <div class="service">
        <h4>Корпоративный сайт</h4>
        <p>Сайт компании с описанием услуг, команды и контактами. Полностью адаптивный и SEO-оптимизированный.</p>
      </div>
      <div class="service">
        <h4>Интернет-магазин</h4>
        <p>Полноценный магазин с корзиной, оплатой и админкой. Простое управление товарами и заказами.</p>
      </div>
      <div class="service">
        <h4>Редизайн и улучшение</h4>
        <p>Если у вас уже есть сайт, помогу улучшить структуру, дизайн и скорость загрузки.</p>
      </div>
    </div>
  </section>

  <section id="portfolio">
    <h3>Портфолио</h3>
    <div class="portfolio-grid">
      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1504674900247-0877df9cc836" alt="Сайт кофейни">
        <div class="portfolio-content">
          <h4>Сайт кофейни «Aroma Beans»</h4>
          <p>Тёплый уютный дизайн в пастельных тонах. Адаптивная верстка, раздел меню, отзывы клиентов и онлайн-бронирование столика.</p>
        </div>
      </div>
      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1616469829935-c2f8cf289bb7" alt="Лендинг косметолога">
        <div class="portfolio-content">
          <h4>Лендинг косметолога</h4>
          <p>Современный минимализм, мягкие цвета и анимация. Сайт привлекает клиентов с Instagram и упрощает запись на приём.</p>
        </div>
      </div>
      <div class="portfolio-item">
        <img src="https://images.unsplash.com/photo-1607083206965-8e9b5e7d9d3a" alt="Интернет-магазин аксессуаров">
        <div class="portfolio-content">
          <h4>Интернет-магазин аксессуаров «Glow»</h4>
          <p>Магазин с корзиной и оплатой. Простое добавление товаров, стильный интерфейс и лёгкая навигация.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <h3>Связаться со мной</h3>
    <form onsubmit="event.preventDefault(); alert('Спасибо! Я свяжусь с вами.');">
      <input type="text" placeholder="Ваше имя" required />
      <input type="email" placeholder="Ваш email" required />
      <textarea rows="4" placeholder="Ваше сообщение" required></textarea>
      <button type="submit">Отправить</button>
    </form>
  </section>

  <footer>
    © 2025 Alina Web Studio. Все права защищены.
  </footer>
</body>
</html>
