<html lang="el">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Φαρμακειο Μαρια Νικ. Καραμανη | Χανάκια Ηλείας</title>
    <meta name="description" content="Επαγγελματικό φαρμακείο Μαρία Νικ. Καραμάνη στα Χανάκια Ηλείας. Υπηρεσίες υγείας, εμβολιασμοί, δερμοκαλλυντικά.">
    
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --primary-color: #1a5e34;
            --primary-light: #2e7d32;
            --secondary-bg: #f4f9f4;
            --text-dark: #333333;
            --text-light: #ffffff;
            --grey-light: #e0e0e0;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: var(--text-dark);
            background-color: #fff;
        }

        h1, h2, h3 {
            color: var(--primary-color);
            font-weight: 700;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .section-padding {
            padding: 80px 0;
        }

        .text-center {
            text-align: center;
        }

        /* --- Header & Logo Logic --- */
        header {
            background-color: #fff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 0;
        }

        /* Στυλ για το Λογότυπο: Αν δεν φορτώνει η εικόνα, δείχνει ένα όμορφο εικονίδιο */
        .logo-wrapper {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-img {
            height: 60px;
            width: auto;
            display: block;
        }

        /* Placeholder σε περίπτωση που η εικόνα λείπει (όπως στο preview) */
        .logo-placeholder {
            width: 55px;
            height: 55px;
            background-color: var(--primary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
            border: 2px solid white;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        .nav-links {
            display: flex;
            gap: 30px;
            list-style: none;
        }

        .nav-links a {
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary-color);
        }

        /* --- Hero Section --- */
        .hero {
            background: linear-gradient(rgba(26, 94, 52, 0.85), rgba(26, 94, 52, 0.85)), url('https://images.unsplash.com/photo-1631549916768-4119b2e5f926?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            height: 85vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: var(--text-light);
            margin-top: 75px;
        }

        .hero-content h1 {
            color: var(--text-light);
            font-size: clamp(2rem, 5vw, 3.5rem);
            margin-bottom: 20px;
            text-transform: uppercase;
        }

        .hero-content p {
            font-size: 1.2rem;
            margin-bottom: 40px;
            max-width: 800px;
            margin-inline: auto;
            opacity: 0.9;
        }

        /* --- Buttons --- */
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            padding: 14px 28px;
            border-radius: 50px;
            font-weight: 700;
            transition: all 0.3s;
        }

        .btn i { margin-right: 10px; }

        .btn-call { background: white; color: var(--primary-color); }
        .btn-call:hover { transform: scale(1.05); background: var(--secondary-bg); }

        .btn-email { border: 2px solid white; color: white; }
        .btn-email:hover { background: white; color: var(--primary-color); }

        .btn-map { background: var(--primary-light); color: white; }
        .btn-map:hover { background: #388e3c; }

        /* --- Services --- */
        .services-section { background: var(--secondary-bg); }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 50px;
        }

        .service-card {
            background: white;
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
            transition: 0.3s;
        }

        .service-card:hover { transform: translateY(-10px); }

        .service-icon {
            font-size: 3rem;
            color: var(--primary-color);
            margin-bottom: 20px;
        }

        /* --- Info Grid --- */
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 40px;
        }

        .info-box {
            padding: 40px;
            background: white;
            border-radius: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            border-top: 5px solid var(--primary-color);
        }

        .hours-table {
            width: 100%;
            margin-top: 20px;
        }

        .hours-table td {
            padding: 12px 0;
            border-bottom: 1px solid var(--grey-light);
            font-size: 1.05rem;
        }

        .hours-table td:first-child { font-weight: 700; color: var(--primary-color); width: 35%; }

        .map-wrapper {
            height: 300px;
            border-radius: 15px;
            overflow: hidden;
            margin-top: 20px;
        }

        footer {
            background: var(--primary-color);
            color: white;
            padding: 40px 0;
            text-align: center;
        }

        @media (max-width: 768px) {
            .nav-links { display: none; }
            .hero { height: auto; padding: 100px 0; }
            .cta-buttons { flex-direction: column; width: 100%; align-items: center; }
            .btn { width: 90%; justify-content: center; }
        }
    </style>
</head>
<body>

    <header>
        <div class="container navbar">
            <div class="logo-wrapper">
                <!-- Η εικόνα θα δείχνει το placeholder αν αποτύχει να φορτώσει -->
                <img src="1000031151.jpg" alt="Logo" class="logo-img" id="mainLogo" onerror="handleImageError()">
                <div id="fallbackLogo" class="logo-placeholder" style="display:none;">MK</div>
                <div style="font-weight: 700; color: var(--primary-color); line-height: 1.1;">
                    ΦΑΡΜΑΚΕΙΟ<br><span style="font-weight: 400; font-size: 0.9rem;">ΜΑΡΙΑ ΝΙΚ. ΚΑΡΑΜΑΝΗ</span>
                </div>
            </div>
            <nav>
                <ul class="nav-links">
                    <li><a href="#services">Υπηρεσίες</a></li>
                    <li><a href="#contact">Επικοινωνία</a></li>
                    <li><a href="#location">Τοποθεσία</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section class="hero">
        <div class="container hero-content">
            <h1>Φαρμακειο Μαρια Νικ. Καραμανη</h1>
            <p>Επιστημονική κατάρτιση και φροντίδα για την υγεία σας. Βρισκόμαστε στα Χανάκια Ηλείας, έτοιμοι να σας εξυπηρετήσουμε.</p>
            
            <div class="cta-buttons">
                <a href="tel:2621054096" class="btn btn-call"><i class="fa-solid fa-phone"></i> 26210 54096</a>
                <a href="mailto:farmakeiokaramani@gmail.com" class="btn btn-email"><i class="fa-solid fa-envelope"></i> Email</a>
                <!-- Ακριβής σύνδεσμος Google Maps που δόθηκε από τον χρήστη -->
                <a href="https://www.google.com/maps/place/%CE%A6%CE%B1%CF%81%CE%BC%CE%B1%CE%BA%CE%B5%CE%AF%CE%BF+%CE%9C%CE%B1%CF%81%CE%AF%CE%B1+%CE%9D%CE%B9%CE%BA.+%CE%9A%CE%B1%CF%81%CE%B1%CE%BC%CE%AC%CE%BD%CE%B7/@37.7259941,21.3685024,17z/data=!4m14!1m7!3m6!1s0x1360b90020df5fb5:0x84a20fd2ef7d08b9!2zzqbOsc-BzrzOsc66zrXOr86_IM6czrHPgc6vzrEgzp3Ouc66LiDOms6xz4HOsc68zqzOvc63!8m2!3d37.7259941!4d21.3685024!16s%2Fg%2F11wp7r7m5b!3m5!1s0x1360b90020df5fb5:0x84a20fd2ef7d08b9!8m2!3d37.7259941!4d21.3685024!16s%2Fg%2F11wp7r7m5b" target="_blank" class="btn btn-map"><i class="fa-solid fa-location-dot"></i> Οδηγίες</a>
            </div>
        </div>
    </section>

    <section id="services" class="section-padding services-section">
        <div class="container">
            <h2 class="text-center" style="margin-bottom: 50px;">Οι Υπηρεσίες μας</h2>
            <div class="services-grid">
                <div class="service-card">
                    <i class="fa-solid fa-heart-pulse service-icon"></i>
                    <h3>Μέτρηση Πίεσης</h3>
                    <p>Δωρεάν έλεγχος και συμβουλές για την αρτηριακή πίεση.</p>
                </div>
                <div class="service-card">
                    <i class="fa-solid fa-syringe service-icon"></i>
                    <h3>Εμβολιασμοί</h3>
                    <p>Διενέργεια εποχικών εμβολιασμών με ασφάλεια.</p>
                </div>
                <div class="service-card">
                    <i class="fa-solid fa-sparkles service-icon"></i>
                    <h3>Δερμοκαλλυντικά</h3>
                    <p>Επιλεγμένα προϊόντα για την περιποίηση του δέρματος.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="section-padding">
        <div class="container">
            <div class="info-grid">
                <div class="info-box">
                    <h3><i class="fa-regular fa-clock"></i> Ωράριο Λειτουργίας</h3>
                    <table class="hours-table">
                        <tr><td>Δευτέρα</td><td>09:00 - 14:30</td></tr>
                        <tr><td>Τρίτη</td><td>09:00 - 14:30</td></tr>
                        <tr><td>Τετάρτη</td><td>09:00 - 14:30 & 18:00 - 21:00</td></tr>
                        <tr><td>Πέμπτη</td><td>09:00 - 14:30</td></tr>
                        <tr><td>Παρασκευή</td><td>09:00 - 14:30</td></tr>
                        <tr><td>Σάββατο</td><td>10:00 - 14:30</td></tr>
                        <tr><td>Κυριακή</td><td>Κλειστά</td></tr>
                    </table>
                </div>

                <div class="info-box" id="location">
                    <h3><i class="fa-solid fa-map-location-dot"></i> Πού θα μας βρείτε</h3>
                    <p><i class="fa-solid fa-location-pin"></i> Χανάκια, Ηλεία</p>
                    <div class="map-wrapper">
                        <!-- Ενημερωμένος ενσωματωμένος χάρτης -->
                        <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3152.288257007328!2d21.36592747668676!3d37.72599827199732!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1360b90020df5fb5%3A0x84a20fd2ef7d08b9!2zzqbOsc-BzrzOsc66zrXOr86_IM6czrHPgc6vzrEgzp3Ouc66LiDOms6xz4HOsc68zqzOvc63!5e0!3m2!1sel!2sgr!4v1715694567890!5m2!1sel!2sgr" width="100%" height="100%" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 Φαρμακείο Μαρία Νικ. Καραμάνη </p>
        </div>
    </footer>

    <script>
        // Λειτουργία για τη διαχείριση της εικόνας που λείπει στο preview
        function handleImageError() {
            document.getElementById('mainLogo').style.display = 'none';
            document.getElementById('fallbackLogo').style.display = 'flex';
        }
    </script>
</body>
</html>
