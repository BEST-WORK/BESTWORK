<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>BESTWORK - 한국 유학 전문가</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Inter Font -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            scroll-behavior: smooth;
        }
        .icon-small {
            width: 20px;
            height: 20px;
            stroke-width: 2;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Header & Navigation -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <a href="#" class="text-3xl font-extrabold text-indigo-700 tracking-tight rounded-lg p-1">BESTWORK</a>
            
            <!-- Desktop Navigation -->
            <nav class="hidden md:flex space-x-8">
                <a href="#about" class="text-gray-600 hover:text-indigo-600 font-medium transition duration-150 rounded-lg p-2">회사 소개</a>
                <a href="#program" class="text-gray-600 hover:text-indigo-600 font-medium transition duration-150 rounded-lg p-2">유학 프로그램</a>
                <a href="#partners" class="text-gray-600 hover:text-indigo-600 font-medium transition duration-150 rounded-lg p-2">파트너 대학</a>
                <a href="#contact" class="text-white bg-indigo-600 hover:bg-indigo-700 font-semibold py-2 px-4 rounded-full shadow-lg transition duration-150 transform hover:scale-105">무료 상담 신청</a>
            </nav>

            <!-- Mobile Menu Button (Hamburger) -->
            <button id="mobile-menu-button" class="md:hidden text-gray-600 hover:text-indigo-600 p-2 rounded-lg transition duration-150">
                <i data-lucide="menu" class="w-6 h-6"></i>
            </button>
        </div>
        
        <!-- Mobile Navigation (Hidden by default) -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100">
            <nav class="flex flex-col px-4 pt-2 pb-4 space-y-2">
                <a href="#about" class="text-gray-600 hover:bg-gray-100 p-3 rounded-lg font-medium">회사 소개</a>
                <a href="#program" class="text-gray-600 hover:bg-gray-100 p-3 rounded-lg font-medium">유학 프로그램</a>
                <a href="#partners" class="text-gray-600 hover:bg-gray-100 p-3 rounded-lg font-medium">파트너 대학</a>
                <a href="#contact" class="text-indigo-600 hover:bg-indigo-50 p-3 rounded-lg font-medium border border-indigo-200">무료 상담 신청</a>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-white py-20 sm:py-32 overflow-hidden">
        <div class="absolute inset-0 bg-cover bg-center opacity-10" style="background-image: url('https://placehold.co/1920x1080/4F46E5/ffffff?text=Seoul+Skyline');"></div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="lg:w-3/5">
                <p class="text-xl font-semibold text-indigo-600 mb-4 animate-fadeInUp">아시아를 넘어, 한국의 명문대로!</p>
                <h1 class="text-5xl sm:text-6xl lg:text-7xl font-extrabold leading-tight text-gray-900 mb-6">
                    네팔, 스리랑카 학생들을 위한 <span class="text-indigo-600">한국 유학의 꿈</span>을 현실로
                </h1>
                <p class="text-xl text-gray-600 mb-10 max-w-lg">
                    BESTWORK는 네팔, 방글라데시, 스리랑카, 파키스탄 유학생들이 한국의 명문 대학교에 성공적으로 진학하도록 돕는 전문 유학원입니다.
                </p>
                <div class="flex flex-col sm:flex-row space-y-4 sm:space-y-0 sm:space-x-4">
                    <a href="#contact" class="inline-flex items-center justify-center px-8 py-4 border border-transparent text-lg font-bold rounded-full shadow-xl text-white bg-indigo-600 hover:bg-indigo-700 transition duration-300 transform hover:scale-105">
                        <i data-lucide="graduation-cap" class="w-6 h-6 mr-2"></i>
                        나만의 유학 계획 시작하기
                    </a>
                    <a href="#partners" class="inline-flex items-center justify-center px-8 py-4 border border-indigo-600 text-lg font-bold rounded-full text-indigo-600 bg-white hover:bg-indigo-50 transition duration-300 transform hover:scale-105">
                        파트너 대학 살펴보기
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Target Countries Section -->
    <section class="py-16 sm:py-24 bg-indigo-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl sm:text-4xl font-extrabold text-gray-900 mb-12">우리의 유학 네트워크</h2>
            <p class="text-xl text-indigo-700 mb-8">네팔, 방글라데시, 스리랑카, 파키스탄 학생들의 성공적인 유학을 지원합니다.</p>
            
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
                <!-- Nepal -->
                <div class="bg-white p-6 rounded-2xl shadow-lg hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <img src="https://placehold.co/100x70/E5E7EB/4F46E5?text=NEPAL" alt="네팔 국기" class="rounded-lg w-full h-auto mb-4 object-cover">
                    <h3 class="text-2xl font-bold text-gray-900">네팔 (Nepal)</h3>
                    <p class="text-gray-500 mt-2">한국 유학의 꿈이 시작되는 곳</p>
                </div>
                <!-- Bangladesh -->
                <div class="bg-white p-6 rounded-2xl shadow-lg hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <img src="https://placehold.co/100x70/E5E7EB/4F46E5?text=BANGLADESH" alt="방글라데시 국기" class="rounded-lg w-full h-auto mb-4 object-cover">
                    <h3 class="text-2xl font-bold text-gray-900">방글라데시</h3>
                    <p class="text-gray-500 mt-2">밝은 미래를 위한 교두보</p>
                </div>
                <!-- Sri Lanka -->
                <div class="bg-white p-6 rounded-2xl shadow-lg hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <img src="https://placehold.co/100x70/E5E7EB/4F46E5?text=SRI+LANKA" alt="스리랑카 국기" class="rounded-lg w-full h-auto mb-4 object-cover">
                    <h3 class="text-2xl font-bold text-gray-900">스리랑카</h3>
                    <p class="text-gray-500 mt-2">글로벌 인재 양성</p>
                </div>
                <!-- Pakistan -->
                <div class="bg-white p-6 rounded-2xl shadow-lg hover:shadow-2xl transition duration-300 transform hover:-translate-y-1">
                    <img src="https://placehold.co/100x70/E5E7EB/4F46E5?text=PAKISTAN" alt="파키스탄 국기" class="rounded-lg w-full h-auto mb-4 object-cover">
                    <h3 class="text-2xl font-bold text-gray-900">파키스탄</h3>
                    <p class="text-gray-500 mt-2">성공적인 커리어 설계</p>
                </div>
            </div>
        </div>
    </section>


    <!-- Partner Universities Section -->
    <section id="partners" class="py-16 sm:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl sm:text-5xl font-extrabold text-gray-900">파트너 대학 네트워크</h2>
                <p class="mt-4 text-xl text-gray-600">BESTWORK가 연결하는 한국의 명문 대학교들을 만나보세요.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- University Card 1: 숙명여대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">숙명여자대학교 (Sookmyung Women's University)</h3>
                        <p class="mt-2 text-gray-500">대한민국을 이끄는 명문 사학. 여성 리더를 양성하는 최고의 교육 환경을 제공합니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">서울</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>

                <!-- University Card 2: 건국대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">건국대학교 (Konkuk University)</h3>
                        <p class="mt-2 text-gray-500">최첨단 연구와 실용 학문으로 명성이 높은 서울 중심의 종합 대학입니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">서울</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>

                <!-- University Card 3: 서울신학대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">서울신학대학교 (Seoul Theological University)</h3>
                        <p class="mt-2 text-gray-500">기독교 정신을 바탕으로 사회를 이끌 인재를 양성하는 유서 깊은 대학입니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">경기 부천</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>

                <!-- University Card 4: 한라대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">한라대학교 (Halla University)</h3>
                        <p class="mt-2 text-gray-500">강원도의 중심에서 산학 협력과 취업에 강한 실무 중심의 교육을 제공합니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">강원 원주</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>

                <!-- University Card 5: 상지대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">상지대학교 (Sangji University)</h3>
                        <p class="mt-2 text-gray-500">자연 친화적 환경에서 인문, 사회, 공학 등 다양한 분야의 전문성을 키웁니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">강원 원주</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>

                <!-- University Card 6: 송호대 -->
                <div class="bg-white border border-gray-100 rounded-2xl shadow-lg overflow-hidden group hover:shadow-xl transition duration-300">
                    <div class="p-6">
                        <i data-lucide="building" class="text-indigo-600 w-8 h-8 mb-3"></i>
                        <h3 class="text-2xl font-bold text-gray-900">송호대학교 (Songho University)</h3>
                        <p class="mt-2 text-gray-500">실용적이고 전문적인 교육을 통해 현장에 바로 투입될 수 있는 인재를 양성합니다.</p>
                    </div>
                    <div class="bg-indigo-50 p-4 flex justify-between items-center">
                         <span class="text-sm font-semibold text-indigo-700">강원 횡성</span>
                         <a href="#contact" class="text-indigo-600 hover:text-indigo-800 font-medium text-sm">자세히 보기 <i data-lucide="arrow-right" class="icon-small inline-block ml-1"></i></a>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Program/Process Section -->
    <section id="program" class="py-16 sm:py-24 bg-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-4xl sm:text-5xl font-extrabold text-gray-900">BESTWORK의 유학 성공 프로세스</h2>
                <p class="mt-4 text-xl text-gray-600">성공적인 한국 유학을 위한 단계별 맞춤 서비스를 제공합니다.</p>
            </div>

            <ol class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-5 gap-8">
                <!-- Step 1 -->
                <li class="relative p-6 bg-white rounded-2xl shadow-xl border-t-4 border-indigo-600 transition duration-300 hover:shadow-2xl">
                    <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 bg-indigo-600 text-white w-12 h-12 flex items-center justify-center rounded-full text-xl font-bold shadow-lg">1</div>
                    <h3 class="text-xl font-bold mt-4 text-gray-900">개별 상담 및 진로 설정</h3>
                    <p class="mt-2 text-gray-500 text-sm">학생의 배경과 목표에 맞는 최적의 대학 및 전공을 추천합니다.</p>
                </li>
                 <!-- Separator on desktop -->
                 <div class="hidden lg:block relative">
                    <div class="h-1 w-full bg-indigo-200 absolute top-1/2 transform -translate-y-1/2"></div>
                </div>

                <!-- Step 2 -->
                <li class="relative p-6 bg-white rounded-2xl shadow-xl border-t-4 border-indigo-600 transition duration-300 hover:shadow-2xl">
                    <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 bg-indigo-600 text-white w-12 h-12 flex items-center justify-center rounded-full text-xl font-bold shadow-lg">2</div>
                    <h3 class="text-xl font-bold mt-4 text-gray-900">서류 준비 및 번역</h3>
                    <p class="mt-2 text-gray-500 text-sm">복잡한 지원 서류를 완벽하게 준비하고 전문적인 번역을 지원합니다.</p>
                </li>
                 <!-- Separator on desktop -->
                 <div class="hidden lg:block relative">
                    <div class="h-1 w-full bg-indigo-200 absolute top-1/2 transform -translate-y-1/2"></div>
                </div>

                <!-- Step 3 -->
                <li class="relative p-6 bg-white rounded-2xl shadow-xl border-t-4 border-indigo-600 transition duration-300 hover:shadow-2xl">
                    <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 bg-indigo-600 text-white w-12 h-12 flex items-center justify-center rounded-full text-xl font-bold shadow-lg">3</div>
                    <h3 class="text-xl font-bold mt-4 text-gray-900">대학 지원 및 비자 절차</h3>
                    <p class="mt-2 text-gray-500 text-sm">파트너 대학에 직접 지원하고 비자 발급을 위한 모든 절차를 대행합니다.</p>
                </li>
                 <!-- Separator on desktop -->
                 <div class="hidden lg:block relative">
                    <div class="h-1 w-full bg-indigo-200 absolute top-1/2 transform -translate-y-1/2"></div>
                </div>

                <!-- Step 4 -->
                <li class="relative p-6 bg-white rounded-2xl shadow-xl border-t-4 border-indigo-600 transition duration-300 hover:shadow-2xl">
                    <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 bg-indigo-600 text-white w-12 h-12 flex items-center justify-center rounded-full text-xl font-bold shadow-lg">4</div>
                    <h3 class="text-xl font-bold mt-4 text-gray-900">출국 및 초기 정착 지원</h3>
                    <p class="mt-2 text-gray-500 text-sm">한국 입국 후 공항 픽업, 기숙사 안내 등 초기 정착을 돕습니다.</p>
                </li>
                 <!-- Separator on desktop -->
                 <div class="hidden lg:block relative">
                    <div class="h-1 w-full bg-indigo-200 absolute top-1/2 transform -translate-y-1/2"></div>
                </div>

                <!-- Step 5 -->
                <li class="relative p-6 bg-white rounded-2xl shadow-xl border-t-4 border-indigo-600 transition duration-300 hover:shadow-2xl">
                    <div class="absolute -top-6 left-1/2 transform -translate-x-1/2 bg-indigo-600 text-white w-12 h-12 flex items-center justify-center rounded-full text-xl font-bold shadow-lg">5</div>
                    <h3 class="text-xl font-bold mt-4 text-gray-900">지속적인 학업 관리</h3>
                    <p class="mt-2 text-gray-500 text-sm">유학 중에도 한국 생활 및 학업에 필요한 상담을 지속적으로 제공합니다.</p>
                </li>
            </ol>
            
            <div class="text-center mt-16">
                <a href="#contact" class="inline-flex items-center justify-center px-8 py-4 text-xl font-bold rounded-full shadow-lg text-white bg-green-500 hover:bg-green-600 transition duration-300 transform hover:scale-105">
                    <i data-lucide="check-circle" class="w-6 h-6 mr-2"></i>
                    지금 바로 1:1 맞춤 상담 신청하기
                </a>
            </div>

        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-16 sm:py-24">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col lg:flex-row items-center gap-12">
            <div class="lg:w-1/2">
                <p class="text-base font-semibold text-indigo-600 uppercase mb-2">ABOUT BESTWORK</p>
                <h2 class="text-4xl sm:text-5xl font-extrabold text-gray-900 mb-6">최고의 교육 연결을 위한 약속</h2>
                <p class="mt-4 text-lg text-gray-600 leading-relaxed">
                    BESTWORK는 한국 교육 시스템에 대한 깊은 이해와 네팔, 방글라데시, 스리랑카, 파키스탄 현지 학생들에 대한 맞춤형 접근 방식을 결합하여 성공적인 유학 경로를 제시합니다.
                </p>
                <p class="mt-4 text-lg text-gray-600 leading-relaxed">
                    우리는 단순한 유학 대행을 넘어, 학생들이 한국에서 학업을 마치고 글로벌 인재로 성장할 수 있도록 **비전 제시부터 정착까지** 전 과정을 책임집니다. 숙명여대, 건국대 등 명문 대학과의 직접적인 협력 관계를 통해 가장 신뢰할 수 있는 정보를 제공합니다.
                </p>
            </div>
            <div class="lg:w-1/2 w-full">
                <img src="https://placehold.co/600x400/A5B4FC/ffffff?text=Global+Education" alt="글로벌 교육 환경 이미지" class="rounded-3xl shadow-2xl w-full h-auto object-cover">
            </div>
        </div>
    </section>

    <!-- Call to Action / Contact Form -->
    <section id="contact" class="py-16 sm:py-24 bg-indigo-700">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12">
                <h2 class="text-4xl sm:text-5xl font-extrabold text-white">무료 맞춤 상담을 시작하세요</h2>
                <p class="mt-4 text-xl text-indigo-200">여러분의 한국 유학 목표를 알려주시면, 전문 컨설턴트가 빠르게 연락드립니다.</p>
            </div>
            
            <div class="max-w-xl mx-auto bg-white p-8 sm:p-10 rounded-3xl shadow-2xl">
                <form action="#" method="POST" class="space-y-6">
                    <div>
                        <label for="name" class="block text-sm font-medium text-gray-700">이름</label>
                        <input type="text" name="name" id="name" required
                               class="mt-1 block w-full px-4 py-3 border border-gray-300 rounded-xl shadow-sm focus:ring-indigo-500 focus:border-indigo-500 placeholder-gray-400"
                               placeholder="성함 또는 영문 이름">
                    </div>
                    <div>
                        <label for="country" class="block text-sm font-medium text-gray-700">거주 국가</label>
                        <select id="country" name="country" required
                                class="mt-1 block w-full px-4 py-3 border border-gray-300 rounded-xl shadow-sm focus:ring-indigo-500 focus:border-indigo-500">
                            <option value="">선택하세요</option>
                            <option value="Nepal">네팔</option>
                            <option value="Bangladesh">방글라데시</option>
                            <option value="Sri Lanka">스리랑카</option>
                            <option value="Pakistan">파키스탄</option>
                            <option value="Other">기타</option>
                        </select>
                    </div>
                    <div>
                        <label for="email" class="block text-sm font-medium text-gray-700">이메일 주소</label>
                        <input type="email" name="email" id="email" required
                               class="mt-1 block w-full px-4 py-3 border border-gray-300 rounded-xl shadow-sm focus:ring-indigo-500 focus:border-indigo-500 placeholder-gray-400"
                               placeholder="예: student@example.com">
                    </div>
                    <div>
                        <label for="message" class="block text-sm font-medium text-gray-700">문의 내용</label>
                        <textarea id="message" name="message" rows="4"
                                  class="mt-1 block w-full px-4 py-3 border border-gray-300 rounded-xl shadow-sm focus:ring-indigo-500 focus:border-indigo-500 placeholder-gray-400"
                                  placeholder="궁금한 점이나 원하는 프로그램에 대해 간략히 적어주세요."></textarea>
                    </div>
                    <button type="submit" class="w-full flex justify-center py-3 px-4 border border-transparent rounded-full shadow-md text-lg font-bold text-white bg-indigo-600 hover:bg-indigo-700 transition duration-150 transform hover:scale-[1.01]">
                        상담 요청서 제출하기
                    </button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid grid-cols-2 md:grid-cols-4 gap-8 border-b border-gray-700 pb-8 mb-8">
                <!-- Logo/Contact -->
                <div>
                    <h3 class="text-2xl font-extrabold text-indigo-400 mb-3">BESTWORK</h3>
                    <p class="text-sm text-gray-400">한국 유학 전문가</p>
                    <p class="text-sm text-gray-400 mt-4 flex items-center"><i data-lucide="mail" class="icon-small mr-2 text-indigo-400"></i> info@bestwork.com</p>
                    <p class="text-sm text-gray-400 mt-2 flex items-center"><i data-lucide="phone" class="icon-small mr-2 text-indigo-400"></i> +82 (0)XX-XXXX-XXXX</p>
                </div>

                <!-- Quick Links -->
                <div>
                    <h4 class="text-lg font-semibold mb-4">바로가기</h4>
                    <ul class="space-y-2">
                        <li><a href="#about" class="text-gray-400 hover:text-indigo-400 text-sm transition">회사 소개</a></li>
                        <li><a href="#program" class="text-gray-400 hover:text-indigo-400 text-sm transition">유학 프로그램</a></li>
                        <li><a href="#partners" class="text-gray-400 hover:text-indigo-400 text-sm transition">파트너 대학</a></li>
                    </ul>
                </div>

                <!-- Partner Countries -->
                <div>
                    <h4 class="text-lg font-semibold mb-4">주요 국가</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li>네팔 (Nepal)</li>
                        <li>방글라데시 (Bangladesh)</li>
                        <li>스리랑카 (Sri Lanka)</li>
                        <li>파키스탄 (Pakistan)</li>
                    </ul>
                </div>

                <!-- Partner Universities List -->
                <div>
                    <h4 class="text-lg font-semibold mb-4">주요 파트너</h4>
                    <ul class="space-y-2 text-sm text-gray-400">
                        <li>숙명여대, 건국대, 서울신학대</li>
                        <li>한라대, 상지대, 송호대</li>
                    </ul>
                </div>
            </div>

            <div class="text-center pt-8">
                <p class="text-sm text-gray-500">&copy; 2024 BESTWORK. All rights reserved. | 대한민국 서울</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript for Mobile Menu and Icons -->
    <script>
        // Lucide Icons setup
        lucide.createIcons();

        // Mobile Menu Toggle
        document.getElementById('mobile-menu-button').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });

        // Simple form submission handler (prevent default for demo)
        document.querySelector('#contact form').addEventListener('submit', function(e) {
            e.preventDefault();
            // In a real application, you would send this data to a server
            const form = e.target;
            const name = form.elements.name.value;
            
            // Display a non-alert message
            const messageBox = document.createElement('div');
            messageBox.innerHTML = `
                <div class="fixed inset-0 bg-gray-600 bg-opacity-75 flex items-center justify-center z-50 transition-opacity duration-300" id="submit-modal">
                    <div class="bg-white p-8 rounded-xl shadow-2xl max-w-sm w-full text-center transform transition-transform duration-300 scale-100">
                        <i data-lucide="check-circle" class="w-12 h-12 text-green-500 mx-auto mb-4"></i>
                        <h3 class="text-2xl font-bold text-gray-900 mb-3">상담 요청이 접수되었습니다!</h3>
                        <p class="text-gray-600 mb-6">${name}님, 곧 연락드리겠습니다. BESTWORK와 함께 꿈을 펼치세요!</p>
                        <button type="button" onclick="document.getElementById('submit-modal').remove()" class="bg-indigo-600 text-white font-semibold py-2 px-6 rounded-full hover:bg-indigo-700 transition">확인</button>
                    </div>
                </div>
            `;
            document.body.appendChild(messageBox);
            lucide.createIcons(); // Re-render icons in the new modal
            form.reset();
        });
    </script>

</body>
</html>
