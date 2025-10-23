<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Ops Agency - AI Integration Solutions</title>

    <!-- SEO & Social Meta -->
    <meta name="description" content="Smart Ops Agency helps businesses automate and scale through advanced AI integration, automation, and data-driven intelligence.">
    <meta property="og:title" content="Smart Ops Agency - AI Integration Solutions">
    <meta property="og:description" content="Transform your business with AI-powered automation and intelligent system design.">
    <meta property="og:image" content="https://yourdomain.com/preview.jpg">
    <meta property="og:type" content="website">
    <meta name="theme-color" content="#007AFF">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #fff;
            background: #000;
            overflow-x: hidden;
        }

        /* Navigation */
        nav {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            padding: 1rem 5%;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(0, 0, 0, 0.1);
        }

        nav .container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
            font-size: 1.5rem;
            font-weight: 600;
        }

        .logo-icon {
            width: 50px;
            height: 50px;
            background: #000;
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            font-weight: 700;
            color: #007AFF;
        }

        .logo-text {
            display: flex;
            flex-direction: column;
            line-height: 1.2;
        }

        .logo-text .smart,
        .logo-text .ops,
        .logo-text .agency {
            color: #007AFF;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        nav a {
            text-decoration: none;
            color: #000;
            font-weight: 500;
            transition: color 0.3s;
        }

        nav a:hover {
            color: #007AFF;
        }

        /* Hero Section */
        .hero {
            position: relative;
            height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            overflow: hidden;
            margin-top: 80px;
        }

        #orbCanvas {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: 0;
            background: radial-gradient(circle at center, #000 0%, #0a0a0a 100%);
        }

        .hero-content {
            position: relative;
            z-index: 1;
            padding: 2rem;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            font-weight: 700;
            background: linear-gradient(135deg, #fff 0%, #007AFF 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .hero p {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            color: rgba(255, 255, 255, 0.9);
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }

        .cta-button {
            display: inline-block;
            padding: 15px 40px;
            background: #007AFF;
            color: #fff;
            text-decoration: none;
            border-radius: 25px;
            font-weight: 600;
            transition: all 0.3s;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .cta-button:hover {
            background: #0051D5;
            transform: translateY(-2px);
            box-shadow: 0 10px 30px rgba(0, 122, 255, 0.3);
        }

        /* Toast Message */
        .success-toast {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: #007AFF;
            color: #fff;
            padding: 1rem 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0,0,0,0.2);
            animation: fadeInOut 3s ease-in-out;
            z-index: 2000;
            font-weight: 500;
        }

        @keyframes fadeInOut {
            0%,100% { opacity: 0; transform: translateY(20px); }
            10%,90% { opacity: 1; transform: translateY(0); }
        }

        /* Other Sections (kept same styling) */
        section {
            padding: 80px 5%;
            max-width: 1200px;
            margin: 0 auto;
        }

        h2 {
            font-size: 2.5rem;
            margin-bottom: 3rem;
            text-align: center;
            color: #000;
        }

        .services-grid,
        .product-showcase {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .service-card,
        .product-item {
            padding: 2.5rem;
            background: #fff;
            border-radius: 20px;
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.08);
            transition: all 0.3s;
        }

        .service-card:hover,
        .product-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 122, 255, 0.15);
        }

        footer {
            background: #000;
            color: #fff;
            text-align: center;
            padding: 2rem 5%;
        }

        footer p {
            color: rgba(255, 255, 255, 0.7);
        }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
        }
    </style>
</head>

<body>
    <nav>
        <div class="container">
            <div class="logo">
                <div class="logo-icon">SO</div>
                <div class="logo-text">
                    <div><span class="smart">Smart Ops</span></div>
                    <div class="agency">Agency</div>
                </div>
            </div>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero with Soft Glowing Orbs -->
    <section id="home" class="hero">
        <canvas id="orbCanvas"></canvas>
        <div class="hero-content">
            <h1>Transform Your Business with AI</h1>
            <p>Seamlessly integrate cutting-edge artificial intelligence into your operations. We deliver custom AI solutions that drive innovation and accelerate growth.</p>
            <a href="#contact" class="cta-button">Get Started Today</a>
        </div>
    </section>

    <!-- Rest of your sections (unchanged from your original) -->
    <!-- ... Services, Products, About, Contact, Footer ... -->

    <footer>
        <p>&copy; 2025 Smart Ops Agency. All rights reserved.</p>
        <p>Transforming businesses through intelligent automation. Automating Florida 🌴</p>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) target.scrollIntoView({ behavior: 'smooth', block: 'start' });
            });
        });

        // Toast Success Message
        function handleSubmit(e) {
            e.preventDefault();
            const form = e.target;
            const toast = document.createElement('div');
            toast.textContent = 'Message sent successfully!';
            toast.className = 'success-toast';
            document.body.appendChild(toast);
            setTimeout(() => toast.remove(), 3000);
            form.reset();
            return false;
        }

        // Glowing Orbs Canvas
        const canvas = document.getElementById('orbCanvas');
        const ctx = canvas.getContext('2d');
        let orbs = [];

        function resizeCanvas() {
            canvas.width = window.innerWidth;
            canvas.height = document.querySelector('.hero').offsetHeight;
        }
        window.addEventListener('resize', resizeCanvas);
        resizeCanvas();

        class Orb {
            constructor() {
                this.x = Math.random() * canvas.width;
                this.y = Math.random() * canvas.height;
                this.size = Math.random() * 4 + 2;
                this.speedX = (Math.random() - 0.5) * 0.3;
                this.speedY = (Math.random() - 0.5) * 0.3;
                this.color = `rgba(0, 122, 255, ${Math.random() * 0.3 + 0.1})`;
            }
            update() {
                this.x += this.speedX;
                this.y += this.speedY;
                if (this.x < 0 || this.x > canvas.width) this.speedX *= -1;
                if (this.y < 0 || this.y > canvas.height) this.speedY *= -1;
            }
            draw() {
                ctx.beginPath();
                const gradient = ctx.createRadialGradient(this.x, this.y, 0, this.x, this.y, this.size * 5);
                gradient.addColorStop(0, this.color);
                gradient.addColorStop(1, 'rgba(0, 0, 0, 0)');
                ctx.fillStyle = gradient;
                ctx.arc(this.x, this.y, this.size * 5, 0, Math.PI * 2);
                ctx.fill();
            }
        }

        for (let i = 0; i < 50; i++) orbs.push(new Orb());

        function animate() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            orbs.forEach(orb => {
                orb.update();
                orb.draw();
            });
            requestAnimationFrame(animate);
        }
        animate();
    </script>
</body>
</html>
