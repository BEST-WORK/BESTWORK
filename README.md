<html markdown: GFM>
<title: ''>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BEST WORK - 최고의 유학 및 취업 플랫폼</title>
    <!-- Tailwind CSS CDN 로드 --><script src="https://cdn.tailwindcss.com"></script>
    <style>
        /* Custom Font Configuration */
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #f4f7f9; /* 밝은 배경 */
        }
        /* Primary Brand Color: Deep Blue */
        .bg-primary { background-color: #1e3a8a; } 
        .text-primary { color: #1e3a8a; }
        /* Secondary Brand Color: Accent Green/Blue */
        .gradient-text {
            background-image: linear-gradient(45deg, #10b981, #3b82f6); /* 에메랄드와 파랑 그라디언트 */
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-fill-color: transparent;
        }
        /* Active Navigation Link Style */
        .nav-link.active {
            color: #1e3a8a; /* Deep blue for active link */
            font-weight: 700;
            border-bottom: 3px solid #1e3a8a;
            padding-bottom: 0.5rem;
        }
        .nav-link {
            transition: all 0.2s ease-in-out;
        }
        /* Page Transition Effect */
        #app-content {
            transition: opacity 0.3s ease-in-out;
        }
        /* Custom university card hover effect */
        .university-card {
            transition: all 0.3s ease;
        }
        .university-card:hover {
            box-shadow: 0 10px 15px rgba(30, 58, 138, 0.2); /* Shadow with primary color tint */
            transform: translateY(-5px);
        }
        /* New Service Card Styles for richness */
        .service-card {
            transition: all 0.4s ease-in-out;
            border-radius: 1.5rem; /* rounded-2xl */
        }
        .service-card:hover {
            transform: scale(1.02);
            box-shadow: 0 20px 25px rgba(0, 0, 0, 0.1);
        }
        .icon-box {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 4rem; /* w-16 */
            height: 4rem; /* h-16 */
            border-radius: 9999px; /* rounded-full */
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body class="antialiased">

    <!-- 1. 상단 내비게이션 바 (메뉴) --><header class="sticky top-0 z-50 bg-white shadow-xl">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- 로고 --><a href="#home" class="text-3xl font-extrabold gradient-text tracking-wider nav-link-logo">
                    BEST WORK
                </a>

                <!-- 데스크톱 메뉴 --><nav class="hidden md:flex space-x-8 h-full items-center">
                    <a href="#home" class="nav-link text-gray-600 hover:text-blue-600 font-medium text-lg">Home</a>
                    <a href="#about" class="nav-link text-gray-600 hover:text-blue-600 font-medium text-lg">회사 소개</a>
                    <a href="#service" class="nav-link text-gray-600 hover:text-blue-600 font-medium text-lg">핵심 서비스</a>
                    <!-- 새로 추가된 메뉴 --><a href="#affiliates" class="nav-link text-gray-600 hover:text-blue-600 font-medium text-lg">제휴 대학교</a>
                    <a href="#countries" class="nav-link text-gray-600 hover:text-blue-600 font-medium text-lg">주요 거점 국가</a>
                    <a href="#contact" class="px-5 py-2 bg-blue-600 text-white rounded-full hover:bg-blue-700 transition duration-300 shadow-lg font-bold text-lg">문의하기</a>
                </nav>

                <!-- 모바일 메뉴 버튼 --><button id="menu-button" class="md:hidden p-2 rounded-md text-gray-700 hover:bg-gray-100 transition duration-300 focus:outline-none focus:ring-2 focus:ring-blue-500" aria-expanded="false" aria-controls="mobile-menu">
                    <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2.5" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
                </button>
            </div>
        </div>

        <!-- 모바일 메뉴 드롭다운 --><div id="mobile-menu" class="hidden md:hidden bg-white shadow-inner pb-2" aria-labelledby="menu-button">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#home" class="mobile-nav-link block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-50">Home</a>
                <a href="#about" class="mobile-nav-link block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-50">회사 소개</a>
                <a href="#service" class="mobile-nav-link block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-50">핵심 서비스</a>
                <a href="#affiliates" class="mobile-nav-link block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-50">제휴 대학교</a> <!-- 모바일 메뉴에도 추가 --><a href="#countries" class="mobile-nav-link block px-3 py-2 rounded-md text-base font-medium text-gray-700 hover:bg-gray-50">주요 거점 국가</a>
                <a href="#contact" class="mt-2 block px-3 py-2 rounded-full text-base font-medium bg-blue-500 text-white text-center hover:bg-blue-600">문의하기</a>
            </div>
        </div>
    </header>
    
    <!-- 2. Main Dynamic Content Area --><main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-10 md:py-16">
        <div id="app-content">
            <!-- Page content will be rendered here by JavaScript --></div>
    </main>

    <!-- 3. 푸터 --><footer class="bg-gray-800 text-gray-400 py-8 mt-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p class="text-xl font-bold text-white mb-2">BEST WORK</p>
            <p class="text-sm">&copy; 2025 BEST WORK. All rights reserved.</p>
            <p class="text-sm mt-1">서울특별시 마포구 월드컵로 196, B105-690호 (성산동)</p>
        </div>
    </footer>

    <!-- 자바스크립트: SPA 라우팅 및 동적 콘텐츠 생성 로직 --><script>
        const APP_CONTENT_ID = 'app-content';
        const contentDiv = document.getElementById(APP_CONTENT_ID);

        /**
         * 2-1. Page Content Functions (Returns HTML string for each page)
         */

        // --- Home Page ---
        function getHomePageContent() {
            return `
                <!-- Home Section (Fancy Hero) --><section id="home-content" class="relative bg-gray-900 text-white min-h-[50vh] md:min-h-[65vh] flex items-center justify-center rounded-2xl shadow-2xl overflow-hidden p-6">
                    <!-- Background Placeholder --><div class="absolute inset-0 bg-cover bg-center opacity-30" style="background-image: url('https://placehold.co/1920x1080/0f172a/ffffff?text=Global+Aspiration');"></div>
                    <div class="absolute inset-0 bg-black opacity-60"></div>

                    <!-- Content --><div class="relative z-10 text-center py-10 md:py-20">
                        <h1 class="text-4xl sm:text-6xl lg:text-7xl font-extrabold mb-4 leading-tight">
                            <span class="gradient-text">Join The Best,</span>
                            <br class="hidden sm:block"> Be The Best
                        </h1>
                        <p class="text-lg sm:text-xl text-gray-300 max-w-4xl mx-auto mb-10 font-light">
                            외국인이 유학과 취업을 통해 <span class="font-semibold text-white">대한민국에 성공적으로 정착</span> 할 수 있도록 돕는 최고의 파트너입니다.
                        </p>
                        <div class="flex justify-center space-x-4">
                            <a href="#service" class="px-8 py-3 bg-blue-600 text-white text-lg font-semibold rounded-full shadow-xl hover:bg-blue-700 transition duration-300 transform hover:scale-105">
                                서비스 살펴보기
                            </a>
                            <a href="#affiliates" class="px-8 py-3 bg-transparent border-2 border-white text-white text-lg font-semibold rounded-full shadow-xl hover:bg-white hover:text-gray-900 transition duration-300 transform hover:scale-105">
                                제휴 대학교 확인
                            </a>
                        </div>
                    </div>
                </section>
            `;
        }

        // --- About Us Page ---
        function getAboutPageContent() {
            return `
                <!-- About Us Section --><section class="py-16 bg-white rounded-xl shadow-xl">
                    <h2 class="text-5xl font-extrabold text-center text-primary mb-16 border-b-4 border-blue-600 inline-block pb-2">회사 소개 및 비전</h2>
                    <div class="grid md:grid-cols-3 gap-8 p-6">
                        
                        <!-- Section 1: Core Value --><div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-4 border-blue-600">
                            <h3 class="text-3xl font-bold mb-4 text-primary">VISION</h3>
                            <p class="text-2xl font-bold text-blue-600 mb-4">Best Person, Best Position, Best Time</p>
                            <p class="text-gray-600">최고의 인재를, 최고의 자리에, 최고의 타이밍에 배치하여 인재와 기업 모두의 가치를 극대화합니다.</p>
                        </div>

                        <!-- Section 2: Mission --><div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-4 border-green-600">
                            <h3 class="text-3xl font-bold mb-4 text-primary">MISSION</h3>
                            <p class="text-2xl font-bold text-green-600 mb-4">Transform businesses through a best recruitment experience</p>
                            <p class="text-gray-600">최고의 인재 영입 경험을 통해 고객사의 사업을 혁신적으로 변화시키는 것을 목표합니다.</p>
                        </div>

                        <!-- Section 3: Strength --><div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-4 border-primary">
                            <h3 class="text-3xl font-bold mb-4 text-primary">강점 및 역할</h3>
                            <p class="text-gray-600 mb-4 leading-relaxed">
                                해외 직접 진출 경험을 바탕으로, **현지인들의 니즈와 현지 상황을 깊이 이해**하고 유학생 및 근로자를 공급하는 가교 역할을 수행합니다.
                            </p>
                             <ul class="text-sm text-gray-700 mt-1 space-y-1">
                                <li>대한민국 대학교와 우수 외국인 유학생 연결</li>
                                <li>유학(D-2/D-4)부터 취업(E-7), 거주(F-2)까지 생애주기 비자 프로그램 운영</li>
                            </ul>
                        </div>
                    </div>
                </section>
            `;
        }

        // --- Service Page (RICHLY ENHANCED with Monogram SVGs) ---
        function getServicePageContent() {
            // Enhanced SVG Components for Monograms (More colorful and detailed)
            
            // 1. Tech Talent (Microchip/Innovation) - Blue/Yellow/Deep Blue Palette
            const svgMonogramTech = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="4" y="4" width="16" height="16" rx="3" fill="#3b82f6" stroke="#1e3a8a" stroke-width="1.5"/>
                    <circle cx="12" cy="12" r="3" fill="#fcd34d"/>
                    <path d="M12 7V5M12 19V17M7 12H5M19 12H17" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M6 18L7 17M18 6L17 7M18 18L17 17M6 6L7 7" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round" stroke-opacity="0.8"/>
                    <path d="M10 12h-1M14 12h1" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            `; // Stylized Microchip/Processor with deep blue and gold accents

            // 2. University Partnership (Connection/Education) - Green/Blue/White Palette
            const svgMonogramUniversity = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="3" y="10" width="18" height="10" rx="2" fill="#d1fae5" stroke="#059669" stroke-width="1.5"/>
                    <path d="M12 10L19 6L12 2L5 6L12 10" fill="#a7f3d0" stroke="#059669" stroke-width="1.5" stroke-linejoin="round"/>
                    <path d="M5 6L12 10M19 6L12 10" stroke="#059669" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M12 10V20" stroke="#059669" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M6 15L18 15" stroke="#059669" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M8 17L16 17" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            `; // Stylized Graduation Cap and Building/Diploma

            // 3. Global Network (Interconnected World) - Blue/Green/White Palette
            const svgMonogramGlobal = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="12" cy="12" r="10" fill="#bfdbfe" stroke="#3b82f6" stroke-width="1.5"/>
                    <path d="M12 2a15.3 15.3 0 014 10a15.3 15.3 0 01-4 10a15.3 15.3 0 01-4-10a15.3 15.3 0 014-10z" stroke="#3b82f6" stroke-width="1.5"/>
                    <path d="M2.05 12h19.9" stroke="#3b82f6" stroke-width="1.5"/>
                    <!-- Connection Nodes --><circle cx="6" cy="12" r="1.5" fill="#10b981"/>
                    <circle cx="18" cy="8" r="1.5" fill="#fcd34d"/>
                    <circle cx="14" cy="16" r="1.5" fill="#ef4444"/>
                    <!-- Dynamic lines --><path d="M6 12L18 8M18 8L14 16M14 16L6 12" stroke="#1e3a8a" stroke-width="0.5" stroke-linecap="round" stroke-opacity="0.7"/>
                </svg>
            `; // Dynamic Globe with multiple colored connection points

            // 4. Enhanced VISA Roadmap SVG - Dynamic Path and Clearer Color Coding
            const svgMonogramVisaRoadmap = `
                <svg class="w-full h-auto" viewBox="0 0 800 300" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <!-- Define Gradient for Road --><defs>
                        <linearGradient id="roadGradient" x1="0" y1="0" x2="1" y2="0">
                            <stop offset="0%" stop-color="#3b82f6"/>
                            <stop offset="50%" stop-color="#10b981"/>
                            <stop offset="100%" stop-color="#1e3a8a"/>
                        </linearGradient>
                    </defs>

                    <!-- Background Line (Road) using Gradient --><path d="M50 150 C 200 100, 400 200, 750 150" stroke="url(#roadGradient)" stroke-width="20" stroke-linecap="round" class="shadow-lg"/>

                    <!-- Phase 1: D-2/D-4 (유학) - Blue --><circle cx="50" cy="150" r="25" fill="#3b82f6"/>
                    <text x="50" y="155" fill="white" font-size="18" font-weight="extrabold" text-anchor="middle">D-2</text>
                    <text x="50" y="205" fill="#1e3a8a" font-size="20" font-weight="bold" text-anchor="middle">유학</text>
                    
                    <!-- Phase 2: E-7 (취업) - Green --><circle cx="400" cy="175" r="25" fill="#10b981"/>
                    <text x="400" y="180" fill="white" font-size="18" font-weight="extrabold" text-anchor="middle">E-7</text>
                    <text x="400" y="225" fill="#1e3a8a" font-size="20" font-weight="bold" text-anchor="middle">취업</text>

                    <!-- Phase 3: F-2 (정착) - Deep Blue --><circle cx="750" cy="150" r="25" fill="#1e3a8a"/>
                    <text x="750" y="155" fill="white" font-size="18" font-weight="extrabold" text-anchor="middle">F-2</text>
                    <text x="750" y="205" fill="#1e3a8a" font-size="20" font-weight="bold" text-anchor="middle">정착</text>

                    <!-- Arrow Tip (End Goal) --><path d="M720 150 L 760 140 L 760 160 Z" fill="#1e3a8a" transform="translate(10, 0)"/>
                </svg>
            `;

            // NEW! More detailed and varied icons for "High-Tech Talent"
            const iconHighTechChips = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <rect x="3" y="3" width="7" height="7" rx="1" fill="#facc15"/>
                    <rect x="14" y="3" width="7" height="7" rx="1" fill="#ef4444"/>
                    <rect x="3" y="14" width="7" height="7" rx="1" fill="#3b82f6"/>
                    <rect x="14" y="14" width="7" height="7" rx="1" fill="#10b981"/>
                    <path d="M10.5 7.5h3M10.5 16.5h3M7.5 10.5v3M16.5 10.5v3" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            `; // Multiple colorful chips

            const iconHighTechNetwork = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="6" cy="6" r="3" fill="#3b82f6"/>
                    <circle cx="18" cy="6" r="3" fill="#10b981"/>
                    <circle cx="12" cy="18" r="3" fill="#facc15"/>
                    <path d="M6 6L18 6M6 6L12 18M18 6L12 18" stroke="#1e3a8a" stroke-width="1.5" stroke-linecap="round"/>
                </svg>
            `; // Network nodes and connections

            const iconHighTechAI = `
                <svg class="w-16 h-16" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M12 2C6.477 2 2 6.477 2 12s4.477 10 10 10 10-4.477 10-10S17.523 2 12 2z" fill="#bfdbfe"/>
                    <path d="M12 4a8 8 0 00-8 8M12 4a8 8 0 018 8" stroke="#3b82f6" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M8 10L10 12L8 14M16 10L14 12L16 14" stroke="#10b981" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M10 10C10 9 10 9 10 9" stroke="#ef4444" stroke-width="1.5" stroke-linecap="round"/>
                    <path d="M14 10C14 9 14 9 14 9" stroke="#ef4444" stroke-width="1.5" stroke-linecap="round"/>
                    <circle cx="12" cy="12" r="1.5" fill="#1e3a8a"/>
                </svg>
            `; // Abstract AI brain/processing unit

            return `
                <!-- Service Section: 듀얼 핵심 솔루션 (Updated with Elaborate Icons) --><section class="py-16 bg-white rounded-3xl shadow-2xl">
                    <h2 class="text-5xl sm:text-6xl font-extrabold text-center mb-4 leading-tight">
                        <span class="gradient-text">BEST WORK의 듀얼 핵심 솔루션</span>
                    </h2>
                    <p class="text-center text-xl text-gray-700 mb-16 max-w-4xl mx-auto">
                        유학과 취업을 넘어 대한민국 정착까지, 외국인 인재의 전 여정을 함께하는 독보적인 전략을 제시합니다.
                    </p>

                    <div class="max-w-7xl mx-auto p-6">
                        
                        <!-- 1. Global Talent & University Connection - Richer Layout --><h3 class="text-4xl font-extrabold text-left text-primary mb-8 border-l-4 border-blue-600 pl-4">
                            01. 글로벌 인재 발굴 및 대학 연결 <span class="text-gray-500 text-xl font-normal">(Talent Acquisition & University Link)</span>
                        </h3>
                        
                        <!-- Feature + Monogram Grid --><div class="grid lg:grid-cols-3 gap-8 mb-16">
                            <!-- Feature 1: High-Tech Talent (Card with NEW Elaborate Icons) --><div class="service-card bg-blue-50 p-6 rounded-xl shadow-xl flex flex-col justify-between border-t-4 border-blue-600">
                                <div>
                                    <div class="icon-box bg-blue-600 text-white mb-4">
                                        <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.75 17L9.25 10m-.75 7a4 4 0 01-4-4v-3m.75 4a4 4 0 004 4m0-4h2.5M15.5 17l.75-7m-.75 7a4 4 0 01-4-4v-3m4 4a4 4 0 004 4m0-4h2.5M10.25 10v3m3.5-3v3M12 12h.01"></path></svg>
                                    </div>
                                    <h4 class="text-2xl font-bold text-primary mb-2">첨단 산업 이공계 인재</h4>
                                    <p class="text-gray-600 text-base">대학원 유학을 통해 한국의 핵심 성장 동력에 기여할 **우수 이공계 인재**를 발굴 및 양성합니다.</p>
                                </div>
                                <!-- Display multiple elaborate icons for High-Tech Talent --><div class="mt-5 p-4 bg-white rounded-lg shadow-inner flex justify-around items-center space-x-2">
                                    ${iconHighTechChips}
                                    ${iconHighTechNetwork}
                                    ${iconHighTechAI}
                                </div>
                            </div>

                            <!-- Feature 2: University Partnership (Card with Elaborate Icon) --><div class="service-card bg-blue-50 p-6 rounded-xl shadow-xl flex flex-col justify-between border-t-4 border-blue-600">
                                <div>
                                    <div class="icon-box bg-blue-600 text-white mb-4">
                                        <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14v7M12 3v2"></path></svg>
                                    </div>
                                    <h4 class="text-2xl font-bold text-primary mb-2">대학 유학생 연결 시스템</h4>
                                    <p class="text-gray-600 text-base">학업 성취 열망이 높은 유학생에게 **최적의 대한민국 대학교**를 추천 및 연결합니다.</p>
                                </div>
                                <!-- Elaborate SVG for University --><div class="mt-5 p-4 bg-white rounded-lg shadow-inner flex justify-center items-center">
                                    ${svgMonogramUniversity}
                                </div>
                            </div>

                            <!-- Feature 3: Global Network (Card with Elaborate Icon) --><div class="service-card bg-blue-50 p-6 rounded-xl shadow-xl flex flex-col justify-between border-t-4 border-blue-600">
                                <div>
                                    <div class="icon-box bg-blue-600 text-white mb-4">
                                        <svg class="w-7 h-7" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h14a2 2 0 012 2v14a2 2 0 01-2 2H5a2 2 0 01-2-2V5z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v18M3 12h18"></path></svg>
                                    </div>
                                    <h4 class="text-2xl font-bold text-primary mb-2">6대 전략 시장 확보</h4>
                                    <p class="text-gray-600 text-base">현지 네트워크와 경험을 바탕으로 **6대 거점 국가**의 우수한 인재를 안정적으로 확보합니다.</p>
                                </div>
                                <!-- Elaborate SVG for Global --><div class="mt-5 p-4 bg-white rounded-lg shadow-inner flex justify-center items-center">
                                    ${svgMonogramGlobal}
                                </div>
                            </div>
                        </div>

                        <!-- Separator --><div class="my-16 max-w-4xl mx-auto border-t-2 border-gray-200"></div>

                        <!-- 2. Life Cycle VISA Program - Richer Layout --><h3 class="text-4xl font-extrabold text-left text-primary mb-8 border-l-4 border-green-600 pl-4">
                            02. Life Cycle VISA Program 운영 <span class="text-gray-500 text-xl font-normal">(Settlement & VISA Roadmap)</span>
                        </h3>
                        
                        <!-- VISA Flow (Timeline with Large SVG) --><div class="grid lg:grid-cols-2 gap-10 items-center">
                            
                            <!-- Large SVG for VISA Roadmap --><div class="rounded-xl shadow-2xl overflow-hidden p-8 bg-white border border-green-200 order-last lg:order-first">
                                <!-- Enhanced SVG for Roadmap -->${svgMonogramVisaRoadmap}
                            </div>

                            <!-- VISA Timeline --><div class="space-y-8 relative pl-6 before:content-[''] before:absolute before:left-0 before:top-0 before:bottom-0 before:w-1 before:bg-green-300 order-first lg:order-last">
                                <p class="text-lg text-gray-700 font-medium pb-2">
                                    성공적인 한국 정착을 위한 <span class="text-green-600 font-bold">생애 주기 맞춤형 비자 로드맵</span>을 제공합니다.
                                </p>
                                
                                <!-- Phase 1: D-2/D-4 (유학/연수) --><div class="relative">
                                    <span class="absolute -left-3.5 top-1 w-7 h-7 bg-blue-600 rounded-full shadow-lg flex items-center justify-center text-white font-bold text-sm">1</span>
                                    <div class="bg-blue-50 p-5 rounded-xl shadow-lg ml-4 transition duration-300 hover:bg-blue-100">
                                        <h4 class="text-xl font-bold text-blue-700">D-2/D-4 (유학/연수)</h4>
                                        <p class="text-gray-600 text-sm mt-1">대학 입학, 한국어 연수 과정을 통한 초기 안정화 단계.</p>
                                    </div>
                                </div>

                                <!-- Phase 2: E-7 (전문 취업) --><div class="relative">
                                    <span class="absolute -left-3.5 top-1 w-7 h-7 bg-green-600 rounded-full shadow-lg flex items-center justify-center text-white font-bold text-sm">2</span>
                                    <div class="bg-green-50 p-5 rounded-xl shadow-lg ml-4 transition duration-300 hover:bg-green-100">
                                        <h4 class="text-xl font-bold text-green-700">E-7 (전문 취업)</h4>
                                        <p class="text-gray-600 text-sm mt-1">졸업 후 전문 직종 취업 연계 및 필수 비자 전환 지원.</p>
                                    </div>
                                </div>

                                <!-- Phase 3: F-2 (거주 비자) --><div class="relative">
                                    <span class="absolute -left-3.5 top-1 w-7 h-7 bg-primary rounded-full shadow-lg flex items-center justify-center text-white font-bold text-sm">3</span>
                                    <div class="bg-blue-50 p-5 rounded-xl shadow-lg ml-4 transition duration-300 hover:bg-blue-100">
                                        <h4 class="text-xl font-bold text-primary">F-2 (거주 비자)</h4>
                                        <p class="text-gray-600 text-sm mt-1">장기적인 대한민국 정착을 위한 최종 단계 컨설팅.</p>
                                    </div>
                                </div>

                                <p class="mt-6 text-sm text-gray-500 italic ml-4">
                                    *BEST WORK는 비자 전문가와의 협력을 통해 법률적 안정성을 확보합니다.
                                </p>
                            </div>
                        </div>
                    </div>
                </section>
            `;
        }

        // --- Affiliated Universities Page (NEW) ---
        function getAffiliatesPageContent() {
            // 로고 이미지 URL을 대학교 이니셜을 사용한 플레이스홀더로 교체했습니다.
            const universities = [
                // [로고 URL 구조] https://placehold.co/80x80/{배경색}/{글자색}?text={텍스트}
                { name: '건국대학교', tag: 'konkuk', location: '서울 광진구', 
                  logoUrl: 'https://placehold.co/80x80/1e3a8a/ffffff?text=KU', 
                  features: ['서울 중심 최고 입지', '공학 및 첨단 산업 분야 강세', '대규모 유학생 프로그램 운영'] },
                { name: '숙명여자대학교', tag: 'sookmyung', location: '서울 용산구', 
                  logoUrl: 'https://placehold.co/80x80/4f46e5/ffffff?text=SM', 
                  features: ['역사와 전통을 가진 명문 여대', '글로벌 리더 육성 특화 프로그램', '다양한 인문/사회/예술 분야 강세'] },
                { name: '서울신학대학교', tag: 'seoultheo', location: '경기 부천시', 
                  logoUrl: 'https://placehold.co/80x80/047857/ffffff?text=STU', 
                  features: ['기독교 정신 기반 인재 양성', '특성화된 학과 및 안정된 교육 환경', '글로벌 봉사 및 교류 활동 활발'] },
                { name: '한라대학교', tag: 'halla', location: '강원 원주시', 
                  logoUrl: 'https://placehold.co/80x80/9333ea/ffffff?text=HL', 
                  features: ['강원 지역 명문 사학', '미래 모빌리티/AI 등 특성화 교육', '산학 협력을 통한 취업 연계 강화'] },
                { name: '상지대학교', tag: 'sangji', location: '강원 원주시', 
                  logoUrl: 'https://placehold.co/80x80/ca8a04/ffffff?text=SJU', 
                  features: ['전통 있는 지역 사립 대학', '한의학과, 디자인 등 특성화 학과', '캠퍼스 내 안정적인 유학 생활 환경 제공'] },
                { name: '송호대학교', tag: 'songho', location: '강원 횡성군', 
                  logoUrl: 'https://placehold.co/80x80/dc2626/ffffff?text=SH', 
                  features: ['실무 중심의 전문 인재 양성', '지역 사회 맞춤형 교육 특화', 'BEST WORK와 국제교류 및 입학자원 발굴 협력'] },
            ];

            return `
                <section class="py-16 bg-white rounded-xl shadow-xl">
                    <h2 class="text-5xl font-extrabold text-center text-primary mb-16 border-b-4 border-blue-600 inline-block pb-2">BEST WORK 제휴 대학교</h2>
                    <p class="text-center text-xl text-gray-700 mb-10 max-w-4xl mx-auto">
                        BEST WORK는 우수한 유학생 유치를 위해 대한민국 전역의 명문 대학 및 특성화 대학과 공식적으로 협력하고 있습니다.
                    </p>
                    
                    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8 p-6">
                        ${universities.map(uni => `
                            <div class="university-card bg-gray-50 p-6 rounded-xl shadow-lg border-t-8 border-blue-400">
                                <div class="flex items-center mb-4">
                                    <!-- 로고 이미지로 교체 --><img src="${uni.logoUrl}" alt="${uni.name} 로고" class="w-12 h-12 rounded-full mr-4 shadow-md flex-shrink-0" 
                                         onerror="this.onerror=null; this.src='https://placehold.co/80x80/a1a1aa/ffffff?text=${uni.tag.toUpperCase()}'">
                                    <h3 class="text-2xl font-bold text-primary">${uni.name}</h3>
                                </div>
                                <p class="text-lg font-semibold text-gray-700 mb-3">${uni.location}</p>
                                <ul class="text-gray-600 space-y-2 list-none text-base">
                                    ${uni.features.map(feature => `
                                        <li class="flex items-start">
                                            <svg class="w-5 h-5 mr-2 text-blue-600 flex-shrink-0 mt-1" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.618a.999.999 0 011.414 0l1.414 1.414a.999.999 0 010 1.414L11.414 21H3v-8.414L18.586 3.414z"></path></svg>
                                            ${feature}
                                        </li>
                                    `).join('')}
                                </ul>
                                <a href="#contact" class="mt-4 inline-block text-blue-600 font-bold hover:underline">유학 프로그램 문의하기 &rarr;</a>
                            </div>
                        `).join('')}
                    </div>
                </section>
            `;
        }


        // --- Countries Page ---
        function getCountriesPageContent() {
            return `
                <!-- Major Countries Section --><section class="py-16 bg-white rounded-xl shadow-xl">
                    <h2 class="text-5xl font-extrabold text-center text-primary mb-16 border-b-4 border-blue-600 inline-block pb-2">주요 거점 국가: 6대 전략 시장</h2>
                    <p class="text-center text-xl text-gray-700 mb-10 max-w-3xl mx-auto">
                        BEST WORK는 현지 직접 진출 경험을 바탕으로, 각 국가의 인력 상황과 문화적 특성을 깊이 이해하고 있습니다.
                    </p>
                    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8 p-6">
                        
                        <!-- 네팔 (Nepal) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-green-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Nepal Flag">🇳🇵</span>
                                <h3 class="text-2xl font-bold text-primary">네팔 (Nepal)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**고용허가제 1위:** 근로자 수 1위 달성 국가로 인력 풍부.</li>
                                <li>**언어적 이점:** 영어 공용어, 한국어 어순 유사.</li>
                                <li>**인력 특성:** 성실하고 온건, 낮은 불법체류자 비율.</li>
                            </ul>
                        </div>
                        
                        <!-- 베트남 (Vietnam) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-blue-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Vietnam Flag">🇻🇳</span>
                                <h3 class="text-2xl font-bold text-primary">베트남 (Vietnam)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**경제 관계:** 대한민국 3대 교역국, 아세안 1위 교역국.</li>
                                <li>**문화적 동질성:** 유교 문화의 영향권 및 K-Culture 수용.</li>
                                <li>**교육 투자:** 가처분 소득의 20%를 교육에 투자하는 높은 교육열.</li>
                            </ul>
                        </div>
                        
                        <!-- 방글라데시 (Bangladesh) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-green-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Bangladesh Flag">🇧🇩</span>
                                <h3 class="text-2xl font-bold text-primary">방글라데시 (Bangladesh)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**청년 인구:** 세계 8위 인구 대국, 젊은 인력 잠재력 풍부.</li>
                                <li>**교육 환경:** 영어가 널리 사용되어 유학 적응 유리.</li>
                                <li>**인재 특성:** 높은 성실성과 근면성을 갖춘 우수 인재 공급 가능.</li>
                            </ul>
                        </div>
                        
                        <!-- 미얀마 (Myanmar) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-blue-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Myanmar Flag">🇲🇲</span>
                                <h3 class="text-2xl font-bold text-primary">미얀마 (Myanmar)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**성장 잠재력:** 동남아시아의 신흥 시장으로 발전 가능성 높음.</li>
                                <li>**K-Culture:** 한류에 대한 높은 관심, 문화적 이해도가 빠름.</li>
                                <li>**인력 규모:** 대규모의 젊은 노동력을 활용할 수 있는 잠재 시장.</li>
                            </ul>
                        </div>
                        
                        <!-- 스리랑카 (Sri Lanka) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-green-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Sri Lanka Flag">🇱🇰</span>
                                <h3 class="text-2xl font-bold text-primary">스리랑카 (Sri Lanka)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**높은 교육열:** 아시아 내 높은 문해율 및 이공계 유학 관심도 높음.</li>
                                <li>**노동 숙련도:** 해외 취업 경험이 풍부한 숙련된 인력 확보 용이.</li>
                            </ul>
                        </div>
                        
                        <!-- 몽골 (Mongolia) --><div class="bg-gray-50 p-6 rounded-xl shadow-lg border-l-8 border-blue-600 hover:shadow-xl transition duration-300">
                            <div class="flex items-center mb-3">
                                <span class="text-3xl mr-3" role="img" aria-label="Mongolia Flag">🇲🇳</span>
                                <h3 class="text-2xl font-bold text-primary">몽골 (Mongolia)</h3>
                            </div>
                            <ul class="text-gray-600 space-y-2 list-disc list-inside text-base ml-4">
                                <li>**친숙도:** 한국어 능력자가 많고 한국말만으로 생활 가능 수준.</li>
                                <li>**경험 인력:** 인구의 10% 가량이 한국 노동 경험 보유.</li>
                            </ul>
                        </div>
                    </div>
                </section>
            `;
        }

        // --- Contact Page ---
        function getContactPageContent() {
            return `
                <!-- Contact Section --><section class="py-16 bg-white rounded-xl shadow-xl">
                    <h2 class="text-5xl font-extrabold text-center text-primary mb-16 border-b-4 border-blue-600 inline-block pb-2">문의하기</h2>
                    
                    <div class="grid md:grid-cols-2 gap-10 max-w-4xl mx-auto p-6">
                        
                        <!-- 연락처 정보 --><div class="p-8 rounded-xl shadow-xl bg-primary text-white flex flex-col justify-center">
                            <h3 class="text-3xl font-bold mb-6 text-green-400 border-b border-blue-700 pb-3">Contact Information</h3>
                            
                            <div class="space-y-6">
                                <div class="flex items-start space-x-4">
                                    <svg class="w-8 h-8 text-green-400 flex-shrink-0 mt-1" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 5.26c.45.3.9.3 1.35 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"></path></svg>
                                    <div>
                                        <p class="text-sm text-gray-300">대표 이메일 (파트너십 / 제휴 문의)</p>
                                        <a href="mailto:koreabestwork@gmail.com" class="text-xl font-semibold hover:underline text-white break-words">koreabestwork@gmail.com</a>
                                    </div>
                                </div>
                                
                                <div class="flex items-start space-x-4">
                                    <svg class="w-8 h-8 text-green-400 flex-shrink-0 mt-1" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.828 0l-4.243-4.243a8 8 0 1111.314 0z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z"></path></svg>
                                    <div>
                                        <p class="text-sm text-gray-300">주소</p>
                                        <p class="text-white text-base font-semibold">서울특별시 마포구 월드컵로 196, B105-690호</p>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- 문의 폼 (Mock-up) --><div class="bg-gray-50 p-8 rounded-xl shadow-lg border-t-8 border-green-600">
                            <h3 class="text-3xl font-bold mb-6 text-primary">온라인 상담 신청</h3>
                            <form onsubmit="handleFormSubmit(event)">
                                <div class="mb-4">
                                    <label for="name" class="block text-gray-700 font-semibold mb-2">성함/기관명</label>
                                    <input type="text" id="name" name="name" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-blue-600 focus:border-blue-600" required>
                                </div>
                                <div class="mb-6">
                                    <label for="message" class="block text-gray-700 font-semibold mb-2">문의 내용</label>
                                    <textarea id="message" name="message" rows="5" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:ring-blue-600 focus:border-blue-600" required></textarea>
                                </div>
                                <button type="submit" class="w-full bg-blue-600 text-white font-bold py-3 rounded-lg hover:bg-blue-700 transition duration-300 shadow-md text-lg">문의 접수하기</button>
                            </form>
                            <!-- Custom Message Box for form submission --><div id="message-box" class="mt-4 p-4 text-center bg-green-100 text-green-800 rounded-lg hidden font-semibold"></div>
                        </div>
                    </div>
                </section>
            `;
        }
        
        // Dummy function for form submission (Prevents alert/confirm)
        function handleFormSubmit(event) {
            event.preventDefault();
            const messageBox = document.getElementById('message-box');
            messageBox.textContent = '문의가 성공적으로 접수되었습니다. 최대한 빠르게 연락드리겠습니다. 감사합니다.';
            messageBox.classList.remove('hidden', 'bg-red-100', 'text-red-800');
            messageBox.classList.add('bg-green-100', 'text-green-800');
            event.target.reset(); // Clear form
            setTimeout(() => {
                messageBox.classList.add('hidden');
            }, 5000);
        }

        /**
         * 2-2. SPA Navigation Logic
         */
        const routes = {
            'home': { content: getHomePageContent, title: 'Home' },
            'about': { content: getAboutPageContent, title: '회사 소개 및 비전' },
            'service': { content: getServicePageContent, title: '핵심 서비스 전략' },
            'affiliates': { content: getAffiliatesPageContent, title: '제휴 대학교' }, // New Route
            'countries': { content: getCountriesPageContent, title: '주요 거점 국가' },
            'contact': { content: getContactPageContent, title: '문의하기' },
        };

        function updateActiveNav(currentHash) {
            const navLinks = document.querySelectorAll('.nav-link, .mobile-nav-link');
            navLinks.forEach(link => {
                const linkHash = link.getAttribute('href').substring(1);
                
                // Reset styles
                link.classList.remove('active', 'text-blue-600', 'font-bold');
                link.classList.add('text-gray-600', 'font-medium');

                // Apply active style
                if (linkHash === currentHash) {
                    link.classList.add('active', 'text-blue-600', 'font-bold');
                    link.classList.remove('text-gray-600');
                }
            });
        }

        function closeMobileMenu() {
            const menuButton = document.getElementById('menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            if (!mobileMenu.classList.contains('hidden')) {
                menuButton.setAttribute('aria-expanded', 'false');
                mobileMenu.classList.add('hidden');
            }
        }

        function navigate() {
            const hash = window.location.hash.substring(1) || 'home';
            const route = routes[hash] || routes['home'];
            
            // Apply page transition effect
            contentDiv.style.opacity = 0;
            setTimeout(() => {
                contentDiv.innerHTML = route.content();
                contentDiv.style.opacity = 1;

                document.title = `BEST WORK - ${route.title}`;
                
                updateActiveNav(hash);
                closeMobileMenu(); // Close menu on navigation

                window.scrollTo({ top: 0, behavior: 'smooth' });
            }, 150); // Delay for fade effect
        }

        // Initialize mobile menu toggle logic
        document.addEventListener('DOMContentLoaded', () => {
            const menuButton = document.getElementById('menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const navLinks = document.querySelectorAll('.mobile-nav-link, .nav-link-logo');

            menuButton.addEventListener('click', () => {
                const isExpanded = menuButton.getAttribute('aria-expanded') === 'true' || false;
                menuButton.setAttribute('aria-expanded', !isExpanded);
                mobileMenu.classList.toggle('hidden');
            });

            // Ensure navigation links in the mobile menu close the menu
            navLinks.forEach(link => {
                link.addEventListener('click', closeMobileMenu);
            });

            // Initialize routing
            window.addEventListener('load', navigate);
            window.addEventListener('hashchange', navigate);

            if (!window.location.hash) {
                window.location.hash = '#home';
            }
        });
    </script>
</body>
</html>
