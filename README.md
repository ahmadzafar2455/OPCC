# OPCC
Ocean Pearl Carpet Cleaning website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ocean Pearl Carpet Cleaning - Sydney</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="nav-container">
            <a href="#" class="logo">
                <img src="https://i.ibb.co/ccQscss/OP-logo.jpg" alt="Ocean Pearl Carpet Cleaning" border="0">
            </a>
            <nav>
                <ul>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#areas">Areas</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
            <div class="quote-container">
                <a href="#contact" class="cta-button">Get Quote</a>
                <div class="phone-number">0424 444 488</div>
            </div>
        </div>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h1>Professional Carpet Cleaning Services</h1>
            <p>Experience the finest deep steam carpet cleaning in Sydney</p>
            <p class="hero-feature">Using industrial-grade machines for faster drying time with no chemical smell!</p>
            <a href="#contact" class="cta-button">Schedule Now</a>
        </div>
    </section>

    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="service-grid">
            <div class="service-card">
                <h3>Deep Steam Cleaning</h3>
                <p>Professional-grade steam cleaning for all types of carpets using industrial equipment for faster drying times</p>
            </div>
            <div class="service-card">
                <h3>Stain Removal</h3>
                <p>Specialized treatment for tough stains and spots with eco-friendly products, ensuring no harsh chemical smells</p>
            </div>
            <div class="service-card">
                <h3>Upholstery Cleaning</h3>
                <p>Refresh and restore your furniture's appearance with our gentle yet effective cleaning methods</p>
            </div>
        </div>
        <div class="features-box">
            <h3>Why Choose Us?</h3>
            <ul>
                <li>Industrial-grade equipment for superior cleaning</li>
                <li>Faster drying times - enjoy your clean carpets sooner</li>
                <li>No chemical after-smell - safe for your family</li>
                <li>Eco-friendly cleaning solutions</li>
                <li>Professional and experienced technicians</li>
            </ul>
        </div>
    </section>

    <section id="areas" class="areas">
        <div class="areas-content">
            <h2>Areas We Serve in Sydney</h2>
            <div class="areas-grid">
                <ul>
                    <li>Eastern Suburbs</li>
                    <li>Inner West</li>
                    <li>CBD & Surrounds</li>
                    <li>North Sydney</li>
                </ul>
                <ul>
                    <li>Northern Beaches</li>
                    <li>North Shore</li>
                    <li>Hills District</li>
                    <li>Sutherland Shire</li>
                </ul>
                <ul>
                    <li>Western Sydney</li>
                    <li>South Western Sydney</li>
                    <li>St George Area</li>
                    <li>Parramatta Region</li>
                </ul>
            </div>
        </div>
    </section>

    <section class="contact" id="contact">
        <h2>Get In Touch</h2>
        <form class="contact-form" action="send_email.php" method="POST" onsubmit="showSuccessMessage(event)">
            <input type="text" name="firstName" placeholder="First Name" required>
            <input type="text" name="lastName" placeholder="Last Name" required>
            <input type="email" name="email" placeholder="Email" required>
            <input type="tel" name="phone" placeholder="Phone" required>
            <textarea name="message" rows="5" placeholder="Message" required></textarea>
            <button type="submit" class="cta-button">Send Message</button>
        </form>
        <div class="success-message" id="successMessage">
            Thank you for contacting Ocean Pearl Carpet Cleaning. We will get back to you shortly!
        </div>
    </section>

    <footer>
        <div class="footer-content">
            <div>
                <h3>Ocean Pearl Carpet Cleaning</h3>
                <p>Professional carpet cleaning services you can trust in Sydney</p>
            </div>
            <div>
                <h3>Contact</h3>
                <p>Phone: 0424 444 488</p>
                <p>Email: oceanpearl@outlook.com.au</p>
            </div>
            <div>
                <h3>Hours</h3>
                <p>Monday - Sunday</p>
                <p>8:00 AM - 6:00 PM</p>
            </div>
        </div>
    </footer>

    <script>
        function showSuccessMessage(event) {
            event.preventDefault();
            document.getElementById('successMessage').classList.add('show');
            document.querySelector('.contact-form').reset();
            
            // Hide success message after 5 seconds
            setTimeout(() => {
                document.getElementById('successMessage').classList.remove('show');
            }, 5000);
        }
    </script>
</body>
</html>
