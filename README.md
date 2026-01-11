<html lang="tr" style="scroll-behavior: smooth;">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fusion Robotics 7682 | It Should Work In Theory</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <style>
        body { font-family: 'Roboto', sans-serif; background: #001233; color: #e5e7eb; }
        .navbar { backdrop-filter: blur(10px); background: rgba(0, 18, 51, 0.8); }
        .section { scroll-margin-top: 80px; padding: 4rem 1.5rem; border-bottom: 1px solid #1e3a8a; }
        
        /* Takım Renkleri: Koyu Mavi, Açık Mavi, Beyaz */
        .text-fusion-light { color: #00a8e8; }
        .bg-fusion-dark { background-color: #001233; }
        .bg-fusion-blue { background-color: #002366; }
        .border-fusion { border-color: #00a8e8; }

        .timeline::before {
            content: ''; position: absolute; top: 0; left: 50%; width: 4px;
            height: 100%; background: linear-gradient(to bottom, #00a8e8, #002366);
            transform: translateX(-50%);
        }
        .timeline-item { position: relative; width: 45%; background: #002366; padding: 1.5rem; border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.3); transition: 0.3s; }
        .timeline-item:hover { transform: scale(1.02); }
        .timeline-item.left { margin-left: 55%; }
        .timeline-item.right { margin-right: 55%; }
        
        .robot-card { background: #002366; border-top: 4px solid #00a8e8; transition: 0.3s; }
        .robot-card:hover { transform: translateY(-10px); }

        @media (max-width: 768px) {
            .timeline::before { left: 20px; }
            .timeline-item { width: calc(100% - 60px); margin-left: 40px !important; }
        }
    </style>
</head>
<body>

    <nav class="navbar fixed top-0 w-full z-50 py-4 px-6 flex justify-between items-center border-b border-blue-900">
        <div class="text-2xl font-bold text-white"><span class="text-fusion-light">FUSION</span> 7682</div>
        <div class="hidden md:flex space-x-6">
            <a href="#home" class="hover:text-fusion-light transition">Ana Sayfa</a>
            <a href="#about" class="hover:text-fusion-light transition">Hakkımızda</a>
            <a href="#events" class="hover:text-fusion-light transition">Başarılar</a>
            <a href="#robots" class="hover:text-fusion-light transition">Robotlar</a>
            <a href="#contact" class="hover:text-fusion-light transition">İletişim</a>
        </div>
        <div class="lang-toggle">
            <button class="bg-blue-800 px-3 py-1 rounded text-sm font-bold">TR</button>
        </div>
    </nav>

    <section id="home" class="min-h-screen flex items-center justify-center text-center bg-gradient-to-b from-black to-fusion-dark">
        <div class="p-8">
            <h1 class="text-6xl font-extrabold text-white mb-4">FUSION ROBOTICS</h1>
            <p class="text-2xl text-fusion-light italic mb-8">"It Should Work In Theory"</p>
            <a href="#events" class="px-8 py-3 bg-blue-600 text-white rounded-full font-bold hover:bg-blue-500 transition">Serüvenimizi Gör</a>
        </div>
    </section>

    <section id="about" class="section">
        <div class="max-w-5xl mx-auto grid md:grid-cols-2 gap-12 items-center">
            <div>
                <h2 class="text-4xl font-bold text-fusion-light mb-6">Hakkımızda</h2>
                <p class="text-lg leading-relaxed">
                    Füsun Yönder Anadolu Lisesi'nin kalbinde doğan <b>Fusion Robotics #7682</b>, teoriyi pratiğe döken bir mühendislik topluluğudur. 
                    Bahçelievler'den yola çıkarak uluslararası arenalarda (FRC, Teknofest) okulumuzu ve ülkemizi temsil ediyoruz. 
                    Mottorumuz olan <i>"It Should Work In Theory"</i> ile her soruna bilimsel bir merakla yaklaşıyoruz.
                </p>
            </div>
            <div class="bg-blue-900 p-8 rounded-2xl text-center border-2 border-dashed border-fusion">
                <span class="text-6xl font-bold">#7682</span>
                <p class="mt-2 font-bold tracking-widest">FÜSUN YÖNDER ANADOLU LİSESİ</p>
            </div>
        </div>
    </section>

    <section id="events" class="section">
        <h2 class="text-4xl font-bold text-center text-fusion-light mb-16">Başarı Yolculuğumuz</h2>
        <div class="timeline relative max-w-5xl mx-auto">
            
            <div class="timeline-item left mb-8">
                <span class="text-fusion-light font-bold">2024</span>
                <h3 class="text-xl font-bold">Aerospace Valley Regional</h3>
                <p class="text-gray-400">ABD California'da düzenlenen yarışmada 7. olduk.</p>
            </div>

            <div class="timeline-item right mb-8">
                <span class="text-fusion-light font-bold">2023</span>
                <h3 class="text-xl font-bold">Haliç Regional</h3>
                <p class="text-gray-400">Finallere yükseldik, En İyi 3. İttifak başarısı.</p>
            </div>

            <div class="timeline-item left mb-8">
                <span class="text-fusion-light font-bold">2022</span>
                <h3 class="text-xl font-bold">Pendik Off-Season</h3>
                <p class="text-fusion-light font-bold">🏆 Şampiyon (Winner)</p>
                <p class="text-gray-400">İttifakımızla birlikte birincilik kupasını kaldırdık.</p>
            </div>

            <div class="timeline-item right mb-8">
                <span class="text-fusion-light font-bold">2021</span>
                <h3 class="text-xl font-bold">Teknofest</h3>
                <p class="text-fusion-light font-bold">🥈 Türkiye İkincisi</p>
                <p class="text-gray-400">Eğitim Teknolojileri alanında 243 takım arasından 2. olduk.</p>
            </div>

            <div class="timeline-item left mb-8">
                <span class="text-fusion-light font-bold">2019</span>
                <h3 class="text-xl font-bold">GameX Expo Off-Season</h3>
                <p class="text-gray-400">Yarı finallere çıkma başarısı gösterdik.</p>
            </div>

        </div>
    </section>

    <section id="robots" class="section bg-black bg-opacity-30">
        <h2 class="text-4xl font-bold text-center text-fusion-light mb-12">Robotlarımız</h2>
        <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 text-center">
            <div class="robot-card p-8 rounded-xl">
                <h3 class="text-2xl font-bold mb-2">Sezon 2024</h3>
                <p class="text-fusion-light font-mono">Status: Retired</p>
                <p class="mt-4 text-gray-400 italic">Aerospace Valley Prototipi</p>
            </div>
            <div class="robot-card p-8 rounded-xl border-fusion shadow-2xl">
                <h3 class="text-2xl font-bold mb-2">Sezon 2022</h3>
                <p class="text-green-400 font-mono">Status: Winner</p>
                <p class="mt-4 text-gray-400 italic">Pendik Off-Season Champion</p>
            </div>
            <div class="robot-card p-8 rounded-xl opacity-70">
                <h3 class="text-2xl font-bold mb-2">Sezon 2019</h3>
                <p class="text-gray-400 font-mono">Status: Legacy</p>
                <p class="mt-4 text-gray-400 italic">Early Prototypes</p>
            </div>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="max-w-5xl mx-auto grid md:grid-cols-2 gap-12">
            <div class="bg-fusion-blue p-8 rounded-2xl">
                <h2 class="text-3xl font-bold text-fusion-light mb-6">Bize Ulaşın</h2>
                <p class="mb-4">📍 Bahçelievler / İstanbul</p
