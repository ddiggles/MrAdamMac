# MrAdamMac
Website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Name — Composer & Songwriter</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --bg-color: #0d0d0d;
            --text-color: #f5f5f5;
            --muted-text: #a0a0a0;
            --accent-color: #d4af37;
            --card-bg: #161616;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.8)), url('YOUR_HERO_PHOTO.jpg') no-repeat center center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 0 20px;
        }

        .hero h1 {
            font-size: clamp(2.5rem, 5vw, 4.5rem);
            font-weight: 600;
            letter-spacing: -1px;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: clamp(1rem, 2vw, 1.25rem);
            color: var(--muted-text);
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 30px;
        }

        .cta-buttons {
            display: flex;
            gap: 15px;
        }

        .btn {
            padding: 12px 28px;
            border: 1px solid var(--text-color);
            background: transparent;
            color: var(--text-color);
            text-decoration: none;
            font-size: 0.9rem;
            font-weight: 500;
            transition: all 0.3s ease;
            border-radius: 4px;
        }

        .btn:hover {
            background: var(--text-color);
            color: var(--bg-color);
        }

        /* Section Layouts */
        section {
            padding: 100px 8vw;
            max-width: 1400px;
            margin: 0 auto;
        }

        h2.section-title {
            font-size: 2rem;
            font-weight: 500;
            margin-bottom: 40px;
            letter-spacing: -0.5px;
            border-left: 3px solid var(--accent-color);
            padding-left: 15px;
        }

        /* Music Section */
        .spotify-container {
            background: var(--card-bg);
            border-radius: 12px;
            padding: 20px;
            border: 1px solid #222;
        }

        /* Video Section */
        .video-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
            height: 0;
            border-radius: 8px;
            overflow: hidden;
            background: var(--card-bg);
        }

        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: 0;
        }

        /* Photography Gallery */
        .photo-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .photo-card {
            overflow: hidden;
            border-radius: 8px;
            aspect-ratio: 4/5;
            background: var(--card-bg);
        }

        .photo-card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }

        .photo-card:hover img {
            transform: scale(1.04);
        }

        /* Footer */
        footer {
            background: #080808;
            padding: 60px 8vw;
            text-align: center;
            border-top: 1px solid #1a1a1a;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 30px;
            margin-bottom: 25px;
        }

        .social-links a {
            color: var(--muted-text);
            text-decoration: none;
            font-size: 1rem;
            transition: color 0.2s ease;
        }

        .social-links a:hover {
            color: var(--accent-color);
        }

        .copyright {
            color: var(--muted-text);
            font-size: 0.85rem;
        }
    </style>
</head>
<body>

    <!-- Hero Section -->
    <header class="hero">
        <h1>Your Name</h1>
        <p>Composer & Songwriter</p>
        <div class="cta-buttons">
            <a href="#music" class="btn">Listen</a>
            <a href="#visuals" class="btn">Watch</a>
        </div>
    </header>

    <!-- Spotify Section -->
    <section id="music">
        <h2 class="section-title">Selected Works</h2>
        <div class="spotify-container">
            <!-- Replace YOUR_SPOTIFY_URI with your track/album/playlist embed code -->
            <iframe style="border-radius:12px" src="https://open.spotify.com/embed/artist/YOUR_SPOTIFY_URI?utm_source=generator&theme=0" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div>
    </section>

    <!-- YouTube Video Section -->
    <section id="visuals">
        <h2 class="section-title">Film Scoring & Reels</h2>
        <div class="video-grid">
            <div class="video-wrapper">
                <!-- Replace with your YouTube Embed URL -->
                <iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID_1" title="YouTube video player" allowfullscreen></iframe>
            </div>
            <div class="video-wrapper">
                <iframe src="https://www.youtube.com/embed/YOUR_VIDEO_ID_2" title="YouTube video player" allowfullscreen></iframe>
            </div>
        </div>
    </section>

    <!-- Photo Gallery Section -->
    <section id="gallery">
        <h2 class="section-title">Gallery</h2>
        <div class="photo-grid">
            <div class="photo-card">
                <img src="photo1.jpg" alt="Press Photo 1">
            </div>
            <div class="photo-card">
                <img src="photo2.jpg" alt="Press Photo 2">
            </div>
            <div class="photo-card">
                <img src="photo3.jpg" alt="Press Photo 3">
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="social-links">
            <a href="https://spotify.com/yourprofile" target="_blank">Spotify</a>
            <a href="https://youtube.com/yourchannel" target="_blank">YouTube</a>
            <a href="https://instagram.com/yourhandle" target="_blank">Instagram</a>
            <a href="mailto:your@email.com">Contact</a>
        </div>
        <p class="copyright">&copy; 2026 Your Name. All rights reserved.</p>
    </footer>

</body>
</html>
