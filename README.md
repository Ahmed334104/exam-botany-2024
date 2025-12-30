<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>حل امتحان Bot 101 - General Botany (I) - One Piece & Tower of God Style</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* استيراد خطوط أنيقة */
        @import url('https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Rubik:wght@400;500;700&display=swap');
        
        :root {
            --one-piece-red: #c00a27;
            --one-piece-yellow: #ffcc00;
            --one-piece-blue: #0066cc;
            --tog-purple: #4a235a;
            --tog-gold: #d4af37;
            --tog-blue: #1a5276;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Cairo', 'Rubik', sans-serif;
            background: linear-gradient(135deg, #0a0a2a 0%, #1a1a4a 50%, #0a2a2a 100%);
            color: #f0f8ff;
            line-height: 1.6;
            direction: rtl;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }
        
        /* تأثيرات الخلفية */
        .bg-anime-elements {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -2;
            opacity: 0.1;
            background-image: 
                radial-gradient(circle at 10% 20%, var(--one-piece-red) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, var(--tog-purple) 0%, transparent 20%),
                radial-gradient(circle at 50% 50%, var(--one-piece-blue) 0%, transparent 30%);
        }
        
        .container {
            max-width: 1300px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 1;
        }
        
        /* تصميم رأس الصفحة على شكل جولي روجر + شعار تاور أوف جود */
        header {
            background: linear-gradient(45deg, rgba(12, 35, 64, 0.9) 0%, rgba(26, 54, 93, 0.9) 50%, rgba(42, 82, 122, 0.9) 100%);
            color: white;
            padding: 30px 0;
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            text-align: center;
            border: 3px solid var(--one-piece-yellow);
            position: relative;
            overflow: hidden;
        }
        
        header::before {
            content: "";
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, transparent 30%, rgba(192, 10, 39, 0.1) 70%, transparent 71%);
            animation: rotate 20s linear infinite;
            z-index: 0;
        }
        
        @keyframes rotate {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }
        
        .header-content {
            padding: 0 20px;
            position: relative;
            z-index: 1;
        }
        
        .university-logo {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 20px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        
        .anime-logos {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-top: 20px;
            margin-bottom: 20px;
        }
        
        .anime-logo {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            color: white;
            font-weight: bold;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
        }
        
        .one-piece-logo {
            background: linear-gradient(45deg, var(--one-piece-red), var(--one-piece-yellow));
            border: 2px solid var(--one-piece-yellow);
        }
        
        .tog-logo {
            background: linear-gradient(45deg, var(--tog-purple), var(--tog-gold));
            border: 2px solid var(--tog-gold);
        }
        
        .university-logo i {
            font-size: 3rem;
            color: var(--one-piece-yellow);
            text-shadow: 0 0 10px rgba(255, 204, 0, 0.7);
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            text-shadow: 3px 3px 0 #000, 0 0 15px var(--one-piece-blue);
            background: linear-gradient(to right, var(--one-piece-yellow), #fff, var(--tog-gold));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            font-weight: 800;
            letter-spacing: 1px;
        }
        
        .exam-info {
            background-color: rgba(0, 0, 0, 0.6);
            padding: 20px;
            border-radius: 15px;
            margin-top: 20px;
            display: inline-block;
            border: 2px solid var(--tog-purple);
            box-shadow: 0 0 15px rgba(74, 35, 90, 0.7);
            backdrop-filter: blur(5px);
        }
        
        .exam-info p {
            margin: 8px 0;
            font-size: 1.1rem;
        }
        
        .exam-info i {
            color: var(--tog-gold);
            margin-left: 10px;
        }
        
        /* تصميم التبويب للغة */
        .language-tabs {
            display: flex;
            justify-content: center;
            margin-bottom: 40px;
            background-color: rgba(12, 35, 64, 0.8);
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.6);
            border: 2px solid var(--one-piece-red);
            backdrop-filter: blur(10px);
        }
        
        .tab {
            flex: 1;
            text-align: center;
            padding: 20px;
            font-weight: 700;
            font-size: 1.2rem;
            cursor: pointer;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            color: white;
        }
        
        .tab:hover {
            background-color: rgba(192, 10, 39, 0.3);
        }
        
        .tab.active {
            background: linear-gradient(to right, rgba(192, 10, 39, 0.8), rgba(74, 35, 90, 0.8));
            color: white;
            box-shadow: inset 0 0 15px rgba(0, 0, 0, 0.5);
        }
        
        .tab::before {
            content: "";
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.7s;
        }
        
        .tab:hover::before {
            left: 100%;
        }
        
        /* أقسام المحتوى */
        .content-section {
            display: none;
            background-color: rgba(20, 30, 48, 0.85);
            padding: 35px;
            border-radius: 20px;
            margin-bottom: 40px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.7);
            border: 2px solid var(--tog-blue);
            backdrop-filter: blur(10px);
            position: relative;
            overflow: hidden;
        }
        
        .content-section::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 100px;
            height: 100px;
            background: linear-gradient(45deg, transparent, var(--one-piece-red), transparent);
            transform: rotate(45deg) translate(-70px, -70px);
        }
        
        .content-section.active {
            display: block;
            animation: fadeInUp 0.8s ease;
        }
        
        @keyframes fadeInUp {
            from { opacity: 0; transform: translateY(30px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .section-title {
            color: var(--one-piece-yellow);
            font-size: 2rem;
            margin-bottom: 30px;
            padding-bottom: 15px;
            border-bottom: 4px solid var(--one-piece-red);
            display: flex;
            align-items: center;
            gap: 15px;
            text-shadow: 2px 2px 0 #000;
            position: relative;
        }
        
        .section-title::after {
            content: "";
            position: absolute;
            bottom: -4px;
            right: 0;
            width: 100px;
            height: 4px;
            background: linear-gradient(to right, var(--one-piece-red), transparent);
        }
        
        .section-title i {
            font-size: 1.8rem;
            color: var(--tog-gold);
            text-shadow: 0 0 10px rgba(212, 175, 55, 0.7);
        }
        
        .question-block {
            margin-bottom: 35px;
            padding: 25px;
            background: rgba(10, 25, 47, 0.7);
            border-radius: 15px;
            border-right: 6px solid var(--tog-purple);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.4);
            transition: transform 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .question-block:hover {
            transform: translateX(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.6);
        }
        
        .question-block::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 8px;
            height: 100%;
            background: linear-gradient(to bottom, var(--one-piece-red), var(--tog-purple));
        }
        
        .question-title {
            color: #fff;
            font-size: 1.5rem;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
            gap: 15px;
            text-shadow: 1px 1px 2px #000;
        }
        
        .question-title i {
            color: var(--one-piece-yellow);
            text-shadow: 0 0 8px rgba(255, 204, 0, 0.7);
        }
        
        .answer-list {
            list-style-type: none;
            margin-right: 25px;
        }
        
        .answer-list li {
            margin-bottom: 15px;
            padding: 15px;
            background: rgba(30, 40, 60, 0.7);
            border-radius: 10px;
            border: 1px solid rgba(100, 100, 150, 0.3);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }
        
        .answer-list li:hover {
            transform: translateX(-10px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.4);
            border-color: var(--tog-gold);
        }
        
        .answer-list li::before {
            content: "";
            position: absolute;
            top: 0;
            right: 0;
            width: 5px;
            height: 100%;
            background: rgba(192, 10, 39, 0.5);
        }
        
        .correct-answer {
            background: rgba(20, 80, 40, 0.5) !important;
            border-right: 5px solid #4CAF50 !important;
            font-weight: 700;
        }
        
        .correct-answer::before {
            background: #4CAF50 !important;
        }
        
        .mcq-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.4);
        }
        
        .mcq-table th, .mcq-table td {
            padding: 15px 20px;
            text-align: right;
            border-bottom: 1px solid rgba(100, 100, 150, 0.3);
        }
        
        .mcq-table th {
            background: linear-gradient(to right, rgba(192, 10, 39, 0.8), rgba(74, 35, 90, 0.8));
            color: white;
            font-weight: 700;
            font-size: 1.1rem;
        }
        
        .mcq-table tr {
            background-color: rgba(30, 40, 60, 0.6);
        }
        
        .mcq-table tr:nth-child(even) {
            background-color: rgba(40, 50, 70, 0.6);
        }
        
        .mcq-table tr:hover {
            background-color: rgba(60, 80, 120, 0.6);
        }
        
        .q-number {
            background: linear-gradient(45deg, var(--one-piece-red), var(--tog-purple));
            color: white;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            margin-left: 10px;
            font-weight: bold;
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.5);
        }
        
        .answer-key {
            background: linear-gradient(to right, rgba(26, 82, 118, 0.8), rgba(42, 122, 122, 0.8));
            padding: 25px;
            border-radius: 15px;
            margin-top: 25px;
            border: 2px solid var(--tog-gold);
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.5);
            position: relative;
            overflow: hidden;
        }
        
        .answer-key h3 {
            color: var(--one-piece-yellow);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .answer-key p {
            margin-bottom: 10px;
            padding: 10px;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 8px;
            border-right: 3px solid var(--one-piece-red);
        }
        
        /* تصميم الشخصيات */
        .anime-characters {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 40px 0;
            gap: 20px;
        }
        
        .character {
            width: 180px;
            height: 250px;
            perspective: 1000px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.7);
        }
        
        .character-inner {
            position: relative;
            width: 100%;
            height: 100%;
            text-align: center;
            transition: transform 0.8s;
            transform-style: preserve-3d;
        }
        
        .character:hover .character-inner {
            transform: rotateY(180deg);
        }
        
        .character-front, .character-back {
            position: absolute;
            width: 100%;
            height: 100%;
            backface-visibility: hidden;
            border-radius: 15px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .character-front {
            background: linear-gradient(45deg, var(--one-piece-red), var(--one-piece-blue));
            color: white;
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        .character-back {
            background: linear-gradient(45deg, var(--tog-purple), var(--tog-blue));
            color: white;
            transform: rotateY(180deg);
            font-size: 0.9rem;
            text-align: center;
        }
        
        .character-icon {
            font-size: 3.5rem;
            margin-bottom: 15px;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.5);
        }
        
        /* تذييل الصفحة */
        footer {
            text-align: center;
            padding: 30px;
            margin-top: 60px;
            color: #aaa;
            font-size: 0.95rem;
            border-top: 2px solid var(--one-piece-red);
            background-color: rgba(10, 20, 40, 0.8);
            border-radius: 20px;
            backdrop-filter: blur(10px);
        }
        
        .footer-note {
            background: linear-gradient(to right, rgba(192, 10, 39, 0.3), rgba(74, 35, 90, 0.3));
            padding: 20px;
            border-radius: 15px;
            margin-top: 20px;
            font-weight: 600;
            color: var(--tog-gold);
            border: 1px solid var(--tog-gold);
        }
        
        /* تصميم متجاوب */
        @media (max-width: 992px) {
            .container {
                padding: 15px;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .content-section {
                padding: 25px;
            }
            
            .section-title {
                font-size: 1.7rem;
            }
            
            .character {
                width: 150px;
                height: 220px;
            }
        }
        
        @media (max-width: 768px) {
            .language-tabs {
                flex-direction: column;
            }
            
            .tab {
                padding: 15px;
            }
            
            .mcq-table {
                display: block;
                overflow-x: auto;
            }
            
            .anime-characters {
                justify-content: center;
            }
        }
        
        @media (max-width: 480px) {
            h1 {
                font-size: 1.7rem;
            }
            
            .section-title {
                font-size: 1.5rem;
            }
            
            .question-title {
                font-size: 1.3rem;
            }
            
            .character {
                width: 130px;
                height: 200px;
            }
        }
    </style>
</head>
<body>
    <!-- تأثيرات خلفية -->
    <div class="bg-anime-elements"></div>
    
    <div class="container">
        <!-- رأس الصفحة -->
        <header>
            <div class="header-content">
                <div class="university-logo">
                    <i class="fas fa-university"></i>
                    <div>
                        <h2>South Valley University</h2>
                        <h3>Department of Botany & Microbiology</h3>
                    </div>
                </div>
                
                <div class="anime-logos">
                    <div class="anime-logo one-piece-logo">OP</div>
                    <div class="anime-logo tog-logo">ToG</div>
                </div>
                
                <h1>Botany (I) - Bot 101 - Exam Solution</h1>
                
                <div class="exam-info">
                    <p><i class="fas fa-calendar-alt"></i> General Botany (I) Exam - January 2025</p>
                    <p><i class="fas fa-users"></i> For 1st year Biology Students</p>
                    <p><i class="fas fa-palette"></i> One Piece & Tower of God Anime Style</p>
                </div>
            </div>
        </header>
        
        <!-- شخصيات الأنمي -->
        <div class="anime-characters">
            <div class="character">
                <div class="character-inner">
                    <div class="character-front" style="background: linear-gradient(45deg, #c00a27, #b3001e);">
                        <div class="character-icon">👒</div>
                        <div>مونكي دي لوفي</div>
                        <div>One Piece</div>
                    </div>
                    <div class="character-back">
                        <p>قبعة القش - ملك القراصنة القادم</p>
                        <p>يمتلك قدرة فاكهة الشيطان (غومو غومو نو مي)</p>
                    </div>
                </div>
            </div>
            
            <div class="character">
                <div class="character-inner">
                    <div class="character-front" style="background: linear-gradient(45deg, #0066cc, #0052a3);">
                        <div class="character-icon">⚔️</div>
                        <div>رورونوا زورو</div>
                        <div>One Piece</div>
                    </div>
                    <div class="character-back">
                        <p>صياد القراصنة - أفضل سياف في الطاقم</p>
                        <p>يستخدم أسلوب السيف الثلاثي (سانتوريو)</p>
                    </div>
                </div>
            </div>
            
            <div class="character">
                <div class="character-inner">
                    <div class="character-front" style="background: linear-gradient(45deg, #4a235a, #3d1c4a);">
                        <div class="character-icon">👑</div>
                        <div>الملك الزاهد</div>
                        <div>Tower of God</div>
                    </div>
                    <div class="character-back">
                        <p>أحد المحاربين العشرة العظماء</p>
                        <p>يستخدم الشينسو الأسود</p>
                    </div>
                </div>
            </div>
            
            <div class="character">
                <div class="character-inner">
                    <div class="character-front" style="background: linear-gradient(45deg, #1a5276, #154360);">
                        <div class="character-icon">🌟</div>
                        <div>بام</div>
                        <div>Tower of God</div>
                    </div>
                    <div class="character-back">
                        <p>الصاعد غير المنتظم</p>
                        <p>يمتلك قدرات فريدة في التحكم في الشينسو</p>
                    </div>
                </div>
            </div>
        </div>
        
        <!-- تبويب اللغات -->
        <div class="language-tabs">
            <div class="tab active" data-lang="ar">الحل باللغة العربية</div>
            <div class="tab" data-lang="en">Solution in English</div>
        </div>
        
        <!-- قسم الحل باللغة العربية -->
        <div id="arabic-section" class="content-section active">
            <div class="section-title">
                <i class="fas fa-leaf"></i>
                السؤال الأول: تعريف المصطلحات والكتابة القصيرة
            </div>
            
            <div class="question-block">
                <div class="question-title">
                    <i class="fas fa-question-circle"></i>
                    <span>أ: التعريف (أربعة مصطلحات فقط - 5 درجات)</span>
                </div>
                <ul class="answer-list">
                    <li class="correct-answer"><strong>ساق منتفخ (Stem Bulb):</strong> نوع من السيقان الأرضية المتخصصة لتخزين الغذاء، مثل بصلة البصل.</li>
                    <li class="correct-answer"><strong>جذر متسلق (Climbing root):</strong> جذور هوائية تنمو من العقد الساقية لتساعد النبات على التسلق على الدعامات.</li>
                    <li class="correct-answer"><strong>جذور تنفسية (Pneumatophores):</strong> جذور هوائية خاصة بالنباتات التي تنمو في التربة الفقيرة بالأكسجين (مثل المانجروف)، تساعد في التنفس.</li>
                    <li class="correct-answer"><strong>إنبات هوائي (Epigeal germination):</strong> نوع من إنبات البذور حيث ترفع الفلقات فوق سطح التربة.</li>
                    <li><strong>تعديل الورقة (Leaf Modification):</strong> تحورات الأوراق لأداء وظائف غير التركيب الضوئي، مثل التحول إلى أشواك أو محاليق.</li>
                </ul>
            </div>
            
            <div class="question-block">
                <div class="question-title">
                    <i class="fas fa-question-circle"></i>
                    <span>ب: الكتابة القصيرة (موضوعين فقط - 5 درجات)</span>
                </div>
                <ul class="answer-list">
                    <li class="correct-answer">
                        <strong>1- وظائف القفيصة الفيروسية:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>حماية المادة الوراثية للفيروس</li>
                            <li>المساعدة في التعلق بالخلية المضيفة</li>
                            <li>تسهيل دخول الفيروس إلى الخلية</li>
                            <li>توفير الشكل المحدد للفيروس</li>
                        </ul>
                    </li>
                    <li class="correct-answer">
                        <strong>2- مجموعات البكتيريا بناءً على استجابتها للأكسجين الغازي:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>بكتيريا هوائية (Aerobic): تحتاج إلى أكسجين</li>
                            <li>بكتيريا لاهوائية (Anaerobic): لا تحتاج إلى أكسجين وقد يسبب لها ضرراً</li>
                            <li>بكتيريا لاهوائية اختيارية (Facultative anaerobic): يمكنها العيش مع أو بدون أكسجين</li>
                            <li>بكتيريا محبة للأكسجين القليل (Microaerophilic): تحتاج إلى كميات قليلة من الأكسجين</li>
                        </ul>
                    </li>
                    <li>
                        <strong>3- أنماط التغذية في الفطريات:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>تغذية رمية (Saprophytic): على المادة العضوية الميتة</li>
                            <li>تغذية تطفلية (Parasitic): على كائن حي آخر</li>
                            <li>تغذية تبادلية (Mutualistic): علاقة منفعة متبادلة مع كائن آخر</li>
                        </ul>
                    </li>
                </ul>
            </div>
            
            <div class="section-title">
                <i class="fas fa-list-ol"></i>
                السؤال الثاني: أسئلة الاختيار من متعدد (40 سؤالاً - كل نقطة 0.75 درجة)
            </div>
            
            <table class="mcq-table">
                <thead>
                    <tr>
                        <th width="10%">رقم السؤال</th>
                        <th width="60%">السؤال</th>
                        <th width="30%">الإجابة الصحيحة</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><span class="q-number">1</span></td>
                        <td>...... مجموعة غير متحركة وخيطية من الطحالب الخضراء</td>
                        <td class="correct-answer">ج - Chlorococcine</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">2</span></td>
                        <td>...... لها هيكل سيليسي (frustule)</td>
                        <td class="correct-answer">د - Diatoms</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">3</span></td>
                        <td>...... تحتوي بالإضافة إلى الكلوروفيل، على أصباغ التمثيل الضوئي الأخرى مثل Phycobilins</td>
                        <td class="correct-answer">أ - Blue green</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">4</span></td>
                        <td>...... هو نوع من إعادة التركيب الذي يتضمن تبادل الحمض النووي البكتيري في العاثيات</td>
                        <td class="correct-answer">ج - Transduction</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">5</span></td>
                        <td>الفيروسات التي تهاجم البكتيريا تعرف باسم ......</td>
                        <td class="correct-answer">أ - Bacteriophages</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">6</span></td>
                        <td>...... من فطر Puccinia graminis يمكن أن تصيب أوراق نبات القمح</td>
                        <td class="correct-answer">أ - Uredospores</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">7</span></td>
                        <td>...... بكتيريا ممرضة، تسبب أمراض خطيرة في الكائنات المضيفة</td>
                        <td class="correct-answer">ج - Parasitic</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">8</span></td>
                        <td>...... تفتقر إلى دورة تكاثر جنسية معروفة ويقال أنها "ناقصة"</td>
                        <td class="correct-answer">د - Deuteromycota</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">9</span></td>
                        <td>...... البكتيريا تصنع مركبات عضوية من مواد غير عضوية باستخدام الطاقة المنبعثة من أكسدة المواد غير العضوية</td>
                        <td class="correct-answer">ب - Chemosynthetic</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">10</span></td>
                        <td>عند بداية نقص النيتروجين أثناء ظروف التزهير، تتطور بعض الخلايا في Nostoc إلى ...... والتي تحول غاز النيتروجين إلى أمونيوم</td>
                        <td class="correct-answer">أ - heterocysts</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">11</span></td>
                        <td>في شكله المعدي، خارج الخلية، يسمى جسيم الفيروس ......</td>
                        <td class="correct-answer">أ - Virion</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">12</span></td>
                        <td>في العديد من ...... تتكون الجدران الخلوية من السليلوز مع كميات كبيرة من السيليكا</td>
                        <td class="correct-answer">ب - Chrysophytes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">13</span></td>
                        <td>الجزء الخارجي من الخلية في ...... يتكون من طبقة صلبة ولكن مرنة تسمى الغشاء المتقطع (pellicle)</td>
                        <td class="correct-answer">د - Euglena</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">14</span></td>
                        <td>...... نباتات تحتوي على نسيج الخشب واللحاء وتعتمد في انتشارها على الأبواغ وليس البذور</td>
                        <td class="correct-answer">ب - Pteridophytes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">15</span></td>
                        <td>وجود الصبغة البنية fucoxanthin في ...... يسمح بامتصاص أطوال موجية من الضوء تخترق الماء</td>
                        <td class="correct-answer">د - Fucus</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">16</span></td>
                        <td>...... الأشنيات شبيهة بالأوراق، مع صفائح مسطحة من الأنسجة غير مرتبطة بإحكام</td>
                        <td class="correct-answer">ب - Foliose</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">17</span></td>
                        <td>في ......، الجيل المشيجي هو السائد والجيل البوغي مرتبط ومعتمد على الجيل المشيجي للتغذية</td>
                        <td class="correct-answer">أ - Bryophyta</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">18</span></td>
                        <td>منتجات تخزين الطعام في Chrysophytes هي زيوت أو عديد السكاريد ......</td>
                        <td class="correct-answer">ب - leucosin</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">19</span></td>
                        <td>التلقيح في عاريات البذور بواسطة ......</td>
                        <td class="correct-answer">د - wind</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">20</span></td>
                        <td>الهيفات الفطرية متعددة الخلايا التي لها خلايا منفصلة تسمى ......</td>
                        <td class="correct-answer">ج - septate</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">21</span></td>
                        <td>...... تغطي سطح الجذر</td>
                        <td class="correct-answer">ب - pneumatophores</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">22</span></td>
                        <td>في البذور، ...... يقع بين البرعم والفلقات</td>
                        <td class="correct-answer">ب - epicotyl</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">23</span></td>
                        <td>جنين البذرة يتكون من ......</td>
                        <td class="correct-answer">د - all answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">24</span></td>
                        <td>يمكن أن تتحول الورقة إلى بنية خيطية حساسة تعرف باسم ......</td>
                        <td class="correct-answer">ب - tendril</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">25</span></td>
                        <td>أثناء إنبات البذور، يتم امتصاص الماء بشكل رئيسي من خلال ......</td>
                        <td class="correct-answer">ج - micropyle</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">26</span></td>
                        <td>...... هي سيقان ضعيفة تستلقي أفقياً على الأرض ولها نظام جذري واحد</td>
                        <td class="correct-answer">د - Prostrate stems</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">27</span></td>
                        <td>أي من الوظائف التالية تنطبق على الجذور الدعامية؟</td>
                        <td class="correct-answer">ب - Mechanical support</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">28</span></td>
                        <td>حافة الورقة تكون ...... عندما تحتوي على عدة نتوءات مستديرة</td>
                        <td class="correct-answer">د - crenate</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">29</span></td>
                        <td>أي من المعلومات التالية صحيح عن الجذور العقدية؟</td>
                        <td class="correct-answer">د - All answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">30</span></td>
                        <td>أي من النباتات التالية من النباتات المزهرة؟</td>
                        <td class="correct-answer">د - (A & C)</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">31</span></td>
                        <td>الجزء الصالح للأكل في البصل هو ......</td>
                        <td class="correct-answer">ب - stem</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">32</span></td>
                        <td>أي مما يلي يمثل تحوراً في الورقة؟</td>
                        <td class="correct-answer">د - No answer</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">33</span></td>
                        <td>البذور غير الإندوسبيرمية تخزن الغذاء في ......</td>
                        <td class="correct-answer">أ - cotyledons</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">34</span></td>
                        <td>الجزر هو مثال على ...... الجذر الوتدي</td>
                        <td class="correct-answer">ب - conical</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">35</span></td>
                        <td>نبات الحامول نبات طفيلي، يستخدم الممصات لامتصاص التغذية من ...... البرسيم</td>
                        <td class="correct-answer">ب - stem</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">36</span></td>
                        <td>ما هو نوع التفرع في الصورة التالية؟</td>
                        <td class="correct-answer">ب - Sympodial branching</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">37</span></td>
                        <td>تتصل الأوراق بالساق عند ......</td>
                        <td class="correct-answer">أ - nodes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">38</span></td>
                        <td>أي من هذه يساعد الجذور المتسلقة على التمسك بالدعم بقوة؟</td>
                        <td class="correct-answer">د - All answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">39</span></td>
                        <td>الجذور الهوائية هي استرطابية، مما يعني أنها ......</td>
                        <td class="correct-answer">ج - absorb moisture from air</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">40</span></td>
                        <td>الجذور الهوائية هي استرطابية، مما يعني أنها ......</td>
                        <td class="correct-answer">ج - absorb moisture from air</td>
                    </tr>
                </tbody>
            </table>
            
            <div class="answer-key">
                <h3><i class="fas fa-key"></i> ملخص الإجابات 1-40:</h3>
                <p>1: ج | 2: د | 3: أ | 4: ج | 5: أ | 6: أ | 7: ج | 8: د | 9: ب | 10: أ</p>
                <p>11: أ | 12: ب | 13: د | 14: ب | 15: د | 16: ب | 17: أ | 18: ب | 19: د | 20: ج</p>
                <p>21: ب | 22: ب | 23: د | 24: ب | 25: ج | 26: د | 27: ب | 28: د | 29: د | 30: د</p>
                <p>31: ب | 32: د | 33: أ | 34: ب | 35: ب | 36: ب | 37: أ | 38: د | 39: ج | 40: ج</p>
            </div>
        </div>
        
        <!-- قسم الحل باللغة الإنجليزية -->
        <div id="english-section" class="content-section">
            <div class="section-title">
                <i class="fas fa-leaf"></i>
                Question 1: Definition and Short Answers
            </div>
            
            <div class="question-block">
                <div class="question-title">
                    <i class="fas fa-question-circle"></i>
                    <span>A: Identification (Four terms only - 5 Marks)</span>
                </div>
                <ul class="answer-list">
                    <li class="correct-answer"><strong>Stem Bulb:</strong> A type of specialized underground stem for food storage, like an onion bulb.</li>
                    <li class="correct-answer"><strong>Climbing root:</strong> Aerial roots that grow from stem nodes to help the plant climb supports.</li>
                    <li class="correct-answer"><strong>Pneumatophores:</strong> Specialized aerial roots of plants growing in oxygen-poor soil (like mangroves), aiding in respiration.</li>
                    <li class="correct-answer"><strong>Epigeal germination:</strong> A type of seed germination where cotyledons are raised above the soil surface.</li>
                    <li><strong>Leaf Modification:</strong> Modifications of leaves to perform functions other than photosynthesis, like transformation into spines or tendrils.</li>
                </ul>
            </div>
            
            <div class="question-block">
                <div class="question-title">
                    <i class="fas fa-question-circle"></i>
                    <span>B: Brief Writing (Two topics only - 5 Marks)</span>
                </div>
                <ul class="answer-list">
                    <li class="correct-answer">
                        <strong>1- Functions of virus capsid:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>Protection of the viral genetic material</li>
                            <li>Assistance in attachment to host cell</li>
                            <li>Facilitation of virus entry into the cell</li>
                            <li>Providing the specific shape of the virus</li>
                        </ul>
                    </li>
                    <li class="correct-answer">
                        <strong>2- Groups of bacteria based on their response to gaseous oxygen:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>Aerobic bacteria: Require oxygen</li>
                            <li>Anaerobic bacteria: Do not require oxygen and may be harmed by it</li>
                            <li>Facultative anaerobic bacteria: Can live with or without oxygen</li>
                            <li>Microaerophilic bacteria: Require small amounts of oxygen</li>
                        </ul>
                    </li>
                    <li>
                        <strong>3- Nutrition mode in fungi:</strong>
                        <ul style="margin-right: 20px; margin-top: 8px;">
                            <li>Saprophytic nutrition: On dead organic matter</li>
                            <li>Parasitic nutrition: On another living organism</li>
                            <li>Mutualistic nutrition: Mutually beneficial relationship with another organism</li>
                        </ul>
                    </li>
                </ul>
            </div>
            
            <div class="section-title">
                <i class="fas fa-list-ol"></i>
                Question 2: Multiple Choice Questions (40 questions - Each 0.75 Mark)
            </div>
            
            <table class="mcq-table">
                <thead>
                    <tr>
                        <th width="10%">No.</th>
                        <th width="60%">Question</th>
                        <th width="30%">Correct Answer</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td><span class="q-number">1</span></td>
                        <td>...... group are non-motile & filamentous chlorophytes</td>
                        <td class="correct-answer">C - Chlorococcine</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">2</span></td>
                        <td>...... have a siliceous skeleton (frustule)</td>
                        <td class="correct-answer">D - Diatoms</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">3</span></td>
                        <td>...... algae contain in addition to chlorophyll, other photosynthetic pigments, such as Phycobilins</td>
                        <td class="correct-answer">A - Blue green</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">4</span></td>
                        <td>...... is a type of recombination that involves the exchanging of bacterial DNA in bacteriophages</td>
                        <td class="correct-answer">C - Transduction</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">5</span></td>
                        <td>Viruses that attack bacteria are known as ......</td>
                        <td class="correct-answer">A - Bacteriophages</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">6</span></td>
                        <td>...... of Puccinia graminis can infect the leaves of wheat plant.</td>
                        <td class="correct-answer">A - Uredospores</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">7</span></td>
                        <td>...... bacteria are pathogenic bacteria, causing serious diseases in the host organisms.</td>
                        <td class="correct-answer">C - Parasitic</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">8</span></td>
                        <td>...... lack a known sexual cycle of reproduction and are said to be "imperfect"</td>
                        <td class="correct-answer">D - Deuteromycota</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">9</span></td>
                        <td>...... bacteria manufacture organic compounds from inorganic raw materials utilizing energy liberated from the oxidation of inorganic substances</td>
                        <td class="correct-answer">B - Chemosynthetic</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">10</span></td>
                        <td>At the onset of nitrogen limitation during bloom conditions, certain cells in Nostoc evolve into ...... which convert nitrogen gas into ammonium.</td>
                        <td class="correct-answer">A - heterocysts</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">11</span></td>
                        <td>In its infective form, outside the cell, a virus particle is called a ......</td>
                        <td class="correct-answer">A - Virion</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">12</span></td>
                        <td>In many ...... the cell walls are composed of cellulose with large quantities of silica.</td>
                        <td class="correct-answer">B - Chrysophytes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">13</span></td>
                        <td>The outer part of the cell in ...... consists of a firm but flexible layer called a pellicle, or periplast.</td>
                        <td class="correct-answer">D - Euglena</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">14</span></td>
                        <td>...... plants with xylem and phloem whose dispersal relies on spores not seeds.</td>
                        <td class="correct-answer">B - Pteridophytes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">15</span></td>
                        <td>The presence of the brown pigment fucoxanthin in ...... allows the absorption of wavelengths of light that penetrate the water</td>
                        <td class="correct-answer">D - Fucus</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">16</span></td>
                        <td>...... lichen is leaf-like, with flat sheets of tissue not tightly bound.</td>
                        <td class="correct-answer">B - Foliose</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">17</span></td>
                        <td>In ......, the gametophyte generation is dominant and the sporophyte is attached and dependent upon the gametophyte for nutrition.</td>
                        <td class="correct-answer">A - Bryophyta</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">18</span></td>
                        <td>The food storage products of Chrysophytes are oils or the polysaccharide ......</td>
                        <td class="correct-answer">B - leucosin</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">19</span></td>
                        <td>Pollination in Gymnosperms by ......</td>
                        <td class="correct-answer">D - wind</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">20</span></td>
                        <td>Multicellular fungal hyphae that have separate cells are called ......</td>
                        <td class="correct-answer">C - septate</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">21</span></td>
                        <td>Lenticels cover the root surface of ......</td>
                        <td class="correct-answer">B - pneumatophores</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">22</span></td>
                        <td>In seeds the ...... lies between the plumule and the cotyledons.</td>
                        <td class="correct-answer">B - epicotyl</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">23</span></td>
                        <td>The embryo of the seed consists of ......</td>
                        <td class="correct-answer">D - all answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">24</span></td>
                        <td>Leaf can be modified into a threadlike sensitive structure known as ......</td>
                        <td class="correct-answer">B - tendril</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">25</span></td>
                        <td>During seed germination, water is absorbed mainly through the ......</td>
                        <td class="correct-answer">C - micropyle</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">26</span></td>
                        <td>...... are weak stems that lie horizontally on the ground and having one root system.</td>
                        <td class="correct-answer">D - Prostrate stems</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">27</span></td>
                        <td>Which of the following functions apply for prop roots?</td>
                        <td class="correct-answer">B - Mechanical support</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">28</span></td>
                        <td>Leaf margin is ...... when it has several round processes</td>
                        <td class="correct-answer">D - crenate</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">29</span></td>
                        <td>Which is true about nodulated roots?</td>
                        <td class="correct-answer">D - All answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">30</span></td>
                        <td>Which of the following is flowering plant?</td>
                        <td class="correct-answer">D - (A & C)</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">31</span></td>
                        <td>The edible part of onion is ......</td>
                        <td class="correct-answer">B - stem</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">32</span></td>
                        <td>Which is a leaf modification?</td>
                        <td class="correct-answer">D - No answer</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">33</span></td>
                        <td>Non-endospermous seeds store food in ......</td>
                        <td class="correct-answer">A - cotyledons</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">34</span></td>
                        <td>Carrot is an example of ...... tap root</td>
                        <td class="correct-answer">B - conical</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">35</span></td>
                        <td>Cuscuta is a parasitic plant, it uses haustoria to absorb nutrition from the ...... of Trifolium alexandrinum.</td>
                        <td class="correct-answer">B - stem</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">36</span></td>
                        <td>What is the type of branching in the following picture?</td>
                        <td class="correct-answer">B - Sympodial branching</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">37</span></td>
                        <td>Leaves are attached to the stem at .......</td>
                        <td class="correct-answer">A - nodes</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">38</span></td>
                        <td>Which of these help climbing roots to hold the support firmly?</td>
                        <td class="correct-answer">D - All answers</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">39</span></td>
                        <td>The aerial roots are hygroscopic, that means they .......</td>
                        <td class="correct-answer">C - absorb moisture from air</td>
                    </tr>
                    <tr>
                        <td><span class="q-number">40</span></td>
                        <td>The aerial roots are hygroscopic, that means they .......</td>
                        <td class="correct-answer">C - absorb moisture from air</td>
                    </tr>
                </tbody>
            </table>
            
            <div class="answer-key">
                <h3><i class="fas fa-key"></i> Answer Summary 1-40:</h3>
                <p>1: C | 2: D | 3: A | 4: C | 5: A | 6: A | 7: C | 8: D | 9: B | 10: A</p>
                <p>11: A | 12: B | 13: D | 14: B | 15: D | 16: B | 17: A | 18: B | 19: D | 20: C</p>
                <p>21: B | 22: B | 23: D | 24: B | 25: C | 26: D | 27: B | 28: D | 29: D | 30: D</p>
                <p>31: B | 32: D | 33: A | 34: B | 35: B | 36: B | 37: A | 38: D | 39: C | 40: C</p>
            </div>
        </div>
        
        <!-- تذييل الصفحة -->
        <footer>
            <p>© 2025 South Valley University - Department of Botany & Microbiology</p>
            <p>Botany (I) Exam Solution - Bot 101 - January 2025</p>
            <div class="footer-note">
                <p><i class="fas fa-exclamation-triangle"></i> هذا الحل تم إعداده للأغراض التعليمية فقط. جميع الإجابات قابلة للمراجعة والتدقيق.</p>
                <p><i class="fas fa-palette"></i> تصميم مستوحى من أنمي ون بيس (One Piece) وتاور أوف جود (Tower of God)</p>
                <p><i class="fas fa-graduation-cap"></i> مع تمنياتنا بالنجاح والتوفيق لجميع الطلاب</p>
            </div>
        </footer>
    </div>

    <script>
        // تفعيل التبويب بين اللغتين
        document.addEventListener('DOMContentLoaded', function() {
            const tabs = document.querySelectorAll('.tab');
            const arabicSection = document.getElementById('arabic-section');
            const englishSection = document.getElementById('english-section');
            
            tabs.forEach(tab => {
                tab.addEventListener('click', function() {
                    // إزالة الفئة النشطة من جميع التبويبات
                    tabs.forEach(t => t.classList.remove('active'));
                    
                    // إضافة الفئة النشطة للتبويب المحدد
                    this.classList.add('active');
                    
                    // تحديد القسم المراد عرضه
                    const lang = this.getAttribute('data-lang');
                    
                    if (lang === 'ar') {
                        arabicSection.classList.add('active');
                        englishSection.classList.remove('active');
                    } else {
                        englishSection.classList.add('active');
                        arabicSection.classList.remove('active');
                    }
                });
            });
            
            // تأثيرات إضافية للشخصيات
            const characters = document.querySelectorAll('.character');
            characters.forEach(character => {
                character.addEventListener('mouseenter', function() {
                    this.style.transform = 'scale(1.05)';
                });
                
                character.addEventListener('mouseleave', function() {
                    this.style.transform = 'scale(1)';
                });
            });
            
            // تأثيرات للأسئلة عند التمرير
            const questionBlocks = document.querySelectorAll('.question-block');
            const observerOptions = {
                threshold: 0.1,
                rootMargin: '0px 0px -50px 0px'
            };
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateX(0)';
                    }
                });
            }, observerOptions);
            
            questionBlocks.forEach(block => {
                block.style.opacity = '0';
                block.style.transform = 'translateX(50px)';
                block.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                observer.observe(block);
            });
            
            // تأثيرات للجدول عند التمرير
            const tableRows = document.querySelectorAll('.mcq-table tr');
            tableRows.forEach((row, index) => {
                row.style.opacity = '0';
                row.style.transform = 'translateY(20px)';
                row.style.transition = 'opacity 0.5s ease, transform 0.5s ease';
                
                setTimeout(() => {
                    observer.observe(row);
                }, index * 50);
            });
        });
    </script>
</body>
</html>
