

# sake-2026[index.html](https://github.com/user-attachments/files/26736956/index.html)[script.js](https://github.com/user-attachments/files/26736957/script.js)[style.css](https://github.com/user-attachments/files/26736958/style.css)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>十家酒造 · 清酒品鉴会 | 2026年5月1日</title>
    <!-- 引入高级感字体 -->
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+JP:wght@400;700&family=Noto+Sans+JP:wght@300;400&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- 导航栏 -->
    <nav>
        <div class="logo">SAKE EXPERIENCE</div>
        <div class="nav-links">
            <a href="#about">活动介绍</a>
            <a href="#breweries">参与酒造</a>
            <a href="#info">活动信息</a>
            <button class="nav-btn" onclick="openBooking()">立即预约</button>
        </div>
    </nav>

    <!-- 首页大图 (Hero Section) -->
    <section class="hero">
        <div class="hero-content">
            <h1 class="reveal">十家酒造 · 清酒品鉴会</h1>
            <p class="reveal delay-1">2026年5月1日 · 匠心传承的限定体验</p>
            <button class="main-btn reveal delay-2" onclick="openBooking()">立即预约</button>
        </div>
    </section>

    <!-- 活动介绍 -->
    <section id="about" class="about">
        <div class="container">
            <h2 class="reveal">清酒之魂，品味时光</h2>
            <p class="reveal">这是一场专为清酒爱好者准备的极度奢华之旅。我们邀请了日本著名的十家酒造，带来他们的代表作与限定款。在这里，不仅是品鉴，更是与酿酒大师面对面的专业交流。</p>
            <div class="features reveal">
                <span>● 限定50名额</span>
                <span>● 唎酒师专业讲解</span>
                <span>● 稀有款限定品尝</span>
            </div>
        </div>
    </section>

    <!-- 酒造展示 -->
    <section id="breweries" class="breweries">
        <div class="container">
            <h2 class="reveal">参与酒造</h2>
            <div class="brewery-grid">
                <div class="brewery-card reveal">
                    <div class="card-image" style="background-image: url('https://images.unsplash.com/photo-1571210862729-78a52d3779a2?auto=format&fit=crop&q=80&w=800')"></div>
                    <h3>酒造 01 · 吟咏之心</h3>
                    <p>来自新潟县的百年老店，以极净的水质酿造出品质卓越的纯米大吟酿。</p>
                </div>
                <div class="brewery-card reveal">
                    <div class="card-image" style="background-image: url('https://images.unsplash.com/photo-1606501120239-1606ec82830b?auto=format&fit=crop&q=80&w=800')"></div>
                    <h3>酒造 02 · 岚山风味</h3>
                    <p>坚持古法酿造，每一滴都蕴含着京都岚山的自然灵气。</p>
                </div>
                <!-- 更多酒造占位 -->
                <div class="brewery-card reveal"><h3>酒造 03</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 04</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 05</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 06</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 07</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 08</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 09</h3><p>详细介绍稍后补充...</p></div>
                <div class="brewery-card reveal"><h3>酒造 10</h3><p>详细介绍稍后补充...</p></div>
            </div>
        </div>
    </section>

    <!-- 活动信息 -->
    <section id="info" class="info">
        <div class="container reveal">
            <h2>活动信息</h2>
            <div class="info-details">
                <div class="info-item">
                    <strong>时间</strong>
                    <p>2026年5月1日 | 14:00 - 20:00</p>
                </div>
                <div class="info-item">
                    <strong>地点</strong>
                    <p>日本东京都港区 · 隐秘清酒吧</p>
                </div>
                <div class="info-item">
                    <strong>名额</strong>
                    <p>仅限 VIP 邀请函持有者</p>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <p>&copy; 2026 SAKE EXPERIENCE. All Rights Reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>

function reveal() {
    var reveals = document.querySelectorAll(".reveal");
    for (var i = 0; i < reveals.length; i++) {
        var windowHeight = window.innerHeight;
        var elementTop = reveals[i].getBoundingClientRect().top;
        if (elementTop < windowHeight - 150) {
            reveals[i].classList.add("active");
        }
    }
}
window.addEventListener("scroll", reveal);
window.onload = reveal;

function openBooking() {
    alert("感谢您的关注！\n请添加客服微信：SakeExperience_2026\n我们将为您发送正式邀请函。");
}

* { margin: 0; padding: 0; box-sizing: border-box; }
body { font-family: 'Noto Sans JP', sans-serif; color: #1a1a1a; background-color: #fcfcfc; overflow-x: hidden; }
h1, h2, h3 { font-family: 'Noto Serif JP', serif; }
.container { max-width: 1100px; margin: 0 auto; padding: 0 20px; }
nav { position: fixed; top: 0; width: 100%; display: flex; justify-content: space-between; align-items: center; padding: 20px 50px; background: rgba(255, 255, 255, 0.9); backdrop-filter: blur(10px); z-index: 1000; border-bottom: 1px solid #eee; }
.nav-btn { padding: 8px 20px; background: #1a1a1a; color: white; border: none; cursor: pointer; border-radius: 20px; }
.hero { height: 100vh; background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('https://images.unsplash.com/photo-1528360983277-13d401cdc186?auto=format&fit=crop&q=80&w=2000'); background-size: cover; background-position: center; display: flex; align-items: center; justify-content: center; text-align: center; color: white; }
.hero h1 { font-size: 3.5rem; letter-spacing: 5px; }
.main-btn { padding: 15px 40px; background: transparent; color: white; border: 1px solid white; cursor: pointer; transition: 0.4s; }
.main-btn:hover { background: white; color: #1a1a1a; }
section { padding: 100px 0; }
.brewery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 30px; }
.brewery-card { background: #fff; padding: 20px; border: 1px solid #eee; transition: 0.5s; }
.card-image { height: 200px; background-color: #f0f0f0; margin-bottom: 20px; background-size: cover; }
.reveal { opacity: 0; transform: translateY(30px); transition: all 0.8s ease-out; }
.reveal.active { opacity: 1; transform: translateY(0); }
