<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IvaniHub - Premium Digital Solutions</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3a0ca3;
            --accent: #f72585;
            --light: #f8f9fa;
            --dark: #212529;
            --success: #4cc9f0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
            color: var(--dark);
            line-height: 1.6;
            padding: 20px;
        }
        
        .instructions {
            max-width: 1000px;
            margin: 0 auto 30px;
            background: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .instructions h2 {
            color: var(--secondary);
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--accent);
        }
        
        .steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 20px 0;
        }
        
        .step {
            background: var(--light);
            padding: 20px;
            border-radius: 8px;
            border-left: 4px solid var(--primary);
        }
        
        .step-number {
            display: inline-block;
            background: var(--primary);
            color: white;
            width: 30px;
            height: 30px;
            text-align: center;
            line-height: 30px;
            border-radius: 50%;
            margin-right: 10px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(to right, var(--primary), var(--secondary));
            color: white;
            padding: 20px 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            border-radius: 10px;
            margin-bottom: 30px;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .logo i {
            font-size: 28px;
            color: var(--accent);
        }
        
        .logo h1 {
            font-size: 28px;
            font-weight: 700;
        }
        
        nav ul {
            display: flex;
            list-style: none;
            gap: 25px;
        }
        
        nav a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            padding: 5px 10px;
            border-radius: 4px;
        }
        
        nav a:hover {
            background: rgba(255, 255, 255, 0.2);
        }
        
        .hero {
            text-align: center;
            padding: 40px 20px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            margin-bottom: 30px;
        }
        
        .hero h2 {
            font-size: 32px;
            margin-bottom: 15px;
            color: var(--secondary);
        }
        
        .hero p {
            font-size: 18px;
            color: #666;
            margin-bottom: 25px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 28px;
            background: var(--primary);
            color: white;
            border: none;
            border-radius: 50px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            box-shadow: 0 4px 10px rgba(67, 97, 238, 0.3);
        }
        
        .btn:hover {
            background: var(--secondary);
            transform: translateY(-2px);
            box-shadow: 0 6px 15px rgba(67, 97, 238, 0.4);
        }
        
        .btn-accent {
            background: var(--accent);
            box-shadow: 0 4px 10px rgba(247, 37, 133, 0.3);
        }
        
        .btn-accent:hover {
            background: #d11474;
            box-shadow: 0 6px 15px rgba(247, 37, 133, 0.4);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
        }
        
        .section-title h2 {
            font-size: 32px;
            color: var(--secondary);
            display: inline-block;
            padding-bottom: 10px;
            position: relative;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background: var(--accent);
            border-radius: 2px;
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-bottom: 50px;
        }
        
        .feature-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .feature-card:hover {
            transform: translateY(-5px);
        }
        
        .feature-icon {
            font-size: 40px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        .feature-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
            color: var(--secondary);
        }
        
        .feature-card p {
            color: #666;
        }
        
        .premium {
            background: linear-gradient(135deg, var(--secondary) 0%, var(--primary) 100%);
            color: white;
            padding: 50px 20px;
            border-radius: 10px;
            text-align: center;
            margin-bottom: 50px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }
        
        .premium h2 {
            font-size: 32px;
            margin-bottom: 20px;
        }
        
        .premium p {
            max-width: 700px;
            margin: 0 auto 30px;
            font-size: 18px;
            opacity: 0.9;
        }
        
        .benefits {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        
        .benefit {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            text-align: left;
            display: flex;
            align-items: flex-start;
            gap: 15px;
            backdrop-filter: blur(5px);
        }
        
        .benefit i {
            font-size: 24px;
            color: var(--success);
            flex-shrink: 0;
        }
        
        .benefit h3 {
            margin-bottom: 10px;
            font-size: 18px;
        }
        
        .benefit p {
            font-size: 14px;
            opacity: 0.8;
            margin: 0;
        }
        
        footer {
            background: var(--dark);
            color: white;
            padding: 40px 0;
            text-align: center;
            border-radius: 10px;
        }
        
        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-links a {
            color: white;
            font-size: 20px;
            transition: all 0.3s ease;
        }
        
        .social-links a:hover {
            color: var(--accent);
        }
        
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 15px;
            }
            
            nav ul {
                gap: 15px;
                flex-wrap: wrap;
                justify-content: center;
            }
            
            .hero h2 {
                font-size: 28px;
            }
            
            .hero p {
                font-size: 16px;
            }
            
            .steps {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="instructions">
        <h2>How to View This Website in Google Chrome</h2>
        <p>Follow these simple steps to view your IvaniHub website:</p>
        
        <div class="steps">
            <div class="step">
                <h3><span class="step-number">1</span> Save the HTML file</h3>
                <p>Save this entire code as an HTML file on your computer (e.g., <code>ivanihub.html</code>).</p>
            </div>
            
            <div class="step">
                <h3><span class="step-number">2</span> Open Chrome</h3>
                <p>Launch Google Chrome on your computer.</p>
            </div>
            
            <div class="step">
                <h3><span class="step-number">3</span> Open the file</h3>
                <p>Press <code>Ctrl+O</code> (Windows) or <code>Cmd+O</code> (Mac) to open the file dialog, then select your HTML file.</p>
            </div>
            
            <div class="step">
                <h3><span class="step-number">4</span> Alternatively</h3>
                <p>Right-click the HTML file and choose "Open with" > "Google Chrome".</p>
            </div>
        </div>
        
        <p><strong>Note:</strong> You can also directly copy the entire code and paste it into a new text file, then save it with a .html extension.</p>
    </div>
    
    <div class="container">
        <header>
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-code"></i>
                    <h1>IvaniHub</h1>
                </div>
                <nav>
                    <ul>
                        <li><a href="#">Home</a></li>
                        <li><a href="#">Features</a></li>
                        <li><a href="#">Pricing</a></li>
                        <li><a href="#">Tutorials</a></li>
                        <li><a href="#">Support</a></li>
                    </ul>
                </nav>
            </div>
        </header>
        
        <section class="hero">
            <h2>Welcome to IvaniHub</h2>
            <p>Your premier destination for premium digital tools and resources. Unlock your potential with our powerful solutions.</p>
            <a href="#" class="btn"><i class="fas fa-key"></i> GET IVANIHUB KEY</a>
        </section>
        
        <div class="section-title">
            <h2>Tutorial: Get Your Key</h2>
        </div>
        
        <section class="features">
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-user-plus"></i>
                </div>
                <h3>Create Account</h3>
                <p>Sign up for a free account to get started with our basic features and resources.</p>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-gem"></i>
                </div>
                <h3>Upgrade to Premium</h3>
                <p>Choose a plan that fits your needs and unlock the full potential of IvaniHub.</p>
            </div>
            
            <div class="feature-card">
                <div class="feature-icon">
                    <i class="fas fa-download"></i>
                </div>
                <h3>Download Resources</h3>
                <p>Access our premium library of tools, scripts, and resources for your projects.</p>
            </div>
        </section>
        
        <div class="section-title">
            <h2>Premium Options</h2>
        </div>
        
        <section class="premium">
            <h2>Purchase Premium Key</h2>
            <p>Unlock the full potential of IvaniHub with our affordable premium plans. Choose what works best for you.</p>
            <a href="#" class="btn btn-accent">VIEW PRICING PLANS</a>
            
            <div class="benefits">
                <div class="benefit">
                    <i class="fas fa-check-circle"></i>
                    <div>
                        <h3>Keyless / No Ads Script</h3>
                        <p>Enjoy an uninterrupted experience with no advertisements and keyless access.</p>
                    </div>
                </div>
                
                <div class="benefit">
                    <i class="fas fa-star"></i>
                    <div>
                        <h3>Access Premium Features</h3>
                        <p>Get exclusive access to all premium features and upcoming releases.</p>
                    </div>
                </div>
                
                <div class="benefit">
                    <i class="fas fa-headset"></i>
                    <div>
                        <h3>Priority Support</h3>
                        <p>Receive dedicated support with faster response times and solutions.</p>
                    </div>
                </div>
            </div>
        </section>
    </div>
    
    <footer>
        <div class="container footer-content">
            <div class="logo">
                <i class="fas fa-code"></i>
                <h2>IvaniHub</h2>
            </div>
            <p>&copy; 2023 IvaniHub. All rights reserved.</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-discord"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
        </div>
    </footer>

    <script>
        // Simple animation for buttons
        document.querySelectorAll('.btn').forEach(button => {
            button.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-2px)';
            });
            
            button.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
            });
        });
        
        // Simple animation for feature cards
        document.querySelectorAll('.feature-card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-5px)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0)';
            });
        });
    </script>
</body>
</html
