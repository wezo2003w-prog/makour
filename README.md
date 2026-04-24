<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>محاور | متجر المخاور الفاخر</title>
  <meta name="description" content="متجر محاور لبيع المخاور الفاخرة بألوان عنابي مع أبيض وذهبي. تجربة تسوق سلسة، سريعة، ومناسبة للجوال." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@300;400;500;700;800&display=swap" rel="stylesheet">
  <script src="https://cdn.tailwindcss.com"></script>
  <style>
    :root{
      --bg:#07050a;
      --panel: rgba(255,255,255,.06);
      --panel2: rgba(255,255,255,.08);
      --stroke: rgba(255,255,255,.14);
      --text: rgba(255,255,255,.92);
      --muted: rgba(255,255,255,.70);
      --muted2: rgba(255,255,255,.55);
      --maroon: #7b0f2a;
      --maroon2:#4d0820;
      --gold:#d7b25f;
      --gold2:#f2d28a;
      --shadow: 0 18px 60px rgba(0,0,0,.55);
      --shadow2: 0 14px 38px rgba(0,0,0,.45);
      --radius: 18px;
      --radius2: 24px;
      --ring: 0 0 0 3px rgba(215,178,95,.18);
    }
    *{ box-sizing:border-box; }
    html,body{ height:100%; }
    body{
      margin:0;
      font-family:"Tajawal", system-ui, -apple-system, Segoe UI, Roboto, "Helvetica Neue", Arial, "Noto Sans Arabic", "Apple Color Emoji","Segoe UI Emoji";
      background:
        radial-gradient(1000px 650px at 18% 18%, rgba(215,178,95,.16), transparent 55%),
        radial-gradient(980px 620px at 82% 22%, rgba(123,15,42,.35), transparent 58%),
        radial-gradient(1200px 800px at 50% 110%, rgba(123,15,42,.28), transparent 55%),
        linear-gradient(180deg, #07050a, #06040a 45%, #05030a);
      color: var(--text);
      overflow-x:hidden;
    }
    a{ color:inherit; text-decoration:none; }
    ::selection{ background: rgba(215,178,95,.28); }
    .container-max{ max-width: 1200px; }

    /* Glass + borders */
    .glass{
      background: linear-gradient(180deg, rgba(255,255,255,.09), rgba(255,255,255,.05));
      border: 1px solid rgba(255,255,255,.12);
      box-shadow: var(--shadow2);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
    }
    .glass-strong{
      background: linear-gradient(180deg, rgba(255,255,255,.10), rgba(255,255,255,.06));
      border: 1px solid rgba(255,255,255,.14);
      box-shadow: var(--shadow);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
    }

    /* Buttons */
    .btn{
      display:inline-flex; align-items:center; justify-content:center;
      gap:.6rem;
      padding:.9rem 1.1rem;
      border-radius: 14px;
      border:1px solid transparent;
      font-weight:700;
      transition: transform .15s ease, box-shadow .2s ease, background .2s ease, border-color .2s ease, opacity .2s ease;
      user-select:none;
      will-change: transform;
    }
    .btn:active{ transform: translateY(1px) scale(.99); }
    .btn-primary{
      background: linear-gradient(135deg, rgba(215,178,95,.95), rgba(242,210,138,.82));
      color:#1a0f16;
      box-shadow: 0 14px 36px rgba(215,178,95,.20);
      border-color: rgba(255,255,255,.16);
    }
    .btn-primary:hover{ transform: translateY(-1px); box-shadow: 0 18px 46px rgba(215,178,95,.26); }
    .btn-outline{
      background: rgba(255,255,255,.06);
      border-color: rgba(215,178,95,.35);
      color: rgba(255,255,255,.92);
      box-shadow: 0 12px 28px rgba(0,0,0,.25);
    }
    .btn-outline:hover{ background: rgba(255,255,255,.08); transform: translateY(-1px); }
    .btn-ghost{
      background: transparent;
      border-color: rgba(255,255,255,.12);
      color: rgba(255,255,255,.86);
    }
    .btn-ghost:hover{ background: rgba(255,255,255,.06); }

    .chip{
      display:inline-flex; align-items:center; gap:.5rem;
      padding:.35rem .7rem;
      border-radius: 999px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.06);
      color: rgba(255,255,255,.85);
      font-weight: 700;
      font-size: .86rem;
      white-space: nowrap;
    }

    /* Inputs */
    .field{
      width:100%;
      border-radius: 14px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(255,255,255,.06);
      color: var(--text);
      padding: .95rem 1rem;
      outline: none;
      transition: box-shadow .2s ease, border-color .2s ease, background .2s ease;
    }
    .field::placeholder{ color: rgba(255,255,255,.55); }
    .field:focus{ border-color: rgba(215,178,95,.55); box-shadow: var(--ring); background: rgba(255,255,255,.08); }

    /* Card hover */
    .hover-lift{
      transition: transform .18s ease, box-shadow .22s ease, border-color .22s ease, background .22s ease;
      will-change: transform;
    }
    .hover-lift:hover{
      transform: translateY(-6px);
      box-shadow: 0 22px 70px rgba(0,0,0,.55);
      border-color: rgba(215,178,95,.25);
    }

    /* Header blur on scroll */
    .header{
      position: sticky;
      top: 0;
      z-index: 60;
      border-bottom: 1px solid rgba(255,255,255,.10);
      background: rgba(7,5,10,.52);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      transition: background .2s ease, border-color .2s ease;
    }
    .header.scrolled{
      background: rgba(7,5,10,.72);
      border-color: rgba(215,178,95,.18);
    }

    /* Hero accents */
    .hero-glow{
      position:absolute; inset:-1px;
      background:
        radial-gradient(600px 380px at 30% 30%, rgba(215,178,95,.20), transparent 60%),
        radial-gradient(740px 520px at 80% 40%, rgba(123,15,42,.48), transparent 62%),
        radial-gradient(700px 420px at 50% 110%, rgba(215,178,95,.12), transparent 60%);
      filter: blur(0px);
      pointer-events:none;
      opacity: .95;
    }
    .spark{
      position:absolute;
      width: 6px; height: 6px; border-radius: 999px;
      background: rgba(242,210,138,.9);
      box-shadow: 0 0 18px rgba(242,210,138,.55);
      opacity:.85;
      animation: floaty 6s ease-in-out infinite;
    }
    @keyframes floaty{
      0%,100%{ transform: translateY(0) translateX(0); opacity:.75; }
      50%{ transform: translateY(-14px) translateX(10px); opacity:1; }
    }
    .shine{
      position:absolute; inset:0;
      background: linear-gradient(110deg, transparent 30%, rgba(255,255,255,.14) 45%, transparent 60%);
      transform: translateX(-80%);
      animation: shine 6.2s ease-in-out infinite;
      pointer-events:none;
      opacity:.65;
    }
    @keyframes shine{
      0%{ transform: translateX(-85%); }
      35%{ transform: translateX(110%); }
      100%{ transform: translateX(110%); }
    }

    /* Modal / drawer */
    .overlay{
      position:fixed; inset:0;
      background: rgba(0,0,0,.58);
      display:none;
      z-index: 80;
      padding: 18px;
    }
    .overlay.open{ display:flex; }
    .modal{
      margin:auto;
      width: min(980px, 100%);
      border-radius: 22px;
      overflow:hidden;
      border:1px solid rgba(255,255,255,.14);
      background: linear-gradient(180deg, rgba(255,255,255,.09), rgba(255,255,255,.05));
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      box-shadow: 0 30px 120px rgba(0,0,0,.65);
      transform: translateY(8px) scale(.985);
      opacity: 0;
      transition: transform .18s ease, opacity .18s ease;
      max-height: calc(100vh - 36px);
      display:flex;
      flex-direction:column;
    }
    .overlay.open .modal{
      transform: translateY(0) scale(1);
      opacity: 1;
    }
    .modal-body{
      overflow:auto;
      -webkit-overflow-scrolling: touch;
    }

    .drawer{
      position:fixed;
      top:0; bottom:0;
      left:0;
      width: min(420px, 92vw);
      transform: translateX(-102%);
      transition: transform .22s ease;
      z-index: 90;
      border-right:1px solid rgba(255,255,255,.12);
      background: rgba(7,5,10,.72);
      backdrop-filter: blur(16px);
      -webkit-backdrop-filter: blur(16px);
      box-shadow: 18px 0 70px rgba(0,0,0,.55);
    }
    .drawer.open{ transform: translateX(0); }

    /* Toast */
    .toast-wrap{
      position:fixed;
      bottom:16px;
      right:16px;
      z-index: 120;
      display:flex;
      flex-direction:column;
      gap:10px;
      pointer-events:none;
    }
    .toast{
      pointer-events:auto;
      width: min(360px, calc(100vw - 32px));
      border-radius: 16px;
      border:1px solid rgba(255,255,255,.14);
      background: rgba(15,10,18,.78);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      box-shadow: 0 18px 60px rgba(0,0,0,.55);
      padding: 12px 12px;
      display:flex;
      gap:10px;
      align-items:flex-start;
      animation: toastIn .22s ease both;
    }
    @keyframes toastIn{
      from{ opacity:0; transform: translateY(10px); }
      to{ opacity:1; transform: translateY(0); }
    }

    /* Reduce motion */
    @media (prefers-reduced-motion: reduce){
      *{ animation-duration: 0.001ms !important; animation-iteration-count: 1 !important; transition-duration: 0.001ms !important; scroll-behavior: auto !important; }
    }
  </style>
</head>

<body>
  <!-- Top Header -->
  <header id="siteHeader" class="header">
    <div class="mx-auto container-max px-4">
      <div class="flex items-center justify-between py-3 gap-3">
        <div class="flex items-center gap-3">
          <button id="menuBtn" class="btn btn-ghost h-11 px-3 rounded-xl" aria-label="فتح القائمة">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none">
              <path d="M4 7h16M4 12h16M4 17h16" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
            </svg>
          </button>

          <a href="#home" class="flex items-center gap-3">
            <div class="relative h-11 w-11 rounded-2xl overflow-hidden glass-strong">
              <div class="absolute inset-0" style="background:
                radial-gradient(20px 20px at 30% 30%, rgba(242,210,138,.85), transparent 60%),
                radial-gradient(30px 30px at 70% 70%, rgba(123,15,42,.9), transparent 65%),
                linear-gradient(135deg, rgba(123,15,42,.85), rgba(215,178,95,.22));"></div>
              <div class="absolute inset-0 shine"></div>
              <div class="relative z-10 flex items-center justify-center h-full font-extrabold" style="color:#fff;">
                م
              </div>
            </div>
            <div class="leading-tight">
              <div class="font-extrabold text-lg tracking-tight">محاور</div>
              <div class="text-[12px] text-white/60 -mt-0.5">متجر المخاور الفاخر</div>
            </div>
          </a>
        </div>

        <div class="hidden lg:flex items-center gap-2">
          <a class="chip hover:opacity-90" href="#new">جديدنا</a>
          <a class="chip hover:opacity-90" href="#categories">التصنيفات</a>
          <a class="chip hover:opacity-90" href="#best">الأكثر مبيعًا</a>
          <a class="chip hover:opacity-90" href="#reviews">آراء العملاء</a>
          <a class="chip hover:opacity-90" href="#faq">الأسئلة</a>
        </div>

        <div class="flex items-center gap-2">
          <div class="hidden md:flex items-center gap-2 glass rounded-2xl px-3 h-11 border border-white/10">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M21 21l-4.35-4.35M10.5 18a7.5 7.5 0 1 1 0-15 7.5 7.5 0 0 1 0 15Z" stroke="rgba(255,255,255,.82)" stroke-width="2" stroke-linecap="round"/>
            </svg>
            <input id="searchInput" class="bg-transparent outline-none text-sm text-white/85 placeholder:text-white/50 w-56" placeholder="ابحث عن: ذهبي، ثقيل، بوكس..." />
          </div>

          <button id="openCartBtn" class="btn btn-outline h-11 px-4 rounded-xl relative" aria-label="فتح السلة">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M7 7h14l-1.5 9h-11L7 7Zm0 0L6 3H3" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M9 21a1 1 0 1 0 0-2 1 1 0 0 0 0 2Zm9 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
            </svg>
            <span class="hidden sm:inline">السلة</span>
            <span id="cartCount" class="absolute -top-2 -left-2 h-6 min-w-6 px-2 rounded-full flex items-center justify-center text-xs font-extrabold"
              style="background: linear-gradient(135deg, rgba(215,178,95,.95), rgba(242,210,138,.85)); color:#1a0f16; border:1px solid rgba(255,255,255,.18); display:none;">
              0
            </span>
          </button>

          <a href="#checkout" class="btn btn-primary h-11 px-4 rounded-xl">
            شراء سريع
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M13 5l7 7-7 7M4 12h16" stroke="#1a0f16" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </a>
        </div>
      </div>

      <div class="md:hidden pb-3">
        <div class="flex items-center gap-2 glass rounded-2xl px-3 h-11 border border-white/10">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M21 21l-4.35-4.35M10.5 18a7.5 7.5 0 1 1 0-15 7.5 7.5 0 0 1 0 15Z" stroke="rgba(255,255,255,.82)" stroke-width="2" stroke-linecap="round"/>
          </svg>
          <input id="searchInputMobile" class="bg-transparent outline-none text-sm text-white/85 placeholder:text-white/50 w-full" placeholder="ابحث عن مخورك..." />
        </div>
      </div>
    </div>
  </header>

  <!-- Drawer Menu -->
  <div id="drawer" class="drawer">
    <div class="p-4 border-b border-white/10 flex items-center justify-between">
      <div class="flex items-center gap-3">
        <div class="h-10 w-10 rounded-2xl overflow-hidden glass-strong relative">
          <div class="absolute inset-0" style="background:
            radial-gradient(20px 20px at 30% 30%, rgba(242,210,138,.85), transparent 60%),
            radial-gradient(30px 30px at 70% 70%, rgba(123,15,42,.9), transparent 65%),
            linear-gradient(135deg, rgba(123,15,42,.85), rgba(215,178,95,.22));"></div>
          <div class="absolute inset-0 shine"></div>
          <div class="relative z-10 flex items-center justify-center h-full font-extrabold">م</div>
        </div>
        <div>
          <div class="font-extrabold">محاور</div>
          <div class="text-xs text-white/60 -mt-0.5">قائمة المتجر</div>
        </div>
      </div>
      <button id="closeDrawerBtn" class="btn btn-ghost h-10 px-3 rounded-xl" aria-label="إغلاق القائمة">
        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
          <path d="M6 6l12 12M18 6L6 18" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
        </svg>
      </button>
    </div>

    <div class="p-4 space-y-2">
      <a href="#home" class="btn btn-ghost w-full justify-between">
        الرئيسية
        <span class="text-white/50 text-sm">↩</span>
      </a>
      <a href="#categories" class="btn btn-ghost w-full justify-between">
        التصنيفات
        <span class="text-white/50 text-sm">↩</span>
      </a>
      <a href="#best" class="btn btn-ghost w-full justify-between">
        الأكثر مبيعًا
        <span class="text-white/50 text-sm">↩</span>
      </a>
      <a href="#reviews" class="btn btn-ghost w-full justify-between">
        آراء العملاء
        <span class="text-white/50 text-sm">↩</span>
      </a>
      <a href="#faq" class="btn btn-ghost w-full justify-between">
        الأسئلة الشائعة
        <span class="text-white/50 text-sm">↩</span>
      </a>

      <div class="mt-4 glass rounded-2xl p-4 border border-white/10">
        <div class="flex items-center justify-between gap-2">
          <div>
            <div class="font-extrabold">خصم اليوم</div>
            <div class="text-sm text-white/70">استخدم كود: <span class="font-extrabold text-[var(--gold2)]">MAHAWER10</span></div>
          </div>
          <button class="btn btn-outline h-10 px-4 rounded-xl" id="copyCodeBtn">نسخ</button>
        </div>
      </div>

      <div class="mt-4 text-xs text-white/55 leading-relaxed">
        تواصل: <span class="text-white/70">واتساب</span> • <span class="text-white/70">انستغرام</span> • <span class="text-white/70">سناب</span><br/>
        © <span id="year"></span> محاور. جميع الحقوق محفوظة.
      </div>
    </div>
  </div>

  <!-- Drawer overlay -->
  <div id="drawerOverlay" class="fixed inset-0 bg-black/60 hidden z-[85]"></div>

  <!-- Hero -->
  <main id="home" class="relative">
    <section class="relative overflow-hidden">
      <div class="hero-glow"></div>

      <div class="mx-auto container-max px-4 pt-10 pb-8 md:pt-16 md:pb-14 relative">
        <div class="grid lg:grid-cols-2 gap-10 items-center">
          <div>
            <div class="flex flex-wrap items-center gap-2 mb-4">
              <span class="chip" style="border-color: rgba(215,178,95,.35); background: rgba(215,178,95,.10);">
                <span class="inline-block h-2.5 w-2.5 rounded-full" style="background: linear-gradient(135deg, rgba(215,178,95,.95), rgba(242,210,138,.75));"></span>
                ألوان عنابي • أبيض • ذهبي
              </span>
              <span class="chip">
                شحن سريع داخل المملكة
              </span>
              <span class="chip">
                ضمان جودة
              </span>
            </div>

            <h1 class="text-3xl md:text-5xl font-extrabold leading-[1.15] tracking-tight">
              مخاور فخمة بتصميم <span style="color: var(--gold2); text-shadow: 0 10px 40px rgba(215,178,95,.18);">سلس</span>
              وواجهة <span style="color: rgba(255,255,255,.95);">مريحة</span> للتسوق
            </h1>

            <p class="mt-4 text-white/70 text-base md:text-lg leading-relaxed max-w-xl">
              اختر مخورك من تشكيلتنا المختارة بعناية: تطريز أنيق، أقمشة راقية، وقصّات تناسب الذوق الخليجي.
              كل شيء مصمم ليكون سريعًا، جميلًا، ومناسبًا للجوال.
            </p>

            <div class="mt-6 flex flex-col sm:flex-row gap-3">
              <a href="#new" class="btn btn-primary rounded-2xl px-5">
                تصفّح الجديد
                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                  <path d="M13 5l7 7-7 7M4 12h16" stroke="#1a0f16" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </a>
              <button id="openSizeGuideBtn" class="btn btn-outline rounded-2xl px-5">
                دليل المقاسات
                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                  <path d="M4 7h16M7 4v16M17 4v16M4 17h16" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
                </svg>
              </button>
            </div>

            <div class="mt-6 grid grid-cols-3 gap-3 max-w-xl">
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-[var(--gold2)] font-extrabold text-xl">24–48h</div>
                <div class="text-white/65 text-sm">تجهيز الطلب</div>
              </div>
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-[var(--gold2)] font-extrabold text-xl">+1200</div>
                <div class="text-white/65 text-sm">طلب مُنجز</div>
              </div>
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-[var(--gold2)] font-extrabold text-xl">4.8/5</div>
                <div class="text-white/65 text-sm">تقييم العملاء</div>
              </div>
            </div>
          </div>

          <div class="relative">
            <div class="absolute -top-6 -right-2 spark" style="animation-delay:.2s;"></div>
            <div class="absolute top-20 -left-3 spark" style="animation-delay:1.4s; opacity:.7;"></div>
            <div class="absolute bottom-10 right-6 spark" style="animation-delay:2.2s; opacity:.8;"></div>

            <div class="glass-strong rounded-[28px] border border-white/10 overflow-hidden relative">
              <div class="absolute inset-0 shine"></div>
              <div class="p-5 md:p-6">
                <div class="flex items-center justify-between gap-3">
                  <div class="flex items-center gap-2">
                    <span class="chip" style="background: rgba(123,15,42,.22); border-color: rgba(123,15,42,.45);">عنابي</span>
                    <span class="chip" style="background: rgba(215,178,95,.10); border-color: rgba(215,178,95,.35);">ذهبي</span>
                    <span class="chip">أبيض</span>
                  </div>
                  <button id="surpriseBtn" class="btn btn-ghost h-10 px-4 rounded-xl">
                    اقتراح سريع
                  </button>
                </div>

                <div class="mt-5 grid grid-cols-2 gap-4">
                  <div class="rounded-2xl overflow-hidden border border-white/10 relative" style="background:
                    radial-gradient(120px 120px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
                    linear-gradient(135deg, rgba(123,15,42,.85), rgba(20,12,20,.92));">
                    <div class="absolute inset-0" style="background:
                      radial-gradient(260px 220px at 70% 20%, rgba(215,178,95,.12), transparent 70%),
                      radial-gradient(220px 180px at 40% 90%, rgba(255,255,255,.06), transparent 70%);"></div>
                    <div class="p-4 relative">
                      <div class="text-sm text-white/70">مخور ملكي</div>
                      <div class="font-extrabold text-lg">اللمسة الذهبية</div>
                      <div class="mt-3 text-xs text-white/60 leading-relaxed">
                        تطريز ذهبي فخم على عنابي مطفي، يناسب المناسبات.
                      </div>
                      <div class="mt-4 flex items-end justify-between gap-2">
                        <div>
                          <div class="text-white/60 text-xs">السعر</div>
                          <div class="text-[var(--gold2)] font-extrabold text-xl">399 ر.س</div>
                        </div>
                        <button class="btn btn-primary h-10 px-4 rounded-xl add-to-cart"
                          data-id="mah-001" data-name="مخور اللمسة الذهبية" data-price="399" data-color="عنابي" data-size="M">
                          أضف
                        </button>
                      </div>
                    </div>
                  </div>

                  <div class="rounded-2xl overflow-hidden border border-white/10 relative" style="background:
                    radial-gradient(120px 120px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
                    linear-gradient(135deg, rgba(10,7,14,.92), rgba(123,15,42,.72));">
                    <div class="absolute inset-0" style="background:
                      radial-gradient(260px 220px at 70% 20%, rgba(215,178,95,.12), transparent 70%),
                      radial-gradient(220px 180px at 40% 90%, rgba(255,255,255,.06), transparent 70%);"></div>
                    <div class="p-4 relative">
                      <div class="text-sm text-white/70">مخور عملي</div>
                      <div class="font-extrabold text-lg">أناقة يومية</div>
                      <div class="mt-3 text-xs text-white/60 leading-relaxed">
                        قماش مريح وتفاصيل نظيفة، مثالي للاستخدام اليومي.
                      </div>
                      <div class="mt-4 flex items-end justify-between gap-2">
                        <div>
                          <div class="text-white/60 text-xs">السعر</div>
                          <div class="text-[var(--gold2)] font-extrabold text-xl">249 ر.س</div>
                        </div>
                        <button class="btn btn-outline h-10 px-4 rounded-xl add-to-cart"
                          data-id="mah-002" data-name="مخور أناقة يومية" data-price="249" data-color="عنابي" data-size="L">
                          أضف
                        </button>
                      </div>
                    </div>
                  </div>
                </div>

                <div class="mt-4 glass rounded-2xl p-4 border border-white/10 flex flex-col sm:flex-row sm:items-center sm:justify-between gap-3">
                  <div class="flex items-center gap-3">
                    <div class="h-11 w-11 rounded-2xl flex items-center justify-center"
                      style="background: rgba(215,178,95,.12); border:1px solid rgba(215,178,95,.28);">
                      <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                        <path d="M12 8v4l3 3" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                        <path d="M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" stroke="rgba(255,255,255,.9)" stroke-width="2"/>
                      </svg>
                    </div>
                    <div>
                      <div class="font-extrabold">عروض محدودة</div>
                      <div class="text-sm text-white/65">ينتهي العرض خلال: <span id="dealTimer" class="text-[var(--gold2)] font-extrabold">—</span></div>
                    </div>
                  </div>
                  <a href="#best" class="btn btn-primary h-11 px-5 rounded-2xl">شاهد العروض</a>
                </div>
              </div>
            </div>

            <div class="mt-4 grid grid-cols-3 gap-3">
              <div class="glass rounded-2xl p-3 border border-white/10">
                <div class="text-xs text-white/60">دفع</div>
                <div class="font-extrabold">مدى • فيزا</div>
              </div>
              <div class="glass rounded-2xl p-3 border border-white/10">
                <div class="text-xs text-white/60">استبدال</div>
                <div class="font-extrabold">7 أيام</div>
              </div>
              <div class="glass rounded-2xl p-3 border border-white/10">
                <div class="text-xs text-white/60">خدمة</div>
                <div class="font-extrabold">واتساب</div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </section>

    <!-- Categories -->
    <section id="categories" class="mx-auto container-max px-4 py-10 md:py-14">
      <div class="flex items-end justify-between gap-4">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">التصنيفات</h2>
          <p class="text-white/65 mt-1">فلترة سريعة حسب ذوقك — عنابي أنيق ولمسة ذهبية.</p>
        </div>
        <div class="hidden md:flex items-center gap-2">
          <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn" data-filter="all">الكل</button>
          <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn" data-filter="premium">فاخر</button>
          <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn" data-filter="daily">يومي</button>
          <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn" data-filter="gift">هدايا</button>
        </div>
      </div>

      <div class="mt-6 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-4">
        <button class="glass rounded-2xl p-5 border border-white/10 text-right hover-lift filter-btn" data-filter="premium">
          <div class="flex items-start justify-between">
            <div>
              <div class="text-white/65 text-sm">فئة</div>
              <div class="font-extrabold text-lg">فاخر</div>
            </div>
            <span class="chip" style="background: rgba(215,178,95,.10); border-color: rgba(215,178,95,.35);">ذهبي</span>
          </div>
          <div class="mt-4 text-sm text-white/65 leading-relaxed">تطريز مميز، خامة راقية، تفاصيل لافتة.</div>
        </button>

        <button class="glass rounded-2xl p-5 border border-white/10 text-right hover-lift filter-btn" data-filter="daily">
          <div class="flex items-start justify-between">
            <div>
              <div class="text-white/65 text-sm">فئة</div>
              <div class="font-extrabold text-lg">يومي</div>
            </div>
            <span class="chip" style="background: rgba(255,255,255,.06);">مريح</span>
          </div>
          <div class="mt-4 text-sm text-white/65 leading-relaxed">قصّة مريحة، خفيف، مناسب للدوام.</div>
        </button>

        <button class="glass rounded-2xl p-5 border border-white/10 text-right hover-lift filter-btn" data-filter="gift">
          <div class="flex items-start justify-between">
            <div>
              <div class="text-white/65 text-sm">فئة</div>
              <div class="font-extrabold text-lg">هدايا</div>
            </div>
            <span class="chip" style="background: rgba(123,15,42,.22); border-color: rgba(123,15,42,.45);">عنابي</span>
          </div>
          <div class="mt-4 text-sm text-white/65 leading-relaxed">تغليف فخم وخيارات كتابة إهداء.</div>
        </button>

        <button class="glass rounded-2xl p-5 border border-white/10 text-right hover-lift filter-btn" data-filter="limited">
          <div class="flex items-start justify-between">
            <div>
              <div class="text-white/65 text-sm">فئة</div>
              <div class="font-extrabold text-lg">إصدار محدود</div>
            </div>
            <span class="chip" style="background: rgba(215,178,95,.10); border-color: rgba(215,178,95,.35);">حصري</span>
          </div>
          <div class="mt-4 text-sm text-white/65 leading-relaxed">عدد محدود — احجز قبل نفاد الكمية.</div>
        </button>
      </div>

      <div class="mt-4 md:hidden flex gap-2 overflow-auto pb-2">
        <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn shrink-0" data-filter="all">الكل</button>
        <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn shrink-0" data-filter="premium">فاخر</button>
        <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn shrink-0" data-filter="daily">يومي</button>
        <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn shrink-0" data-filter="gift">هدايا</button>
        <button class="btn btn-ghost h-11 px-4 rounded-xl filter-btn shrink-0" data-filter="limited">محدود</button>
      </div>
    </section>

    <!-- Product Grid -->
    <section id="new" class="mx-auto container-max px-4 pb-10 md:pb-14">
      <div class="flex items-end justify-between gap-4">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">جديدنا</h2>
          <p class="text-white/65 mt-1">اختيارات طازجة — مع ألوان متناسقة عنابي/أبيض/ذهبي.</p>
        </div>
        <div class="flex items-center gap-2">
          <div class="hidden sm:block">
            <select id="sortSelect" class="field h-11 py-0">
              <option value="featured">الترتيب: مميز</option>
              <option value="priceAsc">السعر: من الأقل</option>
              <option value="priceDesc">السعر: من الأعلى</option>
              <option value="ratingDesc">التقييم: الأعلى</option>
            </select>
          </div>
          <button id="viewToggleBtn" class="btn btn-ghost h-11 px-4 rounded-xl" aria-label="تبديل العرض">
            <svg id="gridIcon" width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M4 4h7v7H4V4Zm9 0h7v7h-7V4ZM4 13h7v7H4v-7Zm9 0h7v7h-7v-7Z" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linejoin="round"/>
            </svg>
          </button>
        </div>
      </div>

      <div id="productsWrap" class="mt-6 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4"></div>
    </section>

    <!-- Best Seller -->
    <section id="best" class="mx-auto container-max px-4 pb-10 md:pb-14">
      <div class="glass-strong rounded-[28px] border border-white/10 overflow-hidden relative">
        <div class="absolute inset-0" style="background:
          radial-gradient(640px 380px at 20% 30%, rgba(215,178,95,.18), transparent 60%),
          radial-gradient(680px 420px at 85% 35%, rgba(123,15,42,.50), transparent 62%);"></div>
        <div class="absolute inset-0 shine"></div>

        <div class="relative p-6 md:p-10 grid lg:grid-cols-2 gap-8 items-center">
          <div>
            <div class="flex flex-wrap gap-2 mb-3">
              <span class="chip" style="background: rgba(215,178,95,.12); border-color: rgba(215,178,95,.35);">الأكثر مبيعًا</span>
              <span class="chip">تطريز ذهبي</span>
              <span class="chip">قماش ممتاز</span>
            </div>
            <h3 class="text-2xl md:text-4xl font-extrabold leading-[1.15]">
              مخور <span class="text-[var(--gold2)]">البصمة الذهبية</span>
              <span class="text-white/90">— فخامة ما تنسى</span>
            </h3>
            <p class="mt-3 text-white/70 leading-relaxed">
              تصميم عنابي عميق مع تفاصيل ذهبية ناعمة، يناسب المناسبات ويظهر الفخامة بدون مبالغة.
            </p>

            <div class="mt-5 flex flex-col sm:flex-row gap-3">
              <button class="btn btn-primary rounded-2xl px-6 add-to-cart"
                data-id="mah-006" data-name="مخور البصمة الذهبية" data-price="429" data-color="عنابي" data-size="M">
                أضف للسلة — 429 ر.س
              </button>
              <button class="btn btn-outline rounded-2xl px-6" data-quick="mah-006">
                معاينة سريعة
              </button>
            </div>

            <div class="mt-6 grid grid-cols-3 gap-3">
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-xs text-white/60">الخامة</div>
                <div class="font-extrabold">جبر دبل</div>
              </div>
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-xs text-white/60">المقاس</div>
                <div class="font-extrabold">S–XL</div>
              </div>
              <div class="glass rounded-2xl p-4 border border-white/10">
                <div class="text-xs text-white/60">التقييم</div>
                <div class="font-extrabold">⭐ 4.9</div>
              </div>
            </div>
          </div>

          <div class="relative">
            <div class="grid grid-cols-2 gap-4">
              <div class="glass rounded-2xl p-4 border border-white/10 hover-lift">
                <div class="rounded-2xl h-36 border border-white/10 overflow-hidden relative"
                     style="background: linear-gradient(135deg, rgba(123,15,42,.88), rgba(10,7,14,.92));">
                  <div class="absolute inset-0" style="background:
                    radial-gradient(160px 140px at 30% 25%, rgba(242,210,138,.20), transparent 60%),
                    radial-gradient(220px 180px at 80% 70%, rgba(255,255,255,.06), transparent 70%);"></div>
                </div>
                <div class="mt-3 flex items-center justify-between">
                  <div>
                    <div class="font-extrabold">عنابي مطفي</div>
                    <div class="text-xs text-white/60">لون أساسي</div>
                  </div>
                  <span class="chip">#7b0f2a</span>
                </div>
              </div>

              <div class="glass rounded-2xl p-4 border border-white/10 hover-lift">
                <div class="rounded-2xl h-36 border border-white/10 overflow-hidden relative"
                     style="background: linear-gradient(135deg, rgba(215,178,95,.95), rgba(242,210,138,.70));">
                  <div class="absolute inset-0" style="background:
                    radial-gradient(160px 140px at 30% 25%, rgba(255,255,255,.16), transparent 60%),
                    radial-gradient(220px 180px at 80% 70%, rgba(123,15,42,.10), transparent 70%);"></div>
                </div>
                <div class="mt-3 flex items-center justify-between">
                  <div>
                    <div class="font-extrabold">ذهبي ناعم</div>
                    <div class="text-xs text-white/60">تفاصيل</div>
                  </div>
                  <span class="chip">#d7b25f</span>
                </div>
              </div>

              <div class="glass rounded-2xl p-4 border border-white/10 hover-lift">
                <div class="rounded-2xl h-36 border border-white/10 overflow-hidden relative"
                     style="background: linear-gradient(135deg, rgba(255,255,255,.92), rgba(255,255,255,.16));">
                  <div class="absolute inset-0" style="background:
                    radial-gradient(160px 140px at 30% 25%, rgba(242,210,138,.16), transparent 60%),
                    radial-gradient(220px 180px at 80% 70%, rgba(123,15,42,.12), transparent 70%);"></div>
                </div>
                <div class="mt-3 flex items-center justify-between">
                  <div>
                    <div class="font-extrabold">أبيض فخم</div>
                    <div class="text-xs text-white/60">توازن</div>
                  </div>
                  <span class="chip">#ffffff</span>
                </div>
              </div>

              <div class="glass rounded-2xl p-4 border border-white/10 hover-lift">
                <div class="rounded-2xl h-36 border border-white/10 overflow-hidden relative"
                     style="background: linear-gradient(135deg, rgba(10,7,14,.92), rgba(123,15,42,.70));">
                  <div class="absolute inset-0" style="background:
                    radial-gradient(160px 140px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
                    radial-gradient(220px 180px at 80% 70%, rgba(255,255,255,.06), transparent 70%);"></div>
                </div>
                <div class="mt-3 flex items-center justify-between">
                  <div>
                    <div class="font-extrabold">ليلي</div>
                    <div class="text-xs text-white/60">خلفية</div>
                  </div>
                  <span class="chip">#0a070e</span>
                </div>
              </div>
            </div>

          </div>
        </div>
      </div>
    </section>

    <!-- Reviews -->
    <section id="reviews" class="mx-auto container-max px-4 pb-10 md:pb-14">
      <div class="flex items-end justify-between gap-4">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">آراء العملاء</h2>
          <p class="text-white/65 mt-1">تقييمات حقيقية — لأن الجودة تظهر بالتجربة.</p>
        </div>
        <div class="hidden sm:flex items-center gap-2">
          <span class="chip" style="background: rgba(215,178,95,.12); border-color: rgba(215,178,95,.35);">⭐ 4.8 متوسط</span>
          <span class="chip">إرجاع 7 أيام</span>
        </div>
      </div>

      <div class="mt-6 grid grid-cols-1 md:grid-cols-3 gap-4">
        <div class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <div class="flex items-center justify-between">
            <div class="font-extrabold">نوف</div>
            <div class="text-[var(--gold2)] font-extrabold">⭐ 5.0</div>
          </div>
          <div class="mt-2 text-white/70 leading-relaxed">
            الخامة ممتازة والتطريز الذهبي جدًا راقي. ووصل بسرعة، والتغليف فخم.
          </div>
        </div>
        <div class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <div class="flex items-center justify-between">
            <div class="font-extrabold">عبدالله</div>
            <div class="text-[var(--gold2)] font-extrabold">⭐ 4.7</div>
          </div>
          <div class="mt-2 text-white/70 leading-relaxed">
            مقاسات دقيقة واللون عنابي مثل الصور. تجربة شراء سهلة وسريعة.
          </div>
        </div>
        <div class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <div class="flex items-center justify-between">
            <div class="font-extrabold">سارة</div>
            <div class="text-[var(--gold2)] font-extrabold">⭐ 4.8</div>
          </div>
          <div class="mt-2 text-white/70 leading-relaxed">
            أحببت التفاصيل البيضاء مع الذهبي. مرّة أنيق للمناسبات.
          </div>
        </div>
      </div>
    </section>

    <!-- FAQ -->
    <section id="faq" class="mx-auto container-max px-4 pb-14">
      <div class="flex items-end justify-between gap-4">
        <div>
          <h2 class="text-2xl md:text-3xl font-extrabold">الأسئلة الشائعة</h2>
          <p class="text-white/65 mt-1">كل اللي تحتاجه قبل الشراء.</p>
        </div>
      </div>

      <div class="mt-6 grid grid-cols-1 lg:grid-cols-2 gap-4">
        <details class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <summary class="cursor-pointer font-extrabold">كم مدة الشحن؟</summary>
          <div class="mt-2 text-white/70 leading-relaxed">
            تجهيز الطلب خلال 24–48 ساعة، ثم الشحن حسب المدينة (عادة 2–4 أيام).
          </div>
        </details>
        <details class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <summary class="cursor-pointer font-extrabold">هل يوجد استبدال أو إرجاع؟</summary>
          <div class="mt-2 text-white/70 leading-relaxed">
            نعم خلال 7 أيام بشرط الحفاظ على المنتج بحالته الأصلية.
          </div>
        </details>
        <details class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <summary class="cursor-pointer font-extrabold">كيف أعرف المقاس المناسب؟</summary>
          <div class="mt-2 text-white/70 leading-relaxed">
            افتح دليل المقاسات من الزر أعلى الصفحة، أو اختر “مقاس” وسيظهر توصية سريعة.
          </div>
        </details>
        <details class="glass rounded-2xl p-5 border border-white/10 hover-lift">
          <summary class="cursor-pointer font-extrabold">هل الألوان مطابقة للصور؟</summary>
          <div class="mt-2 text-white/70 leading-relaxed">
            نعم، نستخدم تصوير بألوان قريبة جدًا. قد يختلف بدرجة بسيطة حسب شاشة الجهاز.
          </div>
        </details>
      </div>
    </section>

    <!-- Checkout -->
    <section id="checkout" class="mx-auto container-max px-4 pb-16">
      <div class="grid lg:grid-cols-2 gap-4">
        <div class="glass-strong rounded-[28px] p-6 md:p-8 border border-white/10">
          <h2 class="text-2xl md:text-3xl font-extrabold">إتمام الطلب</h2>
          <p class="text-white/65 mt-1">أدخل بياناتك — الدفع هنا تجريبي (واجهة فقط).</p>

          <div class="mt-6 grid grid-cols-1 md:grid-cols-2 gap-3">
            <div>
              <label class="text-sm text-white/70">الاسم</label>
              <input id="name" class="field mt-2" placeholder="اسمك الكامل" />
            </div>
            <div>
              <label class="text-sm text-white/70">الجوال</label>
              <input id="phone" class="field mt-2" placeholder="05xxxxxxxx" inputmode="tel" />
            </div>
            <div class="md:col-span-2">
              <label class="text-sm text-white/70">العنوان</label>
              <input id="address" class="field mt-2" placeholder="المدينة، الحي، الشارع..." />
            </div>
            <div>
              <label class="text-sm text-white/70">طريقة الدفع</label>
              <select id="payment" class="field mt-2">
                <option value="mada">مدى</option>
                <option value="visa">فيزا / ماستر</option>
                <option value="cod">الدفع عند الاستلام</option>
              </select>
            </div>
            <div>
              <label class="text-sm text-white/70">كود خصم</label>
              <div class="flex gap-2 mt-2">
                <input id="coupon" class="field" placeholder="MAHAWER10" />
                <button id="applyCouponBtn" class="btn btn-outline h-[52px] px-4 rounded-2xl">تطبيق</button>
              </div>
              <div id="couponHint" class="text-xs text-white/55 mt-2"></div>
            </div>
          </div>

          <div class="mt-6 flex flex-col sm:flex-row gap-3">
            <button id="placeOrderBtn" class="btn btn-primary rounded-2xl px-6 flex-1">
              تأكيد الطلب
              <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                <path d="M20 6 9 17l-5-5" stroke="#1a0f16" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </button>
            <button id="clearCartBtn" class="btn btn-ghost rounded-2xl px-6">
              تفريغ السلة
            </button>
          </div>
        </div>

        <div class="glass-strong rounded-[28px] p-6 md:p-8 border border-white/10">
          <div class="flex items-center justify-between">
            <h3 class="text-xl md:text-2xl font-extrabold">ملخص السلة</h3>
            <button id="openCartBtn2" class="btn btn-outline h-11 px-4 rounded-xl">عرض السلة</button>
          </div>

          <div class="mt-5 space-y-3">
            <div class="glass rounded-2xl p-4 border border-white/10 flex items-center justify-between">
              <div class="text-white/70">المجموع الفرعي</div>
              <div class="font-extrabold" id="subtotalText">0 ر.س</div>
            </div>
            <div class="glass rounded-2xl p-4 border border-white/10 flex items-center justify-between">
              <div class="text-white/70">الخصم</div>
              <div class="font-extrabold text-[var(--gold2)]" id="discountText">0 ر.س</div>
            </div>
            <div class="glass rounded-2xl p-4 border border-white/10 flex items-center justify-between">
              <div class="text-white/70">الشحن</div>
              <div class="font-extrabold" id="shippingText">25 ر.س</div>
            </div>
            <div class="glass rounded-2xl p-4 border border-white/10 flex items-center justify-between">
              <div class="text-white/70">الإجمالي</div>
              <div class="font-extrabold text-2xl text-[var(--gold2)]" id="totalText">0 ر.س</div>
            </div>

            <div class="text-xs text-white/55 leading-relaxed">
              ملاحظة: هذا نموذج واجهة (Demo). اربط بوابة دفع وشحن لاحقًا بسهولة.
            </div>
          </div>

          <div class="mt-6 glass rounded-2xl p-5 border border-white/10">
            <div class="flex items-start gap-3">
              <div class="h-11 w-11 rounded-2xl flex items-center justify-center"
                style="background: rgba(123,15,42,.22); border:1px solid rgba(123,15,42,.45);">
                <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                  <path d="M12 2l3 7h7l-5.5 4 2 7-6.5-4.2L5.5 20l2-7L2 9h7l3-7Z" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linejoin="round"/>
                </svg>
              </div>
              <div>
                <div class="font-extrabold">تغليف فاخر</div>
                <div class="text-white/70 text-sm leading-relaxed">
                  بإمكانك إضافة بطاقة إهداء عند التواصل عبر واتساب بعد إتمام الطلب.
                </div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="border-t border-white/10">
      <div class="mx-auto container-max px-4 py-10">
        <div class="grid md:grid-cols-3 gap-6">
          <div>
            <div class="flex items-center gap-3">
              <div class="h-11 w-11 rounded-2xl overflow-hidden glass-strong relative">
                <div class="absolute inset-0" style="background:
                  radial-gradient(20px 20px at 30% 30%, rgba(242,210,138,.85), transparent 60%),
                  radial-gradient(30px 30px at 70% 70%, rgba(123,15,42,.9), transparent 65%),
                  linear-gradient(135deg, rgba(123,15,42,.85), rgba(215,178,95,.22));"></div>
                <div class="absolute inset-0 shine"></div>
                <div class="relative z-10 flex items-center justify-center h-full font-extrabold">م</div>
              </div>
              <div>
                <div class="font-extrabold text-lg">محاور</div>
                <div class="text-xs text-white/60 -mt-0.5">عنابي • أبيض • ذهبي</div>
              </div>
            </div>
            <p class="text-white/65 mt-3 leading-relaxed">
              متجر مخاور بتجربة سريعة وتصميم فاخر. نركز على الجودة والتفاصيل.
            </p>
          </div>

          <div class="glass rounded-2xl p-5 border border-white/10">
            <div class="font-extrabold">روابط</div>
            <div class="mt-3 grid grid-cols-2 gap-2 text-white/75">
              <a href="#new" class="btn btn-ghost justify-between">جديدنا <span class="text-white/40">↩</span></a>
              <a href="#best" class="btn btn-ghost justify-between">الأكثر <span class="text-white/40">↩</span></a>
              <a href="#reviews" class="btn btn-ghost justify-between">الآراء <span class="text-white/40">↩</span></a>
              <a href="#checkout" class="btn btn-ghost justify-between">الدفع <span class="text-white/40">↩</span></a>
            </div>
          </div>

          <div class="glass rounded-2xl p-5 border border-white/10">
            <div class="font-extrabold">النشرة البريدية</div>
            <div class="text-white/65 mt-1 text-sm">عروض وموديلات جديدة (تجريبي).</div>
            <div class="mt-3 flex gap-2">
              <input id="newsletterEmail" class="field" placeholder="بريدك الإلكتروني" inputmode="email" />
              <button id="newsletterBtn" class="btn btn-primary h-[52px] px-4 rounded-2xl">اشتراك</button>
            </div>
            <div class="text-xs text-white/55 mt-2">لن نرسل سبام. وعد.</div>
          </div>
        </div>

        <div class="mt-8 flex flex-col md:flex-row items-start md:items-center justify-between gap-3 text-xs text-white/55">
          <div>© <span id="year2"></span> محاور — تصميم عصري عنابي/ذهبي/أبيض.</div>
          <div class="flex flex-wrap items-center gap-2">
            <span class="chip">سياسة الاستبدال</span>
            <span class="chip">الشروط</span>
            <span class="chip">الخصوصية</span>
          </div>
        </div>
      </div>
    </footer>
  </main>

  <!-- Product Quick View Modal -->
  <div id="modalOverlay" class="overlay" role="dialog" aria-modal="true" aria-label="معاينة المنتج">
    <div class="modal">
      <div class="p-4 md:p-5 border-b border-white/10 flex items-center justify-between gap-3">
        <div class="flex items-center gap-3 min-w-0">
          <div class="h-10 w-10 rounded-2xl overflow-hidden glass relative shrink-0">
            <div id="modalSwatch" class="absolute inset-0"></div>
            <div class="absolute inset-0 shine"></div>
          </div>
          <div class="min-w-0">
            <div id="modalTitle" class="font-extrabold truncate">—</div>
            <div id="modalMeta" class="text-xs text-white/60 truncate">—</div>
          </div>
        </div>
        <button id="closeModalBtn" class="btn btn-ghost h-10 px-3 rounded-xl" aria-label="إغلاق">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M6 6l12 12M18 6L6 18" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
      </div>

      <div class="modal-body p-4 md:p-6 grid lg:grid-cols-2 gap-4">
        <div class="glass rounded-2xl p-4 border border-white/10 overflow-hidden relative">
          <div class="rounded-2xl h-64 md:h-[340px] border border-white/10 overflow-hidden relative" id="modalHero">
            <div class="absolute inset-0" style="background:
              radial-gradient(240px 200px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
              radial-gradient(360px 260px at 80% 70%, rgba(255,255,255,.06), transparent 70%);"></div>
            <div class="absolute inset-0 shine"></div>

            <div class="absolute top-3 right-3 flex gap-2">
              <span id="modalBadge" class="chip" style="background: rgba(215,178,95,.12); border-color: rgba(215,178,95,.35);">مميز</span>
              <span class="chip">ضمان</span>
            </div>

            <div class="absolute bottom-3 left-3 glass rounded-2xl px-3 py-2 border border-white/10">
              <div class="text-xs text-white/65">تقييم</div>
              <div id="modalRating" class="font-extrabold text-[var(--gold2)]">⭐ 4.8</div>
            </div>
          </div>

          <div class="mt-4 grid grid-cols-3 gap-2">
            <button class="btn btn-ghost rounded-xl h-11" data-size="S">S</button>
            <button class="btn btn-ghost rounded-xl h-11" data-size="M">M</button>
            <button class="btn btn-ghost rounded-xl h-11" data-size="L">L</button>
          </div>
          <div class="text-xs text-white/55 mt-2">اختر مقاسًا (تجريبي) — يتم حفظه عند الإضافة للسلة.</div>
        </div>

        <div class="glass rounded-2xl p-5 border border-white/10">
          <div class="flex items-center justify-between gap-3">
            <div>
              <div class="text-sm text-white/60">السعر</div>
              <div id="modalPrice" class="text-3xl font-extrabold text-[var(--gold2)]">—</div>
            </div>
            <div class="text-left">
              <div class="text-sm text-white/60">التوفر</div>
              <div class="font-extrabold">متوفر</div>
            </div>
          </div>

          <div id="modalDesc" class="mt-4 text-white/70 leading-relaxed">
            —
          </div>

          <div class="mt-5 grid grid-cols-2 gap-3">
            <div class="glass rounded-2xl p-4 border border-white/10">
              <div class="text-xs text-white/60">اللون</div>
              <div id="modalColor" class="font-extrabold">—</div>
            </div>
            <div class="glass rounded-2xl p-4 border border-white/10">
              <div class="text-xs text-white/60">الخامة</div>
              <div id="modalFabric" class="font-extrabold">—</div>
            </div>
          </div>

          <div class="mt-5 flex flex-col sm:flex-row gap-3">
            <button id="modalAddBtn" class="btn btn-primary rounded-2xl px-6 flex-1">أضف للسلة</button>
            <a href="#checkout" class="btn btn-outline rounded-2xl px-6">اذهب للدفع</a>
          </div>

          <div class="mt-4 glass rounded-2xl p-4 border border-white/10">
            <div class="flex items-start gap-3">
              <div class="h-10 w-10 rounded-2xl flex items-center justify-center"
                   style="background: rgba(215,178,95,.12); border:1px solid rgba(215,178,95,.28);">
                <svg width="22" height="22" viewBox="0 0 24 24" fill="none" aria-hidden="true">
                  <path d="M20 8h-9l-1-3H4" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M7 13h10l2-5" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M9 21a1 1 0 1 0 0-2 1 1 0 0 0 0 2Zm9 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
                </svg>
              </div>
              <div>
                <div class="font-extrabold">ملاحظة</div>
                <div class="text-sm text-white/70 leading-relaxed">
                  يمكنك اختيار المقاس من الأزرار، وسنضيفه تلقائيًا للسلة.
                </div>
              </div>
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>

  <!-- Size Guide Modal -->
  <div id="sizeOverlay" class="overlay" role="dialog" aria-modal="true" aria-label="دليل المقاسات">
    <div class="modal">
      <div class="p-4 md:p-5 border-b border-white/10 flex items-center justify-between gap-3">
        <div class="font-extrabold">دليل المقاسات</div>
        <button id="closeSizeBtn" class="btn btn-ghost h-10 px-3 rounded-xl" aria-label="إغلاق">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M6 6l12 12M18 6L6 18" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
      </div>
      <div class="modal-body p-4 md:p-6">
        <div class="grid lg:grid-cols-2 gap-4">
          <div class="glass rounded-2xl p-5 border border-white/10">
            <div class="font-extrabold text-lg">توصية سريعة</div>
            <div class="text-white/70 text-sm mt-1">أدخل طولك ووزنك (تجريبي) وسنعطيك مقاسًا مقترحًا.</div>

            <div class="mt-4 grid grid-cols-2 gap-3">
              <div>
                <label class="text-sm text-white/70">الطول (سم)</label>
                <input id="hInput" class="field mt-2" placeholder="170" inputmode="numeric" />
              </div>
              <div>
                <label class="text-sm text-white/70">الوزن (كجم)</label>
                <input id="wInput" class="field mt-2" placeholder="75" inputmode="numeric" />
              </div>
            </div>
            <div class="mt-4 flex gap-2">
              <button id="calcSizeBtn" class="btn btn-primary rounded-2xl px-5">احسب</button>
              <button id="resetSizeBtn" class="btn btn-ghost rounded-2xl px-5">مسح</button>
            </div>
            <div id="sizeResult" class="mt-4 glass rounded-2xl p-4 border border-white/10 text-white/80">
              المقاس المقترح: <span class="text-[var(--gold2)] font-extrabold">—</span>
            </div>
          </div>

          <div class="glass rounded-2xl p-5 border border-white/10">
            <div class="font-extrabold text-lg">جدول تقريبي</div>
            <div class="text-white/70 text-sm mt-1">الأرقام تقريبية وقد تختلف حسب القماش.</div>

            <div class="mt-4 overflow-auto">
              <table class="w-full text-sm" style="border-collapse:separate; border-spacing:0 10px;">
                <thead>
                  <tr class="text-white/65">
                    <th class="text-right px-3">المقاس</th>
                    <th class="text-right px-3">الطول (سم)</th>
                    <th class="text-right px-3">الوزن (كجم)</th>
                  </tr>
                </thead>
                <tbody>
                  <tr class="glass" style="border:1px solid rgba(255,255,255,.10);">
                    <td class="px-3 py-3 rounded-r-2xl font-extrabold">S</td>
                    <td class="px-3 py-3 text-white/75">160–170</td>
                    <td class="px-3 py-3 rounded-l-2xl text-white/75">55–68</td>
                  </tr>
                  <tr class="glass" style="border:1px solid rgba(255,255,255,.10);">
                    <td class="px-3 py-3 rounded-r-2xl font-extrabold">M</td>
                    <td class="px-3 py-3 text-white/75">168–178</td>
                    <td class="px-3 py-3 rounded-l-2xl text-white/75">65–80</td>
                  </tr>
                  <tr class="glass" style="border:1px solid rgba(255,255,255,.10);">
                    <td class="px-3 py-3 rounded-r-2xl font-extrabold">L</td>
                    <td class="px-3 py-3 text-white/75">175–185</td>
                    <td class="px-3 py-3 rounded-l-2xl text-white/75">78–92</td>
                  </tr>
                  <tr class="glass" style="border:1px solid rgba(255,255,255,.10);">
                    <td class="px-3 py-3 rounded-r-2xl font-extrabold">XL</td>
                    <td class="px-3 py-3 text-white/75">182–192</td>
                    <td class="px-3 py-3 rounded-l-2xl text-white/75">90–110</td>
                  </tr>
                </tbody>
              </table>
            </div>

            <div class="mt-3 text-xs text-white/55 leading-relaxed">
              إذا تحب لبس واسع اختر مقاسًا أكبر بدرجة.
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Cart Modal -->
  <div id="cartOverlay" class="overlay" role="dialog" aria-modal="true" aria-label="السلة">
    <div class="modal">
      <div class="p-4 md:p-5 border-b border-white/10 flex items-center justify-between gap-3">
        <div class="flex items-center gap-2">
          <div class="font-extrabold">سلة المشتريات</div>
          <span id="cartItemsBadge" class="chip" style="background: rgba(215,178,95,.12); border-color: rgba(215,178,95,.35);">0 عنصر</span>
        </div>
        <div class="flex items-center gap-2">
          <button id="closeCartBtn" class="btn btn-ghost h-10 px-3 rounded-xl" aria-label="إغلاق">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" aria-hidden="true">
              <path d="M6 6l12 12M18 6L6 18" stroke="rgba(255,255,255,.9)" stroke-width="2" stroke-linecap="round"/>
            </svg>
          </button>
        </div>
      </div>

      <div class="modal-body p-4 md:p-6 grid lg:grid-cols-3 gap-4">
        <div class="lg:col-span-2 space-y-3" id="cartItems"></div>

        <div class="glass rounded-2xl p-5 border border-white/10 h-fit">
          <div class="font-extrabold text-lg">الإجمالي</div>

          <div class="mt-4 space-y-2">
            <div class="flex items-center justify-between text-white/75">
              <span>المجموع الفرعي</span>
              <span class="font-extrabold" id="cartSubtotal">0 ر.س</span>
            </div>
            <div class="flex items-center justify-between text-white/75">
              <span>الشحن</span>
              <span class="font-extrabold" id="cartShipping">25 ر.س</span>
            </div>
            <div class="flex items-center justify-between text-white/75">
              <span>الخصم</span>
              <span class="font-extrabold text-[var(--gold2)]" id="cartDiscount">0 ر.س</span>
            </div>

            <div class="h-px bg-white/10 my-2"></div>
            <div class="flex items-center justify-between">
              <span class="text-white/75">الإجمالي</span>
              <span class="font-extrabold text-2xl text-[var(--gold2)]" id="cartTotal">0 ر.س</span>
            </div>
          </div>

          <div class="mt-4 flex flex-col gap-2">
            <a href="#checkout" class="btn btn-primary rounded-2xl w-full" id="goCheckoutBtn">إتمام الشراء</a>
            <button class="btn btn-outline rounded-2xl w-full" id="continueShoppingBtn">متابعة التسوق</button>
          </div>

          <div class="mt-4 text-xs text-white/55 leading-relaxed">
            تقدر تعدّل الكمية والمقاس من هنا.
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Toasts -->
  <div class="toast-wrap" id="toastWrap"></div>

  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            maroon: '#7b0f2a',
            gold: '#d7b25f'
          }
        }
      }
    };
  </script>

  <script>
    const state = {
      filter: 'all',
      sort: 'featured',
      view: 'grid',
      coupon: null, // {code, type, value}
      selectedSizeByProduct: {},
      cart: []
    };

    const PRODUCTS = [
      { id:'mah-001', name:'مخور اللمسة الذهبية', price:399, rating:4.8, badge:'فاخر', tags:['premium'], color:'عنابي', fabric:'جبر دبل', desc:'عنابي مطفي مع تطريز ذهبي ناعم. حضور قوي وذوق هادئ.', featured:10 },
      { id:'mah-002', name:'مخور أناقة يومية', price:249, rating:4.6, badge:'يومي', tags:['daily'], color:'عنابي', fabric:'كريب راقي', desc:'خفيف ومريح، تفاصيل نظيفة وملائم للاستخدام اليومي.', featured:8 },
      { id:'mah-003', name:'مخور الأبيض المذهب', price:319, rating:4.7, badge:'هدايا', tags:['gift','premium'], color:'أبيض', fabric:'كريب مطور', desc:'أبيض فخم مع خطوط ذهبية خفيفة. خيار هدية ممتاز.', featured:7 },
      { id:'mah-004', name:'مخور خط أبيض', price:279, rating:4.5, badge:'يومي', tags:['daily'], color:'عنابي', fabric:'لينن مخلوط', desc:'عنابي مع خط أبيض نظيف. بسيط وراقي.', featured:6 },
      { id:'mah-005', name:'مخور إصدار محدود', price:459, rating:4.9, badge:'حصري', tags:['limited','premium'], color:'عنابي', fabric:'جبر سوبر', desc:'إصدار محدود بتفاصيل ذهبية أعمق وقصة أنيقة.', featured:9 },
      { id:'mah-006', name:'مخور البصمة الذهبية', price:429, rating:4.9, badge:'الأكثر', tags:['premium','best'], color:'عنابي', fabric:'جبر دبل', desc:'القطعة الأكثر طلبًا: عنابي غني وتطريز ذهبي متوازن.', featured:11 },
      { id:'mah-007', name:'مخور هدية ملكية', price:359, rating:4.8, badge:'هدايا', tags:['gift'], color:'أبيض', fabric:'كريب ملكي', desc:'مناسب للإهداء مع إحساس فاخر وخطوط ذهبية ناعمة.', featured:5 },
      { id:'mah-008', name:'مخور ليلة عنابية', price:389, rating:4.7, badge:'فاخر', tags:['premium'], color:'عنابي', fabric:'مخمل خفيف', desc:'ملمس ناعم ولمعة بسيطة؛ مثالي للطلعات والمناسبات.', featured:4 },
      { id:'mah-009', name:'مخور كلاسيك أبيض', price:229, rating:4.4, badge:'يومي', tags:['daily'], color:'أبيض', fabric:'قطن مخلوط', desc:'أبيض نظيف بقصة مريحة وسهلة العناية.', featured:3 }
    ];

    const fmt = (n) => new Intl.NumberFormat('ar-SA').format(n) + ' ر.س';
    const qs = (s, el=document) => el.querySelector(s);
    const qsa = (s, el=document) => [...el.querySelectorAll(s)];

    function showToast(title, msg){
      const wrap = qs('#toastWrap');
      const t = document.createElement('div');
      t.className = 'toast';
      t.innerHTML = `
        <div class="h-10 w-10 rounded-2xl flex items-center justify-center shrink-0"
          style="background: rgba(215,178,95,.12); border:1px solid rgba(215,178,95,.28);">
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M20 6 9 17l-5-5" stroke="rgba(255,255,255,.92)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
          </svg>
        </div>
        <div class="min-w-0">
          <div class="font-extrabold">${title}</div>
          <div class="text-sm text-white/70 leading-relaxed">${msg}</div>
        </div>
        <button class="btn btn-ghost h-9 px-3 rounded-xl shrink-0" aria-label="إغلاق">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" aria-hidden="true">
            <path d="M6 6l12 12M18 6L6 18" stroke="rgba(255,255,255,.85)" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
      `;
      const closeBtn = t.querySelector('button');
      closeBtn.onclick = () => t.remove();
      wrap.appendChild(t);
      setTimeout(()=>{ t.style.opacity = '0'; t.style.transform='translateY(8px)'; t.style.transition='opacity .2s ease, transform .2s ease'; }, 3200);
      setTimeout(()=> t.remove(), 3500);
    }

    function getCoupon(code){
      const c = (code||'').trim().toUpperCase();
      if(c === 'MAHAWER10') return { code:c, type:'percent', value:10 };
      if(c === 'GOLD25') return { code:c, type:'fixed', value:25 };
      return null;
    }

    function cartCount(){
      return state.cart.reduce((sum, it)=> sum + it.qty, 0);
    }
    function cartSubtotal(){
      return state.cart.reduce((sum, it)=> sum + it.price * it.qty, 0);
    }
    function cartDiscount(subtotal){
      if(!state.coupon) return 0;
      if(state.coupon.type === 'percent') return Math.round(subtotal * (state.coupon.value/100));
      if(state.coupon.type === 'fixed') return Math.min(state.coupon.value, subtotal);
      return 0;
    }
    function shippingCost(subtotal){
      const base = 25;
      if(subtotal >= 500) return 0;
      if(subtotal === 0) return base;
      return base;
    }

    function updateCartBadge(){
      const count = cartCount();
      const cc = qs('#cartCount');
      const badge = qs('#cartItemsBadge');
      badge.textContent = `${count} عنصر`;
      if(count > 0){
        cc.style.display = 'flex';
        cc.textContent = count;
      }else{
        cc.style.display = 'none';
      }
    }

    function updateSummary(){
      const sub = cartSubtotal();
      const disc = cartDiscount(sub);
      const ship = shippingCost(sub - disc);
      const total = Math.max(0, sub - disc + ship);

      qs('#subtotalText').textContent = fmt(sub);
      qs('#discountText').textContent = fmt(disc);
      qs('#shippingText').textContent = ship === 0 ? 'مجاني' : fmt(ship);
      qs('#totalText').textContent = fmt(total);

      qs('#cartSubtotal').textContent = fmt(sub);
      qs('#cartDiscount').textContent = fmt(disc);
      qs('#cartShipping').textContent = ship === 0 ? 'مجاني' : fmt(ship);
      qs('#cartTotal').textContent = fmt(total);
    }

    function addToCart(productId, opts={}){
      const p = PRODUCTS.find(x => x.id === productId);
      if(!p) return;

      const size = opts.size || state.selectedSizeByProduct[productId] || 'M';
      const key = `${productId}__${size}`;
      const existing = state.cart.find(x => x.key === key);

      if(existing){
        existing.qty += 1;
      } else {
        state.cart.push({
          key,
          id: p.id,
          name: p.name,
          price: p.price,
          color: p.color,
          size,
          qty: 1
        });
      }

      persist();
      renderCart();
      updateCartBadge();
      updateSummary();
      showToast('تمت الإضافة', `${p.name} (مقاس ${size})`);
    }

    function removeFromCart(key){
      state.cart = state.cart.filter(x => x.key !== key);
      persist();
      renderCart();
      updateCartBadge();
      updateSummary();
    }

    function changeQty(key, delta){
      const it = state.cart.find(x => x.key === key);
      if(!it) return;
      it.qty = Math.max(1, it.qty + delta);
      persist();
      renderCart();
      updateCartBadge();
      updateSummary();
    }

    function changeSize(key, newSize){
      const it = state.cart.find(x => x.key === key);
      if(!it) return;
      const baseId = it.id;
      const newKey = `${baseId}__${newSize}`;

      // if item with same product+size exists merge
      const same = state.cart.find(x => x.key === newKey);
      if(same && same !== it){
        same.qty += it.qty;
        state.cart = state.cart.filter(x => x.key !== key);
      }else{
        it.size = newSize;
        it.key = newKey;
      }
      persist();
      renderCart();
      updateCartBadge();
      updateSummary();
    }

    function clearCart(){
      state.cart = [];
      persist();
      renderCart();
      updateCartBadge();
      updateSummary();
      showToast('تم', 'تم تفريغ السلة');
    }

    function renderCart(){
      const wrap = qs('#cartItems');
      if(state.cart.length === 0){
        wrap.innerHTML = `
          <div class="glass rounded-2xl p-6 border border-white/10 text-center">
            <div class="text-2xl font-extrabold text-[var(--gold2)]">السلة فارغة</div>
            <div class="text-white/65 mt-1">ابدأ بإضافة مخورك المفضل.</div>
            <button class="btn btn-primary rounded-2xl px-6 mt-4" id="goNewBtn">تصفح الجديد</button>
          </div>
        `;
        const btn = qs('#goNewBtn');
        if(btn) btn.onclick = () => { closeCart(); location.hash = '#new'; };
        return;
      }

      wrap.innerHTML = state.cart.map(it => {
        const p = PRODUCTS.find(x => x.id === it.id);
        const bg = p?.color === 'أبيض'
          ? 'linear-gradient(135deg, rgba(255,255,255,.90), rgba(255,255,255,.14))'
          : 'linear-gradient(135deg, rgba(123,15,42,.88), rgba(10,7,14,.92))';

        return `
          <div class="glass rounded-2xl p-4 border border-white/10 flex gap-3 items-start">
            <div class="h-20 w-20 rounded-2xl border border-white/10 overflow-hidden relative shrink-0" style="background:${bg}">
              <div class="absolute inset-0" style="background:
                radial-gradient(120px 100px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
                radial-gradient(180px 140px at 80% 70%, rgba(255,255,255,.06), transparent 70%);"></div>
              <div class="absolute inset-0 shine"></div>
            </div>

            <div class="flex-1 min-w-0">
              <div class="flex items-start justify-between gap-2">
                <div class="min-w-0">
                  <div class="font-extrabold truncate">${it.name}</div>
                  <div class="text-xs text-white/60 mt-0.5">لون: ${it.color} • خامة: ${p?.fabric || '—'}</div>
                </div>
                <button class="btn btn-ghost h-10 px-3 rounded-xl remove-item" data-key="${it.key}" aria-label="حذف">
                  <svg width="18" height="18" viewBox="0 0 24 24" fill="none">
                    <path d="M4 7h16M10 11v6M14 11v6M6 7l1 14h10l1-14M9 7V4h6v3" stroke="rgba(255,255,255,.85)" stroke-width="2" stroke-linecap="round"/>
                  </svg>
                </button>
              </div>

              <div class="mt-3 flex flex-wrap items-center gap-2 justify-between">
                <div class="flex items-center gap-2">
                  <span class="chip">المقاس</span>
                  <select class="field !py-0 h-10" style="width: 120px;" data-size-select="${it.key}">
                    ${['S','M','L','XL'].map(s => `<option value="${s}" ${s===it.size?'selected':''}>${s}</option>`).join('')}
                  </select>
                </div>

                <div class="flex items-center gap-2">
                  <button class="btn btn-outline h-10 px-3 rounded-xl qty-btn" data-key="${it.key}" data-delta="-1" aria-label="تقليل">−</button>
                  <span class="chip" style="min-width:64px; justify-content:center;">${it.qty}</span>
                  <button class="btn btn-outline h-10 px-3 rounded-xl qty-btn" data-key="${it.key}" data-delta="1" aria-label="زيادة">+</button>
                </div>
              </div>

              <div class="mt-3 flex items-center justify-between">
                <div class="text-white/60 text-sm">السعر</div>
                <div class="font-extrabold text-[var(--gold2)]">${fmt(it.price * it.qty)}</div>
              </div>
            </div>
          </div>
        `;
      }).join('');

      qsa('.remove-item', wrap).forEach(btn => {
        btn.onclick = () => removeFromCart(btn.dataset.key);
      });
      qsa('.qty-btn', wrap).forEach(btn => {
        btn.onclick = () => changeQty(btn.dataset.key, Number(btn.dataset.delta));
      });
      qsa('select[data-size-select]', wrap).forEach(sel => {
        sel.onchange = () => changeSize(sel.dataset.sizeSelect, sel.value);
      });
    }

    function productCard(p){
      const isWhite = p.color === 'أبيض';
      const bg = isWhite
        ? 'linear-gradient(135deg, rgba(255,255,255,.92), rgba(255,255,255,.12))'
        : 'linear-gradient(135deg, rgba(123,15,42,.88), rgba(10,7,14,.92))';

      const badgeStyle = p.tags.includes('limited')
        ? 'background: rgba(123,15,42,.22); border-color: rgba(123,15,42,.45);'
        : 'background: rgba(215,178,95,.12); border-color: rgba(215,178,95,.35);';

      return `
        <article class="glass rounded-2xl border border-white/10 overflow-hidden hover-lift">
          <div class="relative p-4">
            <div class="rounded-2xl h-44 border border-white/10 overflow-hidden relative" style="background:${bg}">
              <div class="absolute inset-0" style="background:
                radial-gradient(220px 170px at 30% 25%, rgba(242,210,138,.18), transparent 60%),
                radial-gradient(320px 260px at 80% 70%, rgba(255,255,255,.06), transparent 70%);"></div>
              <div class="absolute inset-0 shine"></div>

              <div class="absolute top-3 right-3 flex items-center gap-2">
                <span class="chip" style="${badgeStyle}">${p.badge}</span>
                <span class="chip">⭐ ${p.rating}</span>
              </div>

              <button class="btn btn-ghost h-10 px-4 rounded-xl absolute bottom-3 left-3 quick-view" data-id="${p.id}">
                معاينة
              </button>
            </div>

            <div class="mt-4">
              <div class="flex items-start justify-between gap-3">
                <div class="min-w-0">
                  <h3 class="font-extrabold text-lg truncate">${p.name}</h3>
                  <div class="text-xs text-white/60 mt-0.5">لون: ${p.color} • خامة: ${p.fabric}</div>
                </div>
                <div class="text-left">
                  <div class="text-xs text-white/60">السعر</div>
                  <div class="font-extrabold text-[var(--gold2)] text-xl">${fmt(p.price)}</div>
                </div>
              </div>

              <p class="text-white/70 text-sm leading-relaxed mt-3 line-clamp-2" style="display:-webkit-box; -webkit-line-clamp:2; -webkit-box-orient:vertical; overflow:hidden;">
                ${p.desc}
              </p>

              <div class="mt-4 flex flex-col sm:flex-row gap-2">
                <button class="btn btn-primary rounded-2xl px-5 add-to-cart" data-id="${p.id}" data-name="${p.name}" data-price="${p.price}" data-color="${p.color}" data-size="M">
                  أضف للسلة
                </button>
                <button class="btn btn-outline rounded-2xl px-5 quick-view" data-id="${p.id}">
                  تفاصيل
                </button>
              </div>

              <div class="mt-3 flex flex-wrap gap-2">
                ${p.tags.includes('premium') ? `<span class="chip">تطريز ذهبي</span>` : `<span class="chip">قصة مريحة</span>`}
                ${p.tags.includes('gift') ? `<span class="chip">تغليف هدية</span>` : `<span class="chip">شحن سريع</span>`}
                ${p.tags.includes('limited') ? `<span class="chip" style="background: rgba(123,15,42,.22); border-color: rgba(123,15,42,.45);">كمية محدودة</span>` : ``}
              </div>
            </div>
          </div>
        </article>
      `;
    }

    function filteredProducts(){
      let list = [...PRODUCTS];

      // Search
      const s1 = (qs('#searchInput')?.value || '').trim();
      const s2 = (qs('#searchInputMobile')?.value || '').trim();
      const s = (s2 || s1).toLowerCase();
      if(s){
        list = list.filter(p =>
          (p.name + ' ' + p.color + ' ' + p.fabric + ' ' + p.desc + ' ' + p.tags.join(' '))
            .toLowerCase().includes(s)
        );
      }

      // Filter
      if(state.filter !== 'all'){
        list = list.filter(p => p.tags.includes(state.filter));
      }

      // Sort
      if(state.sort === 'priceAsc') list.sort((a,b)=> a.price - b.price);
      else if(state.sort === 'priceDesc') list.sort((a,b)=> b.price - a.price);
      else if(state.sort === 'ratingDesc') list.sort((a,b)=> b.rating - a.rating);
      else list.sort((a,b)=> (b.featured||0) - (a.featured||0));

      return list;
    }

    function renderProducts(){
      const wrap = qs('#productsWrap');
      const list = filteredProducts();
      if(list.length === 0){
        wrap.innerHTML = `
          <div class="glass rounded-2xl p-8 border border-white/10 text-center sm:col-span-2 lg:col-span-3">
            <div class="text-2xl font-extrabold text-[var(--gold2)]">لا توجد نتائج</div>
            <div class="text-white/65 mt-1">جرّب كلمة بحث مختلفة أو اختر تصنيفًا آخر.</div>
            <button class="btn btn-outline rounded-2xl px-6 mt-4" id="resetFiltersBtn">إعادة الضبط</button>
          </div>
        `;
        qs('#resetFiltersBtn').onclick = () => {
          state.filter = 'all';
          state.sort = 'featured';
          qs('#sortSelect').value = 'featured';
          qsa('.filter-btn').forEach(b => b.classList.remove('!bg-white/10'));
          renderProducts();
        };
        return;
      }

      // view
      if(state.view === 'list'){
        wrap.className = 'mt-6 grid grid-cols-1 gap-4';
      }else{
        wrap.className = 'mt-6 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-4';
      }

      wrap.innerHTML = list.map(productCard).join('');

      qsa('.add-to-cart', wrap).forEach(btn => {
        btn.onclick = () => addToCart(btn.dataset.id, { size: btn.dataset.size || 'M' });
      });
      qsa('.quick-view', wrap).forEach(btn => {
        btn.onclick = () => openQuickView(btn.dataset.id);
      });
    }

    // Quick view modal
    let modalProductId = null;
    let modalSelectedSize = 'M';

    function openQuickView(id){
      const p = PRODUCTS.find(x => x.id === id);
      if(!p) return;
      modalProductId = id;
      modalSelectedSize = state.selectedSizeByProduct[id] || 'M';

      qs('#modalTitle').textContent = p.name;
      qs('#modalMeta').textContent = `⭐ ${p.rating} • ${p.badge}`;
      qs('#modalPrice').textContent = fmt(p.price);
      qs('#modalDesc').textContent = p.desc;
      qs('#modalColor').textContent = p.color;
      qs('#modalFabric').textContent = p.fabric;
      qs('#modalRating').textContent = `⭐ ${p.rating}`;
      qs('#modalBadge').textContent = p.badge;

      const swatch = (p.color === 'أبيض')
        ? 'linear-gradient(135deg, rgba(255,255,255,.92), rgba(255,255,255,.12))'
        : 'linear-gradient(135deg, rgba(123,15,42,.88), rgba(10,7,14,.92))';

      qs('#modalSwatch').style.background = swatch;
      qs('#modalHero').style.background = swatch;

      // size buttons
      qsa('[data-size]', qs('#modalOverlay')).forEach(b=>{
        const isActive = b.dataset.size === modalSelectedSize;
        b.classList.toggle('btn-primary', isActive);
        b.classList.toggle('btn-ghost', !isActive);
      });

      const overlay = qs('#modalOverlay');
      overlay.classList.add('open');
      document.body.style.overflow = 'hidden';
    }

    function closeQuickView(){
      qs('#modalOverlay').classList.remove('open');
      document.body.style.overflow = '';
    }

    // Cart modal
    function openCart(){
      renderCart();
      updateSummary();
      qs('#cartOverlay').classList.add('open');
      document.body.style.overflow = 'hidden';
    }
    function closeCart(){
      qs('#cartOverlay').classList.remove('open');
      document.body.style.overflow = '';
    }

    // Size modal
    function openSizeGuide(){
      qs('#sizeOverlay').classList.add('open');
      document.body.style.overflow = 'hidden';
    }
    function closeSizeGuide(){
      qs('#sizeOverlay').classList.remove('open');
      document.body.style.overflow = '';
    }

    // Drawer
    function openDrawer(){
      qs('#drawer').classList.add('open');
      qs('#drawerOverlay').classList.remove('hidden');
      document.body.style.overflow = 'hidden';
    }
    function closeDrawer(){
      qs('#drawer').classList.remove('open');
      qs('#drawerOverlay').classList.add('hidden');
      document.body.style.overflow = '';
    }

    // Persist
    function persist(){
      localStorage.setItem('mah_cart', JSON.stringify(state.cart));
      localStorage.setItem('mah_coupon', JSON.stringify(state.coupon));
      localStorage.setItem('mah_sizes', JSON.stringify(state.selectedSizeByProduct));
    }
    function restore(){
      try{
        const c = JSON.parse(localStorage.getItem('mah_cart') || '[]');
        const coupon = JSON.parse(localStorage.getItem('mah_coupon') || 'null');
        const sizes = JSON.parse(localStorage.getItem('mah_sizes') || '{}');
        if(Array.isArray(c)) state.cart = c;
        state.coupon = coupon;
        state.selectedSizeByProduct = sizes || {};
      }catch(e){}
    }

    // Deal timer
    function startDealTimer(){
      const el = qs('#dealTimer');
      const end = Date.now() + 1000*60*42 + 1000*18; // 42:18
      const tick = () => {
        const d = Math.max(0, end - Date.now());
        const m = Math.floor(d/60000);
        const s = Math.floor((d%60000)/1000);
        el.textContent = `${String(m).padStart(2,'0')}:${String(s).padStart(2,'0')}`;
      };
      tick();
      setInterval(tick, 1000);
    }

    // Events
    function bind(){
      // Header scroll
      const header = qs('#siteHeader');
      window.addEventListener('scroll', () => {
        header.classList.toggle('scrolled', window.scrollY > 8);
      });

      // Drawer
      qs('#menuBtn').onclick = openDrawer;
      qs('#closeDrawerBtn').onclick = closeDrawer;
      qs('#drawerOverlay').onclick = closeDrawer;
      qsa('#drawer a').forEach(a => a.addEventListener('click', closeDrawer));

      qs('#copyCodeBtn').onclick = async () => {
        try{
          await navigator.clipboard.writeText('MAHAWER10');
          showToast('تم النسخ', 'كود الخصم MAHAWER10');
        }catch(e){
          showToast('ملاحظة', 'انسخ الكود يدويًا: MAHAWER10');
        }
      };

      // Search
      const onSearch = () => renderProducts();
      qs('#searchInput').addEventListener('input', onSearch);
      qs('#searchInputMobile').addEventListener('input', onSearch);

      // Filters
      qsa('.filter-btn').forEach(btn => {
        btn.addEventListener('click', () => {
          state.filter = btn.dataset.filter || 'all';
          // visual
          qsa('.filter-btn').forEach(b => b.classList.remove('!bg-white/10'));
          qsa(`.filter-btn[data-filter="${state.filter}"]`).forEach(b => b.classList.add('!bg-white/10'));
          renderProducts();
        });
      });
      // set default filter style
      qsa('.filter-btn[data-filter="all"]').forEach(b => b.classList.add('!bg-white/10'));

      // Sort
      qs('#sortSelect').addEventListener('change', (e) => {
        state.sort = e.target.value;
        renderProducts();
      });

      // View toggle
      qs('#viewToggleBtn').onclick = () => {
        state.view = state.view === 'grid' ? 'list' : 'grid';
        renderProducts();
        showToast('تم', state.view === 'grid' ? 'عرض شبكي' : 'عرض قائمة');
      };

      // Surprise
      qs('#surpriseBtn').onclick = () => {
        const pick = PRODUCTS[Math.floor(Math.random()*PRODUCTS.length)];
        openQuickView(pick.id);
      };

      // Quick modal close
      qs('#closeModalBtn').onclick = closeQuickView;
      qs('#modalOverlay').addEventListener('click', (e) => {
        if(e.target === qs('#modalOverlay')) closeQuickView();
      });

      // Modal sizes
      qsa('[data-size]', qs('#modalOverlay')).forEach(b => {
        b.onclick = () => {
          modalSelectedSize = b.dataset.size;
          if(modalProductId) state.selectedSizeByProduct[modalProductId] = modalSelectedSize;
          persist();
          qsa('[data-size]', qs('#modalOverlay')).forEach(x=>{
            const active = x.dataset.size === modalSelectedSize;
            x.classList.toggle('btn-primary', active);
            x.classList.toggle('btn-ghost', !active);
          });
        };
      });

      // Modal add
      qs('#modalAddBtn').onclick = () => {
        if(!modalProductId) return;
        state.selectedSizeByProduct[modalProductId] = modalSelectedSize;
        persist();
        addToCart(modalProductId, { size: modalSelectedSize });
      };

      // Open size guide
      qs('#openSizeGuideBtn').onclick = openSizeGuide;
      qs('#closeSizeBtn').onclick = closeSizeGuide;
      qs('#sizeOverlay').addEventListener('click', (e) => {
        if(e.target === qs('#sizeOverlay')) closeSizeGuide();
      });

      // Size calculator
      qs('#calcSizeBtn').onclick = () => {
        const h = Number(qs('#hInput').value);
        const w = Number(qs('#wInput').value);
        let size = 'M';
        if(!h || !w){
          qs('#sizeResult').innerHTML = `المقاس المقترح: <span class="text-[var(--gold2)] font-extrabold">—</span>`;
          showToast('ملاحظة', 'أدخل الطول والوزن');
          return;
        }
        if(w < 68 && h <= 170) size = 'S';
        else if(w <= 80 && h <= 178) size = 'M';
        else if(w <= 92 && h <= 185) size = 'L';
        else size = 'XL';

        qs('#sizeResult').innerHTML = `المقاس المقترح: <span class="text-[var(--gold2)] font-extrabold">${size}</span>`;
        showToast('تم', `المقاس المقترح: ${size}`);
      };
      qs('#resetSizeBtn').onclick = () => {
        qs('#hInput').value = '';
        qs('#wInput').value = '';
        qs('#sizeResult').innerHTML = `المقاس المقترح: <span class="text-[var(--gold2)] font-extrabold">—</span>`;
      };

      // Cart open/close
      qs('#openCartBtn').onclick = openCart;
      qs('#openCartBtn2').onclick = openCart;
      qs('#closeCartBtn').onclick = closeCart;
      qs('#cartOverlay').addEventListener('click', (e) => {
        if(e.target === qs('#cartOverlay')) closeCart();
      });
      qs('#continueShoppingBtn').onclick = () => { closeCart(); location.hash = '#new'; };
      qs('#goCheckoutBtn').onclick = () => { closeCart(); };

      // Coupon
      const applyCoupon = () => {
        const code = (qs('#coupon').value || '').trim();
        const c = getCoupon(code);
        const hint = qs('#couponHint');
        if(!code){
          state.coupon = null;
          hint.textContent = 'أدخل كود خصم (اختياري).';
          persist();
          updateSummary();
          showToast('تم', 'تم مسح الكوبون');
          return;
        }
        if(!c){
          hint.textContent = 'الكود غير صحيح. جرّب MAHAWER10.';
          showToast('غير صحيح', 'الكود غير صالح');
          return;
        }
        state.coupon = c;
        hint.textContent = `تم تطبيق الكود: ${c.code} (${c.type === 'percent' ? c.value+'%' : c.value+' ر.س'})`;
        persist();
        updateSummary();
        showToast('تم', `تم تطبيق ${c.code}`);
      };
      qs('#applyCouponBtn').onclick = applyCoupon;

      // Checkout actions
      qs('#clearCartBtn').onclick = clearCart;
      qs('#placeOrderBtn').onclick = () => {
        const name = qs('#name').value.trim();
        const phone = qs('#phone').value.trim();
        const address = qs('#address').value.trim();
        if(state.cart.length === 0){
          showToast('تنبيه', 'سلتك فارغة');
          openCart();
          return;
        }
        if(!name || !phone || !address){
          showToast('تنبيه', 'أكمل البيانات: الاسم، الجوال، العنوان');
          return;
        }
        showToast('تم استلام الطلب', 'هذا نموذج تجريبي — يمكنك ربط الدفع والشحن لاحقًا.');
        clearCart();
        qs('#name').value = '';
        qs('#phone').value = '';
        qs('#address').value = '';
      };

      // Newsletter
      qs('#newsletterBtn').onclick = () => {
        const email = qs('#newsletterEmail').value.trim();
        if(!email || !email.includes('@')){
          showToast('تنبيه', 'أدخل بريدًا صحيحًا');
          return;
        }
        qs('#newsletterEmail').value = '';
        showToast('تم', 'تم تسجيلك (تجريبي)');
      };

      // Global add-to-cart buttons outside grid
      qsa('.add-to-cart').forEach(btn => {
        btn.addEventListener('click', () => addToCart(btn.dataset.id, { size: btn.dataset.size || 'M' }));
      });

      // Quick view buttons outside grid
      qsa('[data-quick]').forEach(btn => {
        btn.addEventListener('click', () => openQuickView(btn.dataset.quick));
      });

      // Escape
      document.addEventListener('keydown', (e) => {
        if(e.key === 'Escape'){
          closeQuickView();
          closeCart();
          closeSizeGuide();
          closeDrawer();
        }
      });
    }

    // Init
    restore();

    // Year
    const y = new Date().getFullYear();
    qs('#year').textContent = y;
    qs('#year2').textContent = y;

    // Coupon UI restore
    if(state.coupon){
      qs('#coupon').value = state.coupon.code;
      qs('#couponHint').textContent = `تم تطبيق الكود: ${state.coupon.code}`;
    }else{
      qs('#couponHint').textContent = 'أدخل كود خصم (اختياري).';
    }

    updateCartBadge();
    renderProducts();
    renderCart();
    updateSummary();
    startDealTimer();
    bind();
  </script>
</body>
</html>
