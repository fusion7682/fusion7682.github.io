<!DOCTYPE html>
<html lang="tr" style="scroll-behavior:smooth;">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Fusion Robotics 7682 | It Should Work In Theory</title>

<link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">

<style>
body{
    font-family:'Roboto',sans-serif;
    background:#001233;
    color:#e5e7eb;
}

/* Navbar */
.navbar{
    backdrop-filter:blur(12px);
    background:rgba(0,18,51,.85);
}

/* Sections */
.section{
    scroll-margin-top:90px;
    padding:5rem 1.5rem;
    border-bottom:1px solid #1e3a8a;
}

/* Colors */
.text-fusion{color:#00a8e8;}
.bg-fusion-blue{background:#002366;}
.border-fusion{border-color:#00a8e8;}

/* Hero */
.hero-bg{
    background:linear-gradient(to bottom,#000,#001233);
}
.hero-glow{
    text-shadow:0 0 35px rgba(0,168,232,.45);
}

/* Timeline */
.timeline::before{
    content:'';
    position:absolute;
    left:50%;
    top:0;
    width:3px;
    height:100%;
    background:linear-gradient(to bottom,#00a8e8,#002366);
    transform:translateX(-50%);
}

.timeline-item{
    position:relative;
    width:45%;
    background:rgba(0,35,102,.92);
    padding:1.75rem;
    border-radius:16px;
    box-shadow:0 12px 32px rgba(0,0,0,.35);
    transition:.3s;
}
.timeline-item:hover{transform:translateY(-6px);}
.timeline-item.left{margin-left:55%;}
.timeline-item.right{margin-right:55%;}

.timeline-item::before{
    content:'';
    position:absolute;
    top:26px;
    width:14px;
    height:14px;
    background:#00a8e8;
    border-radius:50%;
    box-shadow:0 0 14px rgba(0,168,232,.8);
}
.timeline-item.left::before{left:-34px;}
.timeline-item.right::before{right:-34px;}

/* Robot cards */
.robot-card{
    background:rgba(0,35,102,.9);
    border-top:4px solid #00a8e8;
    backdrop-filter:blur(6px);
    transition:.3s;
}
.robot-card:hover{transform:translateY(-12px);}

/* Scroll animations */
.reveal{
    opacity:0;
    transform:translateY(40px);
    transition:all .9s ease;
}
.reveal-left{
    opacity:0;
    transform:translateX(-60px);
    transition:all .9s ease;
}
.reveal-right{
    opacity:0;
    transform:translateX(60px);
    transition:all .9s ease;
}
.active{
    opacity:1;
    transform:translate(0);
}

/* Mobile */
@media(max-width:768px){
    .timeline::before{left:20px;}
    .timeline-item{
        width:calc(100% - 60px);
        margin-left:40px !important;
        margin-right:0 !important;
    }
}
</style>
</head>

<body>

<!-- NAVBAR -->
<nav class="navbar fixed top-0 w-full z-50 py-4 px-6 flex justify-between items-center border-b border-blue-900">
    <div class="text-2xl font-bold">
        <span class="text-fusion">FUSION</span> 7682
    </div>
    <div class="hidden md:flex space-x-6">
        <a href="#home" class="hover:text-fusion transition">Ana Sayfa</a>
        <a href="#about" class="hover:text-fusion transition">Hakkımızda</a>
        <a href="#events" class="hover:text-fusion transition">Başarılar</a>
        <a href="#robots" class="hover:text-fusion transition">Robotlar</a>
        <a href="#contact" class="hover:text-fusion transition">İletişim</a>
    </div>
    <button class="bg-blue-800 px-3 py-1 rounded text-sm font-bold">TR</button>
</nav>

<!-- HERO -->
<section id="home" class="min-h-screen hero-bg flex items-center justify-center text-center">
    <div>
        <h1 class="text-6xl font-extrabold mb-4 hero-glow reveal">
            FUSION ROBOTICS
        </h1>
        <p class="text-2xl text-fusion italic mb-8 reveal">
            "It Should Work In Theory"
        </p>
        <a href="#events" class="px-8 py-3 bg-blue-600 rounded-full font-bold hover:bg-blue-500 transition reveal">
            Serüvenimizi Gör
        </a>
    </div>
</section>

<!-- ABOUT -->
<section id="about" class="section">
<div class="max-w-5xl mx-auto grid md:grid-cols-2 gap-12 items-center">
    <div class="reveal">
        <h2 class="text-4xl font-bold text-fusion mb-6">Hakkımızda</h2>
        <p class="text-lg leading-relaxed">
            Füsun Yönder Anadolu Lisesi'nde doğan <b>Fusion Robotics #7682</b>,
            teoriyi pratiğe dönüştüren bir mühendislik topluluğudur.
            FRC ve Teknofest sahnelerinde okulumuzu ve ülkemizi temsil ediyoruz.
        </p>
    </div>
    <div class="bg-fusion-blue p-10 rounded-2xl text-center border border-fusion reveal">
        <span class="text-6xl font-bold">#7682</span>
        <p class="mt-3 font-bold tracking-widest">FÜSUN YÖNDER A.L.</p>
    </div>
</div>
</section>

<!-- TIMELINE -->
<section id="events" class="section">
<h2 class="text-4xl font-bold text-center text-fusion mb-16 reveal">
    Başarı Yolculuğumuz
</h2>

<div class="timeline relative max-w-5xl mx-auto space-y-14">

<div class="timeline-item left reveal-left">
    <span class="text-fusion font-bold">2024</span>
    <h3 class="text-xl font-bold">Aerospace Valley Regional</h3>
    <p class="text-gray-400">California – 7.’lik</p>
</div>

<div class="timeline-item right reveal-right">
    <span class="text-fusion font-bold">2023</span>
    <h3 class="text-xl font-bold">Haliç Regional</h3>
    <p class="text-gray-400">En İyi 3. İttifak</p>
</div>

<div class="timeline-item left reveal-left">
    <span class="text-fusion font-bold">2022</span>
    <h3 class="text-xl font-bold">Pendik Off-Season</h3>
    <p class="text-fusion font-bold">🏆 Şampiyon</p>
</div>

<div class="timeline-item right reveal-right">
    <span class="text-fusion font-bold">2021</span>
    <h3 class="text-xl font-bold">Teknofest</h3>
    <p class="text-fusion font-bold">🥈 Türkiye 2.si</p>
</div>

</div>
</section>

<!-- ROBOTS -->
<section id="robots" class="section bg-black bg-opacity-30">
<h2 class="text-4xl font-bold text-center text-fusion mb-12 reveal">
    Robotlarımız
</h2>

<div class="max-w-6xl mx-auto grid md:grid-cols-3 gap-8 text-center">
    <div class="robot-card p-8 rounded-xl reveal">
        <h3 class="text-2xl font-bold">2024</h3>
        <p class="text-fusion font-mono">Retired</p>
    </div>

    <div class="robot-card p-8 rounded-xl shadow-2xl reveal">
        <h3 class="text-2xl font-bold">2022</h3>
        <p class="text-green-400 font-mono">Winner</p>
    </div>

    <div class="robot-card p-8 rounded-xl opacity-70 reveal">
        <h3 class="text-2xl font-bold">2019</h3>
        <p class="text-gray-400 font-mono">Legacy</p>
    </div>
</div>
</section>

<!-- CONTACT -->
<section id="contact" class="section">
<div class="max-w-5xl mx-auto bg-fusion-blue p-10 rounded-2xl text-center reveal">
    <h2 class="text-3xl font-bold text-fusion mb-4">Bize Ulaşın</h2>
    <p>📍 Bahçelievler / İstanbul</p>
</div>
</section>

<!-- JS: Scroll Animations -->
<script>
const elements=document.querySelectorAll('.reveal,.reveal-left,.reveal-right');
const observer=new IntersectionObserver(entries=>{
  entries.forEach(entry=>{
    if(entry.isIntersecting){
      entry.target.classList.add('active');
      observer.unobserve(entry.target);
    }
  });
},{threshold:0.15});
elements.forEach(el=>observer.observe(el));
</script>

</body>
</html>
