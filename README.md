<html lang="ko">
<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title data-lang-key="meta_title">BEST WORK - 외국인 유학생 및 취업 컨설팅</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* CSS Variables */
        :root { --accent: #0b76ef; --muted: #555; --bg-light: #f9f9f9; --nav-height: 60px; }
        /* Reset and Base Styles */
        * { box-sizing: border-box; margin: 0; padding: 0; }
        body, html { 
            /* ⚠️ 수정: height: 100% 대신 min-height: 100% 사용 */
            min-height: 100%; 
            /* ⚠️ 수정: 가로 스크롤 이슈 최소화를 위해 overflow-x: hidden 제거 */
            font-family: -apple-system, BlinkMacSystemFont, "Inter", "Helvetica Neue", Arial, sans-serif; 
            color: #222; 
        }

        /* [전역 콘텐츠 최대 너비 제한] */
        img, video, iframe {
            max-width: 100%;
            height: auto;
            display: block; 
        }

        /* Navigation Bar (Desktop & Base) */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: var(--nav-height); /* 네비게이션바 높이 고정 */
            background: rgba(11, 18, 32, 0.95);
            color: #fff;
            z-index: 1000;
            padding: 0 20px; /* 상하 패딩 제거하고 높이로 조절 */
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .navbar-brand {
            font-size: 24px;
            font-weight: 900;
            color: #fff;
            text-decoration: none;
            transition: color 0.3s;
        }
        .navbar-brand:hover { color: var(--accent); }
        
        .navbar-right-group {
            display: flex;
            align-items: center;
            flex-shrink: 1; 
            min-width: 0; 
        }
        
        .navbar-links {
            display: flex; 
            align-items: center;
        }

        .navbar-links a {
            color: #fff;
            text-decoration: none;
            margin-left: 25px;
            font-weight: 600;
            transition: color 0.3s;
            white-space: nowrap; 
        }
        .navbar-links a:hover { color: var(--accent); }
        
        /* Language Switcher Styles */
        .lang-switcher {
            margin-left: 30px; 
            display: flex;
            align-items: center;
            border: 1px solid #ffffff60;
            border-radius: 6px;
            overflow: hidden;
            white-space: nowrap; 
        }
        .lang-btn {
            background: none;
            border: none;
            color: #fff;
            padding: 5px 10px;
            cursor: pointer;
            font-size: 14px;
            font-weight: 600;
            transition: background 0.2s, color 0.2s;
        }
        .lang-btn.active {
            background: var(--accent);
            color: #fff;
        }
        .lang-btn:not(.active):hover {
            background: #ffffff30;
        }
        
        /* Burger Menu Icon (Hidden on Desktop) */
        .burger-menu {
            display: none;
            background: none;
            border: none;
            color: #fff;
            font-size: 28px;
            cursor: pointer;
            z-index: 1001; /* 메뉴보다 위에 위치 */
        }
        
        /* Mobile Menu (Vertical Navigation) */
        .mobile-menu {
            position: fixed;
            top: var(--nav-height); /* 네비게이션바 바로 아래에서 시작 */
            left: 0;
            width: 100%;
            /* ⚠️ 수정: 모바일 뷰포트 오류 해결을 위해 100vh를 100dvh로 변경 */
            height: calc(100dvh - var(--nav-height));
            background: rgba(11, 18, 32, 0.98);
            z-index: 999;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 40px 20px;
            transform: translateX(100%);
            transition: transform 0.3s ease-in-out;
            overflow-y: auto; /* 내용이 길어지면 스크롤 가능 */
        }

        .mobile-menu.open {
            transform: translateX(0);
        }

        .mobile-menu a {
            color: #fff;
            text-decoration: none;
            font-size: 22px;
            font-weight: 600;
            padding: 15px 0;
            width: 100%;
            text-align: center;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        .mobile-menu a:last-child {
            border-bottom: none;
        }
        
        /* Header (Full Screen Hero) */
        header {
            position: relative;
            /* ⚠️ 수정: 모바일 가로/세로 전환시 뷰포트 오류 해결을 위해 100vh를 100dvh로 변경 및 min-height 추가 */
            min-height: 500px; /* 최소 높이 지정 */
            height: 100dvh; 
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            overflow: hidden;
            /* 배경 이미지/영상이 여백 없이 화면을 덮도록 no-repeat 추가 */
            background: url('https://github.com/BEST-WORK/BESTWORK/blob/main/Adobe%20Express%20-%20IMG_8171%20(1).gif?raw=true') center/cover no-repeat fixed;
            color: #fff;
        }
        header::before {
            content: "";
            position: absolute;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0,0,0,0.45);
            z-index: 0;
        }
        header .overlay {
            position: relative;
            z-index: 2;
            max-width: 800px;
            padding: 24px;
            animation: fadeInUp 2s ease-out;
        }
        .logo { font-size: 60px !important; font-weight: 900; margin-bottom: 20px; animation: fadeIn 2s ease-in-out; text-shadow: 0 6px 14px rgba(0,0,0,0.7); }
        header h1 { font-size: 40px; font-weight: 800; line-height: 1.3; margin-bottom: 16px; text-shadow: 0 4px 12px rgba(0,0,0,0.6); animation: slideIn 3s ease-in-out infinite alternate; }
        header p { font-size: 18px; margin-bottom: 24px; color: #e0e0e0; text-shadow: 0 2px 8px rgba(0,0,0,0.6); animation: fadeIn 4s ease-out; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(40px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        @keyframes slideIn { 0% { letter-spacing: 0px; } 100% { letter-spacing: 2px; } }

        .btn {
            display: inline-block; background: #fff; color: var(--accent); padding: 12px 24px; border-radius: 8px; font-weight: 700; text-decoration: none; transition: background 0.3s; animation: fadeIn 3s ease-in-out;
        }
        .btn:hover { background: #e8e8e8; }

        /* Section Styling */
        section { padding: 100px 20px 80px 20px; background: #fff; color: #222; text-align: center; }
        h2 { font-size: 26px; margin-bottom: 16px; }
        .muted { color: var(--muted); }
        .container { max-width: 1100px; margin: 0 auto; }

        /* Services Section (배경 이미지/영상이 여백 없이 화면을 덮도록 no-repeat 추가) */
        #services {
            position: relative;
            background: url('https://github.com/BEST-WORK/BESTWORK/blob/main/IMG_8690.gif?raw=true') center center/cover no-repeat fixed;
        }
        #services::before { content: ""; position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.65); z-index: 1; }
        #services .container > * { position: relative; z-index: 2; }
        #services h2, #services .muted, #services h3 { color: #fff; }
        #services .muted { color: #e0e0e0; }

        /* Card Styles */
        .card-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; margin-top: 40px; }
        .uni-card {
            background: #fff; border-radius: 12px; box-shadow: 0 6px 15px rgba(0,0,0,0.08); text-align: left; transition: transform 0.3s; overflow: hidden; padding: 25px; border-top: 5px solid var(--accent); 
        }
        .uni-card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.15); }
        .uni-card h3 { font-size: 20px; font-weight: 800; color: #0b1220; margin-bottom: 5px; }
        .uni-card p { font-size: 14px; color: var(--muted); line-height: 1.6; }

        /* Country Card Styles */
        .country-card {
            border-radius: 12px; box-shadow: 0 6px 15px rgba(0,0,0,0.2); text-align: left; transition: transform 0.3s; overflow: hidden; padding: 30px 25px; color: #fff; position: relative; border: none;
        }
        .country-card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.25); }
        .country-card h3 { color: #fff; font-size: 20px; font-weight: 800; margin-bottom: 5px; text-shadow: 0 1px 3px rgba(0, 0, 0, 0.4); }
        .country-card p { color: #f0f0f0; font-size: 14px; line-height: 1.6; text-shadow: 0 1px 3px rgba(0, 0, 0, 0.4); }
        .country-card .flag { font-size: 35px; margin-bottom: 15px; display: block; text-shadow: none; }
        .card-nepal { background: linear-gradient(135deg, #231F20 0%, #E83F3F 100%); }
        .card-bangladesh { background: linear-gradient(135deg, #006A4E 0%, #F42A41 100%); }
        .card-myanmar { background: linear-gradient(135deg, #FECB00 0%, #34B233 50%, #EA2839 100%); }
        .card-srilanka { background: linear-gradient(135deg, #D4AF37 0%, #FF8C00 100%); }
        .card-vietnam { background: linear-gradient(135deg, #DA251D 0%, #D61A13 100%); }

        /* Slider Styles */
        .slider-container { position: relative; max-width: 900px; height: 400px; margin: 0 auto 50px auto; overflow: hidden; border-radius: 12px; box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15); }
        .slider-wrapper { display: flex; height: 100%; transition: transform 0.5s ease-in-out; }
        .slide { min-width: 100%; height: 100%; position: relative; box-sizing: border-box; display: flex; align-items: center; justify-content: center; }
        .slide img { width: 100%; height: 100%; object-fit: cover; display: block; }
        .slider-button {
            position: absolute; top: 50%; transform: translateY(-50%); background: rgba(0, 0, 0, 0.4); color: white; border: none; padding: 10px; cursor: pointer; z-index: 10; font-size: 24px; line-height: 1; border-radius: 50%; width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; transition: background 0.3s; opacity: 0.8;
        }
        .slider-button:hover { background: rgba(0, 0, 0, 0.7); opacity: 1; }
        #prev-button { left: 10px; }
        #next-button { right: 10px; }
        @media (max-width: 768px) {
            .slider-container { height: 300px; }
            .slider-button { width: 30px; height: 30px; font-size: 18px; }
        }

        /* Contact Section */
        #contact-form label { display: block; text-align: left; font-size: 14px; font-weight: 600; margin-bottom: 5px; color: #333; }
        #contact-form input[type="text"], #contact-form input[type="email"], #contact-form textarea { width: 100%; padding: 10px; margin-bottom: 20px; border: 1px solid #ccc; border-radius: 6px; font-size: 16px; transition: border-color 0.3s, box-shadow 0.3s; }
        #contact-form input:focus, #contact-form textarea:focus { border-color: var(--accent); box-shadow: 0 0 0 2px rgba(11, 118, 239, 0.2); outline: none; }
        #contact-form textarea { resize: vertical; min-height: 120px; }
        #contact-form button[type="submit"] { display: block; width: 100%; background: var(--accent); color: #fff; padding: 12px; border: none; border-radius: 8px; font-size: 18px; font-weight: 700; cursor: pointer; transition: background 0.3s, transform 0.1s; }
        #contact-form button[type="submit"]:hover { background: #0959bb; }
        #contact-form button[type="submit"]:active { transform: scale(0.99); }
        .social-links { margin-top: 30px; display: flex; justify-content: center; gap: 35px; padding-top: 30px; }
        .social-links a { font-size: 38px; color: var(--muted); transition: color 0.3s, transform 0.2s; text-decoration: none; }
        .social-links a:hover { transform: scale(1.1); }
        .social-links .fa-instagram:hover { color: #E4405F; }
        .social-links .fa-facebook-f:hover { color: #3B5998; }

        /* Footer Styling */
        footer { background: #0b1220; color: #dfefff; padding: 40px 0; text-align: center; }

        /* Responsive Adjustments (Mobile Optimization) */
        @media (max-width: 900px) {
            .navbar-links a { margin-left: 15px; font-size: 14px; }
        }
        
        @media (max-width: 768px) {
            /* Navbar Link Group, Language Switcher 숨김 (버거 메뉴로 대체) */
            .navbar-links, .lang-switcher {
                display: none;
            }
            
            /* Burger Menu 보임 */
            .burger-menu {
                display: block;
            }
            
            .logo { font-size: 42px !important; }
            header h1 { font-size: 28px; }
            
            .card-grid { grid-template-columns: 1fr; }
            
            /* [회사 소개 섹션 (About) 모바일 레이아웃] */
            #about .container > div {
                flex-direction: column; 
                padding: 0; 
            }
            #about .text-content {
                padding: 20px 0 0 0 !important; 
                text-align: center !important; 
            }
        }
    </style>
</head>
<body data-lang="ko">
    
    <nav class="navbar">
        <a href="#home" class="navbar-brand">BEST WORK</a>
        
        <div class="navbar-right-group">
            <div class="navbar-links">
                <a href="#about" data-lang-key="nav_about">회사 소개</a>
                <a href="#services" data-lang-key="nav_services">주요 서비스</a>
                <a href="#universities" data-lang-key="nav_universities">제휴 대학교</a>
                <a href="#countries" data-lang-key="nav_countries">주요 국가</a>
                <a href="#contact" data-lang-key="nav_contact">문의하기</a>
            </div>

            <div class="lang-switcher">
                <button class="lang-btn active" data-lang-code="ko">KO</button>
                <button class="lang-btn" data-lang-code="en">EN</button>
            </div>
            
            <button class="burger-menu" id="burger-menu-btn" aria-label="메뉴 열기">
                <i class="fas fa-bars"></i>
            </button>
        </div>
    </nav>
    
    <div class="mobile-menu" id="mobile-menu">
        <a href="#about" data-lang-key="nav_about" data-mobile-link>회사 소개</a>
        <a href="#services" data-lang-key="nav_services" data-mobile-link>주요 서비스</a>
        <a href="#universities" data-lang-key="nav_universities" data-mobile-link>제휴 대학교</a>
        <a href="#countries" data-lang-key="nav_countries" data-mobile-link>주요 국가</a>
        <a href="#contact" data-lang-key="nav_contact" data-mobile-link>문의하기</a>
        <div style="margin-top: 30px; display: flex; gap: 10px;">
            <button class="lang-btn active" data-lang-code="ko" data-mobile-lang-btn>KO</button>
            <button class="lang-btn" data-lang-code="en" data-mobile-lang-btn>EN</button>
        </div>
    </div>

    <header id="home">
        <div class="overlay">
            <div class="logo">BEST WORK</div>
            <h1 data-lang-key="header_tagline">유학생·취업 외국인의 성공적인 한국 정착을 돕는 파트너</h1>
            <p data-lang-key="header_desc">글로벌 인재와 기회를 연결하며, 유학 및 취업을 통한 외국인의 성공적인 국내 정착을 지원합니다. 현지 네트워크와 다양한 사업 경험을 바탕으로 대학교 및 기업에 신뢰도 높은 서비스를 제공합니다.</p>
            <a class="btn" href="#about" data-lang-key="header_btn">자세히 알아보기</a> 
        </div>
    </header>

    <section id="about" style="padding: 100px 20px 80px 20px;">
        <div class="container">
            <h2 data-lang-key="about_title">회사 소개</h2>
            <div style="display: flex; flex-direction: row; flex-wrap: wrap; justify-content: center; align-items: center; gap: 40px; margin-top: 40px;"> 

                <div style="flex: 1 1 45%; max-width: 500px; min-width: 300px;">
                    <img src="https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250308_150855_1741415133899.JPG?raw=true" 
                         alt="BEST WORK Executive Meeting" 
                         style="width: 100%; height: auto; border-radius: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.15); object-fit: cover;">
                </div>
                
                <div class="text-content" style="flex: 1 1 50%; max-width: 600px; padding: 0 0 0 40px; text-align: left;">
                    <h3 data-lang-key="about_subtitle" style="font-size: 22px; font-weight: 700; color: var(--accent); margin-bottom: 15px;">글로벌 인재와 한국을 잇는 가장 신뢰받는 가교</h3>
                    
                    <p data-lang-key="about_p1" style="font-size: 16px; color: #444; line-height: 1.8; text-align: left;">BEST WORK는 유학과 취업을 통해 **대한민국에 성공적으로 정착**하고자 하는 외국인에게 전문적인 지원을 제공합니다. 단순히 인력을 배치하는 것을 넘어 인재의 **'생애주기(Life Cycle)'**를 관리하는 통합 솔루션입니다.</p>
                    
                    <p data-lang-key="about_p2" style="font-size: 16px; color: #444; line-height: 1.8; text-align: left; margin-top: 15px;">대학에는 **학업 열정이 높은 우수한 학생**을 소개하고, 기업에는 **최고의 외국인 전문 인력**을 지속적으로 공급하여, 한국 사회에 상호 성장을 위한 다리 역할을 수행합니다.</p>
                    
                    <p data-lang-key="about_p3" style="font-size: 16px; color: #444; line-height: 1.8; text-align: left; margin-top: 15px; font-weight: 600;">현지 국가에 직접 진출하여 서비스업, 유통업 등 다양한 사업을 경험한 노하우가 있습니다. 현지인의 니즈와 상황에 대한 깊은 이해를 바탕으로 가장 신뢰할 수 있는 효과적인 서비스를 제공합니다.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="services">
        <div class="container">
            <h2 data-lang-key="services_title">주요 서비스</h2>
            <p class="muted" data-lang-key="services_desc" style="max-width: 800px; margin: 0 auto 30px;">BEST WORK가 제공하는 핵심 솔루션을 확인하세요. 유학 컨설팅부터 비자 프로그램, 취업 연계까지 맞춤형 서비스를 제공합니다.</p>
            <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 40px; margin-top: 40px; text-align: center;">
                
                <div style="width: 300px; padding: 20px;">
                    <div style="font-size: 40px; color: #fff; margin-bottom: 15px;">🎓</div>
                    <h3 data-lang-key="service1_title" style="font-size: 22px; font-weight: 700; margin-bottom: 10px; color: #fff;">맞춤형 유학 컨설팅</h3>
                    <p data-lang-key="service1_desc" style="font-size: 16px; color: #e0e0e0; line-height: 1.6;">개인의 학업 목표와 적성에 맞춘 최적의 한국 대학 및 전공을 추천하며, 입학 절차 전반에 걸친 밀착 지원을 제공합니다.</p>
                </div>
                
                <div style="width: 300px; padding: 20px;">
                    <div style="font-size: 40px; color: #fff; margin-bottom: 15px;">🛂</div>
                    <h3 data-lang-key="service2_title" style="font-size: 22px; font-weight: 700; margin-bottom: 10px; color: #fff;">생애주기 비자 관리</h3>
                    <p data-lang-key="service2_desc" style="font-size: 16px; color: #e0e0e0; line-height: 1.6;">D-2(유학) 비자부터 E-7(전문직) 비자, 영주권까지, 한국 정착에 필요한 비자 전환에 대한 체계적인 로드맵과 준비 지원을 제공합니다.</p>
                </div>
                
                <div style="width: 300px; padding: 20px;">
                    <div style="font-size: 40px; color: #fff; margin-bottom: 15px;">💼</div>
                    <h3 data-lang-key="service3_title" style="font-size: 22px; font-weight: 700; margin-bottom: 10px; color: #fff;">국내 산업 인재 연계</h3>
                    <p data-lang-key="service3_desc" style="font-size: 16px; color: #e0e0e0; line-height: 1.6;">졸업 후 학생들이 한국에서 안정적인 취업에 성공하고 성공적으로 정착할 수 있도록 국내 산업체와의 인력 연계 서비스를 제공합니다.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="universities">
        <div class="container">
            <h2 data-lang-key="uni_title">제휴 대학교</h2>
            <p class="muted" data-lang-key="uni_desc" style="max-width: 800px; margin: 0 auto 40px;">BEST WORK가 파트너십을 맺은 국내 유수 대학들로, 외국인 유학생에게 최적의 학업 환경을 제공합니다.</p>
            
            <div class="slider-container">
                <div class="slider-wrapper" id="university-slider-wrapper">
                    <div class="slide">
                        <img src="https://github.com/BEST-WORK/BESTWORK/blob/main/IMG_8696.jpg?raw=true" 
                             alt="BEST WORK와 제휴 대학교 업무 협약 사진">
                    </div>
                    <div class="slide">
                        <img src="https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250812_124606.jpg?raw=true" 
                             alt="BEST WORK 해외 파트너와 미팅 사진">
                    </div>
                </div>
                <button class="slider-button" id="prev-button" aria-label="이전 이미지">❮</button>
                <button class="slider-button" id="next-button" aria-label="다음 이미지">❯</button>
            </div>
            
            <div class="card-grid">
                
                <div class="uni-card">
                    <h3 data-lang-key="uni1_title">건국대학교</h3>
                    <p data-lang-key="uni1_desc">서울 광진구에 위치한 명문 사립대학입니다. 생명과학, 공학, 경영 등 다양한 분야에서 우수성을 인정받으며, 활발한 국제 교류 프로그램으로 외국인 학생들에게 인기가 높습니다.</p>
                </div>
                
                <div class="uni-card">
                    <h3 data-lang-key="uni2_title">숙명여자대학교</h3>
                    <p data-lang-key="uni2_desc">대한민국 최초의 민족 사립학교 중 하나로, 여성 리더 양성의 요람으로 불립니다. IT, 인문, 사회과학, 약학 등의 분야에 강하며, 서울 용산 지역에 위치하여 접근성이 좋습니다.</p>
                </div>
                
                <div class="uni-card">
                    <h3 data-lang-key="uni3_title">한라대학교</h3>
                    <p data-lang-key="uni3_desc">강원도 원주에 위치한 산학협력 중심 대학입니다. 공학 및 디자인 분야에 특화되어 있으며, 지역 산업과 연계된 실용적인 교육을 제공하고 있습니다.</p>
                </div>
                
                <div class="uni-card">
                    <h3 data-lang-key="uni4_title">상지대학교</h3>
                    <p data-lang-key="uni4_desc">한의학, 보건복지, 예술 분야에서 높은 경쟁력을 갖춘 대학입니다. 강원 지역의 전통 있는 교육기관으로, 인성 함양과 전문성 강화에 집중하고 있습니다.</p>
                </div>
                
                <div class="uni-card">
                    <h3 data-lang-key="uni5_title">송호대학교</h3>
                    <p data-lang-key="uni5_desc">강원도 횡성에 위치한 전문대학으로, 실무 중심의 직업 교육을 통해 현장에 바로 투입 가능한 인재를 양성합니다. 국제 교류 협력을 통해 외국인 학생 유치에 적극적입니다.</p>
                </div>
                
                <div class="uni-card">
                    <h3 data-lang-key="uni6_title">서울신학대학교</h3>
                    <p data-lang-key="uni6_desc">기독교 정신을 바탕으로 인성과 전문성을 겸비한 글로벌 인재를 육성합니다. 인문, 사회과학, 신학 분야의 심도 있는 학문을 제공하며, 경기도 부천에 위치하고 있습니다.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="countries" style="background: var(--bg-light);">
        <div class="container">
            <h2 data-lang-key="country_title">주요 국가</h2> 
            <p class="muted" data-lang-key="country_desc" style="max-width: 800px; margin: 0 auto 40px;">BEST WORK는 현지 네트워크를 기반으로 다음과 같은 주요 국가에서 한국 유학 및 취업을 희망하는 우수 인재를 체계적으로 발굴하고 지원합니다.</p>
            <div class="card-grid">
                <div class="country-card card-nepal">
                    <span class="flag">🇳🇵</span>
                    <h3 data-lang-key="country1_title">네팔</h3>
                    <p data-lang-key="country1_desc">높은 학구열과 성실함을 자랑하는 인재의 보고입니다. 한국과의 근로자 및 유학생 교류가 오래전부터 활발했으며, 농업 및 제조업 분야에서 한국 경제에 기여하고 있습니다.</p>
                </div>
                <div class="country-card card-bangladesh">
                    <span class="flag">🇧🇩</span>
                    <h3 data-lang-key="country2_title">방글라데시</h3>
                    <p data-lang-key="country2_desc">젊고 역동적인 인구가 풍부한 활기찬 시장입니다. 한국과의 경제 협력이 확대되고 있으며, 특히 섬유 및 제조업 분야에서 유학 후 취업을 희망하는 인재가 늘고 있습니다.</p>
                </div>
                <div class="country-card card-myanmar">
                    <span class="flag">🇲🇲</span>
                    <h3 data-lang-key="country3_title">미얀마</h3>
                    <p data-lang-key="country3_desc">풍부한 자원과 경제 발전 잠재력을 가진 동남아시아의 전략적 거점입니다. 한국 유학에 대한 관심이 급증하고 있으며, 한국 정착을 희망하는 우수 인재를 발굴합니다.</p>
                </div>
                <div class="country-card card-srilanka">
                    <span class="flag">🇱🇰</span>
                    <h3 data-lang-key="country4_title">스리랑카</h3>
                    <p data-lang-key="country4_desc">높은 문해율과 교육 수준을 자랑하는 인도양의 섬나라입니다. IT 및 공학 등 전문 분야에서 한국 대학 및 기업을 목표로 하는 인재들이 많습니다.</p>
                </div>
                <div class="country-card card-vietnam">
                    <span class="flag">🇻🇳</span>
                    <h3 data-lang-key="country5_title">베트남</h3>
                    <p data-lang-key="country5_desc">한국과의 교류가 가장 활발한 핵심 거점 국가입니다. 근로자 파견(E-7 비자) 및 현지 사업 경험을 바탕으로 유학생 모집과 취업 연계에 독보적인 노하우를 보유하고 있습니다.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2 data-lang-key="contact_title">문의하기</h2>
            <p class="muted" data-lang-key="contact_desc" style="max-width: 600px; margin: 0 auto 40px;">BEST WORK와 함께 한국에서의 성공적인 유학 및 정착 여정을 시작하세요. 아래 양식을 작성해 주시면 전문 컨설턴트가 신속하게 답변드리겠습니다.</p>
            
            <div id="contact-form-container" style="max-width: 500px; width: 100%; padding: 30px; background: var(--bg-light); border-radius: 12px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); margin: 0 auto;">
                <form id="contact-form" onsubmit="handleFormSubmit(event)">
                    <label for="name" data-lang-key="form_name_label">이름</label>
                    <input type="text" id="name" name="name" required data-lang-key="form_name_placeholder" data-lang-attr="placeholder" placeholder="성함 또는 회사명">

                    <label for="email" data-lang-key="form_email_label">이메일 주소</label>
                    <input type="email" id="email" name="email" required data-lang-key="form_email_placeholder" data-lang-attr="placeholder" placeholder="example@email.com">

                    <label for="message" data-lang-key="form_message_label">문의 내용</label>
                    <textarea id="message" name="message" required data-lang-key="form_message_placeholder" data-lang-attr="placeholder" placeholder="문의 내용을 상세하게 작성해 주세요. (예: [회사/대학명] 제휴 문의)"></textarea>

                    <button type="submit" data-lang-key="form_submit_btn">문의 접수</button>
                </form>
                
                <div id="submit-message" style="display:none; margin-top: 20px; padding: 15px; border-radius: 8px; background: #e6f3ff; color: var(--accent); font-weight: 700;"></div>

                <div id="email-info" style="margin-top: 20px; border-top: 1px solid #ddd; padding-top: 20px;">
                    <div data-lang-key="contact_email_direct" style="font-size: 16px; font-weight: 600; color: #222; margin-bottom: 5px;">* 이메일 직접 문의</div>
                    <a href="mailto:koreabestwork@gmail.com" style="color: var(--accent); text-decoration: none; font-size: 18px; font-weight: 700;">koreabestwork@gmail.com</a>
                </div>
            </div>
            <div class="social-links">
                <a href="https://www.instagram.com/best_work_korea/" target="_blank" aria-label="BEST WORK Instagram">
                    <i class="fab fa-instagram"></i>
                </a>
                <a href="https://www.facebook.com/best.work.365125/" target="_blank" aria-label="BEST WORK Facebook">
                    <i class="fab fa-facebook-f"></i>
                </a>
            </div>
            
            <p class="muted" data-lang-key="contact_hours" style="margin-top: 30px; font-size: 14px;">(상담 시간: 평일 09:00 ~ 18:00 KST)</p>
        </div>
    </section>

    <footer>
        <div class="container">
            <div style="font-weight:800;font-size:18px">BEST WORK</div>
            <div class="muted" data-lang-key="footer_line1" style="margin-top:6px">외국인 유학생 및 취업 컨설팅 | 한국 정착 파트너</div>
            <div data-lang-key="footer_line2" style="margin-top:12px;font-size:14px">&copy; 2025 BEST WORK. 모든 권리 보유.</div>
        </div>
    </footer>

    <script>
        // --- 1. Language Data (KO/EN) ---
        const LANG_DATA = {
            ko: {
                // Meta
                meta_title: "BEST WORK - 외국인 유학생 및 취업 컨설팅",
                // Navigation
                nav_about: "회사 소개",
                nav_services: "주요 서비스",
                nav_universities: "제휴 대학교",
                nav_countries: "주요 국가",
                nav_contact: "문의하기",
                // Header
                header_tagline: "유학생·취업 외국인의 성공적인 한국 정착을 돕는 파트너",
                header_desc: "글로벌 인재와 기회를 연결하며, 유학 및 취업을 통한 외국인의 성공적인 국내 정착을 지원합니다. 현지 네트워크와 다양한 사업 경험을 바탕으로 대학교 및 기업에 신뢰도 높은 서비스를 제공합니다.",
                header_btn: "자세히 알아보기",
                // About
                about_title: "회사 소개",
                about_subtitle: "글로벌 인재와 한국을 잇는 가장 신뢰받는 가교",
                about_p1: "BEST WORK는 유학과 취업을 통해 **대한민국에 성공적으로 정착**하고자 하는 외국인에게 전문적인 지원을 제공합니다. 단순히 인력을 배치하는 것을 넘어 인재의 **'생애주기(Life Cycle)'**를 관리하는 통합 솔루션입니다.",
                about_p2: "대학에는 **학업 열정이 높은 우수한 학생**을 소개하고, 기업에는 **최고의 외국인 전문 인력**을 지속적으로 공급하여, 한국 사회에 상호 성장을 위한 다리 역할을 수행합니다.",
                about_p3: "현지 국가에 직접 진출하여 서비스업, 유통업 등 다양한 사업을 경험한 노하우가 있습니다. 현지인의 니즈와 상황에 대한 깊은 이해를 바탕으로 가장 신뢰할 수 있는 효과적인 서비스를 제공합니다.",
                // Services
                services_title: "주요 서비스",
                services_desc: "BEST WORK가 제공하는 핵심 솔루션을 확인하세요. 유학 컨설팅부터 비자 프로그램, 취업 연계까지 맞춤형 서비스를 제공합니다.",
                service1_title: "맞춤형 유학 컨설팅",
                service1_desc: "개인의 학업 목표와 적성에 맞춘 최적의 한국 대학 및 전공을 추천하며, 입학 절차 전반에 걸친 밀착 지원을 제공합니다.",
                service2_title: "생애주기 비자 관리",
                service2_desc: "D-2(유학) 비자부터 E-7(전문직) 비자, 영주권까지, 한국 정착에 필요한 비자 전환에 대한 체계적인 로드맵과 준비 지원을 제공합니다.",
                service3_title: "국내 산업 인재 연계",
                service3_desc: "졸업 후 학생들이 한국에서 안정적인 취업에 성공하고 성공적으로 정착할 수 있도록 국내 산업체와의 인력 연계 서비스를 제공합니다.",
                // Universities
                uni_title: "제휴 대학교",
                uni_desc: "BEST WORK가 파트너십을 맺은 국내 유수 대학들로, 외국인 유학생에게 최적의 학업 환경을 제공합니다.",
                uni1_title: "건국대학교",
                uni1_desc: "서울 광진구에 위치한 명문 사립대학입니다. 생명과학, 공학, 경영 등 다양한 분야에서 우수성을 인정받으며, 활발한 국제 교류 프로그램으로 외국인 학생들에게 인기가 높습니다.",
                uni2_title: "숙명여자대학교",
                uni2_desc: "대한민국 최초의 민족 사립학교 중 하나로, 여성 리더 양성의 요람으로 불립니다. IT, 인문, 사회과학, 약학 등의 분야에 강하며, 서울 용산 지역에 위치하여 접근성이 좋습니다.",
                uni3_title: "한라대학교",
                uni3_desc: "강원도 원주에 위치한 산학협력 중심 대학입니다. 공학 및 디자인 분야에 특화되어 있으며, 지역 산업과 연계된 실용적인 교육을 제공하고 있습니다.",
                uni4_title: "상지대학교",
                uni4_desc: "한의학, 보건복지, 예술 분야에서 높은 경쟁력을 갖춘 대학입니다. 강원 지역의 전통 있는 교육기관으로, 인성 함양과 전문성 강화에 집중하고 있습니다.",
                uni5_title: "송호대학교",
                uni5_desc: "강원도 횡성에 위치한 전문대학으로, 실무 중심의 직업 교육을 통해 현장에 바로 투입 가능한 인재를 양성합니다. 국제 교류 협력을 통해 외국인 학생 유치에 적극적입니다.",
                uni6_title: "서울신학대학교",
                uni6_desc: "기독교 정신을 바탕으로 인성과 전문성을 겸비한 글로벌 인재를 육성합니다. 인문, 사회과학, 신학 분야의 심도 있는 학문을 제공하며, 경기도 부천에 위치하고 있습니다.",
                // Countries
                country_title: "주요 국가",
                country_desc: "BEST WORK는 현지 네트워크를 기반으로 다음과 같은 주요 국가에서 한국 유학 및 취업을 희망하는 우수 인재를 체계적으로 발굴하고 지원합니다.",
                country1_title: "네팔",
                country1_desc: "높은 학구열과 성실함을 자랑하는 인재의 보고입니다. 한국과의 근로자 및 유학생 교류가 오래전부터 활발했으며, 농업 및 제조업 분야에서 한국 경제에 기여하고 있습니다.",
                country2_title: "방글라데시",
                country2_desc: "젊고 역동적인 인구가 풍부한 활기찬 시장입니다. 한국과의 경제 협력이 확대되고 있으며, 특히 섬유 및 제조업 분야에서 유학 후 취업을 희망하는 인재가 늘고 있습니다.",
                country3_title: "미얀마",
                country3_desc: "풍부한 자원과 경제 발전 잠재력을 가진 동남아시아의 전략적 거점입니다. 한국 유학에 대한 관심이 급증하고 있으며, 한국 정착을 희망하는 우수 인재를 발굴합니다.",
                country4_title: "스리랑카",
                country4_desc: "높은 문해율과 교육 수준을 자랑하는 인도양의 섬나라입니다. IT 및 공학 등 전문 분야에서 한국 대학 및 기업을 목표로 하는 인재들이 많습니다.",
                country5_title: "베트남",
                country5_desc: "한국과의 교류가 가장 활발한 핵심 거점 국가입니다. 근로자 파견(E-7 비자) 및 현지 사업 경험을 바탕으로 유학생 모집과 취업 연계에 독보적인 노하우를 보유하고 있습니다.",
                // Contact
                contact_title: "문의하기",
                contact_desc: "BEST WORK와 함께 한국에서의 성공적인 유학 및 정착 여정을 시작하세요. 아래 양식을 작성해 주시면 전문 컨설턴트가 신속하게 답변드리겠습니다.",
                form_name_label: "이름",
                form_name_placeholder: "성함 또는 회사명",
                form_email_label: "이메일 주소",
                form_email_placeholder: "example@email.com",
                form_message_label: "문의 내용",
                form_message_placeholder: "문의 내용을 상세하게 작성해 주세요. (예: [회사/대학명] 제휴 문의)",
                form_submit_btn: "문의 접수",
                submit_success: (name) => `✅ 감사합니다, ${name}님! 문의가 성공적으로 접수되었습니다. 최대한 빠르게 답변드리겠습니다.`,
                submit_error: "❗ 필수 정보를 모두 입력해 주세요.",
                contact_email_direct: "* 이메일 직접 문의",
                contact_hours: "(상담 시간: 평일 09:00 ~ 18:00 KST)",
                // Footer
                footer_line1: "외국인 유학생 및 취업 컨설팅 | 한국 정착 파트너",
                footer_line2: "&copy; 2025 BEST WORK. 모든 권리 보유.",
            },
            en: {
                // Meta
                meta_title: "BEST WORK - Foreign Student and Employment Consulting",
                // Navigation
                nav_about: "About Us",
                nav_services: "Key Services",
                nav_universities: "Partner Universities",
                nav_countries: "Key Countries",
                nav_contact: "Contact",
                // Header
                header_tagline: "The Partner Supporting Foreign Students and Workers Settle in Korea",
                header_desc: "We connect global talent with opportunities, helping foreign nationals successfully settle in South Korea through studying and employment. We leverage our on-the-ground network and diverse business experience to provide reliable services to universities and companies.",
                header_btn: "Learn More",
                // About
                about_title: "ABOUT US",
                about_subtitle: "The Most Reliable Bridge Connecting Global Talent and Korea",
                about_p1: "BEST WORK provides professional support to foreign nationals seeking **successful settlement in South Korea** through study and employment. This is an integrated solution that manages the **'Life Cycle'** of talent, going beyond simple placement.",
                about_p2: "We introduce **excellent students passionate about academics** to universities and continuously supply **top foreign professionals** to companies, acting as a bridge for mutual growth within Korean society.",
                about_p3: "We have direct experience in overseas business, including service and distribution sectors in local countries. This deep understanding of local needs and situations allows us to provide the most trustworthy and effective service.",
                // Services
                services_title: "Key Services",
                services_desc: "Explore the core solutions provided by BEST WORK. We offer customized services spanning study abroad consulting, visa programs, and employment linkage.",
                service1_title: "Customized Study Abroad Consulting",
                service1_desc: "We recommend the optimal Korean university and major tailored to individual academic goals and aptitude, providing close support throughout the admission process.",
                service2_title: "Life Cycle Visa Management",
                service2_desc: "From D-2 (Student) to E-7 (Professional) visas and permanent residency, we provide a systematic roadmap and preparation support for visa transitions necessary for settlement in Korea.",
                service3_title: "Local Industry Talent Connection",
                service3_desc: "We connect students with local industries, helping them secure stable employment and settle successfully in Korea after graduation.",
                // Universities
                uni_title: "Partner Universities",
                uni_desc: "These are the leading Korean universities that BEST WORK partners with, providing optimal academic environments for foreign students.",
                uni1_title: "Konkuk University",
                uni1_desc: "A prestigious private university located in Gwangjin-gu, Seoul. It is recognized for excellence in various fields like life sciences, engineering, and business, and is popular among foreign students for its active international exchange programs.",
                uni2_title: "Sookmyung Women's University",
                uni2_desc: "One of South Korea's first national private schools, known as a cradle for female leaders. It is strong in IT, humanities, social sciences, and pharmacy, and its location in the Yongsan area of Seoul offers good accessibility.",
                uni3_title: "Halla University",
                uni3_desc: "A university focused on industry-academia cooperation, located in Wonju, Gangwon-do. It specializes in engineering and design fields and provides practical education linked to local industries.",
                uni4_title: "Sangji University",
                uni4_desc: "A university with high competitiveness in oriental medicine, public health and welfare, and the arts. It is a traditional educational institution in the Gangwon region, focusing on character development and professional enhancement.",
                uni5_title: "Songho University",
                uni5_desc: "A technical college located in Hoengseong, Gangwon-do, training talents who can be immediately placed in the field through practical, job-oriented education. It is proactive in attracting foreign students through international exchange cooperation.",
                uni6_title: "Seoul Theological University",
                uni6_desc: "Fosters global talent with character and expertise based on Christian principles. It offers in-depth studies in humanities, social sciences, and theology, and is located in Bucheon, Gyeonggi-do.",
                // Countries
                country_title: "Key Countries",
                country_desc: "Based on our local networks, BEST WORK systematically discovers and supports excellent talent from the following key countries for study and employment in Korea.",
                country1_title: "Nepal",
                country1_desc: "A source of talented individuals known for high educational zeal and diligence. Exchange of workers and students with Korea has been active for a long time, contributing to the Korean economy in agriculture and manufacturing sectors.",
                country2_title: "Bangladesh",
                country2_desc: "A vibrant market with a rich, young, and dynamic population. Economic cooperation with Korea is expanding, and there is a growing trend of talented individuals seeking post-study employment, especially in the textile and manufacturing sectors.",
                country3_title: "Myanmar",
                country3_desc: "A strategic hub in Southeast Asia with abundant resources and economic development potential. Interest in studying in Korea is rapidly increasing, and we discover excellent talent aspiring to settle in Korea.",
                country4_title: "Sri Lanka",
                country4_desc: "An island nation in the Indian Ocean boasting a high literacy rate and education level. Many talented individuals aim for Korean universities and companies in specialized fields such as IT and engineering.",
                country5_title: "Vietnam",
                country5_desc: "A core base country with the most active exchange with Korea. Based on experience in labor dispatch (E-7 visa) and local business, we possess unique know-how in student recruitment and employment linkage.",
                // Contact
                contact_title: "Contact Us",
                contact_desc: "Start your successful study and settlement journey in Korea with BEST WORK. Please fill out the form below, and a professional consultant will respond promptly.",
                form_name_label: "Name",
                form_name_placeholder: "Your Name or Company Name",
                form_email_label: "Email Address",
                form_email_placeholder: "example@email.com",
                form_message_label: "Message",
                form_message_placeholder: "Please write your inquiry in detail. (e.g., [Company/University Name] Partnership Inquiry)",
                form_submit_btn: "Submit Inquiry",
                submit_success: (name) => `✅ Thank you, ${name}! Your inquiry has been successfully submitted. We will reply as soon as possible.`,
                submit_error: "❗ Please fill in all required information.",
                contact_email_direct: "* Contact directly via Email",
                contact_hours: "(Consultation Hours: Weekdays 09:00 ~ 18:00 KST)",
                // Footer
                footer_line1: "Foreign Student and Employment Consulting | Settlement Partner in Korea",
                footer_line2: "&copy; 2025 BEST WORK. All rights reserved.",
            }
        };

        // --- 2. Language Switching Logic ---
        function setLanguage(langCode) {
            const data = LANG_DATA[langCode];
            if (!data) return;

            // 1. Update all elements with data-lang-key
            document.querySelectorAll('[data-lang-key]').forEach(el => {
                const key = el.getAttribute('data-lang-key');
                let text = data[key];

                if (text) {
                    // Handle dynamic text (e.g., footer)
                    if (key === 'footer_line2' && langCode === 'ko') {
                        // Footer line 2 already contains the full HTML entity in KO, so we use innerHTML
                        el.innerHTML = text;
                    } else if (key.startsWith('meta_')) {
                        // Special handling for meta_title (for the document.title)
                        document.title = text;
                    } else {
                        // Standard text update
                        el.innerHTML = text;
                    }

                    // Handle placeholder/aria-label attributes
                    const attrKey = el.getAttribute('data-lang-attr');
                    if (attrKey && data[key]) {
                        // Check if the text content is a function (like submit_success)
                        if (typeof text === 'function') {
                            // Do nothing for functions here, they are handled during form submission
                        } else {
                            el.setAttribute(attrKey, text);
                        }
                    }
                }
            });

            // 2. Update <html> language attribute
            document.documentElement.lang = langCode;
            document.body.setAttribute('data-lang', langCode);

            // 3. Update active button state (Desktop & Mobile)
            document.querySelectorAll('.lang-btn, [data-mobile-lang-btn]').forEach(btn => {
                btn.classList.remove('active');
                if (btn.getAttribute('data-lang-code') === langCode) {
                    btn.classList.add('active');
                }
            });
            
            // 4. Save preference to localStorage
            localStorage.setItem('preferredLang', langCode);
            
            // 5. Update slider buttons immediately after language switch
            updateSliderButtonAriaLabels(langCode);
            
            // 6. Update burger menu aria-label
            const burgerBtn = document.getElementById('burger-menu-btn');
            if (burgerBtn) {
                burgerBtn.setAttribute('aria-label', langCode === 'ko' ? '메뉴 열기' : 'Open menu');
            }
        }
        
        // Helper function for slider button labels
        function updateSliderButtonAriaLabels(langCode) {
            const prevButton = document.getElementById('prev-button');
            const nextButton = document.getElementById('next-button');
            if (prevButton && nextButton) {
                if (langCode === 'ko') {
                    prevButton.setAttribute('aria-label', '이전 이미지');
                    nextButton.setAttribute('aria-label', '다음 이미지');
                } else {
                    prevButton.setAttribute('aria-label', 'Previous image');
                    nextButton.setAttribute('aria-label', 'Next image');
                }
            }
        }
        
        // --- 3. Mobile Menu Toggle Logic ---
        function toggleMobileMenu() {
            const menu = document.getElementById('mobile-menu');
            const burger = document.getElementById('burger-menu-btn');
            const isMenuOpen = menu.classList.toggle('open');
            
            // Change burger icon based on state
            if (burger) {
                burger.innerHTML = isMenuOpen ? '<i class="fas fa-times"></i>' : '<i class="fas fa-bars"></i>';
                burger.setAttribute('aria-label', isMenuOpen ? '메뉴 닫기' : '메뉴 열기');
            }
            
            // Prevent scrolling on body when mobile menu is open
            document.body.style.overflowY = isMenuOpen ? 'hidden' : 'auto';
        }


        // --- 4. Initial Load and Event Listeners ---
        document.addEventListener('DOMContentLoaded', () => {
            // Slider logic (retained from previous version)
            const sliderWrapper = document.getElementById('university-slider-wrapper');
            const slides = sliderWrapper ? sliderWrapper.querySelectorAll('.slide') : [];
            const totalSlides = slides.length;
            const prevButton = document.getElementById('prev-button');
            const nextButton = document.getElementById('next-button');
            let currentSlide = 0;
            let slideInterval;
            
            function updateSlider() {
                if (!sliderWrapper) return;
                const offset = -currentSlide * 100;
                sliderWrapper.style.transform = `translateX(${offset}%)`;
            }

            function nextSlide() { currentSlide = (currentSlide + 1) % totalSlides; updateSlider(); }
            function prevSlide() { currentSlide = (currentSlide - 1 + totalSlides) % totalSlides; updateSlider(); }
            
            if (prevButton && nextButton) {
                prevButton.addEventListener('click', prevSlide);
                nextButton.addEventListener('click', nextSlide);
            }
            if (totalSlides > 0) {
                updateSlider();
            }
            slideInterval = setInterval(nextSlide, 5000); 

            const sliderContainer = document.querySelector('.slider-container');
            if (sliderContainer) {
                sliderContainer.addEventListener('mouseenter', () => clearInterval(slideInterval));
                sliderContainer.addEventListener('mouseleave', () => {
                    slideInterval = setInterval(nextSlide, 5000);
                });
            }
            
            // Smooth Scrolling Logic
            const navHeight = 60; 
            const headerOffset = navHeight + 20; 

            // Desktop Links
            document.querySelectorAll('.navbar-links a, .btn').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('href');
                    const targetElement = document.querySelector(targetId);

                    if (targetElement) {
                        let targetPosition;
                        if (targetId === '#home') {
                            targetPosition = 0; 
                        } else {
                            // Subtract headerOffset to account for fixed navbar height
                            targetPosition = targetElement.offsetTop - headerOffset;
                        }
                        
                        window.scrollTo({ top: targetPosition, behavior: 'smooth' });
                    }
                });
            });
            
            // Mobile Links - closes menu after click
            document.querySelectorAll('[data-mobile-link]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    toggleMobileMenu(); // Close mobile menu
                    
                    const targetId = this.getAttribute('href');
                    const targetElement = document.querySelector(targetId);

                    if (targetElement) {
                        let targetPosition;
                        if (targetId === '#home') {
                            targetPosition = 0; 
                        } else {
                            targetPosition = targetElement.offsetTop - headerOffset;
                        }
                        
                        // Small timeout to ensure menu is closed before scroll animation starts
                        setTimeout(() => {
                            window.scrollTo({ top: targetPosition, behavior: 'smooth' });
                        }, 100); 
                    }
                });
            });
            
            // Burger Menu Listener
            document.getElementById('burger-menu-btn').addEventListener('click', toggleMobileMenu);

            // --- Language Initialization & Listeners ---
            document.querySelectorAll('.lang-btn, [data-mobile-lang-btn]').forEach(btn => {
                btn.addEventListener('click', (e) => {
                    const langCode = e.target.getAttribute('data-lang-code');
                    setLanguage(langCode);
                });
            });

            // Auto-detect and set initial language
            let initialLang = localStorage.getItem('preferredLang');
            
            // If no preferred language is stored, check browser language
            if (!initialLang) {
                const browserLang = navigator.language.split('-')[0].toLowerCase();
                if (browserLang === 'ko') {
                    initialLang = 'ko';
                } else if (browserLang === 'en') {
                    initialLang = 'en';
                } else {
                    // Default to Korean if browser language is neither KO nor EN
                    initialLang = 'ko';
                }
            }

            setLanguage(initialLang);
        });

        // Form Submission Handler (Updated for multilingual support)
        function handleFormSubmit(e) {
            e.preventDefault();
            
            const name = document.getElementById('name').value;
            const email = document.getElementById('email').value;
            const message = document.getElementById('message').value;

            const submitMessageDiv = document.getElementById('submit-message');
            const currentLang = document.body.getAttribute('data-lang');
            const lang = LANG_DATA[currentLang];

            // Simple validation
            if (!name || !email || !message) {
                submitMessageDiv.style.background = '#ffe6e6';
                submitMessageDiv.style.color = '#cc0000';
                submitMessageDiv.textContent = lang.submit_error;
                submitMessageDiv.style.display = 'block';
                return;
            }

            // Simulate successful submission (as there is no backend)
            submitMessageDiv.style.background = '#e6f3ff';
            submitMessageDiv.style.color = 'var(--accent)';
            // Use the dynamic string function (lang.submit_success is a function)
            submitMessageDiv.textContent = lang.submit_success(name);
            document.getElementById('contact-form').style.display = 'none'; // Hide form
            submitMessageDiv.style.display = 'block';
            
            // Clear form and display it again after a delay
            setTimeout(() => {
                document.getElementById('contact-form').reset();
                submitMessageDiv.style.display = 'none';
                document.getElementById('contact-form').style.display = 'block';
            }, 5000);
        }
    </script>
</body>
</html>
