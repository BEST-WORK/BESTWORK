<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>BEST WORK - 외국인 유학생 및 취업 컨설팅</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    * { margin:0; padding:0; box-sizing:border-box; }
    html, body { width:100%; height:100%; overflow-x:hidden; font-family:-apple-system,BlinkMacSystemFont,"Inter","Helvetica Neue",Arial,sans-serif; }

    /* 배너형 흐르는 텍스트 */
    .marquee {
      position:fixed; top:0; left:0;
      width:100%; background:#0b76ef;
      color:#fff; overflow:hidden;
      white-space:nowrap; z-index:2000;
      font-weight:700; letter-spacing:1px;
      font-size:16px; padding:6px 0;
    }
    .marquee span {
      display:inline-block;
      animation: marquee 18s linear infinite;
    }
    @keyframes marquee {
      from { transform:translateX(100%); }
      to { transform:translateX(-100%); }
    }

    /* Navbar */
    .navbar {
      position:fixed; top:30px; left:0; width:100%;
      background:rgba(11,18,32,0.95); color:#fff;
      display:flex; justify-content:space-between; align-items:center;
      padding:15px 20px; z-index:1000;
    }
    .navbar-brand { font-size:24px; font-weight:900; color:#fff; text-decoration:none; }
    .menu-toggle {
      display:none; flex-direction:column; justify-content:space-between;
      width:25px; height:18px; cursor:pointer;
    }
    .menu-toggle span { height:3px; width:100%; background:#fff; border-radius:3px; }

    .navbar-links {
      display:flex; gap:25px; align-items:center;
    }
    .navbar-links a {
      color:#fff; text-decoration:none; font-weight:600; transition:color .3s;
    }
    .navbar-links a:hover { color:#0b76ef; }

    @media (max-width:768px){
      .menu-toggle{display:flex;}
      .navbar-links{
        display:none; position:fixed; top:80px; left:0; width:100%;
        height:calc(100vh - 80px); background:rgba(11,18,32,0.98);
        flex-direction:column; justify-content:start; align-items:center;
        padding-top:40px; gap:30px;
      }
      .navbar-links.active{display:flex;animation:fadeIn .3s ease-in-out;}
      @keyframes fadeIn{from{opacity:0;transform:translateY(-10px);}to{opacity:1;transform:translateY(0);}}
    }

    /* Header */
    header {
      width:100%; height:100vh;
      background:url('https://github.com/BEST-WORK/BESTWORK/blob/main/Adobe%20Express%20-%20IMG_8171%20(1).gif?raw=true') center/cover repeat fixed;
      display:flex; justify-content:center; align-items:center;
      text-align:center; color:#fff; position:relative; overflow:hidden;
    }
    header::before {
      content:""; position:absolute; top:0; left:0; width:100%; height:100%;
      background:rgba(0,0,0,0.45);
    }
    header .overlay { position:relative; z-index:2; max-width:800px; padding:20px; }

    @keyframes fadeZoomIn {0%{transform:scale(0.5);opacity:0;}100%{transform:scale(1);opacity:1;}}
    @keyframes fadeUp {0%{opacity:0;transform:translateY(30px);}100%{opacity:1;transform:translateY(0);}}

    .logo { font-size:60px; font-weight:900; text-shadow:0 6px 14px rgba(0,0,0,0.7); animation:fadeZoomIn 2s ease-out forwards; }
    header h1 { font-size:30px; font-weight:800; text-shadow:0 4px 12px rgba(0,0,0,0.6); animation:fadeUp 2.2s ease-out forwards; animation-delay:0.5s; opacity:0; }
    header p { font-size:18px; color:#e0e0e0; margin:20px 0; line-height:1.6; animation:fadeUp 2.5s ease-out forwards; animation-delay:0.8s; opacity:0; }
    .btn {
      display:inline-block; background:#fff; color:#0b76ef; padding:12px 24px; border-radius:8px; font-weight:700; text-decoration:none;
      transition:background .3s; animation:fadeUp 2.8s ease-out forwards; animation-delay:1.1s; opacity:0;
    }
    .btn:hover { background:#e8e8e8; }

    /* Scroll animation */
    [data-scroll] { opacity:0; transform:translateY(40px); transition:all .8s ease-out; }
    [data-scroll].visible { opacity:1; transform:translateY(0); }

    /* Section */
    section { width:100%; padding:80px 20px; text-align:center; }
    h2 { font-size:26px; margin-bottom:20px; }
    .container { max-width:1100px; margin:0 auto; }

    /* Services Section */
    #services {
      background:url('https://github.com/BEST-WORK/BESTWORK/blob/main/IMG_8690.gif?raw=true') center/cover fixed;
      position:relative; color:#fff;
    }
    #services::before {
      content:""; position:absolute; top:0; left:0; width:100%; height:100%;
      background:rgba(0,0,0,0.6); z-index:1;
    }
    #services .container>* { position:relative; z-index:2; }
    .service-grid { display:flex; flex-wrap:wrap; justify-content:center; gap:30px; margin-top:40px; }
    .service-item { width:280px; padding:20px; text-align:center; background:rgba(255,255,255,0.1); border-radius:12px; backdrop-filter:blur(3px); transition:transform .3s; }
    .service-item:hover { transform:translateY(-5px); }
    .service-item h3 { font-size:20px; font-weight:700; margin-bottom:10px; }

    /* Cards */
    .card-grid { display:grid; grid-template-columns:repeat(auto-fit,minmax(280px,1fr)); gap:20px; margin-top:30px; }
    .uni-card {
      background:#fff; border-radius:12px; padding:25px; text-align:left;
      box-shadow:0 6px 15px rgba(0,0,0,0.08); transition:transform .3s;
    }
    .uni-card:hover{transform:translateY(-5px);}

    /* Countries */
    .country-card {
      border-radius:12px; padding:25px; color:#fff; text-align:left;
      box-shadow:0 6px 15px rgba(0,0,0,0.2); transition:transform .3s;
    }
    .country-card:hover{transform:translateY(-5px);}
    .flag { font-size:35px; margin-bottom:10px; display:block; }
    .card-nepal { background:linear-gradient(135deg,#231F20,#E83F3F); }
    .card-bangladesh { background:linear-gradient(135deg,#006A4E,#F42A41); }
    .card-myanmar { background:linear-gradient(135deg,#FECB00,#34B233,#EA2839); }
    .card-srilanka { background:linear-gradient(135deg,#D4AF37,#FF8C00); }
    .card-vietnam { background:linear-gradient(135deg,#DA251D,#D61A13); }

    /* Contact */
    form { text-align:left; max-width:500px; margin:0 auto; }
    label { font-weight:600; display:block; margin-bottom:5px; }
    input, textarea {
      width:100%; padding:10px; margin-bottom:15px;
      border:1px solid #ccc; border-radius:6px; font-size:16px;
    }
    button[type=submit] {
      width:100%; background:#0b76ef; color:#fff; border:none;
      border-radius:8px; padding:12px; font-size:16px; font-weight:700;
      cursor:pointer; transition:background .3s;
    }
    button[type=submit]:hover{background:#0959bb;}

    /* Footer */
    footer { background:#0b1220; color:#dfefff; text-align:center; padding:40px 0; }
    .social-links { display:flex; justify-content:center; gap:30px; margin-top:20px; }
    .social-links a { font-size:32px; color:#999; text-decoration:none; transition:color .3s; }
    .social-links a:hover { color:#0b76ef; }

    @media(max-width:768px){
      .logo{font-size:42px;}
      header h1{font-size:24px;}
    }
  </style>
</head>
<body>
  <!-- 배너 텍스트 -->
  <div class="marquee"><span>🌏 Welcome to BEST WORK — Connecting Global Talent to Korea — 외국인 유학생 및 취업 전문 컨설팅 🌏</span></div>

  <!-- NAVBAR -->
  <nav class="navbar">
    <a href="#home" class="navbar-brand">BEST WORK</a>
    <div class="menu-toggle" id="mobile-menu"><span></span><span></span><span></span></div>
    <div class="navbar-links" id="nav-links">
      <a href="#about">회사 소개</a>
      <a href="#services">주요 서비스</a>
      <a href="#universities">제휴 대학교</a>
      <a href="#countries">주요 국가</a>
      <a href="#contact">문의하기</a>
    </div>
  </nav>

  <!-- HEADER -->
  <header id="home">
    <div class="overlay">
      <div class="logo">BEST WORK</div>
      <h1>유학생·취업 외국인의 성공적인 한국 정착을 돕는 파트너</h1>
      <p>글로벌 인재와 기회를 연결하며, 유학 및 취업을 통한 외국인의 성공적인 국내 정착을 지원합니다.</p>
      <a href="#about" class="btn">자세히 알아보기</a>
    </div>
  </header>

  <!-- 이하 동일 (스크롤 애니메이션 섹션들) -->
  <!-- ABOUT, SERVICES, UNIVERSITIES, COUNTRIES, CONTACT, FOOTER 등 위와 동일 코드 유지 -->

  <script>
    // 모바일 메뉴 토글
    const menuToggle=document.getElementById('mobile-menu');
    const navLinks=document.getElementById('nav-links');
    menuToggle.addEventListener('click',()=>navLinks.classList.toggle('active'));
    // 스크롤 이동
    document.querySelectorAll('.navbar-links a').forEach(link=>{
      link.addEventListener('click',e=>{
        e.preventDefault();
        const target=document.querySelector(link.getAttribute('href'));
        if(target){window.scrollTo({top:target.offsetTop-60,behavior:'smooth'});}
        navLinks.classList.remove('active');
      });
    });
    // Scroll animation
    const observer=new IntersectionObserver(entries=>{
      entries.forEach(entry=>{
        if(entry.isIntersecting){entry.target.classList.add('visible');}
      });
    },{threshold:0.2});
    document.querySelectorAll('[data-scroll]').forEach(el=>observer.observe(el));
  </script>
</body>
</html>
