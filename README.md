<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title id="title-text">BEST WORK | Join The Best, Be The Best</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        /* 기본 스타일 및 초기화 */
        body { font-family: 'Malgun Gothic', '맑은 고딕', sans-serif; margin: 0; padding: 0; background-color: #f4f4f4; color: #333; line-height: 1.6; }
        .container { 
            width: 100%; max-width: 600px; margin: 0 auto; background-color: #fff; box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); 
            padding-top: 50px; 
        }
        
        /* ---------------------------------------------------- */
        /* 헤더 (회사 이름 및 언어 선택) */
        /* ---------------------------------------------------- */
        header { 
            background-color: #004d99; color: white; padding: 10px 15px; text-align: center; 
            position: fixed; top: 0; left: 0; right: 0; z-index: 2000; max-width: 600px; margin: 0 auto;
            display: flex; justify-content: space-between; align-items: center; 
        }
        header h1 { margin: 0; font-size: 1.5em; text-align: left; }
        .header-controls { display: flex; align-items: center; }

        /* 언어 선택 버튼 */
        .lang-switch button {
            background-color: #0066cc; color: white; border: 1px solid white; padding: 5px 8px;
            cursor: pointer; font-size: 0.7em; margin-left: 5px; border-radius: 5px; transition: background-color 0.3s;
        }
        .lang-switch button.active { background-color: #ff9900; } 
        
        /* ---------------------------------------------------- */
        /* 1. BEST WORK 섹션 (GIF 배경 및 우측 상단 세로 메뉴) */
        /* ---------------------------------------------------- */
        #home {
            padding-left: 0; padding-right: 0;
            height: 50vh; 
            /* 내부 콘텐츠 중앙 정렬 (h2, p) */
            display: flex; justify-content: center; align-items: center; flex-direction: column;
            text-align: center; border-bottom: none;
            
            background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/Adobe%20Express%20-%20IMG_8171%20(1).gif?raw=true');
            background-size: cover; background-position: center; background-repeat: no-repeat;
            position: relative; /* 메뉴의 absolute 위치 기준점 */
        }
        /* #home::before {
            content: ''; position: absolute; top: 0; left: 0; right: 0; bottom: 0;
            background-color: rgba(0, 0, 0, 0.3); z-index: 1; 
        } */ 
        #home h2 { color: white; border-bottom: none; z-index: 2; margin-bottom: 10px;
            font-size: 1.8em; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
        }
        #home .section-content { color: white; padding: 0 20px; z-index: 2; }
        #home .section-content p { margin: 0; font-size: 1.1em; font-weight: 500; text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.8); }

        /* 인라인 메뉴 스타일 (세로 배치 및 박스 제거) */
        .main-nav-inline {
            z-index: 3; 
            position: absolute; /* 절대 위치 지정 */
            top: 15px; /* 상단에서 15px 떨어진 위치 */
            right: 15px; /* 우측에서 15px 떨어진 위치 */
            display: flex;
            flex-direction: column; /* 세로로 배치 */
            align-items: flex-end; /* 메뉴 항목을 우측 정렬 */
        }
        .main-nav-inline a {
            color: white; 
            text-decoration: none;
            font-weight: 600;
            padding: 3px 0; /* 상하 여백만 부여 (좌우 여백 제거) */
            margin: 3px 0; /* 세로 간격 확보 */
            font-size: 0.9em;
            transition: color 0.3s;
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.9); /* 글자 가시성 확보 */
            /* 네모 박스 스타일 제거 */
            border: none;
            background-color: transparent;
        }
        .main-nav-inline a:hover {
            color: #ff9900; /* 호버 시 주황색 텍스트로 변경 */
            background-color: transparent;
        }
        
        /* ---------------------------------------------------- */
        /* 섹션 공통 및 회사소개 카드 스타일 */
        /* ---------------------------------------------------- */
        section { padding: 20px 15px; border-bottom: 1px solid #eee; }
        section h2 { color: #004d99; border-bottom: 2px solid #004d99; padding-bottom: 5px; font-size: 1.3em; margin-top: 0; }
        
        /* 회사소개 카드 공통 스타일 */
        .card-container { margin-top: 15px; }
        .info-card {
            /* 모든 카드를 동일한 기본 스타일로 통일 */
            border: 1px solid #ddd;
            border-radius: 8px;
            padding: 20px; 
            margin-bottom: 15px;
            background-color: #f9f9f9;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.05);
            transition: transform 0.2s;
        }
        .info-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
        }
        /* 카드 제목 스타일 통일: 파란색 테마 */
        .info-card .card-title {
            font-size: 1.2em;
            font-weight: bold;
            margin-top: 0;
            margin-bottom: 10px;
            color: #004d99; /* 통일된 파란색 */
            border-bottom: 2px solid #0066cc; /* 제목 아래 구분선 추가 */
            padding-bottom: 5px;
        }
        /* 카드 제목 아이콘 색상 통일 (Vision, Mission 아이콘 모두 파란색) */
        .info-card .card-title i {
            margin-right: 8px;
            color: #0066cc;
        }

        /* 주요 사업 리스트 점 제거 */
        ul.no-bullet-list { list-style: none; padding-left: 0; }
        ul.no-bullet-list li { margin-bottom: 5px; } /* 리스트 간격 조정 */


        /* ---------------------------------------------------- */
        /* 2. 서비스 섹션 배경 이미지 및 텍스트 스타일 (밝게, 깔끔하게 수정됨) */
        /* ---------------------------------------------------- */
        #services {
            padding-left: 0; padding-right: 0; 
            height: auto; 
            min-height: 80vh; 
            
            background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/IMG_8690.gif?raw=true');
            background-size: cover;
            background-position: center;
            background-repeat: no-repeat;
            position: relative;
            display: flex; 
            flex-direction: column;
            justify-content: center; 
            align-items: center; 
            text-align: center;
        }
        /* 밝고 깔끔한 디자인을 위해 오버레이 밝기 조정 (0.5 -> 0.2) */
        #services::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background-color: rgba(0, 0, 0, 0.2); /* 어두운 오버레이를 훨씬 밝게 조정 */
            z-index: 1;
        }
        #services h2, #services .section-content {
            z-index: 2; 
            color: white; /* h2는 흰색 유지 */
            padding: 0 15px; 
            max-width: 600px; 
            width: 100%;
            box-sizing: border-box; 
        }
        #services h2 {
            border-bottom: 2px solid #ff9900; 
            padding-bottom: 10px;
            font-size: 1.8em;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
            margin-bottom: 20px;
        }
        /* 새로운 서비스 카드 컨테이너 */
        .service-card {
            background-color: rgba(255, 255, 255, 0.95); /* 깔끔한 반투명 흰색 카드 */
            padding: 15px;
            border-radius: 10px;
            margin-bottom: 20px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
            text-align: left;
            transition: transform 0.3s;
            color: #333; /* 텍스트 색상을 어둡게 */
        }
        .service-card:hover {
            transform: translateY(-3px);
        }

        .service-card .item-title {
            color: #004d99; /* 제목 색상 강조 (다크 블루) */
            font-size: 1.2em;
            font-weight: bold;
            margin-top: 0;
            margin-bottom: 5px;
            border-bottom: 1px dashed #ff9900; /* 주황색 점선 */
            padding-bottom: 5px;
            display: block;
            text-shadow: none;
            text-align: left;
        }
        .service-card p {
            background-color: transparent; /* 이전 배경 제거 */
            padding: 0;
            border-radius: 0;
            margin: 0;
            text-shadow: none;
            color: #333; /* 본문 텍스트 색상 */
        }
        
        /* ---------------------------------------------------- */
        /* 4. 주요 국가 섹션 디자인 */
        /* ---------------------------------------------------- */
        #countries {
            background-color: #e9e9e9;
        }
        .country-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr)); 
            gap: 15px;
            margin-top: 20px;
        }

        .country-card {
            background-color: #ffffff;
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15); 
            transition: transform 0.3s, box-shadow 0.3s;
            border-left: 8px solid #ff9900; 
        }

        .country-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.25);
        }

        .country-card .flag-name {
            font-size: 1.3em;
            font-weight: 800; 
            color: #004d99;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            padding-bottom: 8px;
            border-bottom: 2px solid #eee; 
        }

        .country-card .flag-name span {
            font-size: 2.2em; 
            margin-right: 12px;
            line-height: 1;
        }

        .country-card p {
            font-size: 0.95em;
            color: #333;
            margin: 0;
            text-align: left;
        }
        
        /* ---------------------------------------------------- */
        /* 5. 제휴 대학 섹션 디자인 (롤링 배너 및 카드) */
        /* ---------------------------------------------------- */
        #universities {
            background-color: #f8f8f8; 
            padding-left: 0;
            padding-right: 0;
        }
        #universities h2 {
            padding: 0 15px 5px 15px; /* 제목 좌우 패딩만 추가 */
            margin-bottom: 15px;
        }

        /* 슬라이드쇼 컨테이너 - 높이 확장: 200px -> 300px */
        .university-carousel-wrapper {
            position: relative;
            width: 100%;
            height: 300px; /* 높이 고정 (확장) */
            overflow: hidden;
            margin-bottom: 20px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }

        .university-carousel-item {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-size: cover; /* 배경 이미지 크기 유지 */
            background-position: center;
            transition: opacity 1s ease-in-out;
            opacity: 0; /* 기본적으로 숨김 */
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .university-carousel-item::before {
            content: '';
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            /* 오버레이 색상을 투명도를 낮춰 이미지 선명도 증가 */
            background-color: rgba(0, 77, 153, 0.4); /* Deep Blue overlay (Opacity lowered from 0.7 to 0.4) */
            z-index: 1;
        }

        .university-carousel-item.active {
            opacity: 1;
        }

        #universities-intro-1, #universities-intro-2, #universities-intro-3 {
            color: white;
            font-size: 1.15em; 
            font-weight: 800; 
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.8);
            z-index: 2;
            position: relative;
            margin: 0 20px; /* 텍스트 좌우 여백 */
            text-align: center;
            padding: 5px 10px;
            background-color: rgba(0, 0, 0, 0.3); /* 텍스트 가독성을 위한 배경 추가 */
            border-radius: 5px;
        }

        /* 대학 카드 그리드 */
        .university-content-container {
            padding: 0 15px 20px 15px; /* 섹션 본문 패딩 */
        }

        .university-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); 
            gap: 15px;
            margin-top: 20px;
        }

        .university-card-item {
            background-color: #ffffff;
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
            border: 1px solid #ddd;
            overflow: hidden;
            position: relative;
            border-right: 8px solid #004d99; /* 활동적인 느낌을 주는 강한 오른쪽 경계선 */
        }
        
        /* Image 2 적용: Subtle background texture to the cards */
        .university-card-item.with-texture::after {
            content: '';
            position: absolute;
            top: 0; right: 0; bottom: 0; left: 0;
            background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250812_124606.jpg?raw=true'); 
            background-size: cover;
            opacity: 0.07; 
            z-index: 0;
            pointer-events: none;
        }

        .university-card-item:hover {
            transform: translateY(-8px) scale(1.01); 
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.25);
            border-color: #ff9900; 
        }

        .university-card-item strong {
            display: block;
            font-size: 1.2em;
            color: #004d99; 
            margin-bottom: 10px;
            padding-bottom: 5px;
            border-bottom: 2px dashed #ff9900; 
            position: relative;
            z-index: 1;
        }

        .university-card-item p {
            font-size: 0.95em;
            color: #555;
            margin: 0;
            line-height: 1.5;
            position: relative;
            z-index: 1;
        }

        /* 기타 섹션 스타일 및 데스크탑 뷰 */
        ul.styled-list { display: none; } 

        .contact-info a { color: #0066cc; text-decoration: none; word-break: break-all; }
        .social-links { text-align: center; margin-top: 20px; }
        .social-links a { color: #004d99; font-size: 2em; margin: 0 10px; transition: color 0.3s; }
        footer { text-align: center; font-size: 0.7em; color: #777; padding: 10px; }

        /* Form Styles (Inline) */
        .form-group {
            margin-bottom: 15px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
            color: #333;
        }

        .form-group input, .form-group select, .form-group textarea {
            width: 100%;
            padding: 10px;
            border: 1px solid #ddd;
            border-radius: 5px;
            box-sizing: border-box;
            font-size: 1em;
            font-family: inherit;
        }

        .form-group textarea {
            resize: vertical;
        }

        #c-submit-btn {
            width: 100%;
            background-color: #0066cc;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1em;
            font-weight: bold;
            margin-top: 10px;
            transition: background-color 0.3s;
        }

        #c-submit-btn:hover {
            background-color: #004d99;
        }

        @media (min-width: 601px) {
            header { position: static; max-width: none; justify-content: flex-start; }
            .header-controls { display: flex; margin-left: auto; }
            #services {
                background-attachment: fixed; 
            }
            .country-grid, .university-grid {
                grid-template-columns: repeat(2, 1fr); 
            }
            .university-carousel-wrapper {
                 height: 400px; /* 데스크탑에서 더 크게 */
            }
        }
    </style>
</head>
<body>

<div class="container">

    <header>
        <h1 id="header-h1">BEST WORK</h1>
        <div class="header-controls">
            <div class="lang-switch">
                <button id="lang-ko" onclick="setLanguage('ko')" class="active">KOR</button>
                <button id="lang-en" onclick="setLanguage('en')">ENG</button>
            </div>
        </div>
    </header>

    <section id="home">
        <h2 id="section-home-h2">BEST WORK</h2>
        
        <div class="main-nav-inline" id="main-nav-wrapper-inline">
            </div>

        <div class="section-content">
            <p id="home-intro"></p>
        </div>
    </section>

    <section id="about">
        <h2 id="section-about-h2">회사소개</h2>
        
        <p style="text-align: center; margin-top: 10px; margin-bottom: 20px;">
            <img src="https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250308_150855_1741415133899.JPG?raw=true" alt="BEST WORK Office and People" style="width: 100%; height: auto; border-radius: 8px; box-shadow: 0 4px 8px rgba(0,0,0,0.1);">
        </p>

        <p id="about-core-values-intro" style="text-align: center; margin-top: 20px;">
        </p>
        
        <div class="card-container">
            
            <div class="info-card">
                <h3 class="card-title" id="about-vision-title">
                    <i class="fas fa-eye"></i> VISION
                </h3>
                <p id="about-vision"></p>
            </div>

            <div class="info-card">
                <h3 class="card-title" id="about-mission-title">
                    <i class="fas fa-bullseye"></i> MISSION
                </h3>
                <p id="about-mission"></p>
            </div>

            <div class="info-card">
                <h3 class="card-title" id="about-business-title">
                    <i class="fas fa-handshake"></i> 주요 사업
                </h3>
                <ul class="no-bullet-list" id="about-business-list"></ul>
            </div>
        </div>
    </section>

    <section id="services">
        <h2 id="section-services-h2">서비스 (What We Do?)</h2>
        <div class="section-content">
            
            <div class="service-card">
                <p id="service-consulting-title" class="item-title"></p>
                <p id="service-consulting-content"></p>
            </div>
            
            <div class="service-card">
                <p id="service-visa-title" class="item-title"></p>
                <p id="service-visa-content"></p>
            </div>

            <div class="service-card">
                <p id="service-job-title" class="item-title"></p>
                <p id="service-job-content"></p>
            </div>
            
        </div>
    </section>
    <section id="countries">
        <h2 id="section-countries-h2">주요 국가 🌍</h2>
        <div class="section-content">
            <p id="countries-intro"></p>
            <div class="country-grid" id="countries-grid">
            </div>
        </div>
    </section>

    <section id="universities">
        <h2 id="section-universities-h2">제휴 대학 🎓</h2>
        <div class="university-carousel-wrapper">
            <div class="university-carousel-item active" style="background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/IMG_8696.jpg?raw=true');">
                <p id="universities-intro-1"></p>
            </div>
            <div class="university-carousel-item" style="background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250812_124606.jpg?raw=true');">
                <p id="universities-intro-2"></p>
            </div>
            <div class="university-carousel-item" style="background-image: url('https://github.com/BEST-WORK/BESTWORK/blob/main/Resized_20250308_150855_1741415133899.JPG?raw=true');">
                <p id="universities-intro-3"></p>
            </div>
        </div>
        
        <div class="university-content-container">
            <div class="university-grid" id="universities-grid">
                </div>
        </div>
    </section>
    
    <section id="contact">
        <h2 id="section-contact-h2">Contact</h2>
        <div class="section-content contact-info">
            <p id="contact-email"></p>
            <p id="contact-address"></p>

            <div style="margin-top: 25px; border-top: 1px solid #ddd; padding-top: 15px;">
                <h3 id="modal-title" style="color: #004d99; border-bottom: 2px solid #ff9900; padding-bottom: 5px; margin-top: 0; margin-bottom: 20px; text-align: center; font-size: 1.3em;">1:1 상담 신청</h3>
                <form id="consultation-form">
                    <div class="form-group">
                        <label for="c-name" id="c-name-label">이름:</label>
                        <input type="text" id="c-name" name="name" required placeholder="이름을 입력해주세요">
                    </div>
                    <div class="form-group">
                        <label for="c-contact" id="c-contact-label">연락처:</label>
                        <input type="tel" id="c-contact" name="contact" required placeholder="010-XXXX-XXXX">
                    </div>
                    <div class="form-group">
                        <label for="c-email" id="c-email-label">이메일:</label>
                        <input type="email" id="c-email" name="email" required placeholder="example@email.com">
                    </div>
                    <div class="form-group">
                        <label for="c-topic" id="c-topic-label">상담 분야:</label>
                        <select id="c-topic" name="topic" required>
                            <option value="" disabled selected>상담 분야를 선택해주세요</option>
                            <option value="유학생_유치">유학생 유치</option>
                            <option value="인력_공급">인력 공급 (E-7 비자)</option>
                            <option value="비자_문의">비자 관련 문의 (D2, D4, F2 등)</option>
                            <option value="기타">기타 문의</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label for="c-content" id="c-content-label">상세 내용:</label>
                        <textarea id="c-content" name="content" rows="4" required placeholder="상담 내용을 자세히 적어주세요"></textarea>
                    </div>
                    <button type="submit" id="c-submit-btn">상담 신청 완료</button>
                </form>
                <p id="c-note" style="font-size: 0.8em; color: #777; margin-top: 10px; text-align: center;">신청해주시면 빠르게 연락드리겠습니다.</p>
            </div>

            <div class="social-links">
                <a href="https://www.facebook.com/best.work.365125/" target="_blank" title="Facebook"><i class="fab fa-facebook-square"></i></a>
                <a href="https://www.instagram.com/best_work_korea/" target="_blank" title="Instagram"><i class="fab fa-instagram-square"></i></a>
            </div>
        </div>
    </section>
    
    <footer>
        <p id="footer-text">&copy; 2025 BEST WORK All rights reserved.</p>
    </footer>

</div>

<script>
    // --- 1. 언어별 콘텐츠 데이터 (메뉴 항목 키/ID를 포함) ---
    const translations = {
        'ko': {
            // 메뉴 항목 (키는 HTML ID 접두사, 값은 표시 텍스트)
            'nav_items': [
                { id: 'home', text: 'BEST WORK' },
                { id: 'about', text: '회사소개' },
                { id: 'services', text: '서비스' },
                { id: 'countries', text: '주요 국가' },
                { id: 'universities', text: '제휴 대학' },
                { id: 'contact', text: 'Contact' }
            ],
            // 메타 & 헤더
            'title-text': 'BEST WORK | Join The Best, Be The Best',
            'header-h1': 'BEST WORK',

            // BEST WORK (HOME)
            'section-home-h2': 'BEST WORK',
            'home-intro': 'BEST WORK는 외국인이 유학과 취업을 통해 대한민국에 정착할 수 있도록 지원하며, 외국인과 대한민국의 가교 역할로 함께 성장하는 미래를 만들어갑니다.',

            // 회사소개 (비전/미션 분리)
            'section-about-h2': '회사소개',
            'about-core-values-intro': 'BEST WORK의 핵심 가치 (비전, 미션, 주요 사업)', // 핵심 가치 문구 
            'about-vision-title': 'VISION',
            'about-vision': 'Best Person, Best Position, Best Time (최고의 인재를, 최고의 자리에, 최고의 타이밍에 배치합니다)',
            'about-mission-title': 'MISSION',
            'about-mission': 'Transform businesses through a best recruitment experience (최고의 인재 영입으로 사업을 변화시키자)',
            'about-business-title': '주요 사업',
            // 주요 사업 리스트
            'about-business-list': [
                '대학교에는 학업에 열정적인 유학생을, 기업에는 우수한 인재를 지속적으로 공급합니다.', // 이 항목이 동적으로 번역됩니다.
            ],

            // 서비스 (수정된 3개 항목)
            'section-services-h2': '서비스 (What We Do?)',
            'service-consulting-title': '맞춤형 유학 컨설팅',
            'service-consulting-content': '개인의 학업 목표와 적성에 맞춘 최적의 한국 대학 및 전공을 추천하며, 입학 절차 전반에 걸친 밀착 지원을 제공합니다.',
            'service-visa-title': '생애주기 비자 관리',
            'service-visa-content': 'D-2(유학) 비자부터 E-7(전문직) 비자, 영주권까지, 한국 정착에 필요한 비자 전환에 대한 체계적인 로드맵과 준비 지원을 제공합니다.',
            'service-job-title': '국내 산업 인재 연계',
            'service-job-content': '졸업 후 학생들이 한국에서 안정적인 취업에 성공하고 성공적으로 정착할 수 있도록 국내 산업체와의 인력 연계 서비스를 제공합니다.',
            

            // 주요 국가 (국기 추가됨)
            'section-countries-h2': '주요 국가 🌍',
            'countries-intro': 'BEST WORK는 아래 국가들과 긴밀한 관계를 맺고 유학생 및 근로자 공급 서비스를 제공합니다.',
            'countries-data': [
                { name: '네팔 (Nepal)', flag: '🇳🇵', desc: '고용허가제(EPS)를 통해 많은 근로자가 한국 경제에 기여하고 있으며, 한국과의 개발 협력도 활발한 주요 파트너입니다.' },
                { name: '방글라데시 (Bangladesh)', flag: '🇧🇩', desc: '한국과는 1973년 수교를 맺었으며, 만 명 이상의 근로자들이 한국에 체류하며 경제 교류의 주축을 이루고 있는 주요 인력 공급처입니다.' },
                { name: '스리랑카 (Sri Lanka)', flag: '🇱🇰', desc: '고용허가제(EPS)를 통해 수많은 근로자들이 한국 제조업 등 다양한 분야에서 활동하는 중요한 파트너입니다.' },
                { name: '미얀마 (Myanmar)', flag: '🇲🇲', desc: '한국에 우호적인 관계로 발전했으며, 한류 인기가 높고 신남방정책을 통한 교류 확대가 이어지고 있습니다.' },
                { name: '베트남 (Vietnam)', flag: '🇻🇳', desc: '한국의 주요 무역 상대국 중 하나로, 경제 협력 및 인적 교류가 매우 활발합니다. 한국을 경제 발전 모델로 삼고 있습니다.' },
                { name: '몽골 (Mongolia)', flag: '🇲🇳', desc: '교육 및 근로 목적으로 한국을 찾는 인구가 꾸준히 증가하며 인적 교류가 활발합니다.' }
            ],

            // 제휴 대학
            'section-universities-h2': '제휴 대학 🎓',
            'universities-intro': 'BEST WORK는 아래 대학교들과 유학생 유치를 위해 협력하고 있습니다.',
            'universities-data': [
                { name: '숙명여자대학교', desc: "<strong>'S 리더십'을 갖춘 여성리더 육성</strong>을 목표로 하는 사학으로, 다전공 과정이 유연하며 학생들의 성과가 뛰어납니다." },
                { name: '건국대학교', desc: "(일반 소개): 서울과 충주에 캠퍼스를 둔 사립 종합대학입니다. '창의와 성실'을 교시로 하며, 다양한 학문 분야의 융합과 연구를 통해 국가 및 사회 발전에 기여하고 있습니다." },
                { name: '한라대학교', desc: "<strong>스마트모빌리티융합</strong> 등 특성화 분야를 교육하며, 23개 국제 대학과 학술교류협정을 체결하고 있는 대학입니다." },
                { name: '상지대학교', desc: "(일반 소개): 강원특별자치도 원주시에 위치하며, '경천애인(敬天愛人)'을 건학이념으로 실용적인 인재 양성에 힘쓰고 있습니다." },
                { name: '송호대학교', desc: "<strong>'디지털 헬스케어 전문 인재' 및 '이모빌리티 중심'</strong> 대학을 지향하며, KTX 시대를 맞아 수도권과의 접근성이 우수합니다." },
                { name: '서울신학대학교', desc: "기독교대한성결교회 계열의 대학으로, <strong>'웨슬리안 복음주의'</strong> 전통에 입각하여 기독교 사역자 및 전문인 양성에 중점을 둡니다." }
            ],
            
            // Contact
            'section-contact-h2': 'Contact',
            'contact-email': '<i class="fas fa-envelope"></i> <strong>대표 이메일:</strong> <a href="mailto:koreabestwork@gmail.com">koreabestwork@gmail.com</a>',
            'contact-address': '<i class="fas fa-map-marker-alt"></i> <strong>주소:</strong> 서울특별시 마포구 월드컵로 196', 
            
            // 푸터
            'footer-text': '&copy; 2025 BEST WORK All rights reserved.',
            
            // 폼 요소
            'modal-title': '1:1 상담 신청',
            'c-name-label': '이름:',
            'c-name-placeholder': '이름을 입력해주세요',
            'c-contact-label': '연락처:',
            'c-contact-placeholder': '010-XXXX-XXXX',
            'c-email-label': '이메일:',
            'c-email-placeholder': 'example@email.com',
            'c-topic-label': '상담 분야:',
            'c-topic-option-default': '상담 분야를 선택해주세요',
            'c-topic-option-1': '유학생 유치',
            'c-topic-option-2': '인력 공급 (E-7 비자)',
            'c-topic-option-3': '비자 관련 문의 (D2, D4, F2 등)',
            'c-topic-option-4': '기타 문의',
            'c-content-label': '상세 내용:',
            'c-content-placeholder': '상담 내용을 자세히 적어주세요',
            'c-submit-btn': '상담 신청 완료',
            'c-note': '신청해주시면 빠르게 연락드리겠습니다.',
            'c-alert-success': '상담 신청이 완료되었습니다. 담당자가 곧 연락드리겠습니다.',
        },

        'en': {
            // 메뉴 항목 (키는 HTML ID 접두사, 값은 표시 텍스트)
            'nav_items': [
                { id: 'home', text: 'BEST WORK' },
                { id: 'about', text: 'About Us' },
                { id: 'services', text: 'Services' },
                { id: 'countries', text: 'Key Countries' },
                { id: 'universities', text: 'Partner Univ.' },
                { id: 'contact', text: 'Contact' }
            ],
            // 메타 & 헤더
            'title-text': 'BEST WORK | Join The Best, Be The Best',
            'header-h1': 'BEST WORK',

            // BEST WORK (HOME)
            'section-home-h2': 'BEST WORK',
            'home-intro': 'BEST WORK supports foreigners in settling in South Korea through study and employment, building a future where both foreigners and the Republic of Korea grow together.',

            // 회사소개 (비전/미션 분리)
            'section-about-h2': 'About Us',
            'about-core-values-intro': 'BEST WORK\'s Core Values (Vision, Mission, Core Business)', // 핵심 가치 문구 (영어)
            'about-vision-title': 'VISION',
            'about-vision': 'Best Person, Best Position, Best Time (We place the best talent in the best position at the best time)',
            'about-mission-title': 'MISSION',
            'about-mission': 'Transform businesses through a best recruitment experience',
            'about-business-title': 'Core Business',
            // 주요 사업 리스트
            'about-business-list': [
                'We supply highly motivated international students to universities and continuous excellent talent to corporations.', // 이 항목이 동적으로 번역됩니다.
            ],

            // 서비스 (수정된 3개 항목)
            'section-services-h2': 'Services (What We Do?)',
            'service-consulting-title': 'Customized Study Abroad Consulting',
            'service-consulting-content': 'We recommend the optimal Korean university and major based on individual academic goals and aptitude, providing close support throughout the admission process.',
            'service-visa-title': 'Life Cycle Visa Management',
            'service-visa-content': 'From D-2 (Study) visa to E-7 (Professional) visa and permanent residency, we provide a systematic roadmap and preparation support for visa conversion necessary for settlement in Korea.',
            'service-job-title': 'Domestic Industry Talent Linkage',
            'service-job-content': 'We provide manpower linkage services with domestic industries to help students secure stable employment and successfully settle in Korea after graduation.',
            
            // 주요 국가 (국기 추가됨)
            'section-countries-h2': 'Key Countries 🌍',
            'countries-intro': 'BEST WORK collaborates with the following countries for the supply of international students and workers.',
            'countries-data': [
                { name: 'Nepal', flag: '🇳🇵', desc: 'A major partner, where many workers contribute to the Korean economy through the Employment Permit System (EPS), with active development cooperation.' },
                { name: 'Bangladesh', flag: '🇧🇩', desc: 'Established diplomatic ties in 1973; thousands of Bangladeshi workers reside in Korea, forming a core part of economic exchange and labor supply.' },
                { name: 'Sri Lanka', flag: '🇱🇰', desc: 'An important partner; numerous workers are dispatched to various sectors in Korea, particularly manufacturing, through the EPS.' },
                { name: 'Myanmar', flag: '🇲🇲', desc: 'The relationship with Korea is amicable, with high popularity for the Hallyu wave. Exchange is expanding through Korea\'s New Southern Policy.' },
                { name: 'Vietnam', flag: '🇻🇳', desc: 'One of Korea\'s major trading partners, with highly active economic and human exchange. Vietnam views Korea as a model for economic development.' },
                { name: 'Mongolia', flag: '🇲🇳', desc: 'The population visiting Korea for education and work is steadily increasing, making it an active partner in human exchange.' }
            ],

            // 제휴 대학
            'section-universities-h2': 'Partner Universities 🎓',
            'universities-intro': 'BEST WORK는 아래 대학교들과 유학생 유치를 위해 협력하고 있습니다.',
            'universities-data': [
                { name: 'Sookmyung Women\'s Univ.', desc: "A private university aiming to cultivate female leaders with **'S Leadership'**, known for strong student outcomes and flexible multi-major programs." },
                { name: 'Konkuk University', desc: "(General Info): A private comprehensive university with campuses in Seoul and Chungju, contributing to society through research and the convergence of various academic fields." },
                { name: 'Halla University', desc: "Located in Wonju, specializing in fields like **Smart Mobility Convergence**. It has signed academic exchange agreements with 23 international universities." },
                { name: 'Sangji University', desc: "(General Info): A comprehensive university in Wonju, 강원특별자치도, promoting practical talent development based on the founding philosophy of 'Respect for Heaven, Love for Humanity (敬天愛人).'" },
                { name: 'Songho University', desc: "A university focused on **'Digital Healthcare Professional Talent' and 'e-Mobility'**. It boasts excellent accessibility to the Seoul Metropolitan Area via KTX." },
                { name: 'Seoul Theological Univ.', desc: "A Christian university affiliated with the Holiness Church. Focuses on nurturing Christian ministers and professionals based on the **'Wesleyan Evangelical'** tradition." }
            ],
            
            // Contact
            'section-contact-h2': 'Contact',
            'contact-email': '<i class="fas fa-envelope"></i> <strong>Official Email:</strong> <a href="mailto:koreabestwork@gmail.com">koreabestwork@gmail.com</a>',
            'contact-address': '<i class="fas fa-map-marker-alt"></i> <strong>Address:</strong> 196 World Cup-ro, Mapo-gu, Seoul, Republic of Korea', 

            // 푸터
            'footer-text': '&copy; 2025 BEST WORK All rights reserved.',

            // 폼 요소
            'modal-title': '1:1 Consultation Request',
            'c-name-label': 'Name:',
            'c-name-placeholder': 'Enter your name',
            'c-contact-label': 'Contact No.:',
            'c-contact-placeholder': '+82 10-XXXX-XXXX',
            'c-email-label': 'Email:',
            'c-email-placeholder': 'example@email.com',
            'c-topic-label': 'Consultation Topic:',
            'c-topic-option-default': 'Select consultation topic',
            'c-topic-option-1': 'Student Recruitment',
            'c-topic-option-2': 'Manpower Supply (E-7 Visa)',
            'c-topic-option-3': 'Visa Inquiry (D2, D4, F2, etc.)',
            'c-topic-option-4': 'Other Inquiries',
            'c-content-label': 'Details:',
            'c-content-placeholder': 'Please describe your consultation in detail',
            'c-submit-btn': 'Submit Request',
            'c-note': 'We will contact you shortly after receiving your request.',
            'c-alert-success': 'Your consultation request has been successfully submitted. Our team will contact you shortly.',
        }
    };

    let currentLang = 'ko';
    let slideIndex = 0;

    // --- 2. 콘텐츠 로드 함수 ---
    function loadContent(lang) {
        currentLang = lang;
        const data = translations[lang];

        // 2-1. 단일 텍스트 및 속성 업데이트
        document.getElementById('title-text').textContent = data['title-text'].replace(/<\/?strong>/g, '');
        
        // 섹션 제목 업데이트
        document.getElementById('section-home-h2').textContent = data['section-home-h2'];
        document.getElementById('section-about-h2').textContent = data['section-about-h2'];
        document.getElementById('section-services-h2').textContent = data['section-services-h2'];
        document.getElementById('section-countries-h2').textContent = data['section-countries-h2'];
        document.getElementById('section-universities-h2').textContent = data['section-universities-h2'];
        document.getElementById('section-contact-h2').textContent = data['section-contact-h2'];
        
        // 콘텐츠 본문
        document.getElementById('home-intro').innerHTML = data['home-intro'];
        
        // 회사소개 핵심 가치 문구 업데이트 (strong 태그로 감싸 굵게 표시)
        document.getElementById('about-core-values-intro').innerHTML = `<strong>${data['about-core-values-intro']}</strong>`;
        
        // 회사소개 카드 내용
        document.getElementById('about-vision-title').innerHTML = `<i class="fas fa-eye"></i> ${data['about-vision-title']}`;
        document.getElementById('about-vision').innerHTML = data['about-vision'];
        document.getElementById('about-mission-title').innerHTML = `<i class="fas fa-bullseye"></i> ${data['about-mission-title']}`;
        document.getElementById('about-mission').innerHTML = data['about-mission'];
        document.getElementById('about-business-title').childNodes[1].nodeValue = ` ${data['about-business-title']}`;

        // 서비스 섹션 업데이트 (3개 항목)
        // 이 내용은 이제 service-card div 내의 p 태그로 로드됩니다.
        document.getElementById('service-consulting-title').textContent = data['service-consulting-title'];
        document.getElementById('service-consulting-content').innerHTML = data['service-consulting-content'];
        document.getElementById('service-visa-title').textContent = data['service-visa-title'];
        document.getElementById('service-visa-content').innerHTML = data['service-visa-content'];
        document.getElementById('service-job-title').textContent = data['service-job-title'];
        document.getElementById('service-job-content').innerHTML = data['service-job-content'];

        document.getElementById('countries-intro').textContent = data['countries-intro'];
        
        // 캐러셀 오버레이 텍스트 설정
        document.getElementById('universities-intro-1').textContent = data['universities-intro'];
        document.getElementById('universities-intro-2').textContent = data['universities-intro'];
        document.getElementById('universities-intro-3').textContent = data['universities-intro'];

        document.getElementById('contact-email').innerHTML = data['contact-email'];
        document.getElementById('contact-address').innerHTML = data['contact-address']; 
        
        // Consultation Form localization
        document.getElementById('modal-title').textContent = data['modal-title'];
        document.getElementById('c-name-label').textContent = data['c-name-label'];
        document.getElementById('c-name').placeholder = data['c-name-placeholder'];
        document.getElementById('c-contact-label').textContent = data['c-contact-label'];
        document.getElementById('c-contact').placeholder = data['c-contact-placeholder'];
        document.getElementById('c-email-label').textContent = data['c-email-label'];
        document.getElementById('c-email').placeholder = data['c-email-placeholder'];
        document.getElementById('c-topic-label').textContent = data['c-topic-label'];
        document.getElementById('c-content-label').textContent = data['c-content-label'];
        document.getElementById('c-content').placeholder = data['c-content-placeholder'];
        document.getElementById('c-submit-btn').textContent = data['c-submit-btn'];
        document.getElementById('c-note').textContent = data['c-note'];
        
        // Update select options
        const topicSelect = document.getElementById('c-topic');
        topicSelect.options[0].textContent = data['c-topic-option-default'];
        // 옵션 값이 아닌 텍스트만 업데이트
        topicSelect.options[1].textContent = data['c-topic-option-1'];
        topicSelect.options[2].textContent = data['c-topic-option-2'];
        topicSelect.options[3].textContent = data['c-topic-option-3'];
        topicSelect.options[4].textContent = data['c-topic-option-4'];


        document.getElementById('footer-text').innerHTML = data['footer-text'];

        // 2-2. 인라인 네비게이션 동적 생성
        const mainNavInline = document.getElementById('main-nav-wrapper-inline');
        mainNavInline.innerHTML = '';
        data['nav_items'].forEach(item => {
            const a = document.createElement('a');
            a.href = `#${item.id}`;
            a.textContent = item.text;
            mainNavInline.appendChild(a);
        });

        // 2-3. 리스트 및 테이블 동적 생성
        
        // 회사소개 - 주요 사업 리스트 (점 제거된 리스트 스타일 사용)
        const aboutBusinessList = document.getElementById('about-business-list');
        aboutBusinessList.innerHTML = '';
        data['about-business-list'].forEach(item => {
            const li = document.createElement('li');
            li.innerHTML = item;
            aboutBusinessList.appendChild(li);
        });

        // 주요 국가 그리드 (국기 적용 및 카드 디자인)
        const countriesGrid = document.getElementById('countries-grid');
        countriesGrid.innerHTML = '';
        data['countries-data'].forEach(item => {
            const card = document.createElement('div');
            card.className = 'country-card';
            card.innerHTML = `
                <div class="flag-name">
                    <span>${item.flag}</span>
                    ${item.name}
                </div>
                <p>${item.desc}</p>
            `;
            countriesGrid.appendChild(card);
        });


        // 제휴 대학 그리드 (카드 디자인 적용)
        const universitiesGrid = document.getElementById('universities-grid');
        universitiesGrid.innerHTML = '';
        data['universities-data'].forEach(item => {
            const card = document.createElement('div');
            card.className = 'university-card-item with-texture'; /* 텍스처 클래스 추가 */
            
            // item.desc에 포함된 <strong> 태그를 포함하여 출력
            const description = item.desc;
            const cardContent = `
                <strong>${item.name}</strong>
                <p>${description}</p>
            `;
            card.innerHTML = cardContent;
            universitiesGrid.appendChild(card);
        });
        
        // 2-4. 언어 버튼 활성화/비활성화
        document.getElementById('lang-ko').classList.remove('active');
        document.getElementById('lang-en').classList.remove('active');
        document.getElementById(`lang-${lang}`).classList.add('active');
    }

    // --- 3. 언어 설정 및 저장 함수 (수동 변경) ---
    function setLanguage(lang) {
        localStorage.setItem('bestwork_lang', lang);
        loadContent(lang);
    }
    
    // --- 4. 캐러셀 제어 함수 ---
    function showSlides() {
        const slides = document.getElementsByClassName("university-carousel-item");
        for (let i = 0; i < slides.length; i++) {
            slides[i].classList.remove('active');
        }
        slideIndex++;
        if (slideIndex > slides.length) {slideIndex = 1}    
        slides[slideIndex-1].classList.add('active');
        setTimeout(showSlides, 5000); // 5초마다 이미지 변경
    }

    // --- 5. 초기화 및 자동 감지 ---
    document.addEventListener('DOMContentLoaded', () => {
        let preferredLang = localStorage.getItem('bestwork_lang');

        if (!preferredLang) {
            const browserLang = navigator.language.toLowerCase();
            if (browserLang.includes('ko')) {
                preferredLang = 'ko';
            } else {
                preferredLang = 'en';
            }
        }
        
        loadContent(preferredLang);
        showSlides(); // 캐러셀 시작

        // Form Submission Handler
        const form = document.getElementById('consultation-form');
        form.addEventListener('submit', function(e) {
            e.preventDefault();
            
            // 실제 애플리케이션에서는 fetch() 등을 사용하여 서버로 데이터를 전송해야 합니다.
            // 여기서는 데모용으로 알림창에 데이터와 성공 메시지를 표시합니다.
            const formData = new FormData(form);
            const dataObject = {};
            formData.forEach((value, key) => dataObject[key] = value);

            const successMessage = translations[currentLang]['c-alert-success'];
            console.log("Submitted Data:", dataObject);

            alert(successMessage + '\n\n' + translations[currentLang]['modal-title'] + ' 내역:\n' + 
                  '------------------------------\n' +
                  translations[currentLang]['c-name-label'].replace(':', '') + ': ' + dataObject.name + '\n' +
                  translations[currentLang]['c-contact-label'].replace(':', '') + ': ' + dataObject.contact + '\n' +
                  translations[currentLang]['c-email-label'].replace(':', '') + ': ' + dataObject.email + '\n' +
                  translations[currentLang]['c-topic-label'].replace(':', '') + ': ' + dataObject.topic + '\n' +
                  translations[currentLang]['c-content-label'].replace(':', '') + ': ' + dataObject.content.substring(0, 30) + '...'
            );
            
            // 폼 내용 초기화
            form.reset();
        });
    });
</script>

</body>
</html>
