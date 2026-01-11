<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fusion Robotics #7682 | It Should Work In Theory</title>
    <style>
        /* Renk Paleti: Koyu Mavi, Açık Mavi, Beyaz */
        :root {
            --dark-blue: #002366;
            --light-blue: #00a8e8;
            --white: #ffffff;
            --gray: #f8f9fa;
        }

        body { 
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif; 
            margin: 0; 
            line-height: 1.6; 
            color: #333; 
            background-color: var(--white);
        }

        header { 
            background: var(--dark-blue); 
            color: var(--white); 
            padding: 3rem 1rem; 
            text-align: center; 
            border-bottom: 5px solid var(--light-blue); 
        }

        header h1 { margin: 0; font-size: 2.5rem; letter-spacing: 2px; }
        header p { font-style: italic; opacity: 0.9; margin-top: 10px; }

        nav { 
            background: #001a4d; 
            color: var(--white); 
            text-align: center; 
            padding: 15px; 
            position: sticky; 
            top: 0; 
            z-index: 1000;
        }
        nav a { color: white; margin: 0 15px; text-decoration: none; font-weight: bold; transition: 0.3s; }
        nav a:hover { color: var(--light-blue); }

        .container { max-width: 1100px; margin: auto; padding: 20px; }

        .hero { 
            text-align: center; 
            padding: 60px 20px; 
            background: var(--gray); 
            border-radius: 15px; 
            margin-top: 20px;
            border-left: 10px solid var(--dark-blue);
        }

        .section-title {
            text-align: center;
            color: var(--dark-blue);
            border-bottom: 2px solid var(--light-blue);
            display: inline-block;
            margin-bottom: 30px;
            padding-bottom: 5px;
        }

        .section { margin: 50px 0; text-align: center; }

        /* Başarılar Kart Tasarımı */
        .achievement-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .card { 
            border: none; 
            padding: 25px; 
            border-radius: 12px; 
            background: var(--white); 
            box-shadow: 0 6px 15px rgba(0,0,0,0.1); 
            transition: transform 0.3s;
            text-align: left;
            border-top: 4px solid var(--light-blue);
        }
        .card:hover { transform: translateY(-5px); }
        .card h3 { color: var(--dark-blue); margin-top: 0; }
        .card span { color: var(--light-blue); font-weight: bold; font-size: 0.9rem; }

        footer { 
            background: var(--dark-blue); 
            color: white; 
            text-align: center; 
            padding: 30px; 
            margin-top: 60px; 
        }

        .highlight { color: var(--light-blue); font-weight: bold; }

        @media (max-width: 600px) {
            header h1 { font-size: 1.8rem; }
            nav a { display: block; margin: 10px 0; }
        }
    </style>
</head>
<body>

<header>
    <h1>FUSION ROBOTICS #7682</h1>
    <p>"It Should Work In Theory"</p>
</header>

<nav>
    <a href="#hakkimizda">Hakkımızda</a>
    <a href="#basarilar">Başarılarımız</a>
    <a href="#iletisim">İletişim</a>
</nav>

<div class="container">
    <section id="hakkimizda" class="hero">
        <h2 class="section-title">Biz Kimiz?</h2>
        <p><strong>Füsun Yönder Anadolu Lisesi</strong> bünyesinde kurulan <strong>Fusion Robotics #7682</strong>, teknoloji ve mühendislik tutkusuyla bir araya gelmiş bir FRC takımıdır. Teorideki projelerimizi pratiğe dökerek, robotik dünyasında fark yaratmayı hedefliyoruz.</p>
    </section>

    <section id="basarilar" class="section">
        <h2 class="section-title">Başarı Yolculuğumuz</h2>
        
        <div class="achievement-grid">
            <div class="card">
                <span>FRC 2024</span>
                <h3>Aerospace Valley Regional</h3>
                <p>Amerika'da düzenlenen Aerospace Valley Regional yarışmasında zorlu rakipler arasından sıyrılarak yarışmayı 7. sırada tamamladık.</p>
            </div>

            <div class="card">
                <span>FRC 2023</span>
                <h3>Haliç Regional</h3>
                <p>İttifak takımlarımızla birlikte büyük bir uyumla çalışarak finallere yükseldik ve en iyi 3. ittifak olma başarısını gösterdik.</p>
            </div>

            <div class="card">
                <span>FRC 2022</span>
                <h3>Pendik Off-Season</h3>
                <p>İttifakımızla birlikte turnuva şampiyonu olarak <span class="highlight">"Winner"</span> ödülünü kazandık.</p>
            </div>

            <div class="card">
                <span>FRC 2022</span>
                <h3>Bosphorus Regional</h3>
                <p>Pandemi sonrası ilk saha deneyimimizde teknik arızalara rağmen pes etmeyerek takım ruhunu ve tecrübemizi pekiştirdik.</p>
            </div>

            <div class="card" style="border-top-color: #ff5722;">
                <span>TEKNOFEST 2021</span>
                <h3>Türkiye İkinciliği</h3>
                <p>Eğitim Teknolojileri alanında 243 takım arasından Türkiye ikincisi olarak büyük bir başarıya imza attık.</p>
            </div>

            <div class="card" style="border-top-color: #ff5722;">
                <span>TEKNOFEST 2020</span>
                <h3>Gaziantep Finalleri</h3>
                <p>Gaziantep'te düzenlenen yarışmada projemizle finallere yükselerek takımımızı temsil ettik.</p>
            </div>

            <div class="card">
                <span>FRC 2019</span>
                <h3>GameX Expo Off-Season</h3>
                <p>İstanbul'da düzenlenen turnuvada başarılı bir performans sergileyerek yarı finallere yükseldik.</p>
            </div>

            <div class="card">
                <span>FRC 2019</span>
                <h3>Mersin Off-Season</h3>
                <p>Teknik zorluklarla geçen bu süreç, bize kriz yönetimi ve tecrübe anlamında paha biçilemez deneyimler kazandırdı.</p>
            </div>
        </div>
    </section>

    <section id="iletisim" class="section">
        <h2 class="section-title">İletişim</h2>
        <p>Projemize destek olmak veya ekibimize katılmak için bize ulaşın.</p>
        <p>🏢 <strong>Okul:</strong> Füsun Yönder Anadolu Lisesi</p>
        <p>📍 <strong>Konum:</strong> Bahçelievler / İstanbul</p>
        <p>📧 <strong>E-posta:</strong> info@fusionrobotics7682.com</p>
    </section>
</div>

<footer>
    <p>&copy; 2026 Fusion Robotics #7682 - It Should Work In Theory</p>
    <p><small>Füsun Yönder Anadolu Lisesi Robotik Takımı</small></p>
</footer>

</body>
</html>
