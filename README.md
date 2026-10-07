<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Talent Movie/Music Box</title>

    <meta name="description"
        content="Talent Movie/Music Box - Discover trending movies, music, artists and entertainment.">

    <link rel="stylesheet" href="style.css">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap"
        rel="stylesheet">
</head>

<body>

<!-- ================= NAVIGATION ================= -->

<header class="navbar">

    <div class="logo">
        <span class="logo-icon">▶</span>
        <div>
            <strong>Talent</strong>
            <span>Movie/Music Box</span>
        </div>
    </div>

    <nav id="mainNav">
        <a href="#home">Home</a>
        <a href="#movies">Movies</a>
        <a href="#music">Music</a>
        <a href="#trending">Trending</a>
        <a href="#about">About</a>
    </nav>

    <div class="nav-actions">

        <button class="search-btn" onclick="openSearch()">
            🔍
        </button>

        <button class="login-btn" onclick="showMessage('Login system coming soon!')">
            Sign In
        </button>

        <button class="menu-btn" onclick="toggleMenu()">
            ☰
        </button>

    </div>

</header>


<!-- ================= HERO ================= -->

<section class="hero" id="home">

    <div class="hero-content">

        <span class="hero-label">🔥 #1 TRENDING ENTERTAINMENT</span>

        <h1>
            Entertainment<br>
            <span>Without Limits.</span>
        </h1>

        <p>
            Discover trending movies, hit songs, rising artists and
            unforgettable entertainment — all in one place.
        </p>

        <div class="hero-buttons">

            <button class="primary-btn" onclick="scrollToSection('trending')">
                ▶ Explore Trending
            </button>

            <button class="secondary-btn" onclick="openTrailer('Featured Entertainment')">
                Watch Trailer
            </button>

        </div>

        <div class="hero-stats">

            <div>
                <strong>10K+</strong>
                <span>Movies</span>
            </div>

            <div>
                <strong>50K+</strong>
                <span>Songs</span>
            </div>

            <div>
                <strong>100K+</strong>
                <span>Fans</span>
            </div>

        </div>

    </div>

    <div class="hero-visual">

        <div class="floating-card card-one">
            <span>🎬</span>
            <div>
                <small>NOW TRENDING</small>
                <strong>Movies</strong>
            </div>
        </div>

        <div class="main-poster">

            <div class="poster-content">

                <span>TM</span>

                <h2>
                    THE<br>
                    NEXT<br>
                    CHAPTER
                </h2>

                <p>Talent Original</p>

            </div>

            <div class="poster-glow"></div>

        </div>

        <div class="floating-card card-two">
            <span>🎵</span>
            <div>
                <small>HOT RIGHT NOW</small>
                <strong>Afrobeats</strong>
            </div>
        </div>

    </div>

</section>


<!-- ================= TRENDING BAR ================= -->

<section class="trending-strip">

    <div class="trend-title">
        <span class="live-dot"></span>
        LIVE TRENDS
    </div>

    <div class="ticker">

        <span>🔥 Ikebe — Blaqbonez ft. Asake</span>
        <span>🎬 My Father's Shadow</span>
        <span>🎵 Afrobeats 2026</span>
        <span>🎬 Animals</span>
        <span>🎧 Nigerian Top Charts</span>

    </div>

</section>


<!-- ================= TRENDING ================= -->

<section class="section" id="trending">

    <div class="section-heading">

        <div>
            <span class="eyebrow">WHAT'S HOT</span>
            <h2>Trending <span>Now</span></h2>
        </div>

        <button class="outline-btn" onclick="filterAll()">
            View All →
        </button>

    </div>


    <div class="content-grid">

        <!-- Movie -->
        <article class="media-card movie-card"
            data-category="movie">

            <div class="media-image poster-red">

                <span class="rank">01</span>

                <div class="poster-info">
                    <small>NETFLIX</small>
                    <h3>My Father's<br>Shadow</h3>
                    <p>Drama • Nigeria</p>
                </div>

                <button class="play-button"
                    onclick="openTrailer('My Father’s Shadow')">
                    ▶
                </button>

            </div>

            <div class="media-details">

                <div>
                    <h3>My Father's Shadow</h3>
                    <p>Drama • 2026</p>
                </div>

                <span class="rating">⭐ 8.7</span>

            </div>

        </article>


        <!-- Movie -->
        <article class="media-card movie-card"
            data-category="movie">

            <div class="media-image poster-blue">

                <span class="rank">02</span>

                <div class="poster-info">
                    <small>NEW RELEASE</small>
                    <h3>Animals</h3>
                    <p>Thriller • Drama</p>
                </div>

                <button class="play-button"
                    onclick="openTrailer('Animals')">
                    ▶
                </button>

            </div>

            <div class="media-details">

                <div>
                    <h3>Animals</h3>
                    <p>Thriller • 2026</p>
                </div>

                <span class="rating">⭐ 8.4</span>

            </div>

        </article>


        <!-- Music -->
        <article class="media-card music-card"
            data-category="music">

            <div class="media-image poster-purple">

                <span class="rank">03</span>

                <div class="music-symbol">♫</div>

                <div class="poster-info">
                    <small>HOT TRACK</small>
                    <h3>Ikebe</h3>
                    <p>Blaqbonez ft. Asake</p>
                </div>

                <button class="play-button"
                    onclick="playSong('Ikebe — Blaqbonez ft. Asake')">
                    ▶
                </button>

            </div>

            <div class="media-details">

                <div>
                    <h3>Ikebe</h3>
                    <p>Blaqbonez ft. Asake</p>
                </div>

                <span class="rating">🔥 #1</span>

            </div>

        </article>


        <!-- Movie -->
        <article class="media-card movie-card"
            data-category="movie">

            <div class="media-image poster-gold">

                <span class="rank">04</span>

                <div class="poster-info">
                    <small>NETFLIX</small>
                    <h3>Doing<br>Life</h3>
                    <p>Drama</p>
                </div>

                <button class="play-button"
                    onclick="openTrailer('Doing Life')">
                    ▶
                </button>

            </div>

            <div class="media-details">

                <div>
                    <h3>Doing Life</h3>
                    <p>Drama • 2026</p>
                </div>

                <span class="rating">⭐ 8.2</span>

            </div>

        </article>

    </div>

</section>


<!-- ================= MOVIES ================= -->

<section class="section dark-section" id="movies">

    <div class="section-heading">

        <div>
            <span class="eyebrow">CINEMA</span>
            <h2>Featured <span>Movies</span></h2>
        </div>

        <div class="category-buttons">

            <button class="active" onclick="filterMovies('all', this)">
                All
            </button>

            <button onclick="filterMovies('action', this)">
                Action
            </button>

            <button onclick="filterMovies('drama', this)">
                Drama
            </button>

            <button onclick="filterMovies('comedy', this)">
                Comedy
            </button>

        </div>

    </div>


    <div class="movie-grid" id="movieGrid">

        <article class="movie-tile" data-genre="drama">

            <div class="tile-poster tile-one">

                <span>01</span>

                <div>
                    <small>DRAMA</small>
                    <h3>My Father's Shadow</h3>
                </div>

                <button onclick="openTrailer('My Father’s Shadow')">
                    ▶
                </button>

            </div>

            <h3>My Father's Shadow</h3>
            <p>Drama • Nigeria • 2026</p>

        </article>


        <article class="movie-tile" data-genre="action">

            <div class="tile-poster tile-two">

                <span>02</span>

                <div>
                    <small>THRILLER</small>
                    <h3>Animals</h3>
                </div>

                <button onclick="openTrailer('Animals')">
                    ▶
                </button>

            </div>

            <h3>Animals</h3>
            <p>Thriller • USA • 2026</p>

        </article>


        <article class="movie-tile" data-genre="comedy">

            <div class="tile-poster tile-three">

                <span>03</span>

                <div>
                    <small>COMEDY</small>
                    <h3>The Storm</h3>
                </div>

                <button onclick="openTrailer('The Storm')">
                    ▶
                </button>

            </div>

            <h3>The Storm</h3>
            <p>Comedy • Sweden • 2026</p>

        </article>


        <article class="movie-tile" data-genre="drama">

            <div class="tile-poster tile-four">

                <span>04</span>

                <div>
                    <small>DRAMA</small>
                    <h3>Doing Life</h3>
                </div>

                <button onclick="openTrailer('Doing Life')">
                    ▶
                </button>

            </div>

            <h3>Doing Life</h3>
            <p>Drama • 2026</p>

        </article>


        <article class="movie-tile" data-genre="action">

            <div class="tile-poster tile-five">

                <span>05</span>

                <div>
                    <small>ACTION</small>
                    <h3>Sacrifice</h3>
                </div>

                <button onclick="openTrailer('Sacrifice')">
                    ▶
                </button>

            </div>

            <h3>Sacrifice</h3>
            <p>Action • 2026</p>

        </article>


        <article class="movie-tile" data-genre="comedy">

            <div class="tile-poster tile-six">

                <span>06</span>

                <div>
                    <small>COMEDY</small>
                    <h3>Seriously Single Too</h3>
                </div>

                <button onclick="openTrailer('Seriously Single Too')">
                    ▶
                </button>

            </div>

            <h3>Seriously Single Too</h3>
            <p>Romance • Comedy</p>

        </article>

    </div>

</section>


<!-- ================= MUSIC ================= -->

<section class="section" id="music">

    <div class="section-heading">

        <div>
            <span class="eyebrow">SOUND OF NOW</span>
            <h2>Trending <span>Music</span></h2>
        </div>

        <button class="outline-btn">
            Music Charts →
        </button>

    </div>


    <div class="music-layout">

        <div class="music-feature">

            <div class="vinyl">

                <div class="vinyl-label">
                    TM
                </div>

            </div>

            <div class="music-feature-info">

                <span class="eyebrow">NOW PLAYING</span>

                <h3>Ikebe</h3>

                <p>Blaqbonez ft. Asake</p>

                <div class="music-progress">
                    <div></div>
                </div>

                <div class="music-time">
                    <span>1:24</span>
                    <span>3:12</span>
                </div>

                <div class="player-controls">

                    <button>↶</button>

                    <button class="big-play"
                        onclick="playSong('Ikebe — Blaqbonez ft. Asake')">
                        ▶
                    </button>

                    <button>↷</button>

                </div>

            </div>

        </div>


        <div class="song-list">

            <div class="song active-song"
                onclick="playSong('Ikebe — Blaqbonez ft. Asake')">

                <span class="song-number">01</span>

                <div class="album-art art-one">♫</div>

                <div class="song-info">
                    <strong>Ikebe</strong>
                    <span>Blaqbonez ft. Asake</span>
                </div>

                <span class="song-time">3:12</span>

                <button>▶</button>

            </div>


            <div class="song"
                onclick="playSong('Eja Meja — BNXN ft. Asake')">

                <span class="song-number">02</span>

                <div class="album-art art-two">♪</div>

                <div class="song-info">
                    <strong>Eja Meja</strong>
                    <span>BNXN ft. Asake</span>
                </div>

                <span class="song-time">2:58</span>

                <button>▶</button>

            </div>


            <div class="song"
                onclick="playSong('B4 B4 — Davido, FOLA & Mayorkun')">

                <span class="song-number">03</span>

                <div class="album-art art-three">♫</div>

                <div class="song-info">
                    <strong>B4 B4</strong>
                    <span>Davido, FOLA & Mayorkun</span>
                </div>

                <span class="song-time">3:04</span>

                <button>▶</button>

            </div>


            <div class="song"
                onclick="playSong('Oh No — Rema')">

                <span class="song-number">04</span>

                <div class="album-art art-four">♪</div>

                <div class="song-info">
                    <strong>Oh No</strong>
                    <span>Rema</span>
                </div>

                <span class="song-time">2:46</span>

                <button>▶</button>

            </div>


            <div class="song"
                onclick="playSong('Ginger — Wizkid ft. Burna Boy')">

                <span class="song-number">05</span>

                <div class="album-art art-five">♫</div>

                <div class="song-info">
                    <strong>Ginger</strong>
                    <span>Wizkid ft. Burna Boy</span>
                </div>

                <span class="song-time">3:14</span>

                <button>▶</button>

            </div>

        </div>

    </div>

</section>


<!-- ================= ARTISTS ================= -->

<section class="section artist-section">

    <div class="section-heading">

        <div>
            <span class="eyebrow">MUSIC WORLD</span>
            <h2>Popular <span>Artists</span></h2>
        </div>

    </div>


    <div class="artist-grid">

        <div class="artist">
            <div class="artist-avatar avatar-one">A</div>
            <h3>Asake</h3>
            <p>Afrobeats</p>
        </div>

        <div class="artist">
            <div class="artist-avatar avatar-two">B</div>
            <h3>Blaqbonez</h3>
            <p>Hip-Hop / Afrobeats</p>
        </div>

        <div class="artist">
            <div class="artist-avatar avatar-three">D</div>
            <h3>Davido</h3>
            <p>Afrobeats</p>
        </div>

        <div class="artist">
            <div class="artist-avatar avatar-four">R</div>
            <h3>Rema</h3>
            <p>Afrobeats</p>
        </div>

        <div class="artist">
            <div class="artist-avatar avatar-five">W</div>
            <h3>Wizkid</h3>
            <p>Afrobeats</p>
        </div>

        <div class="artist">
            <div class="artist-avatar avatar-six">F</div>
            <h3>FOLA</h3>
            <p>Afropop</p>
        </div>

    </div>

</section>


<!-- ================= NEWSLETTER ================= -->

<section class="newsletter">

    <div>

        <span class="eyebrow">TALENT INSIDER</span>

        <h2>Never miss what's <span>trending.</span></h2>

        <p>
            Get the latest movie releases, music drops and entertainment
            stories delivered to you.
        </p>

    </div>

    <form onsubmit="subscribe(event)">

        <input
            type="email"
            id="email"
            placeholder="Enter your email address"
            required
        >

        <button type="submit">
            Subscribe
        </button>

    </form>

</section>


<!-- ================= ABOUT ================= -->

<section class="about" id="about">

    <div class="about-logo">
        <span>TM</span>
    </div>

    <div>

        <span class="eyebrow">ABOUT TALENT</span>

        <h2>Your entertainment universe.</h2>

        <p>
            Talent Movie/Music Box is a modern entertainment discovery
            platform built for movie lovers, music fans and creators.
            Discover what is trending, explore new releases and find
            your next favourite movie or song.
        </p>

    </div>

</section>


<!-- ================= FOOTER ================= -->

<footer>

    <div class="footer-main">

        <div class="footer-brand">

            <div class="logo">

                <span class="logo-icon">▶</span>

                <div>
                    <strong>Talent</strong>
                    <span>Movie/Music Box</span>
                </div>

            </div>

            <p>
                Movies. Music. Culture. Everything you love.
            </p>

        </div>


        <div class="footer-column">

            <h4>Explore</h4>

            <a href="#movies">Movies</a>
            <a href="#music">Music</a>
            <a href="#trending">Trending</a>
            <a href="#about">About</a>

        </div>


        <div class="footer-column">

            <h4>Genres</h4>

            <a href="#">Action</a>
            <a href="#">Drama</a>
            <a href="#">Comedy</a>
            <a href="#">Afrobeats</a>

        </div>


        <div class="footer-column">

            <h4>Connect</h4>

            <a href="#">Facebook</a>
            <a href="#">Instagram</a>
            <a href="#">TikTok</a>
            <a href="#">YouTube</a>

        </div>

    </div>


    <div class="footer-bottom">

        <p>
            © 2026 Talent Movie/Music Box. All rights reserved.
        </p>

        <p>
            Built for entertainment lovers.
        </p>

    </div>

</footer>


<!-- ================= TRAILER MODAL ================= -->

<div class="modal" id="trailerModal">

    <div class="modal-box">

        <button class="close-modal" onclick="closeModal()">
            ×
        </button>

        <div class="video-placeholder">

            <div class="video-play">
                ▶
            </div>

            <h2 id="modalTitle">
                Movie Trailer
            </h2>

            <p>
                Official trailer / preview can be connected here.
            </p>

        </div>

    </div>

</div>


<!-- ================= SEARCH MODAL ================= -->

<div class="search-overlay" id="searchOverlay">

    <div class="search-box">

        <button class="close-search" onclick="closeSearch()">
            ×
        </button>

        <span class="eyebrow">SEARCH TALENT BOX</span>

        <h2>What are you looking for?</h2>

        <input
            type="text"
            id="searchInput"
            placeholder="Search movies, songs or artists..."
            oninput="searchContent()"
        >

        <div id="searchResults"></div>

    </div>

</div>


<!-- ================= TOAST ================= -->

<div class="toast" id="toast">
    <span>✓</span>
    <p id="toastText">Done</p>
</div>


<script src="script.js"></script>

</body>
</html>
