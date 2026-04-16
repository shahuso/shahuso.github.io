<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>География × Литература — межпредметные связи 5–9 класс</title>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600&family=Golos+Text:wght@400;500;600&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box;margin:0;padding:0}
:root{
  --bg:#fafaf8;
  --bg2:#f2f1ec;
  --bg3:#e8e6df;
  --white:#ffffff;
  --text:#1c1c1a;
  --text2:#5a5a55;
  --text3:#9a9a93;
  --accent:#2d6a4f;
  --accent2:#40916c;
  --accent-light:#d8f3dc;
  --accent-dark:#1b4332;
  --warm:#b5451b;
  --border:#dddcd5;
  --border2:#c8c7be;
  --radius:10px;
  --radius-lg:16px;
  --shadow:0 2px 12px rgba(0,0,0,.07);
  --shadow-lg:0 8px 32px rgba(0,0,0,.10);
}
html{scroll-behavior:smooth}
body{font-family:'Golos Text',sans-serif;background:var(--bg);color:var(--text);line-height:1.6;font-size:16px}

/* ─── NAV ─── */
nav{
  position:sticky;top:0;z-index:200;
  background:rgba(250,250,248,.92);
  backdrop-filter:blur(12px);
  border-bottom:1px solid var(--border);
  padding:0 2rem;
}
.nav-inner{max-width:1200px;margin:0 auto;display:flex;align-items:center;justify-content:space-between;height:56px}
.nav-logo{font-family:'Playfair Display',serif;font-size:17px;font-weight:600;color:var(--accent-dark);text-decoration:none;letter-spacing:-.01em}
.nav-logo span{color:var(--warm)}
.nav-links{display:flex;gap:0;list-style:none}
.nav-links a{display:block;padding:0 14px;font-size:13px;font-weight:500;color:var(--text2);text-decoration:none;height:56px;line-height:56px;border-bottom:2px solid transparent;transition:color .15s,border-color .15s}
.nav-links a:hover{color:var(--accent);border-bottom-color:var(--accent)}
.nav-burger{display:none;background:none;border:none;cursor:pointer;padding:4px;color:var(--text)}

/* ─── HERO ─── */
.hero{
  background:var(--accent-dark);
  color:#fff;
  padding:80px 2rem 72px;
  position:relative;
  overflow:hidden;
}
.hero::before{
  content:'';position:absolute;inset:0;
  background:repeating-linear-gradient(45deg,rgba(255,255,255,.02) 0,rgba(255,255,255,.02) 1px,transparent 0,transparent 50%);
  background-size:20px 20px;
}
.hero-inner{max-width:760px;margin:0 auto;position:relative;text-align:center}
.hero-tag{display:inline-block;padding:4px 14px;border-radius:20px;background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);font-size:12px;font-weight:500;letter-spacing:.06em;text-transform:uppercase;margin-bottom:24px;color:rgba(255,255,255,.85)}
.hero h1{font-family:'Playfair Display',serif;font-size:clamp(28px,5vw,48px);font-weight:600;line-height:1.2;margin-bottom:20px;letter-spacing:-.02em}
.hero h1 em{font-style:normal;color:#95d5b2}
.hero p{font-size:17px;color:rgba(255,255,255,.75);max-width:580px;margin:0 auto 36px;line-height:1.7}
.hero-cta{display:inline-flex;align-items:center;gap:8px;padding:13px 28px;background:#fff;color:var(--accent-dark);border-radius:var(--radius);font-weight:600;font-size:15px;text-decoration:none;transition:transform .15s,box-shadow .15s}
.hero-cta:hover{transform:translateY(-2px);box-shadow:0 8px 24px rgba(0,0,0,.2)}
.hero-cta svg{width:16px;height:16px}
.hero-stats{display:flex;justify-content:center;gap:40px;margin-top:52px;padding-top:40px;border-top:1px solid rgba(255,255,255,.12)}
.hero-stat-n{font-family:'Playfair Display',serif;font-size:32px;font-weight:600;color:#fff;display:block}
.hero-stat-l{font-size:13px;color:rgba(255,255,255,.55)}

/* ─── SECTIONS ─── */
section{padding:72px 2rem}
.section-inner{max-width:1200px;margin:0 auto}
.section-label{font-size:11px;font-weight:600;letter-spacing:.1em;text-transform:uppercase;color:var(--accent);margin-bottom:10px}
.section-title{font-family:'Playfair Display',serif;font-size:clamp(22px,3vw,32px);font-weight:600;line-height:1.25;margin-bottom:16px;letter-spacing:-.02em}
.section-lead{font-size:16px;color:var(--text2);max-width:620px;line-height:1.75}

/* ─── ABOUT ─── */
#about{background:var(--white)}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px;align-items:start;margin-top:48px}
.about-cards{display:flex;flex-direction:column;gap:16px}
.about-card{background:var(--bg);border:1px solid var(--border);border-radius:var(--radius-lg);padding:22px 24px;display:flex;gap:16px;align-items:flex-start}
.about-icon{width:40px;height:40px;border-radius:10px;background:var(--accent-light);display:flex;align-items:center;justify-content:center;flex-shrink:0;font-size:18px}
.about-card-title{font-weight:600;font-size:14px;margin-bottom:4px}
.about-card-text{font-size:13px;color:var(--text2);line-height:1.6}
.about-frp{background:var(--bg2);border:1px solid var(--border);border-radius:var(--radius-lg);padding:28px}
.about-frp-title{font-weight:600;font-size:14px;margin-bottom:14px;color:var(--text)}
.frp-list{list-style:none;display:flex;flex-direction:column;gap:8px}
.frp-list li{display:flex;align-items:center;gap:10px;font-size:13px;color:var(--text2)}
.frp-dot{width:8px;height:8px;border-radius:50%;background:var(--accent);flex-shrink:0}

/* ─── HOW TO ─── */
#howto{background:var(--bg2)}
.steps{display:grid;grid-template-columns:repeat(3,1fr);gap:24px;margin-top:40px}
.step{background:var(--white);border:1px solid var(--border);border-radius:var(--radius-lg);padding:28px 24px;position:relative}
.step-num{font-family:'Playfair Display',serif;font-size:40px;font-weight:600;color:var(--accent-light);line-height:1;margin-bottom:12px}
.step-title{font-weight:600;font-size:15px;margin-bottom:8px}
.step-text{font-size:13px;color:var(--text2);line-height:1.65}

/* ─── TABLE SECTION ─── */
#table{background:var(--white)}
.table-wrap-outer{margin-top:40px}

/* ─── TABLE INTERNALS ─── */
.tw-controls{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:12px;align-items:flex-start}
.tw-controls select,.tw-controls input{
  padding:7px 11px;font-size:13px;
  border:1px solid var(--border2);border-radius:var(--radius);
  background:var(--white);color:var(--text);
  font-family:'Golos Text',sans-serif;
  outline:none;transition:border-color .15s;
}
.tw-controls select:focus,.tw-controls input:focus{border-color:var(--accent)}
.tw-srow{display:flex;gap:8px;margin-bottom:12px;flex-wrap:wrap}
.tw-sc{background:var(--bg2);border-radius:var(--radius);padding:10px 16px;flex:1;min-width:90px;border:1px solid var(--border)}
.tw-sl{font-size:11px;color:var(--text2);margin-bottom:2px}
.tw-sv{font-size:20px;font-weight:600;color:var(--text);font-family:'Playfair Display',serif}
.dd-wrap{position:relative;min-width:220px}
.dd-btn{width:100%;padding:7px 11px;font-size:13px;border:1px solid var(--border2);border-radius:var(--radius);background:var(--white);color:var(--text);cursor:pointer;text-align:left;display:flex;justify-content:space-between;align-items:center;gap:6px;font-family:'Golos Text',sans-serif;outline:none;transition:border-color .15s}
.dd-btn:hover{border-color:var(--accent)}
.dd-arrow{font-size:10px;color:var(--text3);transition:transform .15s}
.dd-arrow.open{transform:rotate(180deg)}
.dd-panel{display:none;position:absolute;top:calc(100% + 4px);left:0;min-width:300px;background:var(--white);border:1px solid var(--border2);border-radius:var(--radius-lg);box-shadow:var(--shadow-lg);z-index:9999;padding:8px;max-height:420px;overflow-y:auto}
.dd-panel.open{display:block}
.dd-group{margin-bottom:8px}
.dd-group:last-of-type{margin-bottom:0}
.dd-group-label{font-size:12px;font-weight:500;color:var(--text);padding:5px 8px;margin-bottom:4px;cursor:pointer;border-radius:var(--radius);display:flex;align-items:center;justify-content:space-between;gap:6px;border:1px solid var(--border);background:var(--bg2);transition:background .12s,border-color .12s;user-select:none}
.dd-group-label:hover{border-color:var(--border2);background:var(--bg3)}
.dd-group-label.all-on{background:var(--accent-light);border-color:#74c69d;color:var(--accent-dark)}
.dd-group-label.some-on{border-color:#74c69d}
.group-check{font-size:10px;color:var(--text3);white-space:nowrap;flex-shrink:0}
.dd-group-label.all-on .group-check{color:var(--accent)}
.dd-group-label.some-on .group-check{color:var(--accent2)}
.dd-tags{display:flex;flex-wrap:wrap;gap:4px;padding:0 4px 2px}
.tg{padding:3px 8px;border-radius:20px;font-size:11px;border:1px solid var(--border2);cursor:pointer;background:var(--white);color:var(--text2);transition:all .1s;white-space:nowrap;font-family:'Golos Text',sans-serif}
.tg:hover{border-color:var(--accent);color:var(--text)}
.tg.on{background:var(--accent);color:#fff;border-color:var(--accent)}
.dd-clear{width:100%;padding:6px;font-size:11px;color:var(--text3);background:none;border:none;cursor:pointer;text-align:center;border-top:1px solid var(--border);margin-top:6px;padding-top:8px;font-family:'Golos Text',sans-serif}
.dd-clear:hover{color:var(--text)}
.active-tags{display:flex;flex-wrap:wrap;gap:4px;margin-bottom:10px;min-height:0}
.active-tag{padding:3px 10px;border-radius:20px;font-size:11px;background:var(--accent);color:#fff;cursor:pointer;display:flex;align-items:center;gap:4px}
.active-tag-x{font-size:10px;opacity:.75}
.tw-outer{overflow-x:auto;border:1px solid var(--border);border-radius:var(--radius-lg);box-shadow:var(--shadow)}
table{width:100%;border-collapse:collapse;font-size:13px;table-layout:fixed}
thead tr{background:var(--bg2)}
thead th{padding:10px 12px;text-align:left;font-weight:600;font-size:11px;color:var(--text2);border-bottom:1px solid var(--border2);white-space:nowrap;letter-spacing:.03em;text-transform:uppercase}
th:nth-child(1){width:6%}th:nth-child(2){width:13%}th:nth-child(3){width:17%}th:nth-child(4){width:24%}th:nth-child(5){width:40%}
tbody tr{border-bottom:1px solid var(--border);transition:background .1s}
tbody tr:last-child{border-bottom:none}
tbody tr:hover{background:#f7faf8}
td{padding:10px 12px;vertical-align:top;color:var(--text);line-height:1.5;word-break:break-word}
.cb{display:inline-block;padding:2px 9px;border-radius:20px;font-size:11px;font-weight:600}
.c5{background:#FBEAF0;color:#72243E}.c6{background:#FAEEDA;color:#633806}.c7{background:#EAF3DE;color:#27500A}.c8{background:#E6F1FB;color:#0C447C}.c9{background:#d8f3dc;color:#1b4332}
.sb{display:inline-block;padding:2px 8px;border-radius:6px;font-size:11px;background:var(--bg2);color:var(--text2);border:1px solid var(--border)}
.wl{display:flex;flex-direction:column;gap:3px}
.wi{font-size:12px;color:var(--text2);padding:2px 0;line-height:1.5}
.wi strong{color:var(--text);font-weight:600}
.al{display:flex;flex-direction:column;gap:3px}
.ai{font-size:12px;padding:3px 10px;background:var(--bg);border-radius:0;border-left:2px solid var(--accent2);color:var(--text);line-height:1.55}
.gt{font-size:13px;font-weight:600;color:var(--text);margin-bottom:2px}
.tw-empty{text-align:center;padding:3rem;color:var(--text3);font-size:14px}

/* ─── FEEDBACK ─── */
#feedback{background:var(--accent-dark);color:#fff}
#feedback .section-label{color:#95d5b2}
#feedback .section-title{color:#fff}
#feedback .section-lead{color:rgba(255,255,255,.65)}
.feedback-grid{display:grid;grid-template-columns:1fr 1fr;gap:48px;margin-top:48px;align-items:start}
.feedback-why{display:flex;flex-direction:column;gap:16px}
.fwhy-item{display:flex;gap:12px;align-items:flex-start}
.fwhy-dot{width:6px;height:6px;border-radius:50%;background:#95d5b2;margin-top:7px;flex-shrink:0}
.fwhy-text{font-size:14px;color:rgba(255,255,255,.7);line-height:1.65}
.feedback-form{background:rgba(255,255,255,.06);border:1px solid rgba(255,255,255,.12);border-radius:var(--radius-lg);padding:32px}
.form-group{margin-bottom:18px}
.form-label{display:block;font-size:12px;font-weight:600;letter-spacing:.04em;text-transform:uppercase;color:rgba(255,255,255,.55);margin-bottom:7px}
.form-input,.form-textarea,.form-select{
  width:100%;padding:10px 14px;
  background:rgba(255,255,255,.08);
  border:1px solid rgba(255,255,255,.15);
  border-radius:var(--radius);
  color:#fff;font-size:14px;
  font-family:'Golos Text',sans-serif;
  outline:none;transition:border-color .15s;
}
.form-input::placeholder,.form-textarea::placeholder{color:rgba(255,255,255,.3)}
.form-input:focus,.form-textarea:focus,.form-select:focus{border-color:rgba(255,255,255,.4)}
.form-textarea{resize:vertical;min-height:110px;line-height:1.6}
.form-select option{background:#1b4332;color:#fff}
.form-submit{width:100%;padding:13px;background:#fff;color:var(--accent-dark);border:none;border-radius:var(--radius);font-size:15px;font-weight:600;font-family:'Golos Text',sans-serif;cursor:pointer;transition:transform .15s,opacity .15s}
.form-submit:hover{transform:translateY(-1px);opacity:.92}
.form-submit:active{transform:translateY(0)}
.form-success{display:none;text-align:center;padding:24px;background:rgba(149,213,178,.12);border:1px solid rgba(149,213,178,.3);border-radius:var(--radius);color:#95d5b2;font-size:14px;line-height:1.6}

/* ─── FOOTER ─── */
footer{background:#111;color:rgba(255,255,255,.4);padding:32px 2rem;text-align:center;font-size:13px}
footer a{color:rgba(255,255,255,.5);text-decoration:none}
footer a:hover{color:#fff}
.footer-inner{max-width:1200px;margin:0 auto;display:flex;flex-direction:column;gap:8px;align-items:center}
.footer-logo{font-family:'Playfair Display',serif;font-size:15px;color:rgba(255,255,255,.6);margin-bottom:4px}

/* ─── RESPONSIVE ─── */
@media(max-width:768px){
  .about-grid,.feedback-grid{grid-template-columns:1fr}
  .steps{grid-template-columns:1fr}
  .hero-stats{gap:24px}
  .nav-links{display:none}
  .nav-burger{display:block}
  th:nth-child(2){display:none}td:nth-child(2){display:none}
  th:nth-child(1){width:8%}th:nth-child(3){width:20%}th:nth-child(4){width:28%}th:nth-child(5){width:44%}
}

/* ─── ANIMATIONS ─── */
@keyframes fadeUp{from{opacity:0;transform:translateY(20px)}to{opacity:1;transform:translateY(0)}}
.hero-inner>*{animation:fadeUp .5s ease both}
.hero-tag{animation-delay:.05s}.hero h1{animation-delay:.12s}.hero p{animation-delay:.2s}.hero-cta{animation-delay:.28s}.hero-stats{animation-delay:.36s}
</style>
</head>
<body>

<!-- NAV -->
<nav>
  <div class="nav-inner">
    <a class="nav-logo" href="#">География <span>×</span> Литература</a>
    <ul class="nav-links">
      <li><a href="#about">О проекте</a></li>
      <li><a href="#howto">Как пользоваться</a></li>
      <li><a href="#table">Таблица</a></li>
      <li><a href="#feedback">Предложить идею</a></li>
    </ul>
    <button class="nav-burger" onclick="document.querySelector('.nav-links').style.display=document.querySelector('.nav-links').style.display==='flex'?'none':'flex'">
      <svg width="20" height="20" viewBox="0 0 20 20" fill="none"><path d="M2 5h16M2 10h16M2 15h16" stroke="currentColor" stroke-width="1.5" stroke-linecap="round"/></svg>
    </button>
  </div>
</nav>

<!-- HERO -->
<section class="hero">
  <div class="hero-inner">
    <span class="hero-tag">Межпредметные связи</span>
    <h1>Как связать <em>географию</em><br>и литературу на уроке</h1>
    <p>Справочник для учителей географии 5–9 классов. Все темы ФРП — с подобранными произведениями и конкретными аспектами интеграции.</p>
    <a href="#table" class="hero-cta">
      <svg viewBox="0 0 16 16" fill="none" stroke="currentColor" stroke-width="2"><path d="M8 3v10M3 8l5 5 5-5"/></svg>
      Открыть таблицу
    </a>
    <div class="hero-stats">
      <div><span class="hero-stat-n">35</span><span class="hero-stat-l">тем по географии</span></div>
      <div><span class="hero-stat-n">120+</span><span class="hero-stat-l">произведений</span></div>
      <div><span class="hero-stat-n">5</span><span class="hero-stat-l">классов (5–9)</span></div>
    </div>
  </div>
</section>

<!-- ABOUT -->
<section id="about">
  <div class="section-inner">
    <div class="section-label">О проекте</div>
    <h2 class="section-title">Зачем нужен этот справочник</h2>
    <p class="section-lead">ФГОС требует реализации межпредметных связей, но найти конкретные произведения под конкретную тему географии — долго. Здесь всё собрано в одном месте.</p>
    <div class="about-grid">
      <div class="about-cards">
        <div class="about-card">
          <div class="about-icon">📚</div>
          <div>
            <div class="about-card-title">Привязка к ФРП</div>
            <div class="about-card-text">Каждая строка таблицы соответствует конкретному разделу и теме федеральной рабочей программы по географии 5–9 классов.</div>
          </div>
        </div>
        <div class="about-card">
          <div class="about-icon">🔍</div>
          <div>
            <div class="about-card-title">Аспекты интеграции</div>
            <div class="about-card-text">Для каждого произведения указано не просто «подходит», а конкретно — какой географический факт или понятие можно раскрыть через этот текст.</div>
          </div>
        </div>
        <div class="about-card">
          <div class="about-icon">🗺️</div>
          <div>
            <div class="about-card-title">Программа по литературе 5–9</div>
            <div class="about-card-text">Все произведения взяты из программы по литературе, которую ученики проходят параллельно. Никаких «внепрограммных» текстов.</div>
          </div>
        </div>
      </div>
      <div class="about-frp">
        <div class="about-frp-title">Разделы ФРП, охваченные в таблице</div>
        <ul class="frp-list">
          <li><span class="frp-dot"></span>5 класс — география как наука, литосфера, Земля-планета</li>
          <li><span class="frp-dot"></span>6 класс — гидросфера, атмосфера, биосфера, природные комплексы</li>
          <li><span class="frp-dot"></span>7 класс — материки и океаны, народы мира, глобальные проблемы</li>
          <li><span class="frp-dot"></span>8 класс — природа России, климат, реки, природные зоны, население</li>
          <li><span class="frp-dot"></span>9 класс — хозяйство России, районирование, регионы страны</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<!-- HOW TO -->
<section id="howto">
  <div class="section-inner">
    <div class="section-label">Как пользоваться</div>
    <h2 class="section-title">Три шага до готовой интеграции</h2>
    <p class="section-lead">Найти нужный материал можно за минуту.</p>
    <div class="steps">
      <div class="step">
        <div class="step-num">01</div>
        <div class="step-title">Выберите класс</div>
        <div class="step-text">Используйте выпадающий список «Все классы», чтобы показать только строки нужного года обучения — от 5 до 9 класса.</div>
      </div>
      <div class="step">
        <div class="step-num">02</div>
        <div class="step-title">Найдите тему</div>
        <div class="step-text">Введите ключевое слово в строку поиска (например «Волга», «климат», «Кавказ») или выберите категорию тегов в выпадающем фильтре «Тема / теги».</div>
      </div>
      <div class="step">
        <div class="step-num">03</div>
        <div class="step-title">Используйте на уроке</div>
        <div class="step-text">В столбце «Аспекты интеграции» — конкретные формулировки, что именно разбирать в произведении. Можно брать напрямую в план урока.</div>
      </div>
    </div>
  </div>
</section>

<!-- TABLE -->
<section id="table">
  <div class="section-inner">
    <div class="section-label">Таблица интеграции</div>
    <h2 class="section-title">Все темы — произведения — аспекты</h2>
    <p class="section-lead">35 тем, 120+ произведений. Фильтруйте по классу, теме или ищите по ключевому слову.</p>
    <div class="table-wrap-outer" id="tableApp"></div>
  </div>
</section>

<!-- FEEDBACK -->
<section id="feedback">
  <div class="section-inner">
    <div class="section-label">Предложить идею</div>
    <h2 class="section-title">Сделаем справочник лучше вместе</h2>
    <p class="section-lead">Знаете произведение, которого не хватает? Нашли неточность? Напишите — таблица обновляется.</p>
    <div class="feedback-grid">
      <div class="feedback-why">
        <div class="fwhy-item"><span class="fwhy-dot"></span><span class="fwhy-text">Предложить произведение, которого нет в таблице</span></div>
        <div class="fwhy-item"><span class="fwhy-dot"></span><span class="fwhy-text">Исправить ошибку или неточность в аспектах интеграции</span></div>
        <div class="fwhy-item"><span class="fwhy-dot"></span><span class="fwhy-text">Попросить добавить новую тему из ФРП</span></div>
        <div class="fwhy-item"><span class="fwhy-dot"></span><span class="fwhy-text">Поделиться опытом использования на уроке</span></div>
        <div class="fwhy-item"><span class="fwhy-dot"></span><span class="fwhy-text">Задать любой вопрос автору</span></div>
      </div>
      <div>
        <div class="feedback-form">
          <form id="feedbackForm">
            <div class="form-group">
              <label class="form-label">Ваше имя</label>
              <input class="form-input" type="text" placeholder="Иванова Мария Петровна" name="name">
            </div>
            <div class="form-group">
              <label class="form-label">Тип предложения</label>
              <select class="form-select form-input" name="type">
                <option value="">Выберите тип...</option>
                <option>Добавить произведение</option>
                <option>Исправить ошибку</option>
                <option>Добавить новую тему</option>
                <option>Поделиться опытом</option>
                <option>Другое</option>
              </select>
            </div>
            <div class="form-group">
              <label class="form-label">Ваше предложение</label>
              <textarea class="form-textarea" placeholder="Опишите, что нужно добавить или изменить. Например: в тему «Реки России» (8 класс) добавить повесть Астафьева «Царь-рыба» с аспектом экологии Енисея." name="message"></textarea>
            </div>
            <div class="form-group">
              <label class="form-label">E-mail (необязательно)</label>
              <input class="form-input" type="email" placeholder="для ответа" name="email">
            </div>
            <button type="submit" class="form-submit">Отправить предложение</button>
          </form>
          <div class="form-success" id="formSuccess">
            Спасибо! Ваше предложение получено.<br>Постараюсь учесть его при следующем обновлении таблицы.
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- FOOTER -->
<footer>
  <div class="footer-inner">
    <div class="footer-logo">География × Литература</div>
    <div>Межпредметные связи по ФРП 2022 · 5–9 классы</div>
    <div>Составлено для учителей географии · <span id="fyear"></span></div>
  </div>
</footer>

<script>
document.getElementById('fyear').textContent = new Date().getFullYear();

// ─── FORM ───
document.getElementById('feedbackForm').addEventListener('submit', function(e) {
  e.preventDefault();
  this.style.display = 'none';
  document.getElementById('formSuccess').style.display = 'block';
});

// ─── TABLE DATA ───
const TAG_GROUPS=[
  {label:"Природа и оболочки Земли",tags:["литосфера","рельеф","горы","вулканы","минералы","гидросфера","океан","реки","болото","течения","гидрография","атмосфера","погода","климат","гроза","осадки","сезоны","биосфера","охрана природы"]},
  {label:"Природные зоны и ландшафты",tags:["природные зоны","тайга","степь","тропики","саванна","субарктика","Амазония","Анды","пейзаж"]},
  {label:"Материки и регионы мира",tags:["материки","Африка","Южная Америка","Северная Америка","Евразия","морские путешествия","острова","карта"]},
  {label:"Россия: природа и регионы",tags:["образ России","пространство","Кавказ","Урал","Волга","Поволжье","Петербург","Москва","Сибирь","Дальний Восток","первопроходцы"]},
  {label:"Население и города",tags:["население","демография","народы","религии","культурные регионы","города","урбанизация","мир"]},
  {label:"Хозяйство и экономика",tags:["хозяйство","экономика","промышленность","ресурсы","нефть","сельское хозяйство","Дон","рекреация"]},
  {label:"Экология и глобальные проблемы",tags:["экология","глобальные проблемы","природопользование"]},
  {label:"История и путешествия",tags:["история","освоение","путешествия","открытия","геополитика","культура"]},
  {label:"Методы и образ географии",tags:["план местности","ориентирование","астрономия","зональность","климатические пояса","сейсмика"]},
];

const D=[
/* ══════════════ 5 КЛАСС ══════════════ */
/* Раздел: Географическое изучение Земли */
{cls:"5",
 sec:"Географическое изучение Земли",
 topic:"История географических открытий",
 works:[
  {a:"А. Никитин",t:"«Хожение за три моря» — первое русское путешествие в Индию (XV в.)"},
  {a:"Жюль Верн",t:"«Дети капитана Гранта» — кругосветное путешествие, материки и океаны"},
  {a:"Жюль Верн",t:"«Таинственный остров» — остров, природные условия, выживание"},
  {a:"Жюль Верн",t:"«Двадцать тысяч лье под водой» — Мировой океан, подводный рельеф"},
  {a:"Р.Л. Стивенсон",t:"«Остров сокровищ» — карта острова, ориентирование, рельеф"},
  {a:"Д. Дефо",t:"«Робинзон Крузо» — остров, природные условия, адаптация человека"},
 ],
 aspects:[
  "«Хожение за три моря» как реальный путевой дневник — источник географических знаний",
  "Карта острова в «Острове сокровищ» — работа с планом местности и условными знаками",
  "«Робинзон Крузо» — человек и природная среда: как условия острова определяют хозяйство",
  "Верн как научный популяризатор географии: точность описаний океанов и материков",
 ],
 tags:["путешествия","открытия","океан","острова","карта","морские путешествия"]},

{cls:"5",
 sec:"Изображения земной поверхности",
 topic:"Планы местности",
 works:[
  {a:"Р.Л. Стивенсон",t:"«Остров сокровищ» — карта острова, стороны света, ориентирование"},
  {a:"Дж.Р.Р. Толкин",t:"«Хоббит» — карта Средиземья: масштаб, условные знаки, легенда карты"},
  {a:"В.К. Арсеньев",t:"«Дерсу Узала» — ориентирование в тайге, чтение природных знаков"},
 ],
 aspects:[
  "Карта острова Стивенсона как упражнение в чтении плана местности и условных знаков",
  "Художественные карты Толкина — анализ масштаба, условных обозначений, легенды",
  "Ориентирование по природным признакам у Арсеньева — сравнение с компасом и азимутом",
  "Сравнение художественной карты с реальной топографической: сходства и отличия",
 ],
 tags:["карта","ориентирование","план местности"]},

{cls:"5",
 sec:"Изображения земной поверхности",
 topic:"Географические карты",
 works:[
  {a:"Р.Л. Стивенсон",t:"«Остров сокровищ» — координаты на карте, долгота и широта"},
  {a:"Жюль Верн",t:"«Таинственный остров» — определение координат места и использование карт"},
  {a:"В.К. Арсеньев",t:"«В дебрях Уссурийского края» — картографирование Дальнего Востока"},
 ],
 aspects:[
  "Карта острова как иллюстрация понятий «масштаб», «координаты», «условные обозначения»",
  "«Таинственный остров» — как герои определяют своё положение: связь с темой координат",
  "Арсеньев как реальный картограф: научные и художественные описания одного пространства",
 ],
 tags:["карта","ориентирование","план местности"]},

{cls:"5",
 sec:"Земля — планета Солнечной системы",
 topic:"Земля — планета Солнечной системы",
 works:[
  {a:"А.С. Пушкин",t:"«Зимнее утро», «Осень» — природные явления, смена сезонов"},
  {a:"С.Я. Маршак",t:"«Двенадцать месяцев» — астрономические явления, смена сезонов"},
  {a:"Н.А. Некрасов",t:"«Мороз, Красный нос» — природные явления зимы"},
  {a:"И.А. Бунин",t:"«Листопад» — смена сезонов, осенний пейзаж"},
 ],
 aspects:[
  "«Двенадцать месяцев» — астрономическая основа смены сезонов, дни равноденствия и солнцестояния",
  "Художественные образы рассвета и заката — связь с суточным вращением Земли",
  "Пейзажная лирика как фенологический дневник: сравнение с данными наблюдений за погодой",
  "Изменение длины дня в текстах разных авторов — иллюстрация поясов освещённости",
 ],
 tags:["сезоны","астрономия","пейзаж"]},

{cls:"5",
 sec:"Оболочки Земли. Литосфера — каменная оболочка Земли",
 topic:"Литосфера — каменная оболочка Земли",
 works:[
  {a:"Жюль Верн",t:"«Путешествие к центру Земли» — внутреннее строение Земли, вулканы, пещеры, Исландия"},
  {a:"Жюль Верн",t:"«Таинственный остров» — вулканический остров, лавовые породы, магматизм"},
  {a:"Дж.Р.Р. Толкин",t:"«Хоббит» — горы Мглистые, пещеры, горный рельеф"},
  {a:"П.П. Бажов",t:"«Малахитовая шкатулка» — горные породы и минералы Урала"},
 ],
 aspects:[
  "«Путешествие к центру Земли» — художественная модель строения Земли: ядро, мантия, кора",
  "Вулканический остров в «Таинственном острове» — магматические горные породы в тексте",
  "Горные породы и минералы в сказах Бажова как иллюстрация состава литосферы",
  "Рельеф в фэнтези-картах и реальных горных системах: сравнение форм и высот",
 ],
 tags:["литосфера","рельеф","горы","вулканы","минералы"]},

/* ══════════════ 6 КЛАСС ══════════════ */
/* Раздел: Оболочки Земли */
{cls:"6",
 sec:"Оболочки Земли",
 topic:"Гидросфера — водная оболочка Земли",
 works:[
  {a:"Жюль Верн",t:"«Двадцать тысяч лье под водой» — рельеф дна, течения, жизнь в океане"},
  {a:"Э. Хемингуэй",t:"«Старик и море» — Атлантика, Гольфстрим, поведение морских животных"},
  {a:"К.Г. Паустовский",t:"«Мещёрская сторона» — реки, озёра, болота средней полосы России"},
  {a:"М.М. Пришвин",t:"«Кладовая солнца» — болото как природный объект, верховые болота, торф"},
  {a:"Н.А. Некрасов",t:"«На Волге» — режим равнинной реки, разлив, питание"},
  {a:"С.Т. Аксаков",t:"«Записки об уженье рыбы» — реки и озёра России, их природа"},
 ],
 aspects:[
  "«Старик и море» — морские течения Атлантики: Гольфстрим, влияние на поведение рыбы",
  "Верн как иллюстратор строения и обитателей Мирового океана: рельеф дна, течения",
  "«Кладовая солнца» — верховое болото: образование, торф, экосистема, роль в природе",
  "Волга у Некрасова как равнинная река: питание, режим, разлив — иллюстрация темы рек",
 ],
 tags:["гидросфера","океан","реки","болото","течения","гидрография"]},

{cls:"6",
 sec:"Оболочки Земли",
 topic:"Атмосфера — воздушная оболочка Земли",
 works:[
  {a:"А.С. Пушкин",t:"«Зимняя дорога», «Зимний вечер» — метель, буря, атмосферные явления"},
  {a:"Ф.И. Тютчев",t:"«Весенняя гроза», «Неохотно и несмело...» — гроза, давление, ветер"},
  {a:"А.Н. Островский",t:"«Гроза» — гроза как природное явление и художественный символ"},
  {a:"А.П. Чехов",t:"«Степь» — описание грозы в степи, изменение погоды, роза ветров"},
  {a:"Л.Н. Толстой",t:"«Детство» — наблюдения за погодой, суточный ход температуры"},
 ],
 aspects:[
  "Гроза у Тютчева и Островского — физика атмосферного явления: давление, электричество",
  "Метель в текстах Пушкина — атмосферные фронты, циклоны, скорость и направление ветра",
  "Описания погоды у Толстого и Чехова как фенологические наблюдения: t°, осадки, ветер",
  "Туман, роса, иней в поэтических текстах — объяснение видов атмосферных осадков",
 ],
 tags:["атмосфера","погода","климат","гроза","осадки"]},

{cls:"6",
 sec:"Оболочки Земли",
 topic:"Биосфера — оболочка жизни",
 works:[
  {a:"М.М. Пришвин",t:"«Кладовая солнца» — природный комплекс болота и леса, флора и фауна"},
  {a:"И.С. Тургенев",t:"«Записки охотника» — растительный и животный мир средней полосы"},
  {a:"В.В. Бианки",t:"«Лесная газета» — сезонные изменения в биосфере, фенология"},
  {a:"Дж. Лондон",t:"«Зов предков», «Белый Клык» — природа субарктики, адаптации животных"},
  {a:"Р. Киплинг",t:"«Книга джунглей» — биосфера тропического леса, приспособления организмов"},
 ],
 aspects:[
  "«Кладовая солнца» — природный комплекс: взаимосвязи компонентов болота и леса",
  "«Книга джунглей» — тропический лес как природная зона: флора, фауна, климат, ярусность",
  "Лондон: субарктика — адаптации животных и человека к суровым условиям среды",
  "«Лесная газета» Бианки как образец фенологических наблюдений — практика 6 класса",
 ],
 tags:["биосфера","природные зоны","экология","охрана природы"]},

{cls:"6",
 sec:"Оболочки Земли",
 topic:"Природно-территориальные комплексы",
 works:[
  {a:"К.Г. Паустовский",t:"«Мещёрская сторона» — природный комплекс Мещёры: лес, болота, реки"},
  {a:"М.М. Пришвин",t:"«Кладовая солнца» — ПТК болота: взаимосвязь компонентов"},
  {a:"И.С. Тургенев",t:"«Бежин луг» — локальный природный комплекс средней полосы"},
  {a:"Антуан де Сент-Экзюпери",t:"«Маленький принц» — бережное отношение к природе, ООПТ"},
 ],
 aspects:[
  "«Мещёрская сторона» — описание локального ПТК: почвы, воды, растительность, животные",
  "«Бежин луг» — характеристика природного комплекса луга по плану (практ. работа 6 кл.)",
  "«Маленький принц» — метафора охраны природы: ООПТ, Всемирное наследие ЮНЕСКО",
  "Сравнение художественного и географического описаний одного природного комплекса",
 ],
 tags:["биосфера","природные зоны","экология","охрана природы"]},

/* ══════════════ 7 КЛАСС ══════════════ */
/* Раздел: Главные закономерности природы Земли */
{cls:"7",
 sec:"Главные закономерности природы Земли",
 topic:"Географическая оболочка",
 works:[
  {a:"Р. Киплинг",t:"«Книга джунглей» — экваториальный и субэкваториальный пояс, зональность"},
  {a:"Жюль Верн",t:"«Вокруг света в 80 дней» — смена природных зон при движении по широте"},
  {a:"Дж. Лондон",t:"«Зов предков» — субарктическая тундра, высотная поясность Аляски"},
 ],
 aspects:[
  "«Вокруг света в 80 дней» — наглядная демонстрация широтной зональности по маршруту героев",
  "«Книга джунглей» — экваториальный пояс: целостность оболочки, ритмичность, зональность",
  "Субарктика у Лондона — высотная поясность и её отличие от широтной зональности",
 ],
 tags:["природные зоны","зональность","климатические пояса","материки"]},

{cls:"7",
 sec:"Главные закономерности природы Земли",
 topic:"Литосфера и рельеф Земли",
 works:[
  {a:"Жюль Верн",t:"«Путешествие к центру Земли» — строение Земли, вулканы, Исландия, сейсмика"},
  {a:"А. Конан Дойл",t:"«Затерянный мир» — древний рельеф Южной Америки, столовые горы (тепуи)"},
  {a:"Жюль Верн",t:"«Таинственный остров» — вулканизм, лавовые породы, сейсмические явления"},
 ],
 aspects:[
  "«Затерянный мир» — столовые горы Южной Америки: тектоника, рельеф, история Земли как планеты",
  "«Путешествие к центру Земли» — строение Земли, вулканизм Исландии и сейсмические пояса",
  "Сейсмические пояса: художественные описания землетрясений как иллюстрация процессов рельефообразования",
 ],
 tags:["рельеф","вулканы","литосфера","материки","сейсмика"]},

{cls:"7",
 sec:"Главные закономерности природы Земли",
 topic:"Атмосфера и климаты Земли",
 works:[
  {a:"Г. Хаггард",t:"«Копи царя Соломона» — климат Южной Африки: сухой и влажный сезон, саванна"},
  {a:"Дж. Лондон",t:"«Зов предков» — субарктический климат Аляски и Юкона"},
  {a:"Жюль Верн",t:"«Вокруг света в 80 дней» — климатические пояса Земли через маршрут"},
  {a:"Э. Хемингуэй",t:"«Снега Килиманджаро» — высотная поясность и климат горной Африки"},
 ],
 aspects:[
  "«Снега Килиманджаро» — смена климатических зон с высотой: от тропической жары до ледника",
  "«Зов предков» — особенности субарктического климата: осадки, температурный режим, ветры",
  "«Вокруг света в 80 дней» — смена климатических поясов: от умеренного до тропического",
  "Климат саванны у Хаггарда: режим осадков, муссоны, сухой и влажный сезон",
 ],
 tags:["климат","природные зоны","материки","атмосфера"]},

{cls:"7",
 sec:"Главные закономерности природы Земли",
 topic:"Мировой океан — основная часть гидросферы",
 works:[
  {a:"Жюль Верн",t:"«Двадцать тысяч лье под водой» — Мировой океан: части, течения, жизнь, рельеф дна"},
  {a:"Э. Хемингуэй",t:"«Старик и море» — Мексиканский залив, Гольфстрим, экология океана"},
  {a:"Г. Мелвилл",t:"«Моби Дик» — Тихий и Атлантический океаны, китобойный промысел"},
  {a:"К.М. Станюкович",t:"«Вокруг света на «Коршуне»» — океанические путешествия, водные массы"},
 ],
 aspects:[
  "Верн — точность описаний течений, обитателей, рельефа дна: сравнение с современными данными",
  "«Старик и море» — Гольфстрим: тёплое течение, его влияние на климат и жизнь океана",
  "«Моби Дик» — промысловые районы Мирового океана, экологические последствия китобойства",
  "Система океанических течений через художественные тексты: тёплые и холодные течения",
 ],
 tags:["океан","течения","морские путешествия","экология","гидросфера"]},

/* Раздел: Человечество на Земле */
{cls:"7",
 sec:"Человечество на Земле",
 topic:"Численность населения",
 works:[
  {a:"Г. Бичер-Стоу",t:"«Хижина дяди Тома» — плотность населения американского Юга, расселение"},
  {a:"Жюль Верн",t:"«Вокруг света в 80 дней» — сравнение плотности населения разных регионов"},
  {a:"Дж. Лондон",t:"«Зов предков» — малонаселённые пространства Аляски и Канады"},
 ],
 aspects:[
  "«Хижина дяди Тома» — историческая демография американского Юга: расселение, урбанизация",
  "«Вокруг света в 80 дней» — сравнение численности и плотности населения по регионам мира",
  "Малонаселённые пространства у Лондона — факторы, влияющие на размещение населения",
 ],
 tags:["население","демография","мир","материки"]},

{cls:"7",
 sec:"Человечество на Земле",
 topic:"Страны и народы мира",
 works:[
  {a:"Жюль Верн",t:"«Вокруг света в 80 дней» — народы Индии, Японии, Америки, культура"},
  {a:"Р. Киплинг",t:"«Книга джунглей», «Ким» — народы Индии, индуизм, культурный регион"},
  {a:"Г. Хаггард",t:"«Копи царя Соломона» — народы Южной Африки, зулусы, традиции"},
  {a:"Дж. Лондон",t:"«Зов предков» — индейцы и эскимосы Аляски и Канады"},
 ],
 aspects:[
  "«Вокруг света в 80 дней» — сравнение культур, религий, быта народов разных регионов мира",
  "«Ким» Киплинга — этнография Индии как культурно-исторического региона: народы, религии",
  "Коренные народы Аляски у Лондона — хозяйство и расселение в субарктике",
  "Зулусы у Хаггарда — народы Африки: образ жизни, хозяйственная деятельность, поселения",
 ],
 tags:["народы","культурные регионы","религии","демография","мир"]},

/* Раздел: Материки и страны */
{cls:"7",
 sec:"Материки и страны",
 topic:"Южные материки",
 works:[
  {a:"Г. Хаггард",t:"«Копи царя Соломона» — саванна, горы, природа Южной Африки"},
  {a:"Дж. Конрад",t:"«Сердце тьмы» — бассейн Конго, экваториальный лес Африки"},
  {a:"Э. Хемингуэй",t:"«Снега Килиманджаро» — высотная поясность, вулканический рельеф"},
  {a:"А. Конан Дойл",t:"«Затерянный мир» — Гвианское нагорье, тепуи, Амазония"},
  {a:"Жюль Верн",t:"«Дети капитана Гранта» — Аргентина, Патагония, Анды, Австралия"},
 ],
 aspects:[
  "«Снега Килиманджаро» — высотная поясность вулканического Килиманджаро от саванны до ледника",
  "«Сердце тьмы» — природа экваториального леса Африки: климат, флора, фауна, река Конго",
  "«Затерянный мир» — Гвианское нагорье, тепуи: тектоника и рельеф Южной Америки",
  "«Дети капитана Гранта» — природные зоны Южной Америки и Австралии: сравнение материков",
 ],
 tags:["Африка","Южная Америка","саванна","тропики","рельеф","природные зоны","материки"]},

{cls:"7",
 sec:"Материки и страны",
 topic:"Северные материки",
 works:[
  {a:"Дж. Лондон",t:"«Зов предков», «Белый Клык» — Аляска, Юкон, субарктика Северной Америки"},
  {a:"М. Твен",t:"«Приключения Гекльберри Финна» — Миссисипи, природные зоны американского Юга"},
  {a:"Ф. Купер",t:"«Последний из могикан» — леса и реки Северной Америки"},
  {a:"Р. Киплинг",t:"«Ким» — природа и народы Евразии: Индия, Гималаи, высотная поясность"},
  {a:"Жюль Верн",t:"«Михаил Строгов» — Западная Сибирь, Урал, тайга, реки Евразии"},
 ],
 aspects:[
  "«Михаил Строгов» — природа Сибири: тайга, реки, климат континентальной Евразии",
  "«Зов предков» — субарктика и тундра Северной Америки: природные условия, животный мир",
  "Гималаи у Киплинга — высотная поясность Евразии: от тропиков до вечных снегов",
  "Миссисипи у Твена — великая река Северной Америки как природный и хозяйственный объект",
 ],
 tags:["Северная Америка","Евразия","тайга","субарктика","реки","материки"]},

/* Раздел: Взаимодействие природы и общества */
{cls:"7",
 sec:"Взаимодействие природы и общества",
 topic:"Взаимодействие природы и общества",
 works:[
  {a:"Антуан де Сент-Экзюпери",t:"«Маленький принц» — бережное отношение к природе, ответственность"},
  {a:"Дж. Лондон",t:"«Морской волк» — промысел и истощение морских ресурсов океана"},
  {a:"Жюль Верн",t:"«Таинственный остров» — рациональное природопользование"},
  {a:"Г. Уэллс",t:"«Война миров» — экологическая катастрофа как модель глобальной проблемы"},
 ],
 aspects:[
  "«Маленький принц» — метафора бережного отношения к природе своей планеты, цели устойчивого развития ООН",
  "«Таинственный остров» — пример рационального природопользования: принципы и методы",
  "«Морской волк» — промысловые ресурсы океана: истощение как экологическая проблема",
  "Глобальные проблемы человечества через художественную литературу и научную фантастику",
 ],
 tags:["экология","глобальные проблемы","природопользование","охрана природы"]},

/* ══════════════ 8 КЛАСС ══════════════ */
/* Раздел: Географическое пространство России */
{cls:"8",
 sec:"Географическое пространство России",
 topic:"История формирования и освоения территории России",
 works:[
  {a:"А.С. Пушкин",t:"«Капитанская дочка» — Оренбургский край, Урал, башкирские степи"},
  {a:"А.С. Пушкин",t:"«История Пугачёва» — географический контекст восстания"},
  {a:"Н.С. Лесков",t:"«Очарованный странник» — странствие по просторам России"},
  {a:"В.К. Арсеньев",t:"«В дебрях Уссурийского края» — освоение Дальнего Востока"},
  {a:"П.П. Ершов",t:"«Конёк-Горбунок» — сибирские мотивы, пространство России"},
 ],
 aspects:[
  "Маршруты первопроходцев на карте — история расширения территории России в XVI–XIX вв.",
  "Оренбургский край у Пушкина как «порубежье» — история заселения Поволжья и Урала",
  "Странничество у Лескова как художественная форма освоения и описания пространства России",
  "Сравнение исторических карт разных эпох с художественными описаниями территорий",
 ],
 tags:["история","образ России","освоение","первопроходцы","пространство"]},

{cls:"8",
 sec:"Географическое пространство России",
 topic:"Географическое положение и границы России",
 works:[
  {a:"Н.В. Гоголь",t:"«Мёртвые души» — дорога, простор, лирические отступления об образе России"},
  {a:"А.Н. Радищев",t:"«Путешествие из Петербурга в Москву» — маршрут, пространство, люди"},
  {a:"А.А. Блок",t:"«Скифы» — Россия между Востоком и Западом, геополитический образ"},
  {a:"Ф.И. Тютчев",t:"«Умом Россию не понять...» — философия пространства страны"},
  {a:"А.С. Пушкин",t:"«Евгений Онегин» — путешествие Онегина, образы разных регионов России"},
 ],
 aspects:[
  "Образ бескрайнего российского пространства — связь с темой ЭГП и границ России",
  "Дорога у Гоголя и Радищева как метафора географии: страны-соседи, ближнее зарубежье",
  "«Скифы» Блока — Россия как Евразия: геокультурное пограничье Запада и Востока",
  "Сравнение художественного образа территории России с её картографическим представлением",
 ],
 tags:["образ России","пространство","геополитика","история"]},

{cls:"8",
 sec:"Географическое пространство России",
 topic:"Административно-территориальное устройство России. Районирование территории",
 works:[
  {a:"Н.В. Гоголь",t:"«Ревизор» — губернский город как административный центр"},
  {a:"М.Е. Салтыков-Щедрин",t:"«История одного города» — образ провинциального губернского города"},
  {a:"А.П. Чехов",t:"«Три сестры» — провинциальный город и тяга к Москве как центру"},
 ],
 aspects:[
  "«Ревизор» — губернский город как административная единица: функции и структура",
  "«История одного города» — административно-территориальное устройство через сатирический образ",
  "«Три сестры» — Москва как главный административный и культурный центр страны",
 ],
 tags:["образ России","города","урбанизация","история"]},

/* Раздел: Природа России */
{cls:"8",
 sec:"Природа России",
 topic:"Природные условия и ресурсы России",
 works:[
  {a:"П.П. Бажов",t:"«Малахитовая шкатулка», «Медной горы Хозяйка» — минеральные ресурсы Урала"},
  {a:"В.П. Астафьев",t:"«Царь-рыба» — биологические ресурсы Сибири, браконьерство"},
  {a:"В.Г. Распутин",t:"«Прощание с Матёрой» — водные ресурсы, природно-ресурсный капитал"},
 ],
 aspects:[
  "Сказы Бажова — минеральные ресурсы Урала (малахит, медь, железо) в художественных образах",
  "«Царь-рыба» — биологические ресурсы рек Сибири: проблема рационального использования",
  "«Прощание с Матёрой» — водные ресурсы и их использование: ГЭС и экологический потенциал",
 ],
 tags:["ресурсы","экология","Урал","Сибирь","гидрография"]},

{cls:"8",
 sec:"Природа России",
 topic:"Геологическое строение, рельеф и полезные ископаемые",
 works:[
  {a:"М.Ю. Лермонтов",t:"«Мцыри» — Кавказские горы, ущелья, горный рельеф"},
  {a:"М.Ю. Лермонтов",t:"«Герой нашего времени» — горный пейзаж Кавказа, тектоника"},
  {a:"А.С. Пушкин",t:"«Кавказский пленник» — природа и рельеф Кавказа"},
  {a:"П.П. Бажов",t:"«Малахитовая шкатулка» — уральские горы, рудники, полезные ископаемые"},
  {a:"Д.Н. Мамин-Сибиряк",t:"«В горах» — горные пейзажи Урала, горнозаводской регион"},
 ],
 aspects:[
  "Точность горных пейзажей Лермонтова — Кавказ как область современного горообразования",
  "«Ущелье», «перевал», «вершина» у Лермонтова — иллюстрация понятий рельефа России",
  "Сказы Бажова — полезные ископаемые Урала: связь между тектоническим строением и ресурсами",
  "Антропогенные формы рельефа: карьеры и отвалы горнодобывающей промышленности в текстах",
 ],
 tags:["рельеф","горы","Кавказ","Урал","пейзаж","литосфера"]},

{cls:"8",
 sec:"Природа России",
 topic:"Климат и климатические ресурсы",
 works:[
  {a:"А.С. Пушкин",t:"«Зимнее утро», «Зимний вечер», «Осень» — сезонность российского климата"},
  {a:"Н.А. Некрасов",t:"«Мороз, Красный нос» — образ русской зимы, суровость климата"},
  {a:"И.А. Бунин",t:"«Антоновские яблоки» — пейзаж русской осени, агроклиматические условия"},
  {a:"С.А. Есенин",t:"«Берёза», «Нивы сжаты, рощи голы...» — смена сезонов в средней полосе"},
  {a:"А.А. Фет",t:"«Ещё майская ночь», «Учись у них — у дуба, у берёзы» — климат России"},
  {a:"Ф.И. Тютчев",t:"«Весенняя гроза», «Есть в осени первоначальной...» — атмосферные явления"},
 ],
 aspects:[
  "Континентальный климат через художественные образы сезонов: резкий контраст зимы и лета",
  "Агроклиматические ресурсы у Бунина — влияние климата на хозяйственную деятельность",
  "Метель, оттепель, белые ночи в текстах — разбор опасных метеорологических явлений России",
  "«Климатическая карта» образов в русской поэзии как иллюстрация климатических поясов",
 ],
 tags:["климат","сезоны","природные зоны","пейзаж","атмосфера"]},

{cls:"8",
 sec:"Природа России",
 topic:"Моря России. Внутренние воды и водные ресурсы",
 works:[
  {a:"Н.А. Некрасов",t:"«На Волге» — Волга как главная речная система России"},
  {a:"А.Н. Островский",t:"«Гроза» — образ Волги, режим реки, прибрежный город"},
  {a:"В.Г. Распутин",t:"«Прощание с Матёрой» — Ангара, каскад ГЭС, затопление территорий"},
  {a:"А.С. Пушкин",t:"«Медный всадник» — Нева, наводнение, опасные гидрологические явления"},
  {a:"М.М. Пришвин",t:"«Кладовая солнца» — болото: многолетняя мерзлота и подземные воды"},
  {a:"В.П. Астафьев",t:"«Царь-рыба» — Енисей, главные речные системы Сибири"},
 ],
 aspects:[
  "Волга у Некрасова и Островского — главная речная система: бассейн, режим, питание",
  "Наводнение в «Медном всаднике» — опасные гидрологические явления на реках России",
  "«Прощание с Матёрой» — каскады ГЭС на Ангаре: водные ресурсы, их потребление и охрана",
  "Болота у Пришвина — подземные воды и многолетняя мерзлота: распространение в России",
 ],
 tags:["реки","Волга","Сибирь","экология","гидрография","гидросфера"]},

{cls:"8",
 sec:"Природа России",
 topic:"Природно-хозяйственные зоны",
 works:[
  {a:"И.С. Тургенев",t:"«Записки охотника» — природа смешанных лесов, Орловская губерния"},
  {a:"М.М. Пришвин",t:"«Кладовая солнца», «Корень жизни» — тайга, болото, лесная зона"},
  {a:"В.П. Астафьев",t:"«Царь-рыба» — сибирская тайга, биоценоз таёжных рек"},
  {a:"А.П. Чехов",t:"«Степь» — степной пейзаж, почвы чернозёмной зоны"},
  {a:"М.А. Шолохов",t:"«Тихий Дон» — донская степь, природа Предкавказья"},
  {a:"К.Г. Паустовский",t:"«Мещёрская сторона» — смешанный лес, болота, охрана природы"},
 ],
 aspects:[
  "Художественный образ природной зоны как иллюстрация к характеристике природно-хозяйственных зон",
  "Флора и фауна в произведениях как признаки зональности: почвы, растительность, животный мир",
  "Степь у Чехова и Шолохова — природно-хозяйственная зона степей: почвы, экологические проблемы",
  "ООПТ в художественных текстах: заповедники и охрана редких видов (Красная книга России)",
 ],
 tags:["природные зоны","тайга","степь","экология","пейзаж","биосфера"]},

/* Раздел: Население России */
{cls:"8",
 sec:"Население России",
 topic:"Численность населения России",
 works:[
  {a:"Н.В. Гоголь",t:"«Мёртвые души» — ревизские сказки как исторический метод переписи"},
  {a:"Н.А. Некрасов",t:"«Кому на Руси жить хорошо» — рождаемость, смертность, судьбы народа"},
  {a:"А.П. Чехов",t:"«Мужики», «В овраге» — демографическая ситуация в деревне XIX в."},
 ],
 aspects:[
  "«Мёртвые души» — ревизские сказки как исторический аналог переписи населения России",
  "«Кому на Руси жить хорошо» — демографические процессы: рождаемость, смертность, миграция",
  "«Мужики» Чехова — естественный прирост населения и факторы смертности в XIX в.",
 ],
 tags:["население","демография","история"]},

{cls:"8",
 sec:"Население России",
 topic:"Территориальные особенности размещения населения России",
 works:[
  {a:"Ф.М. Достоевский",t:"«Преступление и наказание» — топография Петербурга, дворы-колодцы"},
  {a:"Л.Н. Толстой",t:"«Война и мир» — Москва: городская агломерация, пожар 1812 года"},
  {a:"М.А. Булгаков",t:"«Мастер и Маргарита» — топография Москвы 1930-х, городская среда"},
  {a:"А.П. Чехов",t:"«Три сестры» — провинциальный город vs Москва: урбанизация"},
  {a:"А.С. Пушкин",t:"«Медный всадник» — Петербург: основание города, его роль в стране"},
 ],
 aspects:[
  "Топография Петербурга в тексте Достоевского — работа с реальной картой города",
  "Москва у Толстого и Булгакова — крупнейшая городская агломерация в разные эпохи",
  "«Три сестры» — тяга в Москву как отражение урбанизации и неравномерности расселения",
  "«Медный всадник» — Петербург как пример создания нового городского центра: основная полоса расселения",
 ],
 tags:["города","Петербург","Москва","урбанизация","население"]},

{cls:"8",
 sec:"Население России",
 topic:"Народы и религии России",
 works:[
  {a:"А.С. Пушкин",t:"«Капитанская дочка» — башкиры, казаки, народы Поволжья и Урала"},
  {a:"М.Ю. Лермонтов",t:"«Герой нашего времени» — черкесы, осетины, народы Кавказа"},
  {a:"Л.Н. Толстой",t:"«Хаджи-Мурат» — чеченцы, аварцы, мусульманская культура Кавказа"},
  {a:"А.С. Пушкин",t:"«Бахчисарайский фонтан» — крымские татары, ислам, культура Крыма"},
 ],
 aspects:[
  "Этнокультурный портрет народов России в художественных текстах — иллюстрация к карте народов",
  "«Герой нашего времени» и «Хаджи-Мурат» — народы Кавказа: языковые группы, религии",
  "«Капитанская дочка» — многонациональное население Поволжья и Урала: титульные этносы",
  "«Бахчисарайский фонтан» — тюркские народы России, ислам как мировая религия в стране",
 ],
 tags:["народы","религии","Кавказ","культурные регионы","образ России"]},

{cls:"8",
 sec:"Население России",
 topic:"Половой и возрастной состав населения России",
 works:[
  {a:"Н.А. Некрасов",t:"«Кому на Руси жить хорошо» — возрастная структура крестьянства"},
  {a:"И.С. Тургенев",t:"«Отцы и дети» — конфликт поколений как демографическая тема"},
 ],
 aspects:[
  "«Кому на Руси жить хорошо» — половозрастная структура населения XIX в.: мужчины, женщины, дети",
  "«Отцы и дети» — демографическая нагрузка и смена поколений как географическая тема",
 ],
 tags:["население","демография","история"]},

{cls:"8",
 sec:"Население России",
 topic:"Человеческий капитал России",
 works:[
  {a:"И.А. Гончаров",t:"«Обломов» — трудовые ресурсы: инертность vs деятельность"},
  {a:"Н.А. Некрасов",t:"«Кому на Руси жить хорошо» — качество жизни, ИЧР исторически"},
  {a:"М. Горький",t:"«Детство», «В людях» — трудовые ресурсы, рабочая сила, занятость"},
 ],
 aspects:[
  "«Обломов» как художественная иллюстрация к теме трудовых ресурсов и занятости населения",
  "«Кому на Руси жить хорошо» — исторические предпосылки географических различий в уровне жизни",
  "«Детство» Горького — формирование человеческого капитала: образование, профессия, место жительства",
 ],
 tags:["население","экономика","история","города"]},

/* ══════════════ 9 КЛАСС ══════════════ */
/* Раздел: Хозяйство России */
{cls:"9",
 sec:"Хозяйство России",
 topic:"Общая характеристика хозяйства России",
 works:[
  {a:"Н.В. Гоголь",t:"«Мёртвые души» — помещичье хозяйство, отраслевая структура крепостной России"},
  {a:"А.П. Чехов",t:"«Вишнёвый сад» — смена хозяйственного уклада, переход к рыночной экономике"},
  {a:"А.Н. Островский",t:"«Гроза», «Бесприданница» — купечество и торговля как сектор хозяйства"},
  {a:"И.А. Гончаров",t:"«Обломов» — помещичий уклад как тормоз хозяйственного развития"},
 ],
 aspects:[
  "Отраслевая структура хозяйства России исторически: сельское хозяйство, промышленность, торговля",
  "«Вишнёвый сад» — смена хозяйственного уклада: от первичного сектора к третичному",
  "Купечество и торговля у Островского — территориальная структура хозяйства губернского города",
  "ЭГП России через художественные тексты: факторы размещения производства",
 ],
 tags:["хозяйство","экономика","история"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Топливно-энергетический комплекс",
 works:[
  {a:"В.Г. Распутин",t:"«Прощание с Матёрой» — ГЭС на Ангаре: гидроэнергетика и её последствия"},
  {a:"В.П. Астафьев",t:"«Царь-рыба» — влияние ТЭК на окружающую среду Сибири"},
  {a:"Д.Н. Мамин-Сибиряк",t:"«Приваловские миллионы» — горнозаводской Урал, добыча угля"},
 ],
 aspects:[
  "«Прощание с Матёрой» — каскады ГЭС на Ангаре: гидроэлектростанции, энергосистемы, экология",
  "«Царь-рыба» — влияние ТЭК на окружающую среду: загрязнение водоёмов Сибири",
  "Горнозаводской Урал у Мамина-Сибиряка — исторические районы добычи топливных ресурсов",
 ],
 tags:["промышленность","Сибирь","экология","ресурсы","хозяйство"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Металлургический комплекс",
 works:[
  {a:"П.П. Бажов",t:"«Малахитовая шкатулка», «Медной горы Хозяйка» — металлургия Урала"},
  {a:"Д.Н. Мамин-Сибиряк",t:"«Горное гнездо», «Приваловские миллионы» — чёрная и цветная металлургия Урала"},
 ],
 aspects:[
  "Сказы Бажова — Уральская металлургическая база: медь, малахит, чугун, факторы размещения",
  "Мамин-Сибиряк — технология производства металлов и география металлургических центров Урала",
 ],
 tags:["промышленность","Урал","ресурсы","хозяйство"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Машиностроительный комплекс",
 works:[
  {a:"М. Горький",t:"«Мать» — машиностроительный рабочий посёлок, завод как градообразующее предприятие"},
  {a:"А.Т. Твардовский",t:"«Василий Тёркин» — роль машиностроения в годы Великой Отечественной войны"},
 ],
 aspects:[
  "«Мать» Горького — машиностроительное предприятие как основа монофункционального города",
  "«Василий Тёркин» — машиностроение и оборонная промышленность: импортозамещение исторически",
 ],
 tags:["промышленность","хозяйство","города"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Химико-лесной комплекс",
 works:[
  {a:"В.П. Астафьев",t:"«Царь-рыба» — лесные ресурсы Сибири, лесозаготовка и охрана леса"},
  {a:"В.Г. Распутин",t:"«Прощание с Матёрой» — лесное хозяйство и его влияние на окружающую среду"},
  {a:"М.М. Пришвин",t:"«Кладовая солнца» — лесные ресурсы, ООПТ, охрана природы"},
 ],
 aspects:[
  "«Царь-рыба» — лесной комплекс Сибири: лесозаготовка, деревообработка, экологические проблемы",
  "«Прощание с Матёрой» — лесное хозяйство и устойчивое лесопользование: стратегия до 2030 г.",
  "«Кладовая солнца» — особо охраняемые природные территории как форма охраны лесных ресурсов",
 ],
 tags:["промышленность","Сибирь","экология","ресурсы","хозяйство"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Агропромышленный комплекс",
 works:[
  {a:"И.А. Бунин",t:"«Деревня», «Антоновские яблоки» — сельский уклад, земельные ресурсы"},
  {a:"М.А. Шолохов",t:"«Тихий Дон» — донское казачество, растениеводство и животноводство юга"},
  {a:"М.А. Шолохов",t:"«Поднятая целина» — коллективизация, АПК, сельскохозяйственные угодья"},
  {a:"С.А. Есенин",t:"«Анна Снегина» — деревня, поле, сельский труд, Рязанщина"},
  {a:"Ф.А. Абрамов",t:"«Братья и сёстры» — северная деревня, аграрный труд в суровых условиях"},
 ],
 aspects:[
  "«Тихий Дон» — зональная специализация АПК: растениеводство и животноводство донской степи",
  "«Поднятая целина» — коллективизация как изменение территориальной организации АПК",
  "«Братья и сёстры» — АПК Севера: агроклиматические ресурсы и ограничения",
  "Пищевая и лёгкая промышленность через описания крестьянского быта в русской литературе",
 ],
 tags:["сельское хозяйство","Дон","природные зоны","экономика","хозяйство"]},

{cls:"9",
 sec:"Хозяйство России",
 topic:"Инфраструктурный комплекс",
 works:[
  {a:"Н.В. Гоголь",t:"«Мёртвые души» — дороги России, транспортная система страны"},
  {a:"А.Н. Радищев",t:"«Путешествие из Петербурга в Москву» — сухопутный транспортный путь"},
  {a:"Н.А. Некрасов",t:"«Железная дорога» — строительство железных дорог и транспортные узлы"},
  {a:"А.П. Чехов",t:"«Три сестры» — рекреационное хозяйство: провинция и стремление к центру"},
 ],
 aspects:[
  "«Железная дорога» Некрасова — развитие железнодорожного транспорта России: история и значение",
  "«Мёртвые души» — дороги как часть транспортной инфраструктуры: типы и состояние",
  "«Путешествие из Петербурга в Москву» — транспортный путь: расстояния, транспортные узлы",
  "«Три сестры» — рекреационное хозяйство: туристско-рекреационный потенциал провинции",
 ],
 tags:["хозяйство","транспорт","экономика","города","образ России"]},

/* Раздел: Регионы России */
{cls:"9",
 sec:"Регионы России",
 topic:"Западный макрорегион. Европейский Север и Северо-Запад России",
 works:[
  {a:"А.С. Пушкин",t:"«Медный всадник» — Петербург, Нева, наводнение, Северо-Запад"},
  {a:"Ф.М. Достоевский",t:"«Белые ночи» — белые ночи как климатическое явление Северо-Запада"},
  {a:"Н.В. Гоголь",t:"«Петербургские повести» — образ имперского города на Балтике"},
  {a:"А.А. Ахматова",t:"«Реквием», «Стихи о Петербурге» — Петербург как культурный центр"},
  {a:"Ф.А. Абрамов",t:"«Братья и сёстры» — Европейский Север: природа, население, хозяйство"},
 ],
 aspects:[
  "Белые ночи в «Белых ночах» Достоевского — географическое явление: широта, полярный день",
  "«Медный всадник» — Петербург на Балтике: ЭГП, роль в международном разделении труда",
  "«Братья и сёстры» — Европейский Север: природно-ресурсный потенциал, население, хозяйство",
  "Петербург у Пушкина, Гоголя, Ахматовой — Северо-Запад России: социально-экономические проблемы",
 ],
 tags:["Петербург","климат","города","образ России"]},

{cls:"9",
 sec:"Регионы России",
 topic:"Западный макрорегион. Центральная Россия",
 works:[
  {a:"Л.Н. Толстой",t:"«Война и мир» — Москва, Ясная Поляна, Смоленск: ядро Центральной России"},
  {a:"И.С. Тургенев",t:"«Записки охотника» — Орловская, Тульская губернии: природа и хозяйство"},
  {a:"М.А. Булгаков",t:"«Мастер и Маргарита» — топография Москвы: крупнейшая агломерация"},
  {a:"А.П. Чехов",t:"«Три сестры» — провинциальный город ЦФО и Москва как магнит"},
  {a:"И.А. Бунин",t:"«Антоновские яблоки» — природа Орловщины, Центральное Черноземье"},
 ],
 aspects:[
  "Москва у Толстого и Булгакова — Московская агломерация: крупнейший транспортный узел страны",
  "«Записки охотника» — природно-ресурсный потенциал Центрально-Чернозёмного района",
  "«Три сестры» — экономические различия Москвы и провинции: уровень ИЧР по регионам",
  "Работа с литературными картами: маршруты героев по территории Центральной России",
 ],
 tags:["Москва","образ России","история","города","урбанизация"]},

{cls:"9",
 sec:"Регионы России",
 topic:"Западный макрорегион. Поволжье",
 works:[
  {a:"М. Горький",t:"«Детство», «Мои университеты» — Нижний Новгород, хозяйство Поволжья"},
  {a:"А.Н. Островский",t:"«Гроза» — типичный поволжский купеческий город"},
  {a:"Н.А. Некрасов",t:"«На Волге» — Волга как транспортная артерия и хозяйственный стержень"},
  {a:"В.М. Шукшин",t:"«Я пришёл дать вам волю» — Волга, казачество, история Поволжья"},
 ],
 aspects:[
  "Волга у Некрасова и Островского — транспортный коридор Поволжья: исторически и сейчас",
  "Нижний Новгород у Горького — крупный транспортный узел и центр хозяйства Поволжья",
  "«Гроза» — купеческий город Поволжья: классификация городов по функциям",
  "Поволжье как многонациональный регион — народы, ЭГП, социально-экономические проблемы",
 ],
 tags:["Волга","Поволжье","реки","экономика","народы","история"]},

{cls:"9",
 sec:"Регионы России",
 topic:"Западный макрорегион. Юг Европейской части России",
 works:[
  {a:"М.Ю. Лермонтов",t:"«Герой нашего времени» — Тамань, Пятигорск, Кисловодск, КМВ"},
  {a:"А.С. Пушкин",t:"«Кавказский пленник», «Путешествие в Арзрум» — природа Кавказа"},
  {a:"Л.Н. Толстой",t:"«Хаджи-Мурат», «Кавказский пленник» — народы, природа горного Кавказа"},
  {a:"М.А. Шолохов",t:"«Тихий Дон» — природа и хозяйство донской степи, казачество"},
 ],
 aspects:[
  "«Герой нашего времени» — точная география Кавказских Минеральных Вод: рекреационный район",
  "«Тихий Дон» — природно-ресурсный потенциал Дона и Кубани: АПК, перспективы развития",
  "Народы Кавказа у Лермонтова и Толстого — многонациональный регион: проблемы и потенциал",
  "Юг Европейской части как регион с наиболее высоким уровнем социально-экономического развития",
 ],
 tags:["Кавказ","горы","народы","рекреация","сельское хозяйство","Дон"]},

{cls:"9",
 sec:"Регионы России",
 topic:"Западный макрорегион. Урал",
 works:[
  {a:"П.П. Бажов",t:"«Малахитовая шкатулка», «Каменный цветок», «Медной горы Хозяйка»"},
  {a:"Д.Н. Мамин-Сибиряк",t:"«Приваловские миллионы», «Горное гнездо» — горнозаводской Урал"},
  {a:"А.С. Пушкин",t:"«Капитанская дочка» — Оренбургская степь, Урал как природный рубеж"},
  {a:"Б.Л. Пастернак",t:"«Доктор Живаго» — Урал в годы гражданской войны"},
 ],
 aspects:[
  "Сказы Бажова — природно-ресурсный потенциал Урала: металлургический комплекс и его история",
  "Мамин-Сибиряк — классификация субъектов Урала по уровню социально-экономического развития",
  "Урал как природная граница Европы и Азии — в географии и в художественных текстах",
  "ЭГП Урала через художественные тексты: транспортные узлы, промышленные центры",
 ],
 tags:["Урал","промышленность","ресурсы","горы","история","образ России"]},

/* Раздел: Восточный макрорегион */
{cls:"9",
 sec:"Регионы России",
 topic:"Восточный макрорегион. Сибирь и Дальний Восток",
 works:[
  {a:"А.П. Чехов",t:"«Остров Сахалин» — природа, население и хозяйство Дальнего Востока"},
  {a:"В.К. Арсеньев",t:"«Дерсу Узала» — Уссурийская тайга, коренные народы Дальнего Востока"},
  {a:"В.П. Астафьев",t:"«Царь-рыба» — природно-ресурсный потенциал Красноярского края"},
  {a:"В.Г. Распутин",t:"«Прощание с Матёрой» — Ангара, Сибирь: экологические проблемы"},
  {a:"В.М. Шукшин",t:"«Калина красная», рассказы — сибирская деревня, Алтай, Западная Сибирь"},
 ],
 aspects:[
  "«Остров Сахалин» — природно-ресурсный потенциал Дальнего Востока: население, перспективы",
  "«Дерсу Узала» — Уссурийская тайга: коренные народы, промышленные кластеры Дальнего Востока",
  "«Царь-рыба» — экологические проблемы Сибири: состояние окружающей среды и пути решения",
  "Арктическая зона России в контексте «Государственной программы развития Арктики»",
 ],
 tags:["Сибирь","Дальний Восток","тайга","народы","экология","ресурсы"]},

/* Раздел: Россия в современном мире */
{cls:"9",
 sec:"Россия в современном мире",
 topic:"Россия в современном мире",
 works:[
  {a:"Л.Н. Толстой",t:"«Война и мир» — Россия в европейском контексте, международные связи"},
  {a:"А.А. Блок",t:"«Скифы» — Россия между Востоком и Западом, место в мировой цивилизации"},
  {a:"И.С. Тургенев",t:"«Отцы и дети» — Россия и Европа, международные экономические связи"},
  {a:"Ф.М. Достоевский",t:"«Дневник писателя» — место России в системе международных отношений"},
  {a:"А.И. Солженицын",t:"«Матрёнин двор» — Россия: природные и культурные ценности для цивилизации"},
 ],
 aspects:[
  "Место России в системе международного географического разделения труда — через литературный образ",
  "«Скифы» Блока — Россия в составе международных организаций: ЕврАзЭС, СНГ, геополитика",
  "Объекты Всемирного природного и культурного наследия России в художественных текстах",
  "Значение географического пространства России как комплекса природных и культурных ценностей",
 ],
 tags:["образ России","геополитика","история","культурные регионы","пространство"]},
];
// ─── BUILD TABLE APP ───
function buildApp(){
  const app=document.getElementById('tableApp');
  app.innerHTML=`
    <div class="tw-srow" id="twStats"></div>
    <div class="tw-controls">
      <select id="twCf">
        <option value="">Все классы</option>
        <option value="5">5 класс</option>
        <option value="6">6 класс</option>
        <option value="7">7 класс</option>
        <option value="8">8 класс</option>
        <option value="9">9 класс</option>
      </select>
      <div class="dd-wrap" id="ddWrap">
        <button class="dd-btn" id="ddBtn" type="button">
          <span id="ddLabel">Тема / теги</span>
          <span class="dd-arrow" id="ddArrow">▼</span>
        </button>
        <div class="dd-panel" id="ddPanel"></div>
      </div>
      <input type="text" id="twSq" placeholder="Поиск по теме, автору, произведению..." style="min-width:220px;flex:1">
    </div>
    <div class="active-tags" id="activeTags"></div>
    <div class="tw-outer">
      <table id="twTable">
        <thead><tr>
          <th>Класс</th><th>Раздел ФРП</th><th>Тема по географии</th>
          <th>Произведения</th><th>Аспекты интеграции</th>
        </tr></thead>
        <tbody id="twBody"></tbody>
      </table>
      <div class="tw-empty" id="twEmpty" style="display:none">Ничего не найдено</div>
    </div>`;

  buildPanel();
  render();
  document.getElementById('twCf').addEventListener('change',render);
  document.getElementById('twSq').addEventListener('input',render);
  const btn=document.getElementById('ddBtn');
  const panel=document.getElementById('ddPanel');
  const arrow=document.getElementById('ddArrow');
  btn.addEventListener('click',e=>{e.stopPropagation();panel.classList.toggle('open');arrow.classList.toggle('open')});
  document.addEventListener('click',()=>{panel.classList.remove('open');arrow.classList.remove('open')});
  panel.addEventListener('click',e=>e.stopPropagation());
}

function buildPanel(){
  const panel=document.getElementById('ddPanel');
  panel.innerHTML=TAG_GROUPS.map((g,gi)=>`
    <div class="dd-group">
      <div class="dd-group-label" data-gi="${gi}">
        <span>${g.label}</span>
        <span class="group-check">выбрать всё</span>
      </div>
      <div class="dd-tags">${g.tags.map(t=>`<span class="tg" data-tag="${t}">${t}</span>`).join('')}</div>
    </div>`).join('')+`<button class="dd-clear" id="ddClear">Сбросить всё</button>`;

  panel.querySelectorAll('.dd-group-label').forEach(lbl=>{
    lbl.addEventListener('click',e=>{
      e.stopPropagation();
      const gi=parseInt(lbl.dataset.gi);
      const groupTags=TAG_GROUPS[gi].tags;
      const allOn=groupTags.every(t=>isTagOn(t));
      groupTags.forEach(t=>document.querySelectorAll(`.tg[data-tag="${t}"]`).forEach(el=>el.classList.toggle('on',!allOn)));
      updateGroupStates();render();
    });
  });
  panel.querySelectorAll('.tg').forEach(el=>{
    el.addEventListener('click',e=>{
      e.stopPropagation();
      const nowOn=!el.classList.contains('on');
      document.querySelectorAll(`.tg[data-tag="${el.dataset.tag}"]`).forEach(x=>x.classList.toggle('on',nowOn));
      updateGroupStates();render();
    });
  });
  document.getElementById('ddClear').addEventListener('click',e=>{
    e.stopPropagation();
    document.querySelectorAll('.tg').forEach(x=>x.classList.remove('on'));
    updateGroupStates();render();
  });
}

function isTagOn(tag){const el=document.querySelector(`.tg[data-tag="${tag}"]`);return el?el.classList.contains('on'):false}

function updateGroupStates(){
  document.querySelectorAll('.dd-group-label').forEach(lbl=>{
    const gi=parseInt(lbl.dataset.gi);
    const groupTags=TAG_GROUPS[gi].tags;
    const onCount=groupTags.filter(t=>isTagOn(t)).length;
    const check=lbl.querySelector('.group-check');
    lbl.classList.remove('all-on','some-on');
    if(onCount===groupTags.length){lbl.classList.add('all-on');if(check)check.textContent='снять всё';}
    else if(onCount>0){lbl.classList.add('some-on');if(check)check.textContent=`выбрано: ${onCount}`;}
    else{if(check)check.textContent='выбрать всё';}
  });
}

function activeTags(){return[...new Set([...document.querySelectorAll('.tg.on')].map(el=>el.dataset.tag))]}

function updateDdLabel(){
  const at=activeTags();
  const lbl=document.getElementById('ddLabel');
  if(lbl)lbl.textContent=at.length===0?'Тема / теги':at.length===1?at[0]:`Выбрано тегов: ${at.length}`;
}

function renderActivePills(){
  const at=activeTags();
  const c=document.getElementById('activeTags');
  if(!c)return;
  c.innerHTML=at.map(t=>`<span class="active-tag" data-tag="${t}">${t} <span class="active-tag-x">✕</span></span>`).join('');
  c.querySelectorAll('.active-tag').forEach(el=>el.addEventListener('click',()=>{
    document.querySelectorAll(`.tg[data-tag="${el.dataset.tag}"]`).forEach(x=>x.classList.remove('on'));
    updateGroupStates();render();
  }));
}

function render(){
  updateDdLabel();renderActivePills();
  const cls=document.getElementById('twCf').value;
  const q=document.getElementById('twSq').value.toLowerCase();
  const at=activeTags();
  const f=D.filter(row=>{
    if(cls&&row.cls!==cls)return false;
    if(q){const h=(row.topic+row.sec+row.works.map(w=>w.a+w.t).join(' ')+row.aspects.join(' ')).toLowerCase();if(!h.includes(q))return false;}
    if(at.length>0&&!at.some(t=>row.tags.includes(t)))return false;
    return true;
  });
  const tb=document.getElementById('twBody');
  const em=document.getElementById('twEmpty');
  const mt=document.getElementById('twTable');
  if(!tb)return;
  tb.innerHTML=f.map(row=>`<tr>
    <td style="text-align:center"><span class="cb c${row.cls}">${row.cls} кл.</span></td>
    <td><span class="sb">${row.sec}</span></td>
    <td><div class="gt">${row.topic}</div></td>
    <td><div class="wl">${row.works.map(w=>`<div class="wi"><strong>${w.a}</strong> ${w.t}</div>`).join('')}</div></td>
    <td><div class="al">${row.aspects.map(a=>`<div class="ai">${a}</div>`).join('')}</div></td>
  </tr>`).join('');
  if(em)em.style.display=f.length===0?'block':'none';
  if(mt)mt.style.display=f.length===0?'none':'';
  const counts={5:0,6:0,7:0,8:0,9:0};
  f.forEach(r=>counts[r.cls]++);
  const wc=f.reduce((s,r)=>s+r.works.length,0);
  const st=document.getElementById('twStats');
  if(st)st.innerHTML=`
    <div class="tw-sc"><div class="tw-sl">Тем</div><div class="tw-sv">${f.length}</div></div>
    <div class="tw-sc"><div class="tw-sl">5 кл.</div><div class="tw-sv" style="color:#72243E">${counts[5]}</div></div>
    <div class="tw-sc"><div class="tw-sl">6 кл.</div><div class="tw-sv" style="color:#633806">${counts[6]}</div></div>
    <div class="tw-sc"><div class="tw-sl">7 кл.</div><div class="tw-sv" style="color:#27500A">${counts[7]}</div></div>
    <div class="tw-sc"><div class="tw-sl">8 кл.</div><div class="tw-sv" style="color:#0C447C">${counts[8]}</div></div>
    <div class="tw-sc"><div class="tw-sl">9 кл.</div><div class="tw-sv" style="color:#1b4332">${counts[9]}</div></div>
    <div class="tw-sc"><div class="tw-sl">Произведений</div><div class="tw-sv">${wc}</div></div>`;
}

buildApp();
</script>
</body>
</html>
