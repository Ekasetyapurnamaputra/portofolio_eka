<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My portofolio</title>
    <style>
        :root {
            --primary: #2563eb;
            --primary-dark: #1d4ed8;
            --secondary: #f59e0b;
            --dark: #1e293b;
            --light: #f8fafc;
            --gray: #94a3b8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, -apple-system, sans-serif;
        }

        body {
            background-color: #f1f5f9;
            color: var(--dark);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        header {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }

        .profile-picture {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
            margin-bottom: 1.5rem;
        }

        h1 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 0.5rem;
        }

        .tagline {
            font-size: 1.1rem;
            color: var(--gray);
            max-width: 600px;
        }

        .section {
            background-color: white;
            border-radius: 1rem;
            padding: 2rem;
            margin-bottom: 2rem;
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
        }

        .section-title {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 1.5rem;
            position: relative;
            padding-bottom: 0.5rem;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background-color: var(--secondary);
        }

        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .info-item {
            display: flex;
            align-items: flex-start;
        }

        .icon {
            margin-right: 1rem;
            color: var(--primary);
            font-size: 1.2rem;
            min-width: 20px;
        }

        .skills-container {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill {
            background-color: var(--primary);
            color: white;
            padding: 0.5rem 1rem;
            border-radius: 2rem;
            font-size: 0.9rem;
            display: inline-flex;
            align-items: center;
        }

        .skill-web {
            background-color: #2563eb;
        }

        .skill-design {
            background-color: #7c3aed;
        }

        .skill-php {
            background-color: #4f46e5;
        }

        .hobbies-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
            gap: 1rem;
        }

        .hobby-item {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
        }

        .hobby-icon {
            width: 50px;
            height: 50px;
            object-fit: cover;
            margin-bottom: 0.5rem;
            border-radius: 50%;
        }

        footer {
            text-align: center;
            padding: 2rem;
            color: var(--gray);
            font-size: 0.9rem;
        }

        @media (max-width: 768px) {
            .info-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Animation */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .animate {
            animation: fadeIn 0.6s ease-out forwards;
        }

        .delay-1 { animation-delay: 0.2s; }
        .delay-2 { animation-delay: 0.4s; }
        .delay-3 { animation-delay: 0.6s; }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <img src="prtfolioimg.jpg" alt="Foto profil profesional dengan latar belakang biru" class="profile-picture animate">
            <h1 class="animate delay-1">EKA SETYA PURNAMA PUTRA</h1>
        </header>

        <section class="section animate delay-1">
            <h2 class="section-title">Informasi Pribadi</h2>
            <div class="info-grid">
                <div class="info-item">
                    <span class="icon">📅</span>
                    <div>
                        <strong>Usia:</strong>
                        <p>16 Tahun</p>
                    </div>
                </div>
                <div class="info-item">
                    <span class="icon">📍</span>
                    <div>
                        <strong>Lokasi:</strong>
                        <p>Ponorogo, Indonesia</p>
                    </div>
                </div>
                <div class="info-item">
                    <span class="icon">📧</span>
                    <div>
                        <strong>Email:</strong>
                        <p>ekasetyapurnamaputra27@gmail.com</p>
                    </div>
                </div>
                <div class="info-item">
                    <span class="icon">📱</span>
                    <div>
                        <strong>Telepon:</strong>
                        <p>+62 8122 6435 591</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section animate delay-2">
            <h2 class="section-title">Keterampilan</h2>
            <div class="skills-container">
                <span class="skill skill-web">HTML5</span>
                <span class="skill skill-web">CSS3</span>
                <span class="skill skill-php">PHP</span>
                <span class="skill skill-php">MySQL</span>
                <span class="skill skill-php">Laravel</span>
            </div>
        </section>

        <section class="section animate delay-2">
            <h2 class="section-title">Proyek Terbaru</h2>
            <div class="info-grid">
                <div class="info-item">
                    <div>
                        <strong>TUGAS AKHIR DDPKRPL KELAS X</strong>
                        <p>membuat sebuah web tentang toko sepatu online</p>
                        <p>di susun dengan struktur kode html,css,php dan JavaScript</p>
                    </div>
                </div>
                <div class="info-item">
                    <div>
                        <strong>WEB FOTO GALERY</strong>
                        <p>Menggunakan Laravel </p>
                    </div>
                    <div>
                        <strong>Percobaan logika php</strong>
                        <p>Menggunakan struktur kode php dalam pembuatan kalkulator </p>
                    </div>
                </div>
            </div>
        </section>

        <section class="section animate delay-3">
            <h2 class="section-title">Hobi & Minat</h2>
            <div class="hobbies-grid">
                <div class="hobby-item">
                    <img src="https://global-uploads.webflow.com/6100d0111a4ed76bc1b9fd54/616fb657512895ebe4f0e1fb_close-up-man-writing-code-laptop%20(1).jpg" alt="Foto coding di laptop" class="hobby-icon">
                    <span>Coding</span>
                </div>
                <div class="hobby-item">
                    <img src="https://www.infoescola.com/wp-content/uploads/2008/03/futsal_1014853171.jpg" alt="Foto pemain fustal" class="hobby-icon">
                    <span>futsal</span>
                </div>
                <div class="hobby-item">
                    <img src="https://wallsdesk.com/wp-content/uploads/2016/02/volleyball-background.jpg" alt="Foto pemain bola voli" class="hobby-icon">
                    <span>Bola voli</span>
                </div>
                <div class="hobby-item">
                    <img src="https://www.profesionalreview.com/wp-content/uploads/2019/08/Machine-Learning-5.jpeg" alt="Foto Machine Learning" class="hobby-icon">
                    <span>Machine Learning</span>
                </div>
            </div>
        </section>
    </div>

    <footer class="animate delay-3">
        <p>© 2025 Eka setya purnama putra. All rights reserved.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const animatedElements = document.querySelectorAll('.animate');
            animatedElements.forEach(el => {
                el.style.opacity = '0';
            });

            setTimeout(() => {
                animatedElements.forEach(el => {
                    el.style.opacity = '1';
                });
            }, 100);
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });
        });
    </script>
</body>
</html>
