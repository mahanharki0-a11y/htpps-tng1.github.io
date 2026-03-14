# htpps-tng1.github.io
htpps-tng.github.io
<!DOCTYPE html>
<html lang="ku" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TNG | وێبسایتی فەرمی</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
</head>
<body>

    <nav>
        <div class="logo">TNG<span> THE NIGHT</span></div>
        <ul class="nav-links">
            <li><a href="#rules">یاساکان</a></li>
            <li><a href="#staff">ستاف</a></li>
            <li><a href="#gallery">گەلەری</a></li>
        </ul>
        <a href="https://discord.gg/B4XHZPhg" class="join-btn"><i class="fab fa-discord"></i> Discord</a>
    </nav>

    <header>
        <div class="hero">
            <h1>TNG <span class="blue-text"> THE NIGHT</span></h1>
            <p>بەهێزترین سێرڤەری کوردی لە دیسکۆرد</p>
        </div>
    </header>

    <section id="rules" class="container blue-bg">
        <h2 class="section-title">یاساکانی سێرڤەر</h2>
        <div class="rules-grid">
            <div class="rule-box">١. ڕێزگرتن لە هەمووان مەرجە.</div>
            <div class="rule-box">٢. ناردنی هەر جۆرە لینکێک قەدەغەیە.</div>
            <div class="rule-box">٣. بێزارکردنی ئەندامان قەدەغەیە.</div>
        </div>
    </section>

    <section id="staff" class="container">
        <h2 class="section-title">ستافی سێرڤەر</h2>
        <div class="staff-grid">
            <div class="staff-card owner-card">
                <img src="file:///C:/Users/Ali%20Harki/Downloads/f/b1ee6219-f92b-42c3-b71e-265964fb2573.png" alt="Owner">
                <h3>Xala Sya</h3>
                <span>Owner Ship</span>
            </div>
    </section>

    <section id="gallery" class="container blue-bg">
        <h2 class="section-title">گەلەری وێنەکان</h2>
        <div class="gallery-grid">
            <div class="gallery-item"><img src="file:///C:/Users/Ali%20Harki/Downloads/f/Cfx.re_C_Users_dssto_AppData_Local_FiveM_FiveM.exe_Screenshot_2026.03.13_-_00.25.53.94.png" alt="Img 1"></div>
        </div>
    </section>

    <footer>
        <p>Copyright © 2026 - TNG Team</p>
    </footer>

</body>
</html>

<div class="audio-player">
    <button id="music-btn"><i class="fas fa-play"></i> لێدان</button>
    <audio id="https://www.youtube.com/watch?v=8VLXHyHRXjc" loop>
        <source src="your-music-file.mp3" type="audio/mpeg">
        وێبگەڕەکەت پشتگیری دەنگ ناکات.
    </audio>
</div>

<script>
    const music = document.getElementById("https://www.youtube.com/watch?v=8VLXHyHRXjc");
    const btn = document.getElementById("music-btn");

    btn.onclick = function() {
        if (music.paused) {
            music.play();
            btn.innerHTML = '<i class="fas fa-pause"></i> وەستان';
            btn.classList.add("playing");
        } else {
            music.pause();
            btn.innerHTML = '<i class="fas fa-play"></i> لێدان';
            btn.classList.remove("playing");
        }
    };
</script>






:root {
    --main-blue: #007bff;
    --dark-blue: #001f3f;
    --neon-blue: #00d2ff;
    --bg-dark: #050505;
}

* { margin: 0; padding: 0; box-sizing: border-box; font-family: sans-serif; }
body { background-color: var(--bg-dark); color: white; line-height: 1.6; }

/* Navbar */
nav {
    display: flex; justify-content: space-between; align-items: center;
    padding: 20px 8%; background: rgba(0,0,0,0.9);
    position: fixed; width: 100%; top: 0; z-index: 1000;
}
.logo span { color: var(--neon-blue); }
.nav-links { display: flex; list-style: none; }
.nav-links li { margin: 0 15px; }
.nav-links a { color: white; text-decoration: none; transition: 0.3s; }
.nav-links a:hover { color: var(--neon-blue); }

.join-btn {
    background: #5865F2; color: white; padding: 8px 20px;
    border-radius: 5px; text-decoration: none; font-weight: bold;
}

/* Hero Section */
.hero {
    height: 70vh; display: flex; flex-direction: column;
    justify-content: center; align-items: center;
    background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://via.placeholder.com/1920x1080');
    background-size: cover; text-align: center;
}
.blue-text { color: var(--neon-blue); text-shadow: 0 0 10px var(--neon-blue); }

/* پاشبنەمای شین بۆ بەشەکان */
.container { padding: 80px 10%; text-align: center; }
.blue-bg { background-color: var(--dark-blue); border-top: 2px solid var(--neon-blue); border-bottom: 2px solid var(--neon-blue); }
.section-title { font-size: 2.5rem; margin-bottom: 40px; color: var(--neon-blue); }

/* Rules */
.rules-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; }
.rule-box { background: rgba(255,255,255,0.1); padding: 20px; border-radius: 10px; border-right: 5px solid var(--neon-blue); }

/* Staff Section */
.staff-grid { display: flex; justify-content: center; gap: 30px; flex-wrap: wrap; }
.staff-card {
    background: #111; padding: 30px; border-radius: 15px; width: 250px;
    transition: 0.3s; border: 1px solid #333;
}
.staff-card img { width: 120px; height: 120px; border-radius: 50%; margin-bottom: 15px; border: 3px solid var(--neon-blue); }
.staff-card:hover { transform: translateY(-10px); box-shadow: 0 0 20px var(--neon-blue); }
.owner-card { border: 2px solid #ff4b2b; } /* ڕەنگی سوور بۆ ئۆنەر */

/* Gallery */
.gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 15px; }
.gallery-item img { width: 100%; border-radius: 10px; transition: 0.3s; }
.gallery-item img:hover { transform: scale(1.05); }

footer { padding: 30px; background: #000; text-align: center; color: #777; }

.audio-player {
    position: fixed;
    bottom: 20px;
    left: 20px;
    z-index: 9999;
}

#music-btn {
    background: var(--neon-blue);
    color: black;
    border: none;
    padding: 12px 20px;
    border-radius: 50px;
    font-weight: bold;
    cursor: pointer;
    box-shadow: 0 0 15px var(--neon-blue);
    transition: 0.3s;
    display: flex;
    align-items: center;
    gap: 10px;
}

#music-btn.playing {
    background: #ff4b2b;
    box-shadow: 0 0 15px #ff4b2b;
    color: white;
}

#music-btn:hover {
    transform: scale(1.1);
}







