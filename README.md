
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080d19">

<title>MOWAFY Web Design | تصميم مواقع احترافية</title>
<meta name="description" content="MOWAFY Web Design - تصميم وتطوير مواقع احترافية للشركات والمشاريع والأفراد.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>
:root {
  --bg:#080d19;
  --card:#111a2b;
  --gold:#d6ae63;
  --white:#f7f8fc;
  --muted:#a2adbf;
}

* {
  margin:0;
  padding:0;
  box-sizing:border-box;
  scroll-behavior:smooth;
}

body {
  font-family:'Cairo',sans-serif;
  background:var(--bg);
  color:var(--white);
  overflow-x:hidden;
}

a {
  color:inherit;
  text-decoration:none;
}

.container {
  width:min(1120px,90%);
  margin:auto;
}

header {
  position:sticky;
  top:0;
  z-index:100;
  background:rgba(8,13,25,.93);
  backdrop-filter:blur(15px);
  border-bottom:1px solid #ffffff12;
}

.nav {
  min-height:76px;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:15px;
}

.logo {
  font-size:25px;
  font-weight:900;
  color:var(--gold);
  letter-spacing:1px;
}

.logo span {
  color:white;
}

nav {
  display:flex;
  gap:25px;
}

nav a {
  color:#c4ccda;
  font-size:14px;
  transition:.3s;
}

nav a:hover {
  color:var(--gold);
}

.menu-btn {
  display:none;
  background:none;
  color:white;
  border:0;
  font-size:27px;
  cursor:pointer;
}

.hero {
  min-height:620px;
  display:flex;
  align-items:center;
  text-align:center;
  position:relative;
  overflow:hidden;
  background:
    radial-gradient(ellipse at 50% 30%,#c18b3420,transparent 55%);
}

.hero-content {
  max-width:850px;
  margin:auto;
  padding:100px 0;
}

.tag {
  display:inline-block;
  color:var(--gold);
  border:1px solid #d6ae6350;
  background:#d6ae6310;
  border-radius:30px;
  padding:8px 20px;
  font-size:13px;
  margin-bottom:25px;
}

.hero h1 {
  font-size:clamp(35px,7vw,67px);
  line-height:1.35;
  font-weight:900;
  margin-bottom:22px;
}

.hero h1 span {
  color:var(--gold);
}

.hero p {
  color:var(--muted);
  max-width:650px;
  margin:0 auto 32px;
  line-height:2.1;
  font-size:16px;
}

.buttons {
  display:flex;
  justify-content:center;
  flex-wrap:wrap;
  gap:13px;
}

.btn {
  padding:13px 27px;
  border-radius:9px;
  font-family:inherit;
  font-weight:700;
  display:inline-block;
  transition:.3s;
  cursor:pointer;
  border:1px solid transparent;
}

.btn:hover {
  transform:translateY(-4px);
}

.primary {
  background:var(--gold);
  color:#111;
}

.secondary {
  border-color:#ffffff35;
  color:white;
}

.section {
  padding:90px 0;
}

.section-title {
  text-align:center;
  margin-bottom:48px;
}

.section-title small {
  color:var(--gold);
  font-weight:700;
  letter-spacing:2px;
}

.section-title h2 {
  font-size:32px;
  margin:10px 0;
}

.section-title p {
  color:var(--muted);
  font-size:14px;
}

.about-grid {
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:45px;
  align-items:center;
}

.about-box {
  background:linear-gradient(145deg,#162238,#0d1422);
  border:1px solid #ffffff12;
  border-radius:18px;
  padding:35px;
}

.about-box h3 {
  font-size:25px;
  margin-bottom:17px;
  color:var(--gold);
}

.about-box p {
  color:var(--muted);
  line-height:2.2;
}

.features {
  display:grid;
  grid-template-columns:1fr 1fr;
  gap:15px;
  margin-top:25px;
}

.feature {
  padding:17px;
  border-radius:12px;
  background:#ffffff08;
  font-size:14px;
}

.feature b {
  color:var(--gold);
  display:block;
  margin-bottom:5px;
}

.about-visual {
  min-height:330px;
  border:1px solid #d6ae6330;
  border-radius:20px;
  display:flex;
  align-items:center;
  justify-content:center;
  background:
    radial-gradient(circle at center,#d6ae6320,transparent 60%),
    #111a2b;
  text-align:center;
}

.about-visual strong {
  display:block;
  font-size:55px;
  color:var(--gold);
  letter-spacing:3px;
}

.about-visual span {
  color:var(--muted);
  font-size:14px;
}

.services {
  background:#0c1321;
}

.cards {
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.card {
  background:var(--card);
  border:1px solid #ffffff12;
  border-radius:16px;
  padding:27px;
  transition:.3s;
}

.card:hover {
  transform:translateY(-7px);
  border-color:#d6ae6380;
}

.icon {
  width:55px;
  height:55px;
  border-radius:13px;
  background:#d6ae6315;
  color:var(--gold);
  display:grid;
  place-items:center;
  font-size:25px;
  margin-bottom:20px;
}

.card h3 {
  font-size:18px;
  margin-bottom:12px;
}

.card p {
  font-size:13px;
  line-height:2;
  color:var(--muted);
}

.portfolio-grid {
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.project {
  overflow:hidden;
  background:var(--card);
  border:1px solid #ffffff12;
  border-radius:16px;
}

.project-image {
  height:180px;
  display:grid;
  place-items:center;
  background:linear-gradient(135deg,#172944,#263c53);
  color:var(--gold);
  font-size:35px;
  font-weight:900;
}

.project-info {
  padding:20px;
}

.project-info h3 {
  margin-bottom:8px;
}

.project-info p {
  color:var(--muted);
  font-size:13px;
  line-height:1.9;
}

.project-label {
  display:inline-block;
  margin-top:12px;
  color:var(--gold);
  font-size:11px;
}

.steps {
  display:grid;
  grid-template-columns:repeat(3,1fr);
  gap:20px;
}

.step {
  text-align:center;
  padding:28px 20px;
  background:var(--card);
  border-radius:15px;
  border:1px solid #ffffff12;
}

.step-number {
  font-size:35px;
  color:var(--gold);
  font-weight:900;
}

.step h3 {
  margin:10px 0;
}

.step p {
  font-size:13px;
  color:var(--muted);
  line-height:2;
}

.contact {
  background:
    radial-gradient(ellipse at center,#d6ae6314,transparent 65%),
    #0c1321;
}

.contact-box {
  max-width:700px;
  margin:auto;
  background:var(--card);
  padding:35px;
  border:1px solid #ffffff15;
  border-radius:18px;
}

.contact-box input,
.contact-box textarea {
  width:100%;
  padding:14px;
  margin-bottom:14px;
  background:#080d19;
  border:1px solid #ffffff20;
  border-radius:9px;
  color:white;
  font-family:inherit;
  outline:none;
}

.contact-box input:focus,
.contact-box textarea:focus {
  border-color:var(--gold);
}

.contact-box textarea {
  height:120px;
  resize:vertical;
}

.contact-box button {
  width:100%;
  font-size:15px;
}

footer {
  padding:35px 0;
  text-align:center;
  border-top:1px solid #ffffff12;
}

footer .logo {
  margin-bottom:10px;
}

footer p {
  color:var(--muted);
  font-size:12px;
  line-height:2;
}

.whatsapp {
  position:fixed;
  bottom:20px;
  left:20px;
  z-index:99;
  background:#20c875;
  color:#06170d;
  width:55px;
  height:55px;
  border-radius:50%;
  display:grid;
  place-items:center;
  font-size:25px;
  font-weight:bold;
  box-shadow:0 5px 25px #20c87550;
}

@media(max-width:800px) {
  nav {
    display:none;
    position:absolute;
    top:76px;
    right:0;
    left:0;
    background:#101a2b;
    padding:20px;
    flex-direction:column;
    gap:17px;
  }

  nav.active {
    display:flex;
  }

  .menu-btn {
    display:block;
  }

  .about-grid {
    grid-template-columns:1fr;
  }

  .cards,
  .portfolio-grid {
    grid-template-columns:1fr 1fr;
  }

  .steps {
    grid-template-columns:1fr;
  }

  .hero {
    min-height:550px;
  }
}

@media(max-width:520px) {
  .cards,
  .portfolio-grid {
    grid-template-columns:1fr;
  }

  .section {
    padding:65px 0;
  }

  .section-title h2 {
    font-size:26px;
  }

  .about-box,
  .contact-box {
    padding:23px;
  }
}
</style>
</head>

<body>

<header>
  <div class="container nav">
    <a href="#home" class="logo">MOWAFY<span>.</span></a>

    <button class="menu-btn" id="menuBtn" aria-label="فتح القائمة">☰</button>

    <nav id="nav">
      <a href="#home">الرئيسية</a>
      <a href="#about">من نحن</a>
      <a href="#services">خدماتنا</a>
      <a href="#portfolio">أعمالنا</a>
      <a href="#contact">تواصل معنا</a>
    </nav>
  </div>
</header>

<main>

<section class="hero" id="home">
  <div class="container hero-content">
    <span class="tag">MOWAFY WEB DESIGN</span>

    <h1>
      نصنع لك حضورًا رقميًا
      <span>يليق بطموحك</span>
    </h1>

    <p>
      نصمم مواقع إلكترونية عصرية واحترافية تساعد مشروعك على الظهور
      بشكل مميز أمام عملائك، وتمنحك بداية قوية في العالم الرقمي.
    </p>

    <div class="buttons">
      <a href="#contact" class="btn primary">اطلب موقعك الآن</a>
      <a href="#services" class="btn secondary">اكتشف خدماتنا</a>
    </div>
  </div>
</section>

<section class="section" id="about">
  <div class="container">
    <div class="about-grid">

      <div class="about-box">
        <h3>من نحن؟</h3>
        <p>
          MOWAFY Web Design علامة متخصصة في تصميم وتطوير المواقع
          الإلكترونية للأفراد والشركات والمشروعات الصغيرة.
          نركز على التصميم العصري، سهولة الاستخدام، والتوافق مع
          جميع الشاشات.
        </p>

        <div class="features">
          <div class="feature">
            <b>01</b>
            تصميم عصري
          </div>
          <div class="feature">
            <b>02</b>
            متوافق مع الموبايل
          </div>
          <div class="feature">
            <b>03</b>
            سرعة وسهولة
          </div>
          <div class="feature">
            <b>04</b>
            تجربة مميزة
          </div>
        </div>
      </div>

      <div class="about-visual">
        <div>
          <strong>MOWAFY</strong>
          <span>CREATIVE WEB DESIGN</span>
        </div>
      </div>

    </div>
  </div>
</section>

<section class="section services" id="services">
  <div class="container">

    <div class="section-title">
      <small>WHAT WE DO</small>
      <h2>خدماتنا</h2>
      <p>كل ما يحتاجه مشروعك للانطلاق على الإنترنت</p>
    </div>

    <div class="cards">

      <div class="card">
        <div class="icon">✦</div>
        <h3>تصميم المواقع</h3>
        <p>تصميم مواقع عصرية تناسب هوية مشروعك وتظهر خدماتك بشكل احترافي.</p>
      </div>

      <div class="card">
        <div class="icon">▣</div>
        <h3>مواقع الشركات</h3>
        <p>مواقع تعريفية تعرض شركتك وخدماتها وطرق التواصل معها.</p>
      </div>

      <div class="card">
        <div class="icon">◈</div>
        <h3>المتاجر الإلكترونية</h3>
        <p>واجهات عرض للمنتجات تساعد نشاطك التجاري على الوصول للعملاء.</p>
      </div>

      <div class="card">
        <div class="icon">⌘</div>
        <h3>مواقع شخصية</h3>
        <p>صفحات شخصية ومعارض أعمال لعرض خبراتك ومهاراتك.</p>
      </div>

      <div class="card">
        <div class="icon">◎</div>
        <h3>صفحات الهبوط</h3>
        <p>صفحات تسويقية جذابة لعرض خدمة أو منتج محدد.</p>
      </div>

      <div class="card">
        <div class="icon">↗</div>
        <h3>تطوير المواقع</h3>
        <p>تحسين وتحديث واجهات المواقع لتصبح أسهل وأفضل في الاستخدام.</p>
      </div>

    </div>
  </div>
</section>

<section class="section" id="portfolio">
  <div class="container">

    <div class="section-title">
      <small>OUR PORTFOLIO</small>
      <h2>نماذج من أعمالنا</h2>
      <p>أفكار تجريبية توضح أنواع المواقع التي يمكننا تنفيذها</p>
    </div>

    <div class="portfolio-grid">

      <div class="project">
        <div class="project-image">CAFE</div>
        <div class="project-info">
          <h3>موقع كافيه</h3>
          <p>نموذج تجريبي لموقع كافيه يعرض القائمة والخدمات.</p>
          <span class="project-label">DEMO PROJECT</span>
        </div>
      </div>

      <div class="project">
        <div class="project-image">BUSINESS</div>
        <div class="project-info">
          <h3>موقع شركة</h3>
          <p>نموذج تجريبي لموقع شركة لعرض خدماتها وبياناتها.</p>
          <span class="project-label">DEMO PROJECT</span>
        </div>
      </div>

      <div class="project">
        <div class="project-image">STORE</div>
        <div class="project-info">
          <h3>متجر إلكتروني</h3>
          <p>نموذج تجريبي لواجهة متجر لعرض المنتجات.</p>
          <span class="project-label">DEMO PROJECT</span>
        </div>
      </div>

    </div>
  </div>
</section>

<section class="section services">
  <div class="container">

    <div class="section-title">
      <small>HOW WE WORK</small>
      <h2>كيف نعمل؟</h2>
      <p>خطوات بسيطة من أول تواصل حتى استلام موقعك</p>
    </div>

    <div class="steps">

      <div class="step">
        <div class="step-number">01</div>
        <h3>فهم احتياجاتك</h3>
        <p>نتعرف على مشروعك والأفكار التي تريد تنفيذها.</p>
      </div>

      <div class="step">
        <div class="step-number">02</div>
        <h3>التصميم والتنفيذ</h3>
        <p>نبدأ تصميم الموقع وتجهيز الصفحات المطلوبة.</p>
      </div>

      <div class="step">
        <div class="step-number">03</div>
        <h3>التسليم</h3>
        <p>نراجع الموقع ونسلمه بعد الاتفاق على التفاصيل.</p>
      </div>

    </div>
  </div>
</section>

<section class="section contact" id="contact">
  <div class="container">

    <div class="section-title">
      <small>CONTACT US</small>
      <h2>خلينا نبدأ مشروعك</h2>
      <p>اكتب بياناتك وسنتواصل معك عبر واتساب</p>
    </div>

    <div class="contact-box">

      <form id="contactForm">
        <input id="clientName" type="text" placeholder="اسمك" required maxlength="80">

        <input id="clientPhone" type="tel" placeholder="رقم هاتفك" required maxlength="25">

        <input id="clientService" type="text" placeholder="نوع الموقع الذي تحتاجه" required maxlength="100">

        <textarea id="clientMessage" placeholder="اكتب تفاصيل مشروعك..."></textarea>

        <button type="submit" class="btn primary">
          إرسال الطلب عبر واتساب
        </button>
      </form>

    </div>
  </div>
</section>

</main>

<footer>
  <div class="container">
    <div class="logo">MOWAFY<span>.</span></div>
    <p>نحول أفكارك إلى مواقع إلكترونية مميزة.</p>
    <p>© 2026 MOWAFY Web Design. All Rights Reserved.</p>
  </div>
</footer>

<a class="whatsapp" id="whatsappLink" href="#" aria-label="واتساب">W</a>

<script>
// ضع رقم واتساب الخاص بك هنا بكود الدولة
// مثال: 2010XXXXXXXX
const WHATSAPP_NUMBER = "2010XXXXXXXX";

document.getElementById("menuBtn").addEventListener("click",function(){
  document.getElementById("nav").classList.toggle("active");
});

document.querySelectorAll("#nav a").forEach(function(link){
  link.addEventListener("click",function(){
    document.getElementById("nav").classList.remove("active");
  });
});

function openWhatsApp(message){
  if(!/^20\d{10}$/.test(WHATSAPP_NUMBER)){
    alert("يرجى إضافة رقم واتساب الصحيح داخل الكود أولاً.");
    return;
  }

  const url = "https://wa.me/" + WHATSAPP_NUMBER +
    "?text=" + encodeURIComponent(message);

  window.open(url,"_blank");
}

document.getElementById("whatsappLink").addEventListener("click",function(e){
  e.preventDefault();
  openWhatsApp("مرحباً MOWAFY Web Design، أريد الاستفسار عن خدمات تصميم المواقع.");
});

document.getElementById("contactForm").addEventListener("submit",function(e){
  e.preventDefault();

  const name = document.getElementById("clientName").value.trim();
  const phone = document.getElementById("clientPhone").value.trim();
  const service = document.getElementById("clientService").value.trim();
  const message = document.getElementById("clientMessage").value.trim();

  const text =
    "طلب جديد من موقع MOWAFY Web Design\n\n" +
    "الاسم: " + name + "\n" +
    "الهاتف: " + phone + "\n" +
    "نوع الموقع: " + service + "\n" +
    "التفاصيل: " + message;

  openWhatsApp(text);
});
</script>

</body>
</html>
