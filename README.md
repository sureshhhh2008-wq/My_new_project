# My_new_project
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Capture Studio | Professional Photography</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <nav>
        <div class="logo">CAPTURE<span>STUDIO</span></div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#portfolio">Portfolio</a></li>
            <li><a href="#contact">Book a Session</a></li>
        </ul>
    </nav>

    <header id="home" class="hero">
        <div class="hero-content">
            <h1>Moments Frozen in Time</h1>
            <p>High-end editorial and portrait photography.</p>
            <a href="#portfolio" class="btn">View Gallery</a>
        </div>
    </header>

    <section id="portfolio" class="gallery-container">
        <h2>Portfolio</h2>
        <div class="gallery-grid">
            <div class="photo-card"><img src="https://via.placeholder.com/400x500" alt="Portrait"></div>
            <div class="photo-card"><img src="https://via.placeholder.com/400x300" alt="Editorial"></div>
            <div class="photo-card"><img src="https://via.placeholder.com/400x500" alt="Wedding"></div>
            <div class="photo-card"><img src="https://via.placeholder.com/400x300" alt="Nature"></div>
            <div class="photo-card"><img src="https://via.placeholder.com/400x500" alt="Fashion"></div>
            <div class="photo-card"><img src="https://via.placeholder.com/400x300" alt="Event"></div>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2>Book Your Photoshoot</h2>
        <form id="booking-form">
            <input type="text" placeholder="Full Name" required>
            <input type="email" placeholder="Email Address" required>
            <select>
                <option value="portrait">Portrait Session</option>
                <option value="wedding">Wedding Coverage</option>
                <option value="editorial">Editorial/Commercial</option>
            </select>
            <textarea placeholder="Tell me about your vision..."></textarea>
            <button type="submit" class="btn">Send Inquiry</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2026 Capture Studio. All rights reserved.</p>
    </footer>

</body>
</html>
/* General Styles */
* { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', sans-serif; }
body { background-color: #121212; color: #fff; scroll-behavior: smooth; }

/* Navigation */
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 10%;
    background: rgba(0,0,0,0.9);
    position: sticky;
    top: 0;
    z-index: 1000;
}
.logo { font-size: 1.5rem; font-weight: bold; letter-spacing: 2px; }
.logo span { color: #ff3e3e; }
nav ul { display: flex; list-style: none; }
nav ul li { margin-left: 20px; }
nav ul li a { color: white; text-decoration: none; font-size: 0.9rem; transition: 0.3s; }
nav ul li a:hover { color: #ff3e3e; }

/* Hero Section */
.hero {
    height: 80vh;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), 
                url('https://images.unsplash.com/photo-1492691527719-9d1e07e534b4?auto=format&fit=crop&w=1350&q=80');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
}
.hero h1 { font-size: 3.5rem; margin-bottom: 10px; }
.btn {
    display: inline-block;
    padding: 12px 30px;
    background: #ff3e3e;
    color: white;
    text-decoration: none;
    border-radius: 5px;
    margin-top: 20px;
    transition: 0.3s;
}
.btn:hover { background: #e63535; transform: translateY(-3px); }

/* Gallery Grid */
.gallery-container { padding: 80px 10%; }
.gallery-container h2 { text-align: center; margin-bottom: 40px; font-size: 2.5rem; }
.gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    grid-gap: 15px;
}
.photo-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 8px;
    transition: 0.4s ease;
    filter: grayscale(30%);
}
.photo-card img:hover {
    filter: grayscale(0%);
    transform: scale(1.02);
}

/* Contact Form */
.contact-section { padding: 80px 10%; background: #1a1a1a; text-align: center; }
#booking-form {
    max-width: 600px;
    margin: 40px auto 0;
    display: flex;
    flex-direction: column;
}
input, select, textarea {
    padding: 15px;
    margin-bottom: 15px;
    background: #222;
    border: 1px solid #333;
    color: white;
    border-radius: 4px;
}
footer { padding: 40px; text-align: center; font-size: 0.8rem; color: #777; }
