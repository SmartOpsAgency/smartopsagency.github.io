<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Ops Agency - AI Integration Solutions</title>
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
        }

        .logo-text {
            display: flex;
            flex-direction: column;
            line-height: 1.2;
        }

        .logo-text .smart {
            color: #007AFF;
            font-size: 1.3rem;
        }

        .logo-text .ops {
            color: #007AFF;
            font-size: 1.3rem;
        }

        .logo-text .agency {
            color: #007AFF;
            font-size: 0.9rem;
            font-weight: 500;
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
            margin-top: 80px;
            padding: 100px 5% 80px;
            background: linear-gradient(135deg, #000 0%, #1a1a1a 100%);
            color: #fff;
            text-align: center;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            font-weight: 700;
            background: linear-gradient(135deg, #fff 0%, #007AFF 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
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

        /* Section Styles */
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

        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .service-card {
            padding: 2.5rem;
            background: #fff;
            border-radius: 20px;
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.08);
            transition: all 0.3s;
            border: 1px solid rgba(0, 0, 0, 0.05);
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 40px rgba(0, 122, 255, 0.15);
        }

        .service-icon {
            font-size: 3rem;
            margin-bottom: 1rem;
        }

        .service-card h3 {
            color: #007AFF;
            margin-bottom: 1rem;
            font-size: 1.5rem;
        }

        .service-card p {
            color: #666;
            line-height: 1.8;
        }

        /* Products Section */
        .products {
            background: #f9f9f9;
            padding: 80px 5%;
        }

        .product-showcase {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 3rem;
            margin-top: 3rem;
        }

        .product-item {
            background: #fff;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 5px 30px rgba(0, 0, 0, 0.08);
            transition: all 0.3s;
        }

        .product-item:hover {
            transform: scale(1.02);
            box-shadow: 0 15px 50px rgba(0, 0, 0, 0.12);
        }

        .product-header {
            background: linear-gradient(135deg, #007AFF 0%, #0051D5 100%);
            padding: 2rem;
            color: #fff;
        }

        .product-header h3 {
            font-size: 1.8rem;
            margin-bottom: 0.5rem;
        }

        .product-body {
            padding: 2rem;
        }

        .product-body ul {
            list-style: none;
            margin: 1.5rem 0;
        }

        .product-body li {
            padding: 0.8rem 0;
            border-bottom: 1px solid #eee;
            color: #333;
        }

        .product-body li:before {
            content: "✓ ";
            color: #007AFF;
            font-weight: bold;
            margin-right: 0.5rem;
        }

        /* About Section */
        .about {
            background: #000;
            color: #fff;
        }

        .about h2 {
            color: #fff;
        }

        .about-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            font-size: 1.2rem;
            line-height: 2;
            color: rgba(255, 255, 255, 0.9);
        }

        /* Contact Section */
        .contact {
            text-align: center;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
        }

        .contact-form input,
        .contact-form textarea {
            padding: 1rem;
            border: 2px solid #eee;
            border-radius: 10px;
            font-size: 1rem;
            font-family: inherit;
            transition: border-color 0.3s;
        }

        .contact-form input:focus,
        .contact-form textarea:focus {
            outline: none;
            border-color: #007AFF;
        }

        .contact-form textarea {
            min-height: 150px;
            resize: vertical;
        }

        /* Footer */
        footer {
            background: #000;
            color: #fff;
            text-align: center;
            padding: 2rem 5%;
        }

        footer p {
            color: rgba(255, 255, 255, 0.7);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            nav ul {
                gap: 1rem;
            }

            .services-grid,
            .product-showcase {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Navigation -->
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

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h1>Transform Your Business with AI</h1>
        <p>Seamlessly integrate cutting-edge artificial intelligence into your operations. We deliver custom AI solutions that drive innovation and accelerate growth.</p>
        <a href="#contact" class="cta-button">Get Started Today</a>
    </section>

    <!-- Services Section -->
    <section id="services">
        <h2>Our Services</h2>
        <div class="services-grid">
            <div class="service-card">
                <div class="service-icon">🧠</div>
                <h3>AI Consultation</h3>
                <p>Expert guidance on implementing AI strategies tailored to your business needs. We analyze your workflow and identify opportunities for AI enhancement.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">⚙️</div>
                <h3>Custom Integration</h3>
                <p>Seamless integration of AI models into your existing systems. We ensure smooth deployment with minimal disruption to your operations.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📊</div>
                <h3>Data Analytics</h3>
                <p>Transform raw data into actionable insights using advanced machine learning algorithms and predictive analytics.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🤖</div>
                <h3>Automation Solutions</h3>
                <p>Automate repetitive tasks and workflows with intelligent AI systems that learn and adapt to your business processes.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">🔒</div>
                <h3>Security & Compliance</h3>
                <p>Enterprise-grade security measures and compliance frameworks to protect your AI implementations and data.</p>
            </div>
            <div class="service-card">
                <div class="service-icon">📈</div>
                <h3>Ongoing Support</h3>
                <p>24/7 technical support and continuous optimization to ensure your AI solutions deliver maximum value.</p>
            </div>
        </div>
    </section>

    <!-- Products Section -->
    <section id="products" class="products">
        <h2>Our Products</h2>
        <div class="product-showcase">
            <div class="product-item">
                <div class="product-header">
                    <h3>AI ChatBot Pro</h3>
                    <p>Intelligent customer engagement platform</p>
                </div>
                <div class="product-body">
                    <ul>
                        <li>Natural language processing</li>
                        <li>Multi-channel support</li>
                        <li>Sentiment analysis</li>
                        <li>Automated ticket routing</li>
                        <li>Custom training on your data</li>
                        <li>Analytics dashboard</li>
                    </ul>
                    <a href="#contact" class="cta-button" style="width: 100%; text-align: center; margin-top: 1rem;">Learn More</a>
                </div>
            </div>

            <div class="product-item">
                <div class="product-header">
                    <h3>Predictive Analytics Suite</h3>
                    <p>Forecast trends and make data-driven decisions</p>
                </div>
                <div class="product-body">
                    <ul>
                        <li>Advanced forecasting models</li>
                        <li>Real-time data processing</li>
                        <li>Visual insights dashboard</li>
                        <li>Anomaly detection</li>
                        <li>Custom KPI tracking</li>
                        <li>Export & reporting tools</li>
                    </ul>
                    <a href="#contact" class="cta-button" style="width: 100%; text-align: center; margin-top: 1rem;">Learn More</a>
                </div>
            </div>

            <div class="product-item">
                <div class="product-header">
                    <h3>Vision AI Platform</h3>
                    <p>Computer vision for business applications</p>
                </div>
                <div class="product-body">
                    <ul>
                        <li>Image recognition & classification</li>
                        <li>Object detection</li>
                        <li>Quality control automation</li>
                        <li>Facial recognition (optional)</li>
                        <li>Document processing</li>
                        <li>Real-time video analysis</li>
                    </ul>
                    <a href="#contact" class="cta-button" style="width: 100%; text-align: center; margin-top: 1rem;">Learn More</a>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About Smart Ops Agency</h2>
        <div class="about-content">
            <p>At Smart Ops Agency, we bridge the gap between cutting-edge AI technology and practical business solutions. Our team of data scientists, engineers, and AI specialists work together to deliver transformative solutions that drive real results.</p>
            <p>With over a decade of combined experience in machine learning and enterprise software, we've helped hundreds of companies harness the power of AI to streamline operations, enhance customer experiences, and unlock new revenue streams.</p>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Get In Touch</h2>
        <form class="contact-form" onsubmit="return handleSubmit(event)">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <input type="text" placeholder="Company Name">
            <textarea placeholder="Tell us about your project..." required></textarea>
            <button type="submit" class="cta-button">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Smart Ops Agency. All rights reserved.</p>
        <p>Transforming businesses through intelligent automation.</p>
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({ behavior: 'smooth', block: 'start' });
                }
            });
        });

        // Form submission
        function handleSubmit(e) {
            e.preventDefault();
            alert('Thank you for your message! We will get back to you shortly.');
            e.target.reset();
            return false;
        }

        // Add scroll effect to nav
        let lastScroll = 0;
        window.addEventListener('scroll', () => {
            const nav = document.querySelector('nav');
            const currentScroll = window.pageYOffset;
            
            if (currentScroll > 50) {
                nav.style.boxShadow = '0 2px 20px rgba(0,0,0,0.1)';
            } else {
                nav.style.boxShadow = 'none';
            }
            
            lastScroll = currentScroll;
        });
    </script>
</body>
</html>
