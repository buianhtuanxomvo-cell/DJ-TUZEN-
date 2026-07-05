<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DJ TUZEN | OFFICIAL BOOKING PROFILE</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@600;800;900&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --bg-color: #07030e;
            --card-bg: rgba(18, 9, 32, 0.65);
            --card-hover: rgba(26, 13, 46, 0.85);
            --primary-neon: #00f0ff; 
            --secondary-neon: #ff007f; 
            --accent-orange: #ff6600; 
            --accent-green: #00ff66; 
            --text-main: #f3f0f7;
            --text-muted: #a59cb5;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        html { scroll-behavior: smooth; }
        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-main);
            line-height: 1.7;
            overflow-x: hidden;
            background-image: 
                linear-gradient(rgba(0, 240, 255, 0.015) 1px, transparent 1px),
                linear-gradient(90deg, rgba(0, 240, 255, 0.015) 1px, transparent 1px),
                radial-gradient(circle at 0% 15%, rgba(255, 0, 127, 0.12) 0%, transparent 50%),
                radial-gradient(circle at 100% 85%, rgba(0, 240, 255, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 50% 50%, rgba(112, 0, 255, 0.06) 0%, transparent 70%);
            background-size: 40px 40px, 40px 40px, auto, auto, auto;
            background-attachment: fixed;
        }

        body.lock-scroll { overflow: hidden; height: 100vh; }

        /* --- LED MATRIX BACKGROUND CLOUD --- */
        .led-bg-grid {
            position: fixed; top: 0; left: 0; width: 100vw; height: 100vh;
            pointer-events: none; z-index: 0; display: grid;
            grid-template-columns: repeat(auto-fill, minmax(60px, 1fr));
            grid-template-rows: repeat(auto-fill, minmax(60px, 1fr));
            gap: 4px; padding: 4px; opacity: 0.25;
        }
        .led-dot {
            background: rgba(255, 255, 255, 0.01); border-radius: 50%;
            animation: ledFlash 4s infinite ease-in-out;
        }
        @keyframes ledFlash {
            0%, 100% { background: rgba(255, 255, 255, 0.01); box-shadow: none; }
            50% { background: var(--primary-neon); box-shadow: 0 0 10px var(--primary-neon); }
        }
        .led-dot:nth-child(3n) { animation-delay: 0.5s; }
        .led-dot:nth-child(5n) { animation-name: ledFlashPink; animation-delay: 1.2s; }
        @keyframes ledFlashPink {
            0%, 100% { background: rgba(255, 255, 255, 0.01); box-shadow: none; }
            50% { background: var(--secondary-neon); box-shadow: 0 0 10px var(--secondary-neon); }
        }

        /* --- CYBER SPLASH WELCOME SCREEN --- */
        #welcome-screen {
            position: fixed; top: 0; left: 0; width: 100vw; height: 100vh;
            background-color: #030106; z-index: 9999; display: flex;
            justify-content: center; align-items: center; cursor: pointer;
            transition: transform 0.8s cubic-bezier(0.77, 0, 0.175, 1), opacity 0.6s ease;
            overflow: hidden;
        }
        #welcome-screen.fade-out { transform: translateY(-100vh); opacity: 0; pointer-events: none; }
        .welcome-bg-overlay {
            position: absolute; top: 0; left: 0; width: 100%; height: 100%;
            background: 
                radial-gradient(circle at 20% 20%, rgba(0, 240, 255, 0.2) 0%, transparent 40%),
                radial-gradient(circle at 80% 30%, rgba(255, 0, 127, 0.22) 0%, transparent 45%),
                linear-gradient(135deg, #05020a 0%, #020105 100%);
            z-index: 1;
        }
        .welcome-inner-layout {
            position: relative; z-index: 2; width: 100%; max-width: 1100px;
            padding: 0 40px; display: grid; grid-template-columns: 1.1fr 0.9fr;
            align-items: center; gap: 50px;
        }
        .welcome-text-side { display: flex; flex-direction: column; align-items: flex-start; }
        .welcome-badge-tag {
            font-family: 'Orbitron', sans-serif; font-size: 0.75rem; color: #fff;
            background: linear-gradient(90deg, rgba(0, 240, 255, 0.15), rgba(255, 0, 127, 0.15));
            border: 1px solid rgba(0, 240, 255, 0.4); padding: 6px 16px; border-radius: 4px;
            letter-spacing: 4px; text-transform: uppercase; margin-bottom: 20px; font-weight: 800;
        }
        .welcome-title {
            font-family: 'Orbitron', sans-serif; font-size: 4rem; font-weight: 900;
            text-transform: uppercase; color: #fff; line-height: 1.1;
        }
        .welcome-title span {
            background: linear-gradient(90deg, #00f0ff, #ff007f);
            -webkit-background-clip: text; -webkit-text-fill-color: transparent;
        }
        .welcome-subtitle {
            font-family: 'Orbitron', sans-serif; font-size: 1.25rem; color: var(--accent-orange);
            letter-spacing: 4px; margin-top: 15px; margin-bottom: 25px;
        }
        .welcome-desc { font-size: 1rem; color: var(--text-muted); max-width: 500px; margin-bottom: 30px; }
        .logo-frame-container { position: relative; width: 280px; height: 280px; display: flex; align-items: center; justify-content: center; }
        .radar-glow-ring {
            position: absolute; width: 100%; height: 100%; border-radius: 50%;
            border: 2px dashed rgba(0, 240, 255, 0.3); animation: spinDisc 25s linear infinite;
        }
        @keyframes spinDisc { 100% { transform: rotate(360deg); } }
        .welcome-logo { width: 85%; height: 85%; object-fit: cover; border-radius: 50%; border: 2px solid rgba(255, 255, 255, 0.1); z-index: 2; }

        /* --- CONTENT WRAPPER --- */
        .container { max-width: 800px; margin: 0 auto; padding: 60px 20px; position: relative; z-index: 5; }
        header { text-align: center; margin-bottom: 50px; }
        .brand-title { font-family: 'Orbitron', sans-serif; font-size: 2.6rem; font-weight: 900; letter-spacing: 4px; text-shadow: 0 0 15px rgba(0, 240, 255, 0.4); }
        .brand-subtitle { font-family: 'Orbitron', sans-serif; font-size: 0.95rem; color: var(--text-muted); letter-spacing: 5px; text-transform: uppercase; margin-top: 5px; }

        /* --- MAIN CARD --- */
        .card {
            background: var(--card-bg); border: 1px solid rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(16px); -webkit-backdrop-filter: blur(16px);
            padding: 40px; border-radius: 20px; margin-bottom: 45px; box-shadow: 0 20px 45px rgba(0, 0, 0, 0.5);
        }
        .card.card-commit {
            border: 1px solid rgba(255, 0, 127, 0.3);
            box-shadow: 0 0 25px rgba(255, 0, 127, 0.1);
        }
        .section-title { font-family: 'Orbitron', sans-serif; font-size: 1.25rem; text-transform: uppercase; letter-spacing: 2px; margin-bottom: 30px; display: flex; align-items: center; gap: 14px; }
        .section-title i { color: var(--primary-neon); }
        .card-commit .section-title i { color: var(--secondary-neon); }
        .responsive-img { width: 100%; height: auto; border-radius: 12px; display: block; border: 1px solid rgba(255, 255, 255, 0.08); margin-bottom: 25px; }

        /* --- TAB NAVIGATION --- */
        .tab-navigation-bar { display: flex; background: rgba(0, 0, 0, 0.4); border: 1px solid rgba(255, 255, 255, 0.05); padding: 6px; border-radius: 12px; margin-bottom: 30px; gap: 5px; }
        .tab-btn { flex: 1; background: transparent; border: none; color: var(--text-muted); font-family: 'Orbitron', sans-serif; font-size: 0.85rem; font-weight: 700; padding: 12px 10px; border-radius: 8px; cursor: pointer; text-transform: uppercase; display: flex; align-items: center; justify-content: center; gap: 8px; transition: all 0.3s ease; }
        .tab-btn.active { background: rgba(0, 240, 255, 0.1); color: var(--primary-neon); border: 1px solid rgba(0, 240, 255, 0.25); }
        .tab-content-panel { display: none; }
        .tab-content-panel.active { display: block; animation: fadeInTab 0.4s ease forwards; }
        @keyframes fadeInTab { from { opacity: 0; transform: translateY(10px); } to { opacity: 1; transform: translateY(0); } }

        /* --- PROFILE TAB --- */
        .profile-layout { display: grid; grid-template-columns: 1fr 1.2fr; gap: 35px; align-items: center; }
        .profile-info { display: flex; flex-direction: column; gap: 20px; }
        .profile-bio { font-size: 0.98rem; color: var(--text-muted); text-align: justify; }
        .profile-stats-grid { display: flex; flex-direction: column; gap: 15px; }
        .stat-item { background: rgba(255, 255, 255, 0.02); border: 1px solid rgba(255, 255, 255, 0.04); padding: 14px 18px; border-radius: 10px; display: flex; align-items: center; gap: 15px; }
        .stat-icon-wrapper { width: 40px; height: 40px; background: rgba(0, 240, 255, 0.08); border-radius: 8px; display: flex; align-items: center; justify-content: center; color: var(--primary-neon); }
        .stat-details span { display: block; font-size: 0.78rem; color: var(--text-muted); text-transform: uppercase; }
        .stat-details p { font-family: 'Orbitron', sans-serif; font-weight: 700; color: #fff; }

        /* --- MEDIA TAB --- */
        .media-showcase-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; }
        .video-wrapper-box { background: rgba(0, 0, 0, 0.4); border: 1px solid rgba(255, 255, 255, 0.05); border-radius: 12px; overflow: hidden; }
        .video-wrapper-box iframe { width: 100%; aspect-ratio: 16 / 9; display: block; background: #000; }
        .video-caption-info { padding: 12px 16px; background: rgba(15, 8, 26, 0.9); }
        .video-caption-info h4 { font-size: 0.9rem; color: #fff; white-space: nowrap; overflow: hidden; text-overflow: ellipsis; }
        .video-caption-info p { font-size: 0.75rem; color: var(--primary-neon); margin-top: 2px; }

        /* --- CALENDAR TAB --- */
        .calendar-dashboard { background: rgba(0, 0, 0, 0.3); border: 1px solid rgba(255, 255, 255, 0.04); border-radius: 14px; padding: 24px; }
        .calendar-header-title { display: flex; justify-content: space-between; align-items: center; margin-bottom: 20px; padding-bottom: 12px; border-bottom: 1px solid rgba(255, 255, 255, 0.05); }
        .calendar-controls { display: flex; align-items: center; gap: 15px; }
        .calendar-controls button { background: rgba(255, 255, 255, 0.05); border: 1px solid rgba(255, 255, 255, 0.1); color: #fff; width: 32px; height: 32px; border-radius: 6px; cursor: pointer; }
        #current-month-year { font-family: 'Orbitron', sans-serif; font-size: 1.1rem; min-width: 140px; text-align: center; }
        .calendar-status-legend { display: flex; gap: 15px; font-size: 0.75rem; }
        .legend-tag { display: flex; align-items: center; gap: 6px; }
        .legend-tag .dot { width: 8px; height: 8px; border-radius: 50%; }
        .legend-tag .dot.status-show { background: var(--accent-green); }
        .legend-tag .dot.status-busy { background: var(--secondary-neon); }
        .calendar-weekdays-row { display: grid; grid-template-columns: repeat(7, 1fr); text-align: center; margin-bottom: 10px; font-size: 0.75rem; font-weight: 700; color: var(--text-muted); }
        .calendar-days-grid { display: grid; grid-template-columns: repeat(7, 1fr); gap: 8px; }
        .calendar-day-cell { aspect-ratio: 1; border: 1px solid rgba(255, 255, 255, 0.03); border-radius: 8px; display: flex; padding: 8px; font-size: 0.85rem; font-family: 'Orbitron', sans-serif; color: rgba(255, 255, 255, 0.2); position: relative; }
        .calendar-day-cell.other-month { opacity: 0.15; pointer-events: none; }
        .calendar-day-cell.has-show { background: linear-gradient(135deg, rgba(0, 255, 102, 0.08) 0%, rgba(0, 0, 0, 0.3) 100%); border-color: rgba(0, 255, 102, 0.3); color: #fff; cursor: pointer; }
        .calendar-day-cell.has-show::after { content: "SHOW"; position: absolute; bottom: 4px; right: 4px; font-size: 0.5rem; color: var(--accent-green); font-weight: 900; }
        .calendar-day-cell.is-busy { background: linear-gradient(135deg, rgba(255, 0, 127, 0.08) 0%, rgba(0, 0, 0, 0.3) 100%); border-color: rgba(255, 0, 127, 0.2); color: #fff; }
        .calendar-day-cell.is-busy::after { content: "BẬN"; position: absolute; bottom: 4px; right: 4px; font-size: 0.5rem; color: var(--secondary-neon); font-weight: 900; }
        .calendar-day-cell.active-show { border-color: var(--primary-neon) !important; box-shadow: 0 0 12px rgba(0, 240, 255, 0.3); }
        .schedule-location-box { margin-top: 18px; background: rgba(0, 255, 102, 0.04); border: 1px solid rgba(0, 255, 102, 0.15); padding: 14px 18px; border-radius: 10px; display: none; align-items: center; gap: 12px; }

        /* --- COMMITMENT STYLES --- */
        .commit-wrapper-list { display: flex; flex-direction: column; gap: 26px; }
        .commit-row-item { display: flex; gap: 20px; align-items: flex-start; }
        .commit-badge-icon { background: rgba(255, 0, 127, 0.08); border: 1px solid rgba(255, 0, 127, 0.3); color: var(--secondary-neon); width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; border-radius: 10px; flex-shrink: 0; font-size: 1.1rem; }
        .commit-content h4 { color: #fff; font-size: 1.1rem; font-weight: 700; margin-bottom: 6px; }
        .commit-content p { font-size: 0.92rem; color: var(--text-muted); line-height: 1.6; }

        /* --- PRICING SECTION --- */
        .pricing-tier-grid { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; margin-top: 25px; margin-bottom: 30px; }
        .price-column-card { background: rgba(0, 0, 0, 0.3); border: 1px solid rgba(255, 255, 255, 0.04); border-radius: 14px; padding: 24px 16px; text-align: center; position: relative; }
        .price-column-card.featured-combo { border: 1px solid rgba(255, 102, 0, 0.4); background: linear-gradient(180deg, rgba(255, 102, 0, 0.05) 0%, rgba(0, 0, 0, 0.4) 100%); }
        .popular-badge { position: absolute; top: -12px; left: 50%; transform: translateX(-50%); background: linear-gradient(90deg, #ff3300, #ff6600); color: #fff; font-family: 'Orbitron', sans-serif; font-size: 0.65rem; font-weight: 900; padding: 4px 14px; border-radius: 6px; letter-spacing: 1px; box-shadow: 0 4px 10px rgba(255,102,0,0.3); }
        .tier-header h3 { font-family: 'Orbitron', sans-serif; font-size: 1.1rem; color: #fff; margin-bottom: 5px; }
        .price-column-card.featured-combo .tier-header h3 { color: var(--accent-orange); }
        .tier-header .tier-subtitle { font-size: 0.75rem; color: var(--text-muted); margin-bottom: 20px; display: block; }
        .tier-price-box .old-num { text-decoration: line-through; color: rgba(255,255,255,0.25); font-size: 0.88rem; display: block; margin-bottom: 2px; }
        .tier-price-box .current-num { font-family: 'Orbitron', sans-serif; font-size: 1.6rem; font-weight: 900; color: #fff; }
        .price-column-card.featured-combo .current-num { color: var(--accent-orange); }
        .tier-price-box .unit-tag { font-size: 0.75rem; color: var(--text-muted); display: block; margin-top: 2px; margin-bottom: 15px; }
        .tier-features { list-style: none; padding: 0; text-align: left; border-top: 1px solid rgba(255, 255, 255, 0.05); padding-top: 15px; }
        .tier-features li { font-size: 0.82rem; color: var(--text-muted); margin-bottom: 10px; display: flex; gap: 8px; align-items: flex-start; }
        .tier-features li i { color: var(--primary-neon); font-size: 0.85rem; margin-top: 3px; }
        .price-column-card.featured-combo .tier-features li i { color: var(--accent-orange); }

        /* --- CREW DUO DESCRIPTION --- */
        .duo-crew-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 24px; margin-top: 15px; padding-top: 10px; }
        .crew-card-item { background: rgba(0, 0, 0, 0.15); padding: 22px; border-radius: 12px; border: 1px solid rgba(255, 255, 255, 0.03); }
        .crew-card-item h4 { font-family: 'Orbitron', sans-serif; font-size: 0.95rem; font-weight: 800; color: #fff; margin-bottom: 10px; display: flex; align-items: center; gap: 10px; letter-spacing: 1px; }
        .crew-card-item h4 i { font-size: 0.9rem; }
        .crew-card-item.c-dj h4 i { color: var(--primary-neon); }
        .crew-card-item.c-mc h4 i { color: #00f0ff; }
        .crew-card-item p { font-size: 0.86rem; color: var(--text-muted); line-height: 1.6; text-align: justify; }

        /* --- CONTACT CHANNELS --- */
        .booking-channels { display: grid; grid-template-columns: repeat(3, 1fr); gap: 15px; margin-bottom: 25px; }
        .channel-btn { display: flex; flex-direction: column; align-items: center; justify-content: center; gap: 12px; background: rgba(255, 255, 255, 0.02); padding: 22px 15px; border-radius: 12px; border: 1px solid rgba(255, 255, 255, 0.04); text-decoration: none; color: var(--text-main); transition: all 0.3s ease; text-align: center; }
        .channel-btn span { font-size: 0.72rem; color: var(--text-muted); text-transform: uppercase; letter-spacing: 1px; display: block; margin-bottom: 2px; }
        .channel-btn p { font-family: 'Orbitron', sans-serif; font-weight: 700; font-size: 1rem; }
        .channel-btn.c-phone p { font-family: 'Inter', sans-serif; }
        .channel-btn.c-zalo p { font-family: 'Inter', sans-serif; }
        .channel-btn.c-phone:hover { border-color: var(--accent-green); color: var(--accent-green); box-shadow: 0 0 12px rgba(0,255,102,0.15); }
        .channel-btn.c-zalo:hover { border-color: #0084ff; color: #0084ff; box-shadow: 0 0 12px rgba(0,132,255,0.15); }
        .channel-btn.c-fb:hover { border-color: #1877f2; color: #1877f2; box-shadow: 0 0 12px rgba(24,119,242,0.15); }
        .location-footer-box { background: rgba(0, 240, 255, 0.03); border: 1px solid rgba(0, 240, 255, 0.08); padding: 16px; border-radius: 10px; text-align: center; font-size: 0.9rem; }

        /* --- RESPONSIVE MEDIA QUERIES --- */
        @media (max-width: 900px) {
            .welcome-inner-layout { grid-template-columns: 1fr; gap: 30px; text-align: center; }
            .welcome-text-side { align-items: center; order: 2; }
            .welcome-visual-side { order: 1; }
            .welcome-title { font-size: 3rem; }
        }
        @media (max-width: 720px) {
            .pricing-tier-grid { grid-template-columns: 1fr; gap: 24px; }
            .media-showcase-grid { grid-template-columns: 1fr; gap: 16px; }
            .tab-navigation-bar { display: grid; grid-template-columns: 1fr 1fr 1fr; border-radius: 14px; gap: 6px; }
            .tab-btn { font-size: 0.8rem; padding: 10px 5px; }
            .duo-crew-grid { grid-template-columns: 1fr; gap: 16px; }
        }
        @media (max-width: 650px) {
            .card { padding: 25px 20px; }
            .profile-layout { grid-template-columns: 1fr; text-align: center; }
            .booking-channels { grid-template-columns: 1fr; }
            .channel-btn { flex-direction: row; justify-content: flex-start; padding: 15px 20px; gap: 20px; text-align: left; }
            .brand-title { font-size: 2.1rem; }
        }
        footer { text-align: center; font-size: 0.75rem; color: rgba(255, 255, 255, 0.15); margin-top: 60px; letter-spacing: 3px; font-family: 'Orbitron', sans-serif; }
    </style>
</head>
<body class="lock-scroll">

    <!-- CYBER SPLASH WELCOME SCREEN -->
    <div id="welcome-screen" onclick="enterWebsite()">
        <div class="welcome-bg-overlay"></div>
        <div class="welcome-inner-layout">
            <div class="welcome-text-side">
                <div class="welcome-badge-tag">Verified Artist</div>
                <h1 class="welcome-title">DJ <span>TUZEN</span></h1>
                <div class="welcome-subtitle">The Sound of Nightlife</div>
                <p class="welcome-desc">Chào mừng bạn đến với không gian âm nhạc điện tử đỉnh cao. Cuộn chuột hoặc chạm màn hình để khám phá profile & lịch biểu diễn.</p>
            </div>
            <div class="welcome-visual-side">
                <div class="logo-frame-container">
                    <div class="radar-glow-ring"></div>
                    <img id="welcome-logo-img" src="https://images.unsplash.com/photo-1516873240891-4bf014598ab4?w=400" alt="DJ TUZEN" class="welcome-logo">
                </div>
            </div>
        </div>
    </div>

    <!-- BACKGROUND GRID LAYOUT -->
    <div class="led-bg-grid">
        <div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div>
        <div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div>
        <div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div>
        <div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div><div class="led-dot"></div>
    </div>

    <div class="container">
        <header>
            <h1 class="brand-title">DJ TUZEN</h1>
            <div class="brand-subtitle">Booking Information</div>
        </header>

        <!-- MAIN NAVIGATION CONTAINER CARD -->
        <div class="card">
            <h2 class="section-title"><i class="fa-solid fa-circle-user"></i> Profile Artist</h2>
            
            <div class="tab-navigation-bar">
                <button class="tab-btn active" onclick="switchProfileTab(event, 'tab-bio')"><i class="fa-solid fa-id-card"></i> Tiểu sử</button>
                <button class="tab-btn" onclick="switchProfileTab(event, 'tab-media')"><i class="fa-solid fa-photo-film"></i> Media Video</button>
                <button class="tab-btn" onclick="switchProfileTab(event, 'tab-schedule')"><i class="fa-solid fa-calendar-days"></i> Lịch Trình</button>
            </div>

            <!-- TAB 1: BIOGRAPHY -->
            <div id="tab-bio" class="tab-content-panel active">
                <div class="profile-layout">
                    <div>
                        <img id="artist-avatar" src="https://images.unsplash.com/photo-1516873240891-4bf014598ab4?w=500" alt="DJ TUZEN" class="responsive-img" style="margin-bottom:0;">
                    </div>
                    <div class="profile-info">
                        <p class="profile-bio">
                            DJ TUZEN là nghệ sĩ âm nhạc cá tính với tư duy mix-set hiện đại, nhạy bén trong việc nắm bắt tâm lý đám đông. Anh luôn biết cách biến hóa playlist linh hoạt từ giai điệu tinh tế lúc đón khách đến các set nhạc bùng nổ năng lượng, mang lại không khí After-Party đẳng cấp và khác biệt.
                        </p>
                        <div class="profile-stats-grid">
                            <div class="stat-item">
                                <div class="stat-icon-wrapper"><i class="fa-solid fa-hourglass-half"></i></div>
                                <div class="stat-details">
                                    <span>Kinh nghiệm diễn</span>
                                    <p>4 Năm Chuyên Nghiệp</p>
                                </div>
                            </div>
                            <div class="stat-item">
                                <div class="stat-icon-wrapper"><i class="fa-solid fa-sliders"></i></div>
                                <div class="stat-details">
                                    <span>Dòng nhạc sở trường</span>
                                    <p>Vinahouse, Houselak, Techno, Psytrance...</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- TAB 2: LIVE PERFORMANCE MEDIA -->
            <div id="tab-media" class="tab-content-panel">
                <div class="media-showcase-grid">
                    <div class="video-wrapper-box">
                        <!-- THAY ĐỔI: Sử dụng iframe hỗ trợ Youtube Embed mượt mà -->
                        <iframe id="video-player-1" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        <div class="video-caption-info">
                            <h4 id="video-title-1">Set Nhạc Bùng Nổ Sân Khấu</h4>
                            <p><i class="fa-regular fa-clock"></i> Live Mix</p>
                        </div>
                    </div>
                    <div class="video-wrapper-box">
                        <!-- THAY ĐỔI: Sử dụng iframe hỗ trợ Youtube Embed mượt mà -->
                        <iframe id="video-player-2" src="" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        <div class="video-caption-info">
                            <h4 id="video-title-2">After-Party Đám Cưới Trẻ Trung</h4>
                            <p><i class="fa-regular fa-clock"></i> Event Mix</p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- TAB 3: AUTOMATIC TIMELINE SCHEDULE -->
            <div id="tab-schedule" class="tab-content-panel">
                <div class="calendar-dashboard">
                    <div class="calendar-header-title">
                        <div class="calendar-controls">
                            <button onclick="changeMonth(-1)"><i class="fa-solid fa-angle-left"></i></button>
                            <span id="current-month-year">Tháng 07 / 2026</span>
                            <button onclick="changeMonth(1)"><i class="fa-solid fa-angle-right"></i></button>
                        </div>
                        <div class="calendar-status-legend">
                            <div class="legend-tag"><span class="dot status-show"></span> Có Show</div>
                            <div class="legend-tag"><span class="dot status-busy"></span> Bận</div>
                        </div>
                    </div>
                    <div class="calendar-weekdays-row">
                        <span>T2</span><span>T3</span><span>T4</span><span>T5</span><span>T6</span><span>T7</span><span>CN</span>
                    </div>
                    <div class="calendar-days-grid" id="calendar-days-container"></div>
                </div>
                <div class="schedule-location-box" id="location-details-box">
                    <i class="fa-solid fa-location-crosshairs"></i>
                    <p id="location-text-content">Chọn ngày có show để xem địa điểm diễn.</p>
                </div>
            </div>
        </div>

        <!-- PRICING TIERS DASHBOARD -->
        <div class="card">
            <h2 class="section-title"><i class="fa-solid fa-receipt"></i> Dịch Vụ & Báo Giá</h2>
            
            <div class="pricing-tier-grid">
                <!-- Gói DJ Lẻ -->
                <div class="price-column-card">
                    <div class="tier-header">
                        <h3>Gói DJ Lẻ</h3>
                        <span class="tier-subtitle">Set diễn cá nhân bùng nổ</span>
                    </div>
                    <div class="tier-price-box">
                        <span class="old-num" id="dj-old">3.000.000đ</span>
                        <span class="current-num" id="dj-current">2.500.000</span>
                        <span class="unit-tag">VND / Show</span>
                    </div>
                    <ul class="tier-features">
                        <li><i class="fa-solid fa-check"></i> DJ TUZEN biểu diễn trực tiếp</li>
                        <li><i class="fa-solid fa-check"></i> Thời gian: 90 - 120 phút</li>
                        <li><i class="fa-solid fa-check"></i> Mixset nhạc thiết kế riêng</li>
                    </ul>
                </div>
                
                <!-- Gói MC Lẻ -->
                <div class="price-column-card">
                    <div class="tier-header">
                        <h3>Gói MC Lẻ</h3>
                        <span class="tier-subtitle">Khuấy động giữ nhiệt tiệc</span>
                    </div>
                    <div class="tier-price-box">
                        <span class="old-num" id="mc-old">1.500.000đ</span>
                        <span class="current-num" id="mc-current">1.000.000</span>
                        <span class="unit-tag">VND / Show</span>
                    </div>
                    <ul class="tier-features">
                        <li><i class="fa-solid fa-check"></i> MC Hype chuyên nghiệp</li>
                        <li><i class="fa-solid fa-check"></i> Tương tác khán giả liên tục</li>
                        <li><i class="fa-solid fa-check"></i> Dẫn dắt mini-game (nếu có)</li>
                    </ul>
                </div>
                
                <!-- Gói Combo -->
                <div class="price-column-card featured-combo">
                    <div class="popular-badge">POPULAR</div>
                    <div class="tier-header">
                        <h3>Gói Combo</h3>
                        <span class="tier-subtitle">Sự lựa chọn tối ưu nhất</span>
                    </div>
                    <div class="tier-price-box">
                        <span class="old-num" id="combo-old">3.500.000đ</span>
                        <span class="current-num" id="combo-current">2.600.000</span>
                        <span class="unit-tag">VND / Combo</span>
                    </div>
                    <ul class="tier-features">
                        <li><i class="fa-solid fa-check"></i> Đủ cặp đôi DJ TUZEN & MC HYPE</li>
                        <li><i class="fa-solid fa-check"></i> Phối hợp ăn ý giữ lửa 100%</li>
                        <li><i class="fa-solid fa-check"></i> Tiết kiệm ngay 200.000đ</li>
                    </ul>
                </div>
            </div>

            <!-- ĐOẠN MÔ TẢ NHÂN SỰ CHÍNH XÁC NHƯ TRONG ẢNH -->
            <div class="duo-crew-grid">
                <div class="crew-card-item c-dj">
                    <h4><i class="fa-solid fa-compact-disc"></i> DJ TUZEN</h4>
                    <p>Thiết kế màu sắc âm nhạc độc bản cho từng sự kiện, điều phối mạch cảm xúc qua từng giai điệu từ nhẹ nhàng đến bùng nổ cực đỉnh.</p>
                </div>
                <div class="crew-card-item c-mc">
                    <h4><i class="fa-solid fa-microphone-lines"></i> MC HYPE</h4>
                    <p>Bắt nhịp đám đông, giữ nhiệt sân khấu liên tục, tương tác hoàn hảo với DJ giúp khách mời cháy hết mình.</p>
                </div>
            </div>
        </div>

        <!-- KHỐI CAM KẾT CHẤT LƯỢNG SHOW -->
        <div class="card card-commit">
            <h2 class="section-title"><i class="fa-solid fa-shield-halved"></i> CAM KẾT CHẤT LƯỢNG SHOW</h2>
            <div class="commit-wrapper-list">
                <div class="commit-row-item">
                    <div class="commit-badge-icon"><i class="fa-regular fa-clock"></i></div>
                    <div class="commit-content">
                        <h4>Tuyệt đối đúng giờ</h4>
                        <p>Đội ngũ luôn có mặt trước giờ diễn tối thiểu 45 phút để kiểm tra kỹ thuật hệ thống âm thanh (Soundcheck) và rà soát kịch bản cùng Ban tổ chức.</p>
                    </div>
                </div>
                <div class="commit-row-item">
                    <div class="commit-badge-icon"><i class="fa-regular fa-user"></i></div>
                    <div class="commit-content">
                        <h4>Phong cách biểu diễn cá tính & Nghiêm túc</h4>
                        <p>Trang phục hiện đại, năng động (streetwear) phù hợp tinh thần tiệc cưới trẻ trung. Cam kết không sử dụng các chất kích thích trước và trong suốt show diễn.</p>
                    </div>
                </div>
                <div class="commit-row-item">
                    <div class="commit-badge-icon"><i class="fa-solid fa-server"></i></div>
                    <div class="commit-content">
                        <h4>An toàn kỹ thuật tuyệt đối</h4>
                        <p>Luôn trang bị sẵn 02 USB lưu trữ độc lập đã được xử lý nhạc chuyên nghiệp cùng thiết bị backup, đảm bảo âm nhạc mượt mà không lo gián đoạn kỹ thuật.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- FAST BOOKING CONTACT SYSTEM -->
        <div class="card">
            <h2 class="section-title"><i class="fa-regular fa-paper-plane"></i> ĐẶT LỊCH BIỂU DIỄN</h2>
            <div class="booking-channels">
                <a href="tel:0969113083" class="channel-btn c-phone">
                    <span>HOTLINE ĐẶT SHOW</span>
                    <p>0969.113.083</p>
                </a>
                <a href="https://zalo.me/0969113083" target="_blank" class="channel-btn c-zalo">
                    <span>ZALO TƯ VẤN</span>
                    <p>0969.113.083</p>
                </a>
                <a href="https://www.facebook.com/" target="_blank" class="channel-btn c-fb">
                    <span>FACEBOOK PROFILE</span>
                    <p>DJ TUZEN</p>
                </a>
            </div>
            <div class="location-footer-box">
                <i class="fa-solid fa-location-dot"></i> Hoạt động chính tại <strong>Phú Thọ, Hòa Bình</strong> và toàn quốc.
            </div>
        </div>

        <footer>© 2026 DJ TUZEN • THIẾT KẾ BỞI AI COLLABORATOR</footer>
    </div>

    <!-- MAIN INTERACTIVE ENGINE JAVASCRIPT -->
    <script>
        // 🛑 ĐIỀN ID BẢNG TÍNH GOOGLE SHEETS CỦA BẠN VÀO ĐÂY
        const SHEET_ID = '1kVuDlf-Yqcvoba5jhyQ_AHRGhPZcQyYzvTEMWm86dKM'; 
        
        let scheduleDatabase = {};
        let calendarDate = new Date(); 

        // Hàm tiện ích phân tách lấy ID Video YouTube và tạo link Embed chuẩn
        function getYoutubeEmbedUrl(url) {
            if (!url) return '';
            let videoId = '';
            if (url.includes('youtu.be/')) {
                videoId = url.split('youtu.be/')[1].split(/[?#]/)[0];
            } else if (url.includes('youtube.com/watch')) {
                const urlParams = new URLSearchParams(new URL(url).search);
                videoId = urlParams.get('v');
            } else if (url.includes('youtube.com/embed/')) {
                return url;
            }
            return videoId ? `https://www.youtube.com/embed/${videoId}` : '';
        }

        async function fetchSheetsData() {
            try {
                // 1. Đồng bộ Tab Profile (Đã sửa lỗi gọi biến cứng chuỗi ID cũ gây crash)
                const resProfile = await fetch(`https://docs.google.com/spreadsheets/d/${SHEET_ID}/gviz/tq?tqx=out:json&sheet=Profile`);
                const textProfile = await resProfile.text();
                const dataProfile = JSON.parse(textProfile.substr(47).slice(0, -2));
                
                dataProfile.table.rows.forEach(row => {
                    const key = row.c[0]?.v;
                    const val = row.c[1]?.v;
                    if(key === 'avatar_url' && val) {
                        document.getElementById('artist-avatar').src = val;
                        document.getElementById('welcome-logo-img').src = val;
                    }
                    // THAY ĐỔI: Sử dụng bộ bóc tách link Embed cho iframe
                    if(key === 'video_1_url' && val) document.getElementById('video-player-1').src = getYoutubeEmbedUrl(val);
                    if(key === 'video_2_url' && val) document.getElementById('video-player-2').src = getYoutubeEmbedUrl(val);
                    if(key === 'video_title_1' && val) document.getElementById('video-title-1').innerText = val;
                    if(key === 'video_title_2' && val) document.getElementById('video-title-2').innerText = val;
                });

                // 2. Đồng bộ Tab Schedule
                const resSchedule = await fetch(`https://docs.google.com/spreadsheets/d/${SHEET_ID}/gviz/tq?tqx=out:json&sheet=Schedule`);
                const textSchedule = await resSchedule.text();
                const dataSchedule = JSON.parse(textSchedule.substr(47).slice(0, -2));
                
                dataSchedule.table.rows.forEach(row => {
                    const rawDate = row.c[0]?.v; 
                    const type = row.c[1]?.v;     
                    const loc = row.c[2]?.v || ''; 
                    if (rawDate) {
                        scheduleDatabase[rawDate] = { type: type, location: loc };
                    }
                });

                // 3. Đồng bộ Tab Pricing
                const resPricing = await fetch(`https://docs.google.com/spreadsheets/d/${SHEET_ID}/gviz/tq?tqx=out:json&sheet=Pricing`);
                const textPricing = await resPricing.text();
                const dataPricing = JSON.parse(textPricing.substr(47).slice(0, -2));
                
                dataPricing.table.rows.forEach(row => {
                    const tier = row.c[0]?.v;
                    const oldPrice = row.c[1]?.v;
                    const curPrice = row.c[2]?.v;
                    if(tier === 'Gói DJ Lẻ') {
                        document.getElementById('dj-old').innerText = oldPrice;
                        document.getElementById('dj-current').innerText = curPrice;
                    } else if(tier === 'Gói MC Lẻ') {
                        document.getElementById('mc-old').innerText = oldPrice;
                        document.getElementById('mc-current').innerText = curPrice;
                    } else if(tier === 'Gói Combo') {
                        document.getElementById('combo-old').innerText = oldPrice;
                        document.getElementById('combo-current').innerText = curPrice;
                    }
                });

                renderCalendar();
            } catch (error) {
                console.error("Lỗi cấu trúc hoặc sai ID Google Sheets:", error);
            }
        }

        function enterWebsite() {
            document.getElementById('welcome-screen').classList.add('fade-out');
            document.body.classList.remove('lock-scroll');
        }

        window.addEventListener('wheel', function(e) {
            if (e.deltaY > 0 && !document.getElementById('welcome-screen').classList.contains('fade-out')) { enterWebsite(); }
        });

        function switchProfileTab(event, tabId) {
            document.querySelectorAll('.tab-content-panel').forEach(panel => panel.classList.remove('active'));
            document.querySelectorAll('.tab-btn').forEach(tab => tab.classList.remove('active'));
            document.getElementById(tabId).classList.add('active');
            event.currentTarget.classList.add('active');
            if (tabId === 'tab-schedule') { renderCalendar(); }
        }

        function renderCalendar() {
            const container = document.getElementById('calendar-days-container');
            const monthYearLabel = document.getElementById('current-month-year');
            const locationBox = document.getElementById('location-details-box');
            
            locationBox.style.display = "none";
            container.innerHTML = "";

            const year = calendarDate.getFullYear();
            const month = calendarDate.getMonth();
            monthYearLabel.innerText = `Tháng ${String(month + 1).padStart(2, '0')} / ${year}`;

            let firstDayIndex = new Date(year, month, 1).getDay();
            firstDayIndex = firstDayIndex === 0 ? 6 : firstDayIndex - 1;

            const totalDaysCurrent = new Date(year, month + 1, 0).getDate();
            const totalDaysPrev = new Date(year, month, 0).getDate();

            for (let i = firstDayIndex - 1; i >= 0; i--) {
                const cell = document.createElement('div');
                cell.className = 'calendar-day-cell other-month';
                cell.innerText = totalDaysPrev - i;
                container.appendChild(cell);
            }

            for (let day = 1; day <= totalDaysCurrent; day++) {
                const cell = document.createElement('div');
                cell.className = 'calendar-day-cell';
                cell.innerText = day;

                const dateKey = `${year}-${String(month + 1).padStart(2, '0')}-${String(day).padStart(2, '0')}`;
                
                if (scheduleDatabase[dateKey]) {
                    const data = scheduleDatabase[dateKey];
                    if (data.type === 'show') {
                        cell.classList.add('has-show');
                        cell.addEventListener('click', function() {
                            document.querySelectorAll('.calendar-day-cell').forEach(c => c.classList.remove('active-show'));
                            cell.classList.add('active-show');
                            document.getElementById('location-text-content').innerHTML = `Ngày ${day}/${month+1}: Show diễn tại <strong>${data.location}</strong>`;
                            locationBox.style.display = "flex";
                        });
                    } else if (data.type === 'busy') {
                        cell.classList.add('is-busy');
                    }
                }
                container.appendChild(cell);
            }

            const totalCellsRendered = firstDayIndex + totalDaysCurrent;
            const remainingCells = totalCellsRendered % 7 === 0 ? 0 : 7 - (totalCellsRendered % 7);
            for (let day = 1; day <= remainingCells; day++) {
                const cell = document.createElement('div');
                cell.className = 'calendar-day-cell other-month';
                cell.innerText = day;
                container.appendChild(cell);
            }
        }

        function changeMonth(direction) {
            calendarDate.setMonth(calendarDate.getMonth() + direction);
            renderCalendar();
        }

        document.addEventListener("DOMContentLoaded", fetchSheetsData);
    </script>
</body>
</html>
