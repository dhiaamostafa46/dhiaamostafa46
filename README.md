<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dhiaa Mostafa - GitHub README</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #2563eb;
            --secondary: #0ea5e9;
            --accent: #f43f5e;
            --dark: #1e293b;
            --light: #f8fafc;
            --github-bg: #0d1117;
            --github-border: #30363d;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Tajawal', sans-serif;
        }
        
        body {
            background-color: var(--github-bg);
            color: var(--light);
            line-height: 1.6;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
        }
        
        .github-container {
            border: 1px solid var(--github-border);
            border-radius: 6px;
            padding: 30px;
            margin-bottom: 30px;
            background-color: var(--dark);
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
        }
        
        .header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
            padding: 30px 0;
            border-bottom: 1px solid var(--github-border);
        }
        
        .animated-text {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 15px;
            background: linear-gradient(90deg, var(--primary), var(--secondary), var(--accent));
            background-size: 200% auto;
            background-clip: text;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            animation: gradient 3s linear infinite;
        }
        
        .subtitle {
            font-size: 1.4rem;
            color: var(--secondary);
            margin-bottom: 20px;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid var(--primary);
            margin: 0 auto 20px;
            overflow: hidden;
            box-shadow: 0 0 25px rgba(37, 99, 235, 0.5);
            animation: pulse 2s infinite;
        }
        
        .profile-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .badges {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }
        
        .badge {
            display: inline-block;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
        }
        
        h2 {
            font-size: 1.8rem;
            margin: 30px 0 20px;
            color: var(--secondary);
            padding-bottom: 10px;
            border-bottom: 2px solid var(--github-border);
        }
        
        h3 {
            font-size: 1.4rem;
            margin: 25px 0 15px;
            color: var(--primary);
        }
        
        p {
            margin-bottom: 15px;
            font-size: 1.1rem;
        }
        
        ul, ol {
            margin-bottom: 20px;
            padding-left: 20px;
        }
        
        li {
            margin-bottom: 8px;
            font-size: 1.1rem;
        }
        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 20px;
            margin: 25px 0;
        }
        
        .card {
            background: rgba(30, 41, 59, 0.6);
            border: 1px solid var(--github-border);
            border-radius: 6px;
            padding: 20px;
            transition: transform 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }
        
        .stats {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            gap: 15px;
            margin: 30px 0;
        }
        
        .stat {
            text-align: center;
            padding: 15px;
            background: rgba(30, 41, 59, 0.6);
            border-radius: 6px;
            border: 1px solid var(--github-border);
            min-width: 150px;
        }
        
        .stat-number {
            font-size: 2rem;
            font-weight: 700;
            color: var(--primary);
            margin-bottom: 5px;
        }
        
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 20px 0;
        }
        
        .tech-item {
            padding: 8px 15px;
            background: linear-gradient(135deg, var(--primary), var(--secondary));
            border-radius: 20px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 30px 0;
        }
        
        .social-links a {
            color: var(--light);
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }
        
        .social-links a:hover {
            color: var(--primary);
        }
        
        .animated-element {
            display: inline-block;
            animation: bounce 2s infinite;
        }
        
        @keyframes gradient {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        @keyframes pulse {
            0%, 100% { box-shadow: 0 0 20px rgba(37, 99, 235, 0.5); }
            50% { box-shadow: 0 0 40px rgba(37, 99, 235, 0.8); }
        }
        
        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        @media (max-width: 768px) {
            .animated-text {
                font-size: 2rem;
            }
            
            .subtitle {
                font-size: 1.2rem;
            }
            
            .grid {
                grid-template-columns: 1fr;
            }
            
            .stats {
                flex-direction: column;
                align-items: center;
            }
        }
    </style>
</head>
<body>
    <div class="github-container">
        <div class="header">
            <div class="profile-img">
                <img src="https://via.placeholder.com/150" alt="Dhiaa Mostafa">
            </div>
            <h1 class="animated-text">مرحباً 👋، أنا ضياء مصطفى</h1>
            <p class="subtitle">مهندس برمجيات أول | متخصص في DevOps وتطوير الويب الكامل</p>
            
            <div class="badges">
                <span class="badge">📅 9 سبتمبر 1995</span>
                <span class="badge">📍 الرياض، السعودية</span>
                <span class="badge">📧 dhiaamostafa.dev@gmail.com</span>
            </div>
            
            <div class="social-links">
                <a href="https://www.linkedin.com/in/dhiaa-mostafa-qaid" target="_blank"><i class="fab fa-linkedin"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
        </div>
        
        <h2>⚡ عني</h2>
        <p>أنا مطور بخبرة في بناء <strong>مواقع وتطبيقات ويب وجوال</strong> للشركات الصغيرة والمتوسطة. أتخصص في <strong>HTML, CSS, PHP, jQuery, Laravel, وFlutter</strong>، وأضمن إدارة كاملة للمشروع من البداية إلى النهاية مع تواصل واضح طوال الطريق.</p>
        
        <h2>📊 إحصائيات</h2>
        <div class="stats">
            <div class="stat">
                <div class="stat-number">12,000+</div>
                <div class="stat-label">ساعة عمل</div>
            </div>
            <div class="stat">
                <div class="stat-number">30+</div>
                <div class="stat-label">مشروع مكتمل</div>
            </div>
            <div class="stat">
                <div class="stat-number">30+</div>
                <div class="stat-label">عميل راضي</div>
            </div>
        </div>
        
        <h2>🚀 مهاراتي التقنية</h2>
        <div class="tech-stack">
            <div class="tech-item"><i class="fab fa-html5"></i> HTML5</div>
            <div class="tech-item"><i class="fab fa-css3-alt"></i> CSS3</div>
            <div class="tech-item"><i class="fab fa-js"></i> JavaScript</div>
            <div class="tech-item"><i class="fab fa-php"></i> PHP</div>
            <div class="tech-item"><i class="fab fa-laravel"></i> Laravel</div>
            <div class="tech-item"><i class="fab fa-react"></i> React</div>
            <div class="tech-item"><i class="fab fa-node"></i> Node.js</div>
            <div class="tech-item"><i class="fab fa-flutter"></i> Flutter</div>
            <div class="tech-item"><i class="fas fa-database"></i> MySQL</div>
            <div class="tech-item"><i class="fab fa-docker"></i> Docker</div>
            <div class="tech-item"><i class="fab fa-aws"></i> AWS</div>
            <div class="tech-item"><i class="fab fa-git"></i> Git</div>
        </div>
        
        <h2>💼 الخبرات العملية</h2>
        <div class="grid">
            <div class="card">
                <h3>🟢 2023 – الحاضر: مهندس برمجيات أول</h3>
                <p><strong>Eyein Technology – السعودية</strong></p>
                <ul>
                    <li>تطوير نظام محاسبة قائم على السحابة (Evix)</li>
                    <li>بناء أنظمة تتبع الخدمات اللوجستية</li>
                    <li>تصميم تطبيقات SaaS متعددة المستأجرين</li>
                </ul>
            </div>
            
            <div class="card">
                <h3>🟡 2022 – 2023: مطور ويب كامل</h3>
                <p><strong>SMART SYSTEM – السعودية</strong></p>
                <ul>
                    <li>بناء أنظمة إدارة المطاعم والفنادق</li>
                    <li>إدارة المشاريع بطريقة Agile</li>
                    <li>تسليم مواقع ويب عالية الجودة</li>
                </ul>
            </div>
            
            <div class="card">
                <h3>🔵 2020 – 2022: مطور ويب كامل</h3>
                <p><strong>ESKYSOFT – اليمن</strong></p>
                <ul>
                    <li>تطوير منصات المدارس والتجارة الإلكترونية والحجوزات</li>
                    <li>الحفاظ على معايير الجودة والأداء</li>
                    <li>استخدام منهجيات Agile</li>
                </ul>
            </div>
        </div>
        
        <h2>📈 إحصائيات GitHub</h2>
        <p>هنا سأعرض إحصائيات GitHub الخاصة بي:</p>
        <div style="text-align: center; margin: 30px 0;">
            <img src="https://github-readme-stats.vercel.app/api?username=dhiaamostafa&show_icons=true&theme=tokyonight" alt="GitHub Stats" style="max-width: 100%;">
            <img src="https://github-readme-streak-stats.herokuapp.com/?user=dhiaamostafa&theme=tokyonight" alt="GitHub Streak" style="max-width: 100%; margin-top: 20px;">
        </div>
        
        <h2>🌐 خدماتي</h2>
        <div class="grid">
            <div class="card">
                <h3>💻 تطوير تطبيقات الويب</h3>
                <p>حلول تطبيقات ويب كاملة مع التركيز على تجربة المستخدم والكفاءة والقابلية للتوسع - من التخطيط إلى الصيانة.</p>
            </div>
            
            <div class="card">
                <h3>🌐 تصميم وتطوير المواقع</h3>
                <p>مواقع ويب responsive وحديثة مصممة لتعكس علامتك التجارية وتعمل على جميع الأجهزة.</p>
            </div>
            
            <div class="card">
                <h3>📱 تطوير تطبيقات الجوال</h3>
                <p>تطبيقات Android/iOS مخصصة باستخدام Flutter بأداء قوي وتصميم جميل وتجربة مستخدم رائعة.</p>
            </div>
        </div>
        
        <h2>📫 كيف تتواصل معي</h2>
        <p>أنا دائماً متحمس للتعاون في مشاريع جديدة ومثيرة للاهتمام. لا تتردد في التواصل معي عبر:</p>
        <ul>
            <li>📧 البريد الإلكتروني: <a href="mailto:dhiaamostafa.dev@gmail.com" style="color: var(--secondary);">dhiaamostafa.dev@gmail.com</a></li>
            <li>📱 الهاتف: <a href="tel:+966533166742" style="color: var(--secondary);">+966 533 166 742</a></li>
            <li>💼 LinkedIn: <a href="https://www.linkedin.com/in/dhiaa-mostafa-qaid" style="color: var(--secondary);">Dhiâa Mostafa Qaid</a></li>
        </ul>
        
        <div style="text-align: center; margin-top: 40px; padding-top: 20px; border-top: 1px solid var(--github-border);">
            <p>شكراً لزيارة ملفي الشخصي! <span class="animated-element">😊</span></p>
            <p>لا تنسى إعطاء ⭐ للمشاريع التي أعجبتك!</p>
        </div>
    </div>

    <script>
        // Simple animation for elements
        document.addEventListener('DOMContentLoaded', function() {
            const animatedElements = document.querySelectorAll('.card, .stat, .tech-item');
            
            animatedElements.forEach((element, index) => {
                element.style.opacity = "0";
                element.style.transform = "translateY(20px)";
                element.style.transition = "opacity 0.5s ease, transform 0.5s ease";
                
                setTimeout(() => {
                    element.style.opacity = "1";
                    element.style.transform = "translateY(0)";
                }, 100 + (index * 100));
            });
        });
    </script>
</body>
</html>
