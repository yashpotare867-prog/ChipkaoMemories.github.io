# ChipkaoMemories.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Chipkao Memories - Custom Fridge Magnets</title>
    <style>
        *{margin:0;padding:0;box-sizing:border-box}
        body{font-family:'Segoe UI',Tahoma,Geneva,Verdana,sans-serif;background:linear-gradient(135deg,#ff9a9e 0%,#fecfef 50%,#fecfef 100%);min-height:100vh;display:flex;align-items:center;justify-content:center;padding:20px}
        .card{background:white;border-radius:25px;padding:40px;box-shadow:0 25px 50px rgba(0,0,0,0.15);text-align:center;max-width:420px;width:100%;position:relative;overflow:hidden}
        .card::before{content:'';position:absolute;top:0;left:0;right:0;height:5px;background:linear-gradient(90deg,#ff6b6b,#ffd93d,#6bcf7f,#4facfe)}
        .logo{max-width:120px;margin:0 auto 25px;display:block;filter:drop-shadow(0 4px 8px rgba(0,0,0,0.1))}
        h1{font-size:2.3em;background:linear-gradient(135deg,#ff6b6b,#4facfe);-webkit-background-clip:text;-webkit-text-fill-color:transparent;font-weight:800;margin-bottom:15px}
        .tagline{font-size:1.25em;color:#555;font-weight:500;margin-bottom:25px;line-height:1.4}
        .features{display:grid;grid-template-columns:repeat(auto-fit,minmax(120px,1fr));gap:15px;margin:30px 0}
        .feature{padding:15px;background:#f8f9ff;border-radius:15px;box-shadow:0 5px 15px rgba(0,0,0,0.08);transition:transform 0.3s}
        .feature:hover{transform:translateY(-5px)}
        .icon{font-size:2em;margin-bottom:8px;display:block}
        .whatsapp-btn{display:inline-block;background:linear-gradient(135deg,#25D366,#128C7E);color:white;padding:20px 50px;border-radius:50px;font-size:1.3em;font-weight:700;text-decoration:none;box-shadow:0 15px 35px rgba(37,211,102,0.4);transition:all 0.3s;position:relative;overflow:hidden}
        .whatsapp-btn:hover{transform:translateY(-3px);box-shadow:0 20px 45px rgba(37,211,102,0.6)}
        .whatsapp-btn:active{transform:translateY(-1px)}
        .pulse{animation:pulse 2s infinite}
        @keyframes pulse{0%,100%{transform:scale(1)}50%{transform:scale(1.05)}}
        .trusted{display:flex;justify-content:center;align-items:center;gap:10px;font-size:0.9em;color:#666;margin-top:25px}
        .stars{color:#ffd93d}
    </style>
</head>
<body>
    <div class="card pulse">
        <img src="https://tinypng.com/backend/opt/download/ex4khtzq2ej2w1fr3trdgwd322gkaj3x/Screenshot%202026-05-02%20071012.png" alt="Chipkao Memories" class="logo">
        <h1>Chipkao Memories</h1>
        <p class="tagline">🎁 Turn your special moments into <strong>custom fridge magnets</strong> that last forever!</p>
        
        <div class="features">
            <div class="feature">
                <span class="icon">⚡</span>
                <strong>Ready in 3 days</strong>
            </div>
            <div class="feature">
                <span class="icon">📦</span>
                <strong>Shipping available</strong>
            </div>
            <div class="feature">
                <span class="icon">⭐</span>
                <strong>4.9★ Rating</strong>
            </div>
        </div>
        
        <a href="https://wa.me/919152917593?text=Hi%20Chipkao!%20🎁%20Saw%20your%20IG%20(@chipkaomemories)%20-%20want%20custom%20fridge%20magnets!%20What's%20the%20price%20&%20how%20to%20order?%20😍" 
           class="whatsapp-btn" 
           onclick="trackClick()">
            💬 Order on WhatsApp Now!
        </a>
        
        <div class="trusted">
            <span class="stars">⭐⭐⭐⭐⭐</span>
            <span>500+ Happy Customers</span>
        </div>
    </div>

    <!-- Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
    <script>
        window.dataLayer = window.dataLayer || [];
        function gtag(){dataLayer.push(arguments);}
        gtag('js', new Date());
        gtag('config', 'G-XXXXXXXXXX');
        
        function trackClick() {
            gtag('event', 'whatsapp_click', {
                'event_category': 'conversion',
                'event_label': 'fridge_magnet_order',
                'value': 50
            });
        }
        
        // Auto-redirect for desktop users
        if(/Mobi|Android/i.test(navigator.userAgent)) {
            setTimeout(() => {
                window.location.href = "https://wa.me/919152917593?text=Hi%20Chipkao!%20🎁%20Saw%20your%20IG%20(@chipkaomemories)%20-%20want%20custom%20fridge%20magnets!%20What's%20the%20price%20&%20how%20to%20order?%20😍";
            }, 2000);
        }
    </script>
</body>
</html>
