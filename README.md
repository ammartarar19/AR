<!DOCTYPE html>
<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AR VIP WEB DEVELOPMENT</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: #0b0b0e;
            color: #ffffff;
            overflow-x: hidden;
        }

        /* Navbar */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 8%;
            background: rgba(15, 15, 20, 0.95);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid rgba(0, 242, 254, 0.2);
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-circle {
            width: 45px;
            height: 45px;
            border-radius: 50%;
            border: 2px solid #00f2fe;
            display: flex;
            justify-content: center;
            align-items: center;
            background: radial-gradient(circle, #00d2ff 0%, #001122 100%);
            box-shadow: 0 0 12px rgba(0, 242, 254, 0.6);
        }

        .logo-circle span {
            font-size: 1.1rem;
            font-weight: bold;
            color: #ffffff;
            letter-spacing: 1px;
        }

        .logo-text {
            font-size: 1.2rem;
            font-weight: bold;
            letter-spacing: 1px;
            color: #ffffff;
        }

        .logo-text span {
            color: #00f2fe;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }

        nav a {
            color: #a0a0b0;
            text-decoration: none;
            font-weight: 500;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00f2fe;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
            background: radial-gradient(circle at center, #141428 0%, #0b0b0e 100%);
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 15px;
            font-weight: 700;
        }

        .hero h1 span {
            color: #00f2fe;
            text-shadow: 0 0 10px rgba(0, 242, 254, 0.5);
        }

        .hero p {
            color: #a0a0b0;
            max-width: 600px;
            margin-bottom: 30px;
            font-size: 1.1rem;
        }

        .btn {
            background: linear-gradient(45deg, #00c6ff, #0072ff);
            color: white;
            padding: 12px 32px;
            border: none;
            border-radius: 25px;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            box-shadow: 0 0 15px rgba(0, 198, 255, 0.4);
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 0 25px rgba(0, 198, 255, 0.8);
        }

        /* Services Section */
        .services {
            padding: 100px 8% 80px;
            text-align: center;
            background-color: #0e0e14;
        }

        .section-title {
            font-size: 2.2rem;
            margin-bottom: 40px;
            color: #ffffff;
        }

        .section-title span {
            color: #00f2fe;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }

        .service-card {
            background: #151520;
            padding: 30px;
            border-radius: 12px;
            border: 1px solid #222235;
            transition: 0.3s;
        }

        .service-card:hover {
            transform: translateY(-5px);
            border-color: #00f2fe;
            box-shadow: 0 5px 20px rgba(0, 242, 254, 0.15);
        }

        .service-card h3 {
            margin-bottom: 15px;
            color: #00f2fe;
            font-size: 1.3rem;
        }

        .service-card p {
            color: #a0a0b0;
            font-size: 0.95rem;
        }

        /* Contact Section */
        .contact {
            padding: 80px 8%;
            text-align: center;
        }

        .contact-form {
            max-width: 500px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .contact-form input, 
        .contact-form textarea {
            width: 100%;
            padding: 14px;
            background: #151520;
            border: 1px solid #222235;
            border-radius: 8px;
            color: white;
            font-size: 1rem;
            outline: none;
            transition: 0.3s;
        }

        .contact-form input:focus, 
        .contact-form textarea:focus {
            border-color: #00f2fe;
            box-shadow: 0 0 8px rgba(0, 242, 254, 0.4);
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 20px;
            background: #07070a;
            color: #777;
            border-top: 1px solid #151520;
            font-size: 0.9rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            header {
                padding: 15px 5%;
            }
            nav ul {
                display: none;
            }
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="logo-container">
            <div class="logo-circle">
                <span>AR</span>
            </div>
            <div class="logo-text">VIP <span>DEVELOPMENT</span></div>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <h1>Welcome to <span>AR VIP WEB DEVELOPMENT</span></h1>
        <p>हम आधुनिक, तेज़ और प्रीमियम वेब डिज़ाइन और डेवलपमेंट सेवाएँ प्रदान करते हैं। अपने व्यवसाय को डिजिटल दुनिया में आगे बढ़ाएं।</p>
        <a href="#contact" class="btn">Get Started</a>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <h2 class="section-title">Our <span>Services</span></h2>
        <div class="services-grid">
            <div class="service-card">
                <h3>Web Design</h3>
                <p>सुंदर और आधुनिक यूज़र-फ्रेंडली वेबसाइट डिज़ाइन।</p>
            </div>
            <div class="service-card">
                <h3>Web Development</h3>
                <p>तेज़, सुरक्षित और रिस्पॉन्सिव वेब एप्लीकेशन।</p>
            </div>
            <div class="service-card">
                <h3>UI / UX Design</h3>
                <p>बेहतरीन यूज़र एक्सपीरियंस के साथ आकर्षक लेआउट।</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <h2 class="section-title">Contact <span>Us</span></h2>
        <form class="contact-form" onsubmit="event.preventDefault(); alert('Message sent!');">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea rows="5" placeholder="Your Message" required></textarea>
            <button type="submit" class="btn">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 AR VIP WEB DEVELOPMENT. All Rights Reserved.</p>
    </footer>

</body>
</html>
