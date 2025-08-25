<img width="1867" height="925" alt="image" src="https://github.com/user-attachments/assets/f6f5198c-ee74-45e4-afd1-b8187fe7383b" /><!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MyTests.uz - IELTS Test</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary-color: #007bff;
            --primary-dark: #0056b3;
            --success-color: #28a745;
            --danger-color: #dc3545;
            --warning-color: #ffc107;
            --info-color: #17a2b8;
            --light-color: #f8f9fa;
            --dark-color: #343a40;
            --border-color: #e9ecef;
            --shadow-sm: 0 2px 4px rgba(0,0,0,0.1);
            --shadow-md: 0 4px 12px rgba(0,0,0,0.15);
            --shadow-lg: 0 8px 25px rgba(0,0,0,0.15);
            --border-radius: 12px;
            --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Inter', Arial, sans-serif;
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            min-height: 100vh;
            line-height: 1.6;
        }
        
        /* Header */
        .header {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
            padding: 0 20px;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: var(--shadow-sm);
        }
        
        .header-content {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px 0;
        }
        
        .logo {
            font-size: 28px;
            font-weight: 800;
            background: linear-gradient(45deg, var(--primary-color), #6f42c1);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-decoration: none;
            letter-spacing: -0.5px;
        }
        
        .nav-menu {
            display: flex;
            list-style: none;
            gap: 32px;
        }
        
        .nav-menu a {
            color: #333;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
            position: relative;
            padding: 8px 0;
        }
        
        .nav-menu a:hover,
        .nav-menu a.active {
            color: var(--primary-color);
        }
        
        .nav-menu a.active::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: var(--primary-color);
            border-radius: 2px;
        }
        
        .user-actions {
            display: flex;
            gap: 12px;
            align-items: center;
        }
        
        .btn {
            padding: 10px 20px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: var(--transition);
            border: 2px solid;
            display: inline-flex;
            align-items: center;
            gap: 8px;
            text-align: center;
            cursor: pointer;
            font-size: 14px;
        }
        
        .btn-outline {
            color: var(--primary-color);
            border-color: var(--primary-color);
            background: transparent;
        }
        
        .btn-outline:hover {
            background: var(--primary-color);
            color: white;
            transform: translateY(-1px);
            box-shadow: var(--shadow-md);
        }
        
        .btn-primary {
            background: var(--primary-color);
            color: white;
            border-color: var(--primary-color);
        }
        
        .btn-primary:hover {
            background: var(--primary-dark);
            border-color: var(--primary-dark);
            transform: translateY(-1px);
            box-shadow: var(--shadow-md);
        }
        
        /* Main Container */
        .main-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 40px 20px;
        }
        
        .page-header {
            text-align: center;
            margin-bottom: 50px;
            color: white;
        }
        
        .page-title {
            font-size: 48px;
            font-weight: 800;
            margin-bottom: 16px;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
            letter-spacing: -1px;
        }
        
        .page-subtitle {
            font-size: 20px;
            opacity: 0.9;
            font-weight: 400;
            margin-bottom: 30px;
        }
        
        .ielts-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.2);
            color: white;
            padding: 10px 20px;
            border-radius: 25px;
            font-weight: 600;
            backdrop-filter: blur(10px);
        }
        
        /* IELTS Overview */
        .ielts-overview {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 24px;
            margin-bottom: 50px;
        }
        
        .overview-card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: var(--border-radius);
            padding: 24px;
            box-shadow: var(--shadow-md);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: var(--transition);
        }
        
        .overview-card:hover {
            transform: translateY(-4px);
            box-shadow: var(--shadow-lg);
        }
        
        .overview-icon {
            font-size: 32px;
            margin-bottom: 16px;
        }
        
        .overview-title {
            font-size: 18px;
            font-weight: 700;
            color: var(--dark-color);
            margin-bottom: 8px;
        }
        
        .overview-text {
            color: #666;
            font-size: 14px;
        }
        
        /* IELTS Test Modules */
        .ielts-modules {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: var(--border-radius);
            box-shadow: var(--shadow-lg);
            overflow: hidden;
            border: 1px solid rgba(255, 255, 255, 0.2);
            margin-bottom: 40px;
        }
        
        .modules-header {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
            padding: 30px;
            text-align: center;
        }
        
        .modules-header h2 {
            font-size: 28px;
            font-weight: 700;
            margin-bottom: 10px;
        }
        
        .modules-header p {
            opacity: 0.9;
            font-size: 16px;
        }
        
        /* Module Cards Grid */
        .modules-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            padding: 40px;
        }
        
        .module-card {
            background: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow-md);
            transition: var(--transition);
            border: 2px solid transparent;
        }
        
        .module-card:hover {
            transform: translateY(-6px);
            box-shadow: var(--shadow-lg);
            border-color: rgba(240, 147, 251, 0.3);
        }
        
        .module-header {
            padding: 25px;
            text-align: center;
            position: relative;
        }
        
        .listening-header {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
        }
        
        .reading-header {
            background: linear-gradient(135deg, #f093fb 0%, #f5576c 100%);
            color: white;
        }
        
        .writing-header {
            background: linear-gradient(135deg, #4facfe 0%, #00f2fe 100%);
            color: white;
        }
        
        .speaking-header {
            background: linear-gradient(135deg, #43e97b 0%, #38f9d7 100%);
            color: white;
        }
        
        .module-icon {
            font-size: 40px;
            margin-bottom: 12px;
        }
        
        .module-title {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 8px;
        }
        
        .module-duration {
            font-size: 14px;
            opacity: 0.9;
        }
        
        .module-body {
            padding: 25px;
        }
        
        .module-description {
            color: #666;
            margin-bottom: 20px;
            line-height: 1.6;
        }
        
        .module-features {
            margin-bottom: 25px;
        }
        
        .feature-item {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 10px;
            font-size: 14px;
            color: #555;
        }
        
        .feature-icon {
            color: var(--success-color);
            font-weight: bold;
        }
        
        .module-stats {
            display: flex;
            justify-content: space-between;
            margin-bottom: 20px;
            padding: 15px;
            background: var(--light-color);
            border-radius: 8px;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 18px;
            font-weight: 700;
            color: var(--primary-color);
        }
        
        .stat-label {
            font-size: 12px;
            color: #666;
        }
        
        .module-actions {
            display: flex;
            gap: 12px;
        }
        
        .btn-module {
            flex: 1;
            padding: 12px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            text-align: center;
            transition: var(--transition);
            font-size: 14px;
        }
        
        .btn-practice {
            background: var(--primary-color);
            color: white;
            border: 2px solid var(--primary-color);
        }
        
        .btn-practice:hover {
            background: var(--primary-dark);
            transform: translateY(-1px);
        }
        
        .btn-mock {
            background: transparent;
            color: var(--success-color);
            border: 2px solid var(--success-color);
        }
        
        .btn-mock:hover {
            background: var(--success-color);
            color: white;
            transform: translateY(-1px);
        }
        
        /* Pricing Section */
        .pricing-section {
            margin: 60px 0;
        }
        
        .pricing-header {
            text-align: center;
            margin-bottom: 40px;
            color: white;
        }
        
        .pricing-title {
            font-size: 36px;
            font-weight: 700;
            margin-bottom: 16px;
        }
        
        .pricing-subtitle {
            font-size: 18px;
            opacity: 0.9;
        }
        
        .pricing-cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            max-width: 900px;
            margin: 0 auto;
        }
        
        .pricing-card {
            background: rgba(255, 255, 255, 0.95);
            border-radius: var(--border-radius);
            padding: 40px 30px;
            text-align: center;
            box-shadow: var(--shadow-lg);
            transition: var(--transition);
            position: relative;
            overflow: hidden;
        }
        
        .pricing-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 60px rgba(0,0,0,0.2);
        }
        
        .pricing-card.featured {
            border: 3px solid #f093fb;
            transform: scale(1.05);
        }
        
        .featured-badge {
            position: absolute;
            top: 20px;
            right: -30px;
            background: #f093fb;
            color: white;
            padding: 5px 40px;
            transform: rotate(45deg);
            font-size: 12px;
            font-weight: 600;
        }
        
        .plan-name {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 10px;
            color: var(--dark-color);
        }
        
        .plan-price {
            font-size: 40px;
            font-weight: 900;
            color: #f093fb;
            margin-bottom: 20px;
        }
        
        .plan-features {
            text-align: left;
            margin-bottom: 30px;
        }
        
        .plan-feature {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 12px;
            color: #555;
        }
        
        .plan-btn {
            width: 100%;
            padding: 15px;
            background: #f093fb;
            color: white;
            border: none;
            border-radius: 8px;
            font-weight: 600;
            font-size: 16px;
            cursor: pointer;
            transition: var(--transition);
        }
        
        .plan-btn:hover {
            background: #f5576c;
            transform: translateY(-2px);
        }
        
        /* Success Stories */
        .success-stories {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border-radius: var(--border-radius);
            padding: 50px 40px;
            margin: 60px 0;
        }
        
        .stories-header {
            text-align: center;
            margin-bottom: 40px;
            color: white;
        }
        
        .stories-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .story-card {
            background: rgba(255, 255, 255, 0.9);
            border-radius: var(--border-radius);
            padding: 30px;
            box-shadow: var(--shadow-md);
        }
        
        .story-quote {
            font-style: italic;
            font-size: 16px;
            line-height: 1.6;
            margin-bottom: 20px;
            color: #555;
        }
        
        .story-author {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .author-avatar {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: linear-gradient(45deg, #f093fb, #f5576c);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-weight: 700;
            font-size: 18px;
        }
        
        .author-info h4 {
            font-weight: 600;
            color: var(--dark-color);
        }
        
        .author-score {
            color: #f093fb;
            font-weight: 700;
        }
        
        /* Mobile Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                gap: 20px;
            }
            
            .nav-menu {
                flex-wrap: wrap;
                justify-content: center;
                gap: 16px;
            }
            
            .page-title {
                font-size: 36px;
            }
            
            .modules-grid {
                grid-template-columns: 1fr;
                padding: 20px;
            }
            
            .pricing-cards {
                grid-template-columns: 1fr;
            }
            
            .pricing-card.featured {
                transform: none;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="header-content">
            <a href="#" class="logo">MyTests.uz</a>
            <nav>
                <ul class="nav-menu">
                    <li><a href="#">🏠 Bosh sahifa</a></li>
                    <li><a href="#">📊 Multilevel Test</a></li>
                    <li><a href="#" class="active">🎯 IELTS</a></li>
                    <li><a href="#">🏛️ Prezident maktabi</a></li>
                    <li><a href="#">📈 Natijalar</a></li>
                </ul>
            </nav>
            <div class="user-actions">
                <a href="#" class="btn btn-outline">Kirish</a>
                <a href="#" class="btn btn-primary">Ro'yxatdan o'tish</a>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="main-container">
        <div class="page-header">
            <h1 class="page-title">🎯 IELTS PREPARATION</h1>
            <p class="page-subtitle">International English Language Testing System - Xalqaro ingliz tili sertifikati</p>
            <div class="ielts-badge">✨ Professional IELTS tayyorgarlik platformasi</div>
        </div>
        
        <!-- IELTS Overview -->
        <div class="ielts-overview">
            <div class="overview-card">
                <div class="overview-icon">🌍</div>
                <h3 class="overview-title">Xalqaro tan olingan</h3>
                <p class="overview-text">140+ mamlakatda qabul qilinadigan eng mashhur ingliz tili sertifikati</p>
            </div>
            <div class="overview-card">
                <div class="overview-icon">🎓</div>
                <h3 class="overview-title">Ta'lim va ish</h3>
                <p class="overview-text">Universitet kirish va xorijiy kompaniyalarda ish topish uchun zarur</p>
            </div>
            <div class="overview-card">
                <div class="overview-icon">📊</div>
                <h3 class="overview-title">4 ta bo'lim</h3>
                <p class="overview-text">Listening, Reading, Writing va Speaking ko'nikmalarni baholaydi</p>
            </div>
            <div class="overview-card">
                <div class="overview-icon">⭐</div>
                <h3 class="overview-title">9.0 gacha ball</h3>
                <p class="overview-text">Har bir bo'lim uchun 0 dan 9 gacha ball beriladi</p>
            </div>
        </div>

        <!-- IELTS Test Modules -->
        <div class="ielts-modules">
            <div class="modules-header">
                <h2>IELTS Test Bo'limlari</h2>
                <p>Har bir bo'lim uchun alohida tayyorgarlik va amaliyot</p>
            </div>
            
            <div class="modules-grid">
                <!-- Listening Module -->
                <div class="module-card">
                    <div class="module-header listening-header">
                        <div class="module-icon">🎧</div>
                        <h3 class="module-title">LISTENING</h3>
                        <p class="module-duration">30 daqiqa + 10 daqiqa yozish</p>
                    </div>
                    <div class="module-body">
                        <p class="module-description">
                            Audio yozuvlarni tinglash va savollarga javob berish. 4 ta bo'lim: kundalik muloqot, 
                            monolog, ta'lim muhiti va akademik mavzular.
                        </p>
                        <div class="module-features">
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>40 ta savol</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Bir marta tinglash</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Turli aksent va lahjalar</span>
                            </div>
                        </div>
                        <div class="module-stats">
                            <div class="stat">
                                <div class="stat-number">50+</div>
                                <div class="stat-label">Practice testlar</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">20+</div>
                                <div class="stat-label">Mock testlar</div>
                            </div>
                        </div>
                        <div class="module-actions">
                            <a href="#" class="btn-module btn-practice" onclick="startListening()">Practice</a>
                            <a href="#" class="btn-module btn-mock" onclick="mockListening()">Mock Test</a>
                        </div>
                    </div>
                </div>

                <!-- Reading Module -->
                <div class="module-card">
                    <div class="module-header reading-header">
                        <div class="module-icon">📖</div>
                        <h3 class="module-title">READING</h3>
                        <p class="module-duration">60 daqiqa</p>
                    </div>
                    <div class="module-body">
                        <p class="module-description">
                            3 ta matn o'qish va 40 ta savolga javob berish. Matnlar jurnallar, kitoblar, 
                            gazeta va akademik maqolalardan olingan.
                        </p>
                        <div class="module-features">
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>40 ta savol</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>3 ta matn</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Turli savol turlari</span>
                            </div>
                        </div>
                        <div class="module-stats">
                            <div class="stat">
                                <div class="stat-number">60+</div>
                                <div class="stat-label">Practice testlar</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">25+</div>
                                <div class="stat-label">Mock testlar</div>
                            </div>
                        </div>
                        <div class="module-actions">
                            <a href="#" class="btn-module btn-practice" onclick="startReading()">Practice</a>
                            <a href="#" class="btn-module btn-mock" onclick="mockReading()">Mock Test</a>
                        </div>
                    </div>
                </div>

                <!-- Writing Module -->
                <div class="module-card">
                    <div class="module-header writing-header">
                        <div class="module-icon">✍️</div>
                        <h3 class="module-title">WRITING</h3>
                        <p class="module-duration">60 daqiqa</p>
                    </div>
                    <div class="module-body">
                        <p class="module-description">
                            2 ta yozma topshiriq: Task 1 - grafik/jadval tasviri (150 so'z), 
                            Task 2 - esse yozish (250 so'z).
                        </p>
                        <div class="module-features">
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>2 ta topshiriq</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>AI baholash tizimi</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Batafsil feedback</span>
                            </div>
                        </div>
                        <div class="module-stats">
                            <div class="stat">
                                <div class="stat-number">40+</div>
                                <div class="stat-label">Task 1 mavzulari</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">50+</div>
                                <div class="stat-label">Task 2 mavzulari</div>
                            </div>
                        </div>
                        <div class="module-actions">
                            <a href="#" class="btn-module btn-practice" onclick="startWriting()">Practice</a>
                            <a href="#" class="btn-module btn-mock" onclick="mockWriting()">Mock Test</a>
                        </div>
                    </div>
                </div>

                <!-- Speaking Module -->
                <div class="module-card">
                    <div class="module-header speaking-header">
                        <div class="module-icon">🗣️</div>
                        <h3 class="module-title">SPEAKING</h3>
                        <p class="module-duration">11-14 daqiqa</p>
                    </div>
                    <div class="module-body">
                        <p class="module-description">
                            Ekspert bilan jonli suhbat: Part 1 - tanishuv, Part 2 - monolog, 
                            Part 3 - chuqur muhokama.
                        </p>
                        <div class="module-features">
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>3 ta qism</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Professional ekspertlar</span>
                            </div>
                            <div class="feature-item">
                                <span class="feature-icon">✓</span>
                                <span>Real vaqtda baholash</span>
                            </div>
                        </div>
                        <div class="module-stats">
                            <div class="stat">
                                <div class="stat-number">100+</div>
                                <div class="stat-label">Mavzular</div>
                            </div>
                            <div class="stat">
                                <div class="stat-number">24/7</div>
                                <div class="stat-label">Booking</div>
                            </div>
                        </div>
                        <div class="module-actions">
                            <a href="#" class="btn-module btn-practice" onclick="startSpeaking()">Practice</a>
                            <a href="#" class="btn-module btn-mock" onclick="mockSpeaking()">Mock Test</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Pricing Section -->
        <div class="pricing-section">
            <div class="pricing-header">
                <h2 class="pricing-title">💎 Narx Rejalari</h2>
                <p class="pricing-subtitle">Sizga mos bo'lgan rejani tanlang</p>
            </div>
            
            <div class="pricing-cards">
                <div class="pricing-card">
                    <h3 class="plan-name">Asosiy</h3>
                    <div class="plan-price">50,000<span style="font-size: 16px;"> so'm</span></div>
                    <div class="plan-features">
                        <div class="plan-feature">
                            <span class="feature-icon">✓</span>
                            <span>Barcha Practice testlar</span>
                        </div>
                        <div class="plan-feature">
                            <span class="feature-
