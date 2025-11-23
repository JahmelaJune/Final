<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Login</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>
    <!-- Navigation Bar -->
    <nav class="navbar" id="navbar">
        <div class="nav-container">
            <div class="logo">MY PORTFOLIO</div>
            <ul class="nav-menu">
                <li><a href="#home" class="nav-link">Home</a></li>
                <li><a href="#about" class="nav-link">About</a></li>
                <li><a href="#contact" class="nav-link">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Animated Background Flowers -->
    <div class="flower" style="top: 10%; left: 10%; animation-delay: 0s;"></div>
    <div class="flower" style="top: 20%; right: 15%; animation-delay: 2s;"></div>
    <div class="flower" style="bottom: 15%; left: 20%; animation-delay: 4s;"></div>
    <div class="flower" style="top: 60%; right: 10%; animation-delay: 6s;"></div>
    <div class="flower" style="bottom: 30%; left: 50%; animation-delay: 3s;"></div>

    <!-- Login Page -->
    <div class="login-container" id="loginPage">
        <!-- 3D Animation Video Background -->
        <video class="video-background" autoplay muted loop playsinline>
            <source src="087b9931d0a5650f806206abae49231f.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        
        <div class="login-box">
            <h2>Welcome</h2>
            <form id="loginForm">
                <div class="input-group">
                    <label for="username">Username</label>
                    <input type="text" id="username" required>
                </div>
                <div class="input-group">
                    <label for="password">Password</label>
                    <input type="password" id="password" required>
                </div>
                <button type="submit" class="login-btn">Login</button>
            </form>
            <p class="error-message" id="errorMessage"></p>
        </div>
    </div>

    <!-- Portfolio Content -->
    <div class="portfolio-content" id="portfolioContent">
        <!-- Home Section -->
        <section id="home" class="section">
            <div class="portfolio-header">
                <img src="61ec7a62-7783-4ae0-b6a9-61fe63e67ff3.jpg" alt="Profile Picture" class="profile-image">
                <h1>Jahmela June Palaganas</h1>
                <p>Bachelor of Science Information Technology</p>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="section">
            <div class="info-card">
                <div class="info-section">
                    <h3>About Me</h3>
                    <p>Hello! I'm a passionate web developer with a love for creating beautiful and functional websites. I specialize in front-end development and enjoy bringing creative ideas to life through code.</p>
                </div>

                <div class="info-section">
                    <h3>Skills</h3>
                    <p>HTML, CSS, JavaScript, React, Node.js, Responsive Design, UI/UX Design</p>
                </div>

                <!-- Gallery Section -->
                <div class="info-section">
                    <h3>Gallery</h3>
                    <div class="gallery">
                        <div class="gallery-item">
                            <img src="660cdf85-adef-420b-adf6-f540afdb0fc3.jpg" alt="Gallery Image 1">
                        </div>
                        <div class="gallery-item">
                            <img src="0e182bff-546b-4486-b810-e1c27f83eed0.jpg" alt="Gallery Image 2">
                        </div>
                        <div class="gallery-item">
                            <img src="081228cf-9983-48c9-9c78-98802fd0e676.jpg" alt="Gallery Image 3">
                        </div>
                        <div class="gallery-item">
                            <img src="ad1fd8cf-3ec3-4004-809d-abe970aff8a0.jpg" alt="Gallery Image 4">
                        </div>
                        <div class="gallery-item">
                            <img src="d830de72-3495-4203-9f28-1828f8359571.jpg" alt="Gallery Image 5">
                        </div>
                        <div class="gallery-item">
                            <img src="de05b118-143a-4f3f-95b8-f3879638a201.jpg" alt="Gallery Image 6">
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="section">
            <div class="info-card">
                <div class="info-section">
                    <h3>Contact</h3>
                    <p>Email: jahmelajune.palaganas@gmail.edu.ph<br>
                    Location: Cabadbaran, Agusan Del Norte<br>
                    Phone: 09940172332</p>
                </div>

                <button class="logout-btn" id="logoutBtn">Logout</button>
            </div>
        </section>
    </div>

    <!-- Footer with Social Icons -->
    <footer class="footer" id="footer">
        <div class="social-icons">
            <a href="https://www.facebook.com/jahmjun.gonzalez" target="_blank" class="social-link">
                <i class="fab fa-facebook"></i>
            </a>
            <a href="https://www.instagram.com/jahmzie_june?igsh=MWNldmE0Yno3Z2U3eA==" target="_blank" class="social-link">
                <i class="fab fa-instagram"></i>
            </a>
            <a href="jahmelajune@gmail.com" class="social-link">
                <i class="fas fa-envelope"></i>
            </a>
            <a href="09940172332" class="social-link">
                <i class="fas fa-phone"></i>
            </a>
        </div>
        <p>&copy; 2025 Jahmela June. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>




* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    overflow-x: hidden;
    background: linear-gradient(135deg, #e0f4ff 0%, #b8e6ff 100%);
    min-height: 100vh;
}

/* Navigation Bar */
.navbar {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background: rgba(255, 255, 255, 0.95);
    backdrop-filter: blur(10px);
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    z-index: 1000;
    padding: 15px 0;
}

.navbar.hidden {
    display: none;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 30px;
    font-weight: bold;
    color: #4a90a4;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 30px;
}

.nav-link {
    text-decoration: none;
    color: #4a90a4;
    font-size: 16px;
    transition: color 0.3s;
    padding: 5px 10px;
}

.nav-link:hover {
    color: #87ceeb;
}

/* Animated Background Flowers */
.flower {
    position: fixed;
    opacity: 0.3;
    animation: float 15s infinite ease-in-out;
    pointer-events: none;
    width: 60px;
    height: 60px;
    z-index: 0;
}

.flower::before {
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    background: radial-gradient(circle, #87ceeb 20%, transparent 70%);
    clip-path: polygon(
        50% 50%,
        50% 20%, 60% 35%, 80% 35%, 65% 50%,
        80% 65%, 60% 65%, 50% 80%,
        40% 65%, 20% 65%, 35% 50%,
        20% 35%, 40% 35%
    );
}

@keyframes float {
    0%, 100% {
        transform: translateY(0) rotate(0deg);
    }
    50% {
        transform: translateY(-30px) rotate(180deg);
    }
}

/* Login Container */
.login-container {
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
    padding: 20px;
    position: relative;
    z-index: 1;
}

.login-container.hidden {
    display: none;
}

/* Video Background */
.video-background {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -1;
    opacity: 0.4;
}

.login-box {
    background: rgba(255, 255, 255, 0.95);
    padding: 40px;
    border-radius: 20px;
    box-shadow: 0 15px 35px rgba(0, 0, 0, 0.1);
    width: 100%;
    max-width: 400px;
    backdrop-filter: blur(10px);
    animation: floatBox 3s ease-in-out infinite;
    position: relative;
    z-index: 10;
}

@keyframes floatBox {
    0%, 100% {
        transform: translateY(0px);
    }
    50% {
        transform: translateY(-10px);
    }
}

.login-box h2 {
    color: #4a90a4;
    margin-bottom: 30px;
    text-align: center;
    font-size: 28px;
}

.input-group {
    margin-bottom: 20px;
}

.input-group label {
    display: block;
    color: #4a90a4;
    margin-bottom: 8px;
    font-size: 14px;
}

.input-group input {
    width: 100%;
    padding: 12px;
    border: 2px solid #b8e6ff;
    border-radius: 10px;
    font-size: 16px;
    transition: border-color 0.3s;
    background: #f8fcff;
}

.input-group input:focus {
    outline: none;
    border-color: #87ceeb;
}

.login-btn {
    width: 100%;
    padding: 12px;
    background: linear-gradient(135deg, #87ceeb 0%, #4a90a4 100%);
    color: white;
    border: none;
    border-radius: 10px;
    font-size: 16px;
    cursor: pointer;
    transition: transform 0.3s, box-shadow 0.3s;
}

.login-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(135, 206, 235, 0.4);
}

.error-message {
    color: #e74c3c;
    text-align: center;
    margin-top: 15px;
    font-size: 14px;
}

/* Portfolio Content */
.portfolio-content {
    display: none;
    min-height: 100vh;
    padding-top: 80px;
    position: relative;
    z-index: 1;
}

.portfolio-content.active {
    display: block;
    animation: fadeIn 0.8s ease-in;
}

@keyframes fadeIn {
    from {
        opacity: 0;
        transform: translateY(20px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

.section {
    min-height: 100vh;
    padding: 60px 20px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.portfolio-header {
    text-align: center;
}

.profile-image {
    width: 180px;
    height: 180px;
    border-radius: 50%;
    border: 5px solid white;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
    margin-bottom: 20px;
    object-fit: cover;
}

.portfolio-header h1 {
    color: #4a90a4;
    font-size: 36px;
    margin-bottom: 10px;
}

.portfolio-header p {
    color: #5fa8bb;
    font-size: 18px;
}

.info-card {
    max-width: 1000px;
    margin: 0 auto;
    background: rgba(255, 255, 255, 0.95);
    padding: 40px;
    border-radius: 20px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
}

.info-section {
    margin-bottom: 40px;
}

.info-section h3 {
    color: #4a90a4;
    font-size: 22px;
    margin-bottom: 15px;
    border-bottom: 2px solid #b8e6ff;
    padding-bottom: 10px;
}

.info-section p {
    color: #5a5a5a;
    line-height: 1.8;
    font-size: 16px;
}

/* Gallery Section */
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin-top: 20px;
}

.gallery-item {
    position: relative;
    overflow: hidden;
    border-radius: 15px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.gallery-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
}

.gallery-item img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    display: block;
    transition: transform 0.3s;
}

.gallery-item:hover img {
    transform: scale(1.1);
}

.logout-btn {
    display: block;
    margin: 30px auto 0;
    padding: 10px 30px;
    background: #87ceeb;
    color: white;
    border: none;
    border-radius: 10px;
    cursor: pointer;
    transition: background 0.3s;
    font-size: 16px;
}

.logout-btn:hover {
    background: #4a90a4;
}

/* Footer */
.footer {
    display: none;
    background: rgba(255, 255, 255, 0.95);
    padding: 30px 20px;
    text-align: center;
    border-top: 2px solid #b8e6ff;
}

.footer.active {
    display: block;
}

.social-icons {
    display: flex;
    justify-content: center;
    gap: 25px;
    margin-bottom: 15px;
}

.social-link {
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background: linear-gradient(135deg, #87ceeb 0%, #4a90a4 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    font-size: 24px;
    text-decoration: none;
    transition: transform 0.3s, box-shadow 0.3s;
}

.social-link:hover {
    transform: translateY(-5px);
    box-shadow: 0 5px 15px rgba(135, 206, 235, 0.4);
}

.footer p {
    color: #4a90a4;
    font-size: 14px;
}

/* Smooth Scroll */
html {
    scroll-behavior: smooth;
}

/* Responsive Design */
@media (max-width: 768px) {
    .nav-menu {
        gap: 15px;
    }
    
    .nav-link {
        font-size: 14px;
    }
    
    .gallery {
        grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
        gap: 15px;
    }
    
    .profile-image {
        width: 150px;
        height: 150px;
    }
    
    .portfolio-header h1 {
        font-size: 28px;
    }
}



// Get elements
const loginForm = document.getElementById('loginForm');
const loginPage = document.getElementById('loginPage');
const portfolioContent = document.getElementById('portfolioContent');
const logoutBtn = document.getElementById('logoutBtn');
const navbar = document.getElementById('navbar');
const footer = document.getElementById('footer');
const errorMessage = document.getElementById('errorMessage');

// Correct credentials
const correctUsername = 'jahmelajune';
const correctPassword = '12345';

// Login functionality
loginForm.addEventListener('submit', (e) => {
    e.preventDefault();
    
    const username = document.getElementById('username').value;
    const password = document.getElementById('password').value;

    // Check credentials
    if (username === correctUsername && password === correctPassword) {
        // Successful login
        loginPage.classList.add('hidden');
        portfolioContent.classList.add('active');
        navbar.classList.remove('hidden');
        footer.classList.add('active');
        errorMessage.textContent = '';
    } else {
        // Failed login
        errorMessage.textContent = 'Invalid username or password. Please try again.';
        // Clear password field
        document.getElementById('password').value = '';
    }
});

// Logout functionality
logoutBtn.addEventListener('click', () => {
    portfolioContent.classList.remove('active');
    loginPage.classList.remove('hidden');
    navbar.classList.add('hidden');
    footer.classList.remove('active');
    loginForm.reset();
    errorMessage.textContent = '';
});

// Smooth scroll for navigation links
document.querySelectorAll('.nav-link').forEach(link => {
    link.addEventListener('click', (e) => {
        e.preventDefault();
        const targetId = link.getAttribute('href');
        const targetSection = document.querySelector(targetId);
        
        if (targetSection) {
            targetSection.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        }
    });
});
