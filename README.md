# joshuaklaus1.github.io

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Free Movies+</title>
    <!-- Telegram Web App SDK for clean rendering if loaded inside TG -->
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    
    <style>
        :root {
            --bg-color: #0c1020;
            --card-bg: #161b33;
            --accent-green: #63f5b0;
            --accent-blue: #00f0ff;
            --text-color: #ffffff;
            --text-muted: #8fa0c0;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            -webkit-tap-highlight-color: transparent;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            padding: 16px;
            display: flex;
            flex-direction: column;
            align-items: center;
            min-height: 100vh;
        }

        /* Matches the FREE MOVIES+ text design */
        .header {
            text-align: center;
            margin-bottom: 24px;
            margin-top: 10px;
        }

        .header h1 {
            font-size: 2.5rem;
            font-weight: 900;
            text-transform: uppercase;
            font-style: italic;
            letter-spacing: -1px;
            line-height: 1.1;
        }

        .text-green {
            color: var(--accent-green);
        }

        .text-blue {
            color: var(--accent-blue);
        }

        .subtitle {
            color: var(--text-muted);
            font-size: 0.9rem;
            margin-top: 6px;
        }

        /* Layout Structure */
        .grid-container {
            width: 100%;
            max-width: 450px;
            display: grid;
            grid-template-columns: 1fr;
            gap: 14px;
        }

        .movie-card {
            background-color: var(--card-bg);
            border-radius: 12px;
            padding: 16px;
            display: flex;
            flex-direction: column;
            border: 1px solid rgba(255, 255, 255, 0.05);
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
        }

        .movie-title {
            font-size: 1.1rem;
            font-weight: 700;
            margin-bottom: 4px;
        }

        .movie-desc {
            font-size: 0.85rem;
            color: var(--text-muted);
            margin-bottom: 14px;
            line-height: 1.4;
        }

        /* Interactive Monetized Buttons */
        .btn-unlock {
            background: linear-gradient(90deg, #00c6ff 0%, #0072ff 100%);
            color: white;
            border: none;
            padding: 12px;
            border-radius: 8px;
            font-weight: 700;
            font-size: 0.95rem;
            cursor: pointer;
            transition: transform 0.1s ease;
            text-transform: uppercase;
            text-align: center;
            text-decoration: none;
        }

        .btn-unlock:active {
            transform: scale(0.98);
        }

        /* Compliance footer keeping ad network happy */
        .footer {
            margin-top: auto;
            padding: 20px 0 10px 0;
            text-align: center;
            font-size: 0.75rem;
            color: var(--text-muted);
            max-width: 300px;
            line-height: 1.3;
        }
    </style>
</head>
<body>

    <div class="header">
        <h1>
            <span class="text-green">Free</span><br>
            <span class="text-blue">Movies +</span>
        </h1>
        <p class="subtitle">Global Legal Streaming Directories</p>
    </div>

    <div class="grid-container">
        
        <!-- Category 1: Global Plex Catalog -->
        <div class="movie-card">
            <div class="movie-title">🎬 Worldwide Plex Catalog</div>
            <div class="movie-desc">Unlock instant access to over 50,000 free movies and global streaming servers.</div>
            <button class="btn-unlock" onclick="redirectToAd('https://www.plex.tv/watch-free/')">Unlock List</button>
        </div>

        <!-- Category 2: Global Live Channels -->
        <div class="movie-card">
            <div class="movie-title">🍿 Free Live TV Channels</div>
            <div class="movie-desc">Watch hundreds of global live network entertainment streams right from your device.</div>
            <button class="btn-unlock" onclick="redirectToAd('https://support.plex.tv/articles/free-live-tv-streaming-overview/')">Access Channels</button>
        </div>

        <!-- Category 3: YouTube Official Hub -->
        <div class="movie-card">
            <div class="movie-title">🔥 Classic & Indie Cinema</div>
            <div class="movie-desc">Browse thousands of licensed full-length cinema masterpieces available completely free.</div>
            <button class="btn-unlock" onclick="redirectToAd('https://www.youtube.com/feed/storefront?bp=kgEmCGQvY2gvVUNwR3BCbXZwY3NoS01pTTh4R1VnS0NBbUo0Z0JFZ0A%3D')">Open Catalog</button>
        </div>

    </div>

    <div class="footer">
        All directory links point to 100% licensed, global, and public ad-supported streaming networks. No pirated materials are hosted here.
    </div>

    <script>
        // Signal ready state if used inside Telegram native window
        if (window.Telegram && window.Telegram.WebApp) {
            window.Telegram.WebApp.ready();
            window.Telegram.WebApp.expand();
        }

        // Your exact Monetag Direct Link
        const monetagSmartLink = "https://omg10.com/4/11230560";

        function redirectToAd(finalDestination) {
            // First open your Monetag Monetization Link in a new tab to earn cash
            window.open(monetagSmartLink, '_blank');
            
            // Then instantly shift the main window to the legitimate, promised movie source
            window.location.href = finalDestination;
        }
    </script>
</body>
</html>
