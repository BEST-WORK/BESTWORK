<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BEST WORK | Join The Best, Be The Best</title>
    <style>
        /* ==================== 1. CSS (스타일) ==================== */
        :root {
            --main-color: #6C7A63; /* BEST WORK 로고 색상 계열 */
            --light-bg: #F8F8F8;
            --text-color: #333;
        }

        /* 기본 설정 (모바일 최적화) */
        body {
            font-family: 'Malgun Gothic', '맑은 고딕', sans-serif;
            margin: 0;
            padding: 0;
            background-color: white;
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        a {
            color: var(--main-color);
            text-decoration: none;
        }

        /* 헤더 및 내비게이션 */
        header {
            background-color: white;
            padding: 15px 20px;
            box-shadow: 0 2px 4px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--main-color);
        }

        .lang-switch {
            font-size: 14px;
            padding: 5px 10px;
            border: 1px solid var(--main-color);
            border-radius: 5px;
            cursor: pointer;
            color: var(--main-color);
        }

        /* 모바일 메뉴 (햄버거 메뉴 구현) */
        #menu-toggle {
            display: none;
        }

        .menu-icon {
            cursor: pointer;
            display: block; /* 모바일에서만 표시 */
            padding: 10px;
        }

        .menu-icon span {
            display: block;
            width: 25px;
            height: 3px;
            background: var(--main-color);
            margin: 5px 0;
            transition: 0.4s;
        }

        nav {
            position: fixed;
            top: 0;
            right: -100%; /* 숨김 */
            width: 70%;
            max-width: 300px;
            height: 100vh;
            background-color: var(--light-bg);
            box-shadow: -2px 0 5px rgba(0,0,0,0.1);
            transition: right 0.3s;
            padding-top: 60px;
        }

        #menu-toggle:checked ~ nav {
            right: 0; /* 표시 */
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        nav a {
            display: block;
            padding: 15px 20px;
            border-bottom: 1px solid #ddd;
            color: var(--text-color);
            font-size: 16px;
        }

        /* 메인 섹션 스타일 */
        section {
            padding: 40px 20px;
            border-bottom: 1px solid var(--light-bg);
        }

        section:nth-child(even) {
            background-color: var(--light-bg);
        }

        h2 {
            font-size: 24px;
            color: var(--main-color);
            border-bottom: 2px solid var(--main-color);
            padding-bottom: 10px;
            margin-bottom: 25px;
        }

        .content-box {
            background-color: white;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 1px 3px rgba(0,0,0,0.05);
            margin-bottom: 20px;
        }

        .content-box h3 {
            color: var(--text-color);
            margin-top: 0;
            font-size: 18px;
        }

        ul.partner-list {
            list-style: none;
            padding: 0;
        }
        ul.partner-list li {
            padding: 8px 0;
            border-bottom: 1px dotted #ccc;
        }

        /* 푸터 */
        footer {
            text-align: center;
            padding: 20px;
            background-color: var(--text-color);
            color: white;
            font-size: 14px;
        }

        /* 태블릿 및 데스크톱 (Optional, but good practice for mobile-first) */
        @media (min-width: 768px) {
            .menu-icon {
                display: none; /* 데스크톱에서 숨김 */
            }
            header {
                max-width: 1200px;
                margin: auto;
            }
            nav {
                position: static;
                height: auto;
                width: auto;
                background: none;
                box-shadow: none;
                padding-top: 0;
            }
            nav ul {
                display: flex;
                flex-direction: row;
            }
            nav a {
                padding: 10px 15px;
                border-bottom: none;
            }
            section {
                max-width: 1200px;
                margin: auto;
                padding: 60px 20px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="logo">BEST WORK</div>
        <input type="checkbox" id="menu-toggle">
        <label for="menu-toggle" class="menu-icon">
            <span></span>
            <span></span>
            <span></span>
        </label>
        <div id="language-toggle" class="lang-switch" data-lang="ko">English</div>
        
        <nav>
            <ul>
                <li><a href="#about" data-lang-ko="회사 소개" data-lang-en="About Us">회사 소개</a></li>
                <li><a href="#services" data-lang-ko="서비스" data-lang-en="Services">서비스</a></li>
                <li><a href="#universities" data-lang-ko="제휴 대학" data-lang-en="Partner Universities">제휴 대학</a></li>
                <li><a href="#countries" data-lang-ko="제휴 국가" data-lang-en="Partner Countries">제휴 국가</a></li>
                <li><a href="#companies" data-lang-ko="제휴 기업" data-lang-en="Partner Companies">제휴 기업</a></li>
                <li><a href="#contact" data-lang-ko="Contact" data-lang-en="Contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2 data-lang-ko="회사 소개" data-lang-en="About Us">회사 소개</h2>
        <div class="content-box">
            <h3 data-lang-ko="MISSION & VISION" data-lang-en="MISSION & VISION">MISSION & VISION</h3>
            [cite_start]<p data-lang-ko="BESTWORK는 외국인이 유학과 취업을 통해 대한민국에 정착할 수 있도록 지원하며, 외국인과 대한민국의 가교 역할을 통해 함께 성장하는 미래를 만들어갑니다. [cite: 110]" 
               [cite_start]data-lang-en="BESTWORK supports foreigners to settle in Korea through studying and employment, building a future of mutual growth by serving as a bridge between foreigners and Korea. [cite: 110]">
                [cite_start]BESTWORK는 외국인이 유학과 취업을 통해 대한민국에 정착할 수 있도록 지원하며, 외국인과 대한민국의 가교 역할을 통해 함께 성장하는 미래를 만들어갑니다. [cite: 110]
            </p>
            <ul>
                [cite_start]<li data-lang-ko="**VISION**: Best Person, Best Position, Best Time (최고의 인재를, 최고의 자리에, 최고의 타이밍에 배치합니다) [cite: 110]" 
                    [cite_start]data-lang-en="**VISION**: Best Person, Best Position, Best Time (Placing the best talent in the best position at the best time) [cite: 110]">
                    [cite_start]**VISION**: Best Person, Best Position, Best Time (최고의 인재를, 최고의 자리에, 최고의 타이밍에 배치합니다) [cite: 110]
                </li>
                [cite_start]<li data-lang-ko="**MISSION**: 최고의 인재 영입으로 사업을 변화시키자 (Transform businesses through a best recruitment experience) [cite: 110]" 
                    [cite_start]data-lang-en="**MISSION**: Transform businesses through a best recruitment experience [cite: 110]">
                    [cite_start]**MISSION**: 최고의 인재 영입으로 사업을 변화시키자 (Transform businesses through a best recruitment experience) [cite: 110]
                </li>
            </ul>
        </div>
        
        <div class="content-box">
            <h3 data-lang-ko="주요 연혁" data-lang-en="Business History">주요 연혁</h3>
            <ul>
                [cite_start]<li data-lang-ko="**2025.04**: (사)아산테크노밸리 입주기업체협의회 외국인 근로자 공급 업무협약 체결 [cite: 113][cite_start]" data-lang-en="**2025.04**: Signed MOU with Asan Technovalley Resident Company Association for foreign worker supply [cite: 113][cite_start]">**2025.04**: (사)아산테크노밸리 입주기업체협의회 외국인 근로자 공급 업무협약 체결 [cite: 113]</li>
                [cite_start]<li data-lang-ko="**2025.01**: 숙명여자대학교 국제교류 및 입학자원 발굴 협력 지원 협정서 체결 [cite: 113][cite_start]" data-lang-en="**2025.01**: Signed Agreement with Sookmyung Women's University for international exchange and recruitment [cite: 113][cite_start]">**2025.01**: 숙명여자대학교 국제교류 및 입학자원 발굴 협력 지원 협정서 체결 [cite: 113]</li>
                [cite_start]<li data-lang-ko="**2024.11**: 한라대학교 국제교류 및 입학자원 발굴 협력 지원 협정서 체결 [cite: 113][cite_start]" data-lang-en="**2024.11**: Signed Agreement with Halla University for international exchange and recruitment [cite: 113][cite_start]">**2024.11**: 한라대학교 국제교류 및 입학자원 발굴 협력 지원 협정서 체결 [cite: 113]</li>
                [cite_start]<li data-lang-ko="**2023.11**: 베트남 노동 수출 회사(GLC Group 등)와 한국 내 인력 공급 협약 체결 [cite: 112][cite_start]" data-lang-en="**2023.11**: Signed labor supply agreement in Korea with Vietnamese labor export companies (GLC Group, etc.) [cite: 112][cite_start]">**2023.11**: 베트남 노동 수출 회사(GLC Group 등)와 한국 내 인력 공급 협약 체결 [cite: 112]</li>
            </ul>
        </div>
    </section>

    <section id="services">
        <h2 data-lang-ko="주요 서비스" data-lang-en="Key Services">주요 서비스</h2>
        <div class="content-box">
            <h3 data-lang-ko="유학생 유치 및 교육 연계" data-lang-en="International Student Recruitment & Education Linkage">유학생 유치 및 교육 연계</h3>
            [cite_start]<p data-lang-ko="학업 성취에 높은 열망을 가진 우수한 외국인 유학생을 국내 대학교에 소개하고, 제휴 유학원과의 협력을 통해 성공적인 유학 생활을 지원합니다. [cite: 111]" 
               [cite_start]data-lang-en="We introduce outstanding foreign students with high academic aspirations to Korean universities and support their successful study abroad through cooperation with partner agencies. [cite: 111]">
                [cite_start]학업 성취에 높은 열망을 가진 우수한 외국인 유학생을 국내 대학교에 소개하고, 제휴 유학원과의 협력을 통해 성공적인 유학 생활을 지원합니다. [cite: 111]
            </p>
        </div>
        <div class="content-box">
            <h3 data-lang-ko="생애주기 비자 프로그램 운영" data-lang-en="Life Cycle VISA Program Management">생애주기 비자 프로그램 운영</h3>
            [cite_start]<p data-lang-ko="대한민국 정착을 위한 '생애주기 비자 프로그램(Life Cycle VISA Program)'을 운영하며, 유학(D-2/D-4), 취업(E-7), 거주(F-2) 비자에 대해 전문 행정사와 제휴하여 필요한 모든 서비스를 제공합니다. [cite: 111, 112]" 
               [cite_start]data-lang-en="We operate the 'Life Cycle VISA Program' for settlement in Korea, offering all necessary services for Study (D-2/D-4), Employment (E-7), and Residency (F-2) visas in partnership with expert administrative law firms. [cite: 111, 112]">
                [cite_start]대한민국 정착을 위한 '생애주기 비자 프로그램(Life Cycle VISA Program)'을 운영하며, 유학(D-2/D-4), 취업(E-7), 거주(F-2) 비자에 대해 전문 행정사와 제휴하여 필요한 모든 서비스를 제공합니다. [cite: 111, 112]
            </p>
        </div>
        <div class="content-box">
            <h3 data-lang-ko="우수 인재 국내 기업 공급 (E-7)" data-lang-en="Supply of Skilled Foreign Workers to Domestic Companies (E-7)">우수 인재 국내 기업 공급 (E-7)</h3>
            [cite_start]<p data-lang-ko="외국인 근로자 취업비자(E-7) 프로그램을 통해 국내 기업에 우수한 해외 인력을 지속적으로 공급하여 기업의 인력난 해소 및 고용 안정에 기여합니다. [cite: 110, 112]" 
               [cite_start]data-lang-en="Through the E-7 employment visa program for foreign workers, we continuously supply skilled overseas talent to domestic companies, helping to solve labor shortages and stabilize employment. [cite: 110, 112]">
                [cite_start]외국인 근로자 취업비자(E-7) 프로그램을 통해 국내 기업에 우수한 해외 인력을 지속적으로 공급하여 기업의 인력난 해소 및 고용 안정에 기여합니다. [cite: 110, 112]
            </p>
        </div>
    </section>

    <section id="universities">
        <h2 data-lang-ko="제휴 대학" data-lang-en="Partner Universities">제휴 대학</h2>
        <div class="content-box">
            <h3 data-lang-ko="국제 교류 및 유학생 유치 협력 대학" data-lang-en="Partner Universities for International Exchange and Student Recruitment">국제 교류 및 유학생 유치 협력 대학</h3>
            <ul class="partner-list">
                [cite_start]<li><span data-lang-ko="숙명여자대학교" data-lang-en="Sookmyung Women's University">숙명여자대학교</span> [cite: 113]</li>
                [cite_start]<li><span data-lang-ko="한신대학교" data-lang-en="Hanshin University">한신대학교</span> (베트남 유학생 유치 업무 진행) [cite: 113]</li>
                [cite_start]<li><span data-lang-ko="한라대학교" data-lang-en="Halla University">한라대학교</span> [cite: 113]</li>
                [cite_start]<li><span data-lang-ko="송호대학교" data-lang-en="Songho University">송호대학교</span> [cite: 113]</li>
                [cite_start]<li><span data-lang-ko="서울신학대학교" data-lang-en="Seoul Theological University">서울신학대학교</span> (네팔 유학생 유치 업무 진행) [cite: 113]</li>
            </ul>
        </div>
        <div class="content-box">
            <h3 data-lang-ko="제휴 유학원" data-lang-en="Partner Study Abroad Agencies">제휴 유학원</h3>
            <ul class="partner-list">
                [cite_start]<li><span data-lang-ko="네팔 현지 유학원" data-lang-en="Local Study Abroad Agency in Nepal">네팔 현지 유학원</span> [cite: 113]</li>
                [cite_start]<li><span data-lang-ko="방글라데시 현지 유학원" data-lang-en="Local Study Abroad Agency in Bangladesh">방글라데시 현지 유학원</span> [cite: 113]</li>
            </ul>
        </div>
    </section>

    <section id="countries">
        <h2 data-lang-ko="제휴 국가" data-lang-en="Partner Countries">제휴 국가</h2>
        <div class="content-box">
            <h3 data-lang-ko="주요 인력 및 유학생 공급 국가" data-lang-en="Main Countries for Labor and Student Supply">주요 인력 및 유학생 공급 국가</h3>
            <ul class="partner-list">
                [cite_start]<li data-lang-ko="베트남 (Vietnam)" data-lang-en="Vietnam (베트남)">베트남 (Vietnam) [cite: 111, 112]</li>
                [cite_start]<li data-lang-ko="네팔 (Nepal)" data-lang-en="Nepal (네팔)">네팔 (Nepal) [cite: 111, 113]</li>
                [cite_start]<li data-lang-ko="방글라데시 (Bangladesh)" data-lang-en="Bangladesh (방글라데시)">방글라데시 (Bangladesh) [cite: 111, 113]</li>
                [cite_start]<li data-lang-ko="미얀마 (Myanmar)" data-lang-en="Myanmar (미얀마)">미얀마 (Myanmar) [cite: 111]</li>
            </ul>
        </div>
    </section>

    <section id="companies">
        <h2 data-lang-ko="주요 제휴 기업 및 기관" data-lang-en="Key Partner Companies & Organizations">주요 제휴 기업 및 기관</h2>
        <div class="content-box">
            <h3 data-lang-ko="외국인 근로자 공급 제휴" data-lang-en="Foreign Worker Supply Partners">외국인 근로자 공급 제휴</h3>
            <ul class="partner-list">
                [cite_start]<li data-lang-ko="(사)아산테크노밸리 입주기업체협의회" data-lang-en="Asan Technovalley Resident Company Association">(사)아산테크노밸리 입주기업체협의회 [cite: 113]</li>
                [cite_start]<li data-lang-ko="㈜스마일에프엔디" data-lang-en="Smile FND Co., Ltd.">㈜스마일에프엔디 [cite: 113]</li>
                [cite_start]<li data-lang-ko="㈜제이에스시스템즈" data-lang-en="JS Systems Co., Ltd.">㈜제이에스시스템즈 [cite: 113]</li>
                [cite_start]<li data-lang-ko="ORACON" data-lang-en="ORACON">ORACON [cite: 113]</li>
                [cite_start]<li data-lang-ko="베트남 GLC Group, DNC, SEIKO 등 (노동 수출 회사)" data-lang-en="GLC Group, DNC, SEIKO etc. in Vietnam (Labor Export Companies)">베트남 GLC Group, DNC, SEIKO 등 (노동 수출 회사) [cite: 112]</li>
            </ul>
        </div>
    </section>

    <section id="contact">
        <h2 data-lang-ko="Contact" data-lang-en="Contact">Contact</h2>
        <div class="content-box">
            <h3 data-lang-ko="문의 및 연락처" data-lang-en="Inquiries and Contact Information">문의 및 연락처</h3>
            <p data-lang-ko="BEST WORK에 대한 문의 사항은 아래 이메일로 연락 주시면 신속하게 답변드리겠습니다." 
               data-lang-en="For any inquiries regarding BEST WORK, please contact us at the email addresses below. We will respond promptly.">
                BEST WORK에 대한 문의 사항은 아래 이메일로 연락 주시면 신속하게 답변드리겠습니다.
            </p>
            <p>
                [cite_start]<strong data-lang-ko="주요 문의 이메일" data-lang-en="Main Inquiry Email">주요 문의 이메일</strong>: <a href="mailto:isbework@gmail.com">isbework@gmail.com</a> [cite: 114]
            </p>
            <p>
                [cite_start]<strong data-lang-ko="기타 이메일" data-lang-en="Other Email">기타 이메일</strong>: <a href="mailto:koreabestwork@gmail.com">koreabestwork@gmail.com</a> [cite: 114]
            </p>
            [cite_start]<p data-lang-ko="대표이사 박현상 / 이사 김익수" data-lang-en="CEO Park Hyun-sang / Director Kim Ik-soo">대표이사 박현상 / 이사 김익수 [cite: 114]</p>
        </div>
    </section>

    <footer>
        <p data-lang-ko="Copyright &copy; 2025 BEST WORK. All Rights Reserved." data-lang-en="Copyright &copy; 2025 BEST WORK. All Rights Reserved.">
            Copyright &copy; 2025 BEST WORK. All Rights Reserved.
        </p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const langToggle = document.getElementById('language-toggle');
            const dataElements = document.querySelectorAll('[data-lang-ko], [data-lang-en]');
            
            let currentLang = 'ko'; // 기본값은 한국어
            
            // 1. 초기 언어 설정 (OS/브라우저 설정 기반)
            function getInitialLanguage() {
                const userLang = navigator.language || navigator.userLanguage;
                // 한국이 아닌 경우, 또는 영어를 선호하는 경우 'en'으로 설정
                // 실제 서비스에서는 IP 주소 등을 통해 접속 국가를 확인해야 합니다.
                if (userLang.startsWith('en') || !userLang.startsWith('ko')) {
                    return 'en';
                }
                return 'ko';
            }

            function updateText(lang) {
                dataElements.forEach(element => {
                    const koText = element.getAttribute('data-lang-ko');
                    const enText = element.getAttribute('data-lang-en');

                    if (lang === 'ko' && koText) {
                        element.innerHTML = koText;
                        if (element.tagName === 'A') element.textContent = koText;
                    } else if (lang === 'en' && enText) {
                        element.innerHTML = enText;
                        if (element.tagName === 'A') element.textContent = enText;
                    }
                });

                // 언어 버튼 텍스트 업데이트
                langToggle.setAttribute('data-lang', lang);
                langToggle.textContent = lang === 'ko' ? 'English' : '한국어';
                
                // HTML lang 속성 업데이트
                document.documentElement.lang = lang;
            }

            // 초기 로딩 시 언어 설정 적용
            currentLang = getInitialLanguage();
            updateText(currentLang);


            // 2. 언어 변경 버튼 클릭 이벤트
            langToggle.addEventListener('click', () => {
                currentLang = currentLang === 'ko' ? 'en' : 'ko';
                updateText(currentLang);
            });
            
            // 3. 모바일 메뉴 닫기 (메뉴 항목 클릭 시)
            const navLinks = document.querySelectorAll('nav a');
            const menuToggleCheckbox = document.getElementById('menu-toggle');
            navLinks.forEach(link => {
                link.addEventListener('click', () => {
                    if (window.innerWidth < 768) {
                        menuToggleCheckbox.checked = false;
                    }
                });
            });
        });
    </script>
</body>
</html>
