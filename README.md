# ecotech8.github.io
My site
<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>Энергетика и экологические технологии: ветряная энергия</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600&family=Space+Grotesk:wght@500;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#FFFFFF; --card:#F8FAFC; --ink:#0F172A; --muted:#475569; --line:#E2E8F0; --accent:#0D9488; --accent-ink:#FFFFFF; --soft:#CCFBF1;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){--bg:#0B1220;--card:#111B2E;--ink:#F1F5F9;--muted:#94A3B8;--line:#1E293B;--soft:#0F3D3A;}
}
:root[data-theme="dark"]{--bg:#0B1220;--card:#111B2E;--ink:#F1F5F9;--muted:#94A3B8;--line:#1E293B;--soft:#0F3D3A;}
*,*::before,*::after{box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:calc(72px + env(safe-area-inset-top,0px))}
body{margin:0;background:var(--bg);color:var(--ink);font:400 17px/1.65 Inter,system-ui,sans-serif;-webkit-font-smoothing:antialiased}
h1,h2,h3{font-family:"Space Grotesk",Inter,sans-serif;line-height:1.15;margin:0 0 .5em;letter-spacing:-.02em}
h1{font-size:clamp(2rem,5.5vw,3.6rem);font-weight:700}
h2{font-size:clamp(1.6rem,3.5vw,2.3rem);font-weight:700}
h3{font-size:1.2rem;font-weight:700}
p{margin:0 0 1em;max-width:68ch}
a{color:inherit}
.wrap{max-width:1120px;margin:0 auto;padding:0 20px}
section{padding:72px 0}
.lead{color:var(--muted);font-size:1.1rem}
header.nav{position:sticky;top:0;z-index:10;background:var(--bg);border-bottom:1px solid var(--line)}
header.nav::before{content:"";position:fixed;inset:0 0 auto;height:env(safe-area-inset-top,0px);background:var(--bg);z-index:10}
.nav .wrap{display:flex;align-items:center;justify-content:space-between;gap:16px;height:64px}
.logo{font:700 1.05rem "Space Grotesk",sans-serif;text-decoration:none;display:flex;gap:8px;align-items:center}
.logo i{width:14px;height:14px;border-radius:50%;background:var(--accent);display:inline-block}
.nav nav{display:flex;gap:4px;overflow-x:auto;scrollbar-width:none}
.nav nav a{padding:8px 12px;border-radius:8px;text-decoration:none;font-size:.92rem;color:var(--muted);white-space:nowrap}
.nav nav a:hover,.nav nav a:focus-visible{background:var(--card);color:var(--ink)}
a:focus-visible,button:focus-visible,input:focus-visible{outline:3px solid var(--accent);outline-offset:2px}
.hero{padding:64px 0 80px}
.hero .grid{display:grid;grid-template-columns:1.5fr 1fr;gap:40px;align-items:start}
.btn{display:inline-block;background:var(--accent);color:var(--accent-ink);padding:14px 26px;border-radius:10px;font-weight:600;text-decoration:none;transition:transform .15s}
.btn:hover{transform:translateY(-2px)}
.pcard{background:#0F172A;color:#F1F5F9;border-radius:16px;padding:28px}
.pcard dl{margin:0}.pcard dt{color:#5EEAD4;font-size:.85rem;margin-top:14px}.pcard dd{margin:2px 0 0;font-weight:500}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:20px}
.card{background:var(--card);border:1px solid var(--line);border-radius:14px;padding:26px}
.card h3{color:var(--accent)}
.card p:last-child{margin:0}
.two{display:grid;grid-template-columns:repeat(auto-fit,minmax(290px,1fr));gap:20px;margin-bottom:40px}
.card ul{margin:0;padding-left:1.1em;color:var(--muted)}
.card li{margin-bottom:.4em}
.steps{counter-reset:s;list-style:none;margin:0;padding:0;display:grid;gap:12px}
.steps li{counter-increment:s;background:var(--card);border:1px solid var(--line);border-radius:12px;padding:16px 18px 16px 62px;position:relative}

.steps li::before{content:counter(s);position:absolute;left:16px;top:14px;width:32px;height:32px;border-radius:50%;background:var(--accent);color:#fff;display:grid;place-items:center;font:700 .95rem "Space Grotesk"}
.steps b{display:block}
.lab{display:grid;grid-template-columns:1fr 1fr;gap:20px;margin-bottom:24px}
.panel{background:#0F172A;color:#F1F5F9;border-radius:16px;padding:24px;display:flex;flex-direction:column;align-items:center}
.panel svg{width:100%;max-width:300px;height:auto}
.ctrl{background:var(--card);border:1px solid var(--line);border-radius:16px;padding:24px}
.ctrl label{font-weight:600;display:flex;justify-content:space-between}
input[type=range]{width:100%;accent-color:var(--accent);margin:14px 0 22px;height:28px}
.bar{height:14px;background:var(--line);border-radius:7px;overflow:hidden}
.bar span{display:block;height:100%;width:0;background:var(--accent);transition:width .2s}
.big{font:700 2.2rem "Space Grotesk";color:var(--accent);margin:.3em 0 0}
.status{display:inline-block;margin-top:10px;padding:6px 14px;border-radius:99px;background:var(--soft);font-weight:600;font-size:.95rem}
.tw{overflow-x:auto;border:1px solid var(--line);border-radius:14px}
table{border-collapse:collapse;width:100%;min-width:760px;font-size:.95rem}
th,td{padding:14px 16px;text-align:left;vertical-align:top;border-bottom:1px solid var(--line)}
th{background:#0F172A;color:#fff;font-family:"Space Grotesk";font-weight:500}
tr:last-child td{border-bottom:0}
tr.wind td{background:var(--soft);font-weight:500}
.note{margin-top:24px;border-left:4px solid var(--accent);padding:6px 0 6px 18px}
.refs{padding-left:1.2em;color:var(--muted)}.refs li{margin-bottom:.5em}
footer{background:#0F172A;color:#CBD5E1;padding:36px 0;font-size:.92rem}
footer p{margin:.2em 0;max-width:none}
.rv{opacity:0;transform:translateY(18px);transition:opacity .6s,transform .6s}
.rv.in{opacity:1;transform:none}
@media (max-width:760px){.hero .grid,.lab{grid-template-columns:1fr}section{padding:52px 0}.nav nav a{padding:8px 9px}.logo span{display:none}}
@media (prefers-reduced-motion:reduce){html{scroll-behavior:auto}.rv{opacity:1;transform:none;transition:none}.btn{transition:none}}
</style>
</head>
<body>
<header class="nav"><div class="wrap">
  <a class="logo" href="#top"><i></i><span>Ветроэнергетика</span></a>
  <nav aria-label="Разделы">
    <a href="#problem">Проблема</a><a href="#compare">Сравнение</a><a href="#model">Модель</a><a href="#eco">Экология</a><a href="#result">Выводы</a>
  </nav>
</div></header>

<main id="top">
<section class="hero"><div class="wrap grid">
  <div>
    <h1>Энергетика и экологические технологии: ветряная энергия</h1>
    <p class="lead">Мировое потребление электроэнергии растёт каждый год, а привычные тепловые станции сжигают топливо и выбрасывают в атмосферу углекислый газ. Чтобы сохранить и мощность, и чистый воздух, энергетика переходит на возобновляемые источники — прежде всего на ветер.</p>
    <a class="btn" href="#model">Открыть калькулятор и модель</a>
  </div>
  <aside class="pcard" aria-label="Данные проекта">
    <h3>Школьный проект по физике, 2026</h3>
    <dl>
      <dt>Автор</dt><dd>Кельдюшов Никита Михайлович, 10А класс</dd>
      <dt>Школа</dt><dd>МАОУ «СОШ № 7», г. Альметьевск, Республика Татарстан</dd>
      <dt>Руководитель</dt><dd>Садыкова Л. А., учитель физики</dd>
    </dl>
  </aside>
</div></section>

<section id="problem" style="background:var(--card)"><div class="wrap">
  <h2 class="rv">Проблема, цель и гипотеза</h2>
  <div class="cards">
    <article class="card rv"><h3>Проблема</h3><p>Традиционные станции дают большую и стабильную мощность, но загрязняют среду. Чистые источники безопаснее для природы, но их мощность зависит от погоды. Нужно выбрать между мощностью и экологией.</p></article>
    <article class="card rv"><h3>Цель</h3><p>Изучить физические основы ветроэнергетики, сравнить её с традиционной энергетикой и проверить работу ветрогенератора на практической модели.</p></article>

<article class="card rv"><h3>Гипотеза</h3><p>Ветроэнергетика эффективна и экологична даже при умеренных ветрах: мощность быстро растёт со скоростью потока, а при генерации нет вредных выбросов.</p></article>
  </div>
</div></section>

<section id="compare"><div class="wrap">
  <h2 class="rv">Традиционная энергетика и ветроэнергетика</h2>
  <div class="two">
    <article class="card rv"><h3>ТЭС</h3><ul><li>Работает на угле, газе, мазуте; выработка стабильна.</li><li>Удельная теплота сгорания угля q = 27 · 10⁶ Дж/кг.</li><li>КПД до 35–40 %.</li><li>Запасы топлива исчерпаемы.</li></ul></article>
    <article class="card rv"><h3>ГЭС</h3><ul><li>Использует энергию падающей воды.</li><li>Выработка стабильна и легко регулируется.</li><li>Плотины меняют русло реки и затапливают земли.</li></ul></article>
    <article class="card rv"><h3>АЭС</h3><ul><li>Энергия деления ядер урана.</li><li>Очень стабильная и мощная генерация.</li><li>Радиоактивные отходы и риск аварий.</li></ul></article>
  </div>
  <h3 class="rv">Как работает ветрогенератор</h3>
  <ol class="steps rv">
    <li><b>Аэродинамическая подъёмная сила</b>Ветер обтекает профиль лопасти, и разность давлений создаёт силу, раскручивающую ротор.</li>
    <li><b>Механическое вращение</b>Ротор с лопастями вращается на валу под действием этой силы.</li>
    <li><b>Редуктор</b>Увеличивает малую скорость вращения винта до скорости, нужной генератору.</li>
    <li><b>Электромагнитная индукция Фарадея</b>Катушка вращается в магнитном поле, в ней возникает ЭДС индукции.</li>
    <li><b>Стабилизация тока</b>Электроника выпрямляет и стабилизирует ток перед подачей в сеть или потребителю.</li>
  </ol>
</div></section>

<section id="model" style="background:var(--card)"><div class="wrap">
  <h2 class="rv">Физика ветра и модель</h2>
  <p class="lead rv">Мощность ветрового потока пропорциональна кубу скорости: P ~ v³. Если скорость ветра вырастает вдвое, мощность увеличивается в 8 раз.</p>
  <div class="lab rv">
    <div class="panel">
      <svg viewBox="0 0 300 330" role="img" aria-label="Анимированная модель ветрогенератора">
        <g id="wind" stroke="#5EEAD4" stroke-linecap="round" stroke-width="2" fill="none"></g>
        <path d="M162 314 H245 V290" stroke="#64748B" stroke-width="2" fill="none"/>
        <circle id="glow" cx="245" cy="262" r="38" fill="#FDE047" opacity="0"/>
        <rect x="237" y="278" width="16" height="12" rx="2" fill="#64748B"/>
        <circle id="bulb" cx="245" cy="262" r="15" fill="#334155" stroke="#94A3B8" stroke-width="2"/>
        <polygon points="144,110 156,110 162,310 138,310" fill="#94A3B8"/>
        <rect x="110" y="310" width="80" height="8" rx="4" fill="#64748B"/>
        <g id="blades">
          <path d="M150 110 C140 70 142 40 150 14 C158 40 160 70 150 110Z" fill="#5EEAD4"/>
          <path d="M150 110 C140 70 142 40 150 14 C158 40 160 70 150 110Z" fill="#2DD4BF" transform="rotate(120 150 110)"/>
          <path d="M150 110 C140 70 142 40 150 14 C158 40 160 70 150 110Z" fill="#14B8A6" transform="rotate(240 150 110)"/>
        </g>
        <circle cx="150" cy="110" r="10" fill="#F1F5F9"/>
      </svg>
    </div>
    <div class="ctrl">
      <label for="v">Скорость ветра <output id="vo">6 м/с</output></label>
      <input id="v" type="range" min="0" max="15" step="0.5" value="6">
      <div>Относительная мощность потока (по сравнению с 15 м/с)</div>
      <div class="bar" aria-hidden="true"><span id="pb"></span></div>
      <p class="big" id="pv">6 %</p>
      <span class="status" id="st">Слабый ветер</span>
      <p style="margin-top:14px;color:var(--muted);font-size:.95rem">Расчёт: P/P₁₅ = (v / 15)³<br>Лампочка в модели загорается от 3 м/с и светит ярче с ростом мощности.</p>
    </div>
  </div>
  <article class="card rv">
    <h3>Практическая модель из проекта</h3>

<ul>
      <li>Трёхлопастной винт, угол атаки лопастей 20–25°.</li>
      <li>Коллекторный DC-мотор в режиме генератора.</li>
      <li>Мачта, светодиод и мультиметр для измерений.</li>
      <li>Замеры напряжения: от 1,2 В до 3,4 В в зависимости от силы обдува.</li>
    </ul>
  </article>
</div></section>

<section id="eco"><div class="wrap">
  <h2 class="rv">Экологический след</h2>
  <div class="tw rv"><table>
    <thead><tr><th>Станция</th><th>Главные загрязнители</th><th>Экологические риски</th></tr></thead>
    <tbody>
      <tr><td>Угольная ТЭС</td><td>CO₂, оксиды серы и азота, зола</td><td>Кислотные дожди, парниковый эффект, тепловое загрязнение</td></tr>
      <tr><td>Газовая ТЭС</td><td>CO₂, оксиды азота</td><td>Парниковый эффект, тепловое загрязнение</td></tr>
      <tr><td>АЭС</td><td>Радиоактивные отходы</td><td>Хранение отходов, риск аварий, тепловое загрязнение водоёмов</td></tr>
      <tr><td>Крупная ГЭС</td><td>Химических выбросов мало</td><td>Затопление земель, нарушение жизни рыб и русла реки</td></tr>
      <tr class="wind"><td>Ветряная ВЭС</td><td>Нет химических выбросов при генерации</td><td>Шум, влияние на птиц, занимаемая площадь</td></tr>
    </tbody>
  </table></div>
  <p class="note rv">Зимой холодный воздух плотнее, поэтому при той же скорости ветра выработка ветрогенератора выше примерно на 10–15 %.</p>
</div></section>

<section id="result" style="background:var(--card)"><div class="wrap">
  <h2 class="rv">Выводы</h2>
  <ul class="rv" style="max-width:68ch">
    <li>Традиционная энергетика даёт стабильную мощность, но связана с выбросами, исчерпаемым топливом и КПД ТЭС всего 35–40 %.</li>
    <li>Мощность ветра растёт как v³, поэтому даже умеренный ветер даёт заметную энергию.</li>
    <li>Модель показала напряжение 1,2–3,4 В: ток вырабатывается по закону электромагнитной индукции.</li>
    <li>Гипотеза подтверждена: ветроэнергетика эффективна и экологична, в том числе при умеренных ветрах.</li>
  </ul>
  <h3 class="rv" style="margin-top:36px">Список литературы</h3>
  <ol class="refs rv">
    <li>Мякишев Г. Я. и др. Физика. 10 класс.</li>
    <li>Кашкаров А. П.</li>
    <li>Сташко В. И.</li>
    <li>Кривцов В. С.</li>
    <li>Удалов С. Н.</li>
  </ol>
</div></section>
</main>

<footer><div class="wrap">
  <p>Кельдюшов Никита Михайлович, 10А класс, МАОУ «СОШ № 7», г. Альметьевск, Республика Татарстан</p>
  <p>Руководитель: Садыкова Лилия Азатовна, учитель физики · 2026</p>
</div></footer>

<script>
(function(){
  var v=document.getElementById('v'),vo=document.getElementById('vo'),pv=document.getElementById('pv'),
      pb=document.getElementById('pb'),st=document.getElementById('st'),bl=document.getElementById('blades'),
      glow=document.getElementById('glow'),bulb=document.getElementById('bulb'),wg=document.getElementById('wind');
  var streaks=[],NS='http://www.w3.org/2000/svg',cur=6;
  for(var i=0;i<12;i++){var ln=document.createElementNS(NS,'line');wg.appendChild(ln);streaks.push({el:ln,x:Math.random()*360-30,y:18+i*24+Math.random()*10,k:.7+Math.random()*.6});}
  function drawWind(){
    var o=cur<.5?0:Math.min(.8,.2+cur*.05);
    streaks.forEach(function(k){var L=8+cur*3*k.k;
      k.el.setAttribute('x1',k.x.toFixed(1));k.el.setAttribute('x2',(k.x+L).toFixed(1));
      k.el.setAttribute('y1',k.y.toFixed(1));k.el.setAttribute('y2',k.y.toFixed(1));
      k.el.setAttribute('stroke-opacity',o);});
  }
  var angle=0,speed=0,last=performance.now();
  var reduce=window.matchMedia('(prefers-reduced-motion: reduce)').matches;
  function update(){
    var s=parseFloat(v.value),p=Math.pow(s/15,3)*100;
    vo.textContent=s.toString().replace('.',',')+' м/с';
    pv.textContent=(p<10?p.toFixed(1):Math.round(p)).toString().replace('.',',')+' %';
    pb.style.width=p+'%';
    var t;
    if(s<3)t='Штиль: лопасти почти не вращаются';

else if(s<5)t='Слабый старт (3–4 м/с)';
    else if(s<10)t='Рабочий режим';
    else if(s<=12)t='Номинальный режим (10–12 м/с)';
    else t='Сильный ветер';
    st.textContent=t;
    speed=s<3?s*8:s*40;
    cur=s;
    var b=s<3?0:Math.min(1,Math.sqrt(p/100));
    glow.setAttribute('opacity',(b*.55).toFixed(2));
    bulb.setAttribute('fill',b>0?'#FDE047':'#334155');
    bulb.setAttribute('fill-opacity',b>0?(.35+.65*b).toFixed(2):1);
    drawWind();
  }
  function frame(now){
    var dt=(now-last)/1000;last=now;
    if(!reduce){angle=(angle+speed*dt)%360;bl.setAttribute('transform','rotate('+angle.toFixed(1)+' 150 110)');
      streaks.forEach(function(k){k.x+=cur*24*k.k*dt;if(k.x>320){k.x=-50;}});
      drawWind();}
    requestAnimationFrame(frame);
  }
  v.addEventListener('input',update);update();requestAnimationFrame(frame);
  var els=document.querySelectorAll('.rv');
  if('IntersectionObserver' in window){
    var io=new IntersectionObserver(function(e){e.forEach(function(x){if(x.isIntersecting){x.target.classList.add('in');io.unobserve(x.target);}});},{threshold:.12});
    els.forEach(function(el){io.observe(el);});
  }else{els.forEach(function(el){el.classList.add('in');});}
})();
</script>
</body>
</html>
