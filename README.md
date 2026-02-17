<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Luedke Plumbing LLC | Tampa's Trusted Plumber Since 2014</title>
    <meta name="description" content="State licensed, bonded & insured plumbing contractor serving Tampa, FL. Over 10 years experience and 120+ completed projects. Call (813) 523-9534.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Barlow:wght@500;600;700;800;900&family=Barlow+Condensed:wght@600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --blue: #1a4b8c;
            --blue-light: #2a5fa8;
            --blue-dark: #0f3a6e;
            --yellow: #f7d44c;
            --yellow-light: #f9e07a;
            --yellow-dark: #d4b230;
            --black: #111;
            --dark: #1a1a1a;
            --gray-900: #222;
            --gray-700: #444;
            --gray-500: #666;
            --gray-300: #aaa;
            --gray-100: #eee;
            --white: #fff;
            --cream: #f5f3ed;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Barlow', sans-serif;
            background: var(--cream);
            color: var(--gray-900);
            line-height: 1.5;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Utility */
        .text-copper { color: var(--copper); }

        /* Top Bar */
        .top-bar {
            background: var(--blue);
            color: var(--white);
            padding: 10px 0;
            font-size: 13px;
            font-weight: 600;
            letter-spacing: 0.5px;
        }

        .top-bar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 8px;
        }

        .top-bar a {
            color: var(--yellow);
            text-decoration: none;
        }

        /* Header */
        header {
            background: var(--yellow);
            padding: 12px 0;
            border-bottom: 4px solid var(--blue);
        }

        header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .logo-mark {
            width: 44px;
            height: 44px;
            background: var(--blue);
            display: flex;
            align-items: center;
            justify-content: center;
            font-family: 'Barlow Condensed', sans-serif;
            font-weight: 700;
            font-size: 22px;
            color: var(--white);
        }

        .logo-text {
            font-family: 'Barlow Condensed', sans-serif;
            font-weight: 700;
            font-size: 26px;
            color: var(--black);
            text-transform: uppercase;
            letter-spacing: 1px;
            line-height: 1.1;
        }

        .logo-text small {
            display: block;
            font-family: 'Barlow', sans-serif;
            font-size: 11px;
            font-weight: 600;
            color: var(--gray-500);
            letter-spacing: 2px;
        }

        .header-phone {
            display: flex;
            align-items: center;
            gap: 8px;
            color: var(--black);
            text-decoration: none;
            font-weight: 700;
            font-size: 20px;
        }

        .header-phone svg {
            width: 22px;
            height: 22px;
            fill: var(--blue);
        }

        /* Hero */
        .hero {
            position: relative;
            min-height: 520px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            background: var(--yellow);
        }

        .hero-content-wrap {
            padding: 60px 40px 60px 0;
            display: flex;
            align-items: center;
        }

        .hero-content {
            max-width: 540px;
            margin-left: auto;
        }

        .hero h1 {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: clamp(42px, 6vw, 64px);
            font-weight: 700;
            color: var(--blue-dark);
            text-transform: uppercase;
            line-height: 1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: var(--blue);
        }

        .hero-text {
            font-size: 18px;
            color: var(--blue-dark);
            margin-bottom: 28px;
            max-width: 480px;
        }

        .hero-cta {
            display: flex;
            gap: 12px;
            flex-wrap: wrap;
            margin-bottom: 40px;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 14px 24px;
            font-family: 'Barlow', sans-serif;
            font-weight: 700;
            font-size: 14px;
            text-decoration: none;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.15s ease;
            cursor: pointer;
            border: none;
        }

        .btn-copper {
            background: var(--blue);
            color: var(--white);
        }

        .btn-copper:hover {
            background: var(--blue-dark);
        }

        .btn-white {
            background: var(--white);
            color: var(--black);
        }

        .btn-white:hover {
            background: var(--gray-100);
        }

        .btn-outline-dark {
            background: transparent;
            border: 2px solid var(--blue);
            color: var(--blue-dark);
        }

        .btn-outline-dark:hover {
            background: var(--blue);
            color: var(--white);
        }

        .hero-stats {
            display: flex;
            gap: 32px;
            padding-top: 32px;
            border-top: 2px solid rgba(26, 75, 140, 0.2);
        }

        .stat-item {
            text-align: left;
        }

        .stat-num {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: 40px;
            font-weight: 700;
            color: var(--blue);
            line-height: 1;
        }

        .stat-label {
            font-size: 12px;
            color: var(--blue-dark);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .hero-image {
            background: 
                url('https://images.unsplash.com/photo-1585704032915-c3400ca199e7?w=900&q=80') center/cover;
            position: relative;
        }

        .hero-image::before {
            content: '';
            position: absolute;
            left: 0;
            top: 0;
            bottom: 0;
            width: 80px;
            background: linear-gradient(90deg, var(--yellow), transparent);
        }

        /* Photo Band */
        .photo-band {
            display: grid;
            grid-template-columns: repeat(4, 1fr);
            height: 180px;
            background: var(--yellow);
        }

        .photo-band img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            border: 3px solid var(--yellow);
        }

        /* Credentials Bar */
        .cred-bar {
            background: var(--blue);
            padding: 24px 0;
        }

        .cred-bar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
            gap: 20px;
        }

        .cred-item {
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--white);
            font-size: 14px;
            font-weight: 700;
        }

        .cred-item svg {
            width: 20px;
            height: 20px;
            fill: var(--yellow);
        }

        /* Services */
        .services {
            padding: 80px 0;
            background: var(--white);
        }

        .section-label {
            font-size: 12px;
            font-weight: 700;
            color: var(--blue);
            text-transform: uppercase;
            letter-spacing: 3px;
            margin-bottom: 8px;
        }

        .section-title {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: clamp(32px, 4vw, 44px);
            font-weight: 700;
            color: var(--blue-dark);
            text-transform: uppercase;
            margin-bottom: 48px;
        }

        .services-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2px;
            background: var(--gray-100);
        }

        .service-item {
            background: var(--cream);
            padding: 28px 24px;
            display: flex;
            align-items: flex-start;
            gap: 16px;
        }

        .service-icon {
            width: 32px;
            height: 32px;
            flex-shrink: 0;
        }

        .service-icon svg {
            width: 100%;
            height: 100%;
            fill: var(--blue);
        }

        .service-item h3 {
            font-size: 16px;
            font-weight: 700;
            color: var(--black);
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 6px;
        }

        .service-item p {
            font-size: 14px;
            color: var(--gray-500);
            line-height: 1.6;
        }

        /* About Split */
        .about-split {
            display: grid;
            grid-template-columns: 1fr 1fr;
        }

        .about-image {
            min-height: 450px;
            background: 
                url('https://images.unsplash.com/photo-1504328345606-18bbc8c9d7d1?w=900&q=80') center/cover;
        }

        .about-content {
            background: var(--cream);
            padding: 60px 48px;
            display: flex;
            flex-direction: column;
            justify-content: center;
        }

        .about-content .section-label {
            color: var(--blue);
        }

        .about-content .section-title {
            color: var(--blue-dark);
            margin-bottom: 24px;
        }

        .about-content p {
            color: var(--gray-700);
            font-size: 16px;
            line-height: 1.8;
            margin-bottom: 32px;
        }

        .about-list {
            list-style: none;
        }

        .about-list li {
            display: flex;
            align-items: center;
            gap: 12px;
            color: var(--gray-900);
            font-weight: 600;
            font-size: 15px;
            padding: 12px 0;
            border-bottom: 1px solid var(--gray-200);
        }

        .about-list li:last-child {
            border-bottom: none;
        }

        .about-list svg {
            width: 18px;
            height: 18px;
            fill: var(--blue);
        }

        /* CTA */
        .cta {
            padding: 80px 0;
            background: var(--white);
            text-align: center;
        }

        .cta h2 {
            font-family: 'Barlow Condensed', sans-serif;
            font-size: clamp(32px, 5vw, 52px);
            font-weight: 700;
            color: var(--blue);
            text-transform: uppercase;
            margin-bottom: 12px;
        }

        .cta p {
            color: var(--gray-700);
            font-size: 18px;
            margin-bottom: 24px;
        }

        .cta-phone {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            font-family: 'Barlow Condensed', sans-serif;
            font-size: clamp(32px, 5vw, 48px);
            font-weight: 700;
            color: var(--blue);
            text-decoration: none;
            margin-bottom: 28px;
        }

        .cta-phone svg {
            width: 40px;
            height: 40px;
            fill: var(--blue);
        }

        .cta-buttons {
            display: flex;
            gap: 12px;
            justify-content: center;
            flex-wrap: wrap;
        }

        .btn-dark {
            background: var(--blue);
            color: var(--white);
        }

        .btn-dark:hover {
            background: var(--blue-dark);
        }

        .btn-ghost {
            background: transparent;
            border: 2px solid var(--blue);
            color: var(--blue);
        }

        .btn-ghost:hover {
            background: var(--blue);
            color: var(--white);
        }

        /* Footer */
        footer {
            background: var(--blue-dark);
            color: var(--gray-300);
            padding: 48px 0 24px;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-brand .logo-text {
            color: var(--white);
            margin-bottom: 12px;
        }

        .footer-brand p {
            font-size: 14px;
            line-height: 1.7;
        }

        .footer-heading {
            font-size: 12px;
            font-weight: 700;
            color: var(--yellow);
            text-transform: uppercase;
            letter-spacing: 2px;
            margin-bottom: 16px;
        }

        .footer-links {
            list-style: none;
        }

        .footer-links li {
            margin-bottom: 8px;
        }

        .footer-links a {
            color: var(--gray-300);
            text-decoration: none;
            font-size: 14px;
        }

        .footer-links a:hover {
            color: var(--yellow);
        }

        .footer-bottom {
            padding-top: 24px;
            border-top: 1px solid var(--blue);
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 12px;
            font-size: 13px;
        }

        /* Responsive */
        @media (max-width: 900px) {
            .hero {
                grid-template-columns: 1fr;
            }
            .hero-content-wrap {
                padding: 60px 20px;
            }
            .hero-content {
                margin-left: 0;
                max-width: 100%;
            }
            .hero-image {
                min-height: 300px;
            }
            .about-split {
                grid-template-columns: 1fr;
            }
            .about-image {
                min-height: 280px;
            }
            .about-content {
                padding: 48px 24px;
            }
            .footer-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 600px) {
            .hero-image {
                display: none;
            }
            .photo-band {
                grid-template-columns: repeat(2, 1fr);
                height: auto;
            }
            .photo-band img {
                height: 140px;
            }
            .hero-stats {
                flex-wrap: wrap;
                gap: 20px;
            }
            .cred-bar .container {
                justify-content: center;
                text-align: center;
            }
            .footer-bottom {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- Top Bar -->
    <div class="top-bar">
        <div class="container">
            <span>FL License #CFC1429117 — Bonded & Insured</span>
            <span>Tampa & Surrounding Areas — <a href="tel:8135239534">(813) 523-9534</a></span>
        </div>
    </div>

    <!-- Header -->
    <header>
        <div class="container">
            <div class="logo">
                <div class="logo-mark">LP</div>
                <div class="logo-text">
                    Luedke Plumbing
                    <small>Tampa, Florida</small>
                </div>
            </div>
            <a href="tel:8135239534" class="header-phone">
                <svg viewBox="0 0 24 24"><path d="M6.62 10.79c1.44 2.83 3.76 5.14 6.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24 1.12.37 2.33.57 3.57.57.55 0 1 .45 1 1V20c0 .55-.45 1-1 1-9.39 0-17-7.61-17-17 0-.55.45-1 1-1h3.5c.55 0 1 .45 1 1 0 1.25.2 2.45.57 3.57.11.35.03.74-.25 1.02l-2.2 2.2z"/></svg>
                (813) 523-9534
            </a>
        </div>
    </header>

    <!-- Hero -->
    <section class="hero">
        <div class="hero-content-wrap">
            <div class="container">
                <div class="hero-content">
                    <h1>Tampa's <span>Trusted Plumber</span> Since 2014</h1>
                    <p class="hero-text">From emergency repairs to whole-home repiping. Licensed, bonded, insured — and ready when you need us.</p>
                    <div class="hero-cta">
                        <a href="tel:8135239534" class="btn btn-copper">Call Now</a>
                        <a href="#services" class="btn btn-outline-dark">Our Services</a>
                    </div>
                    <div class="hero-stats">
                        <div class="stat-item">
                            <div class="stat-num">10+</div>
                            <div class="stat-label">Years Experience</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-num">121</div>
                            <div class="stat-label">Projects Done</div>
                        </div>
                        <div class="stat-item">
                            <div class="stat-num">Top 8%</div>
                            <div class="stat-label">FL Contractors</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="hero-image"></div>
    </section>

    <!-- Photo Band -->
    <div class="photo-band">
        <img src="https://images.unsplash.com/photo-1621905252507-b35492cc74b4?w=500&q=80" alt="Pipe work">
        <img src="https://images.unsplash.com/photo-1585704032915-c3400ca199e7?w=500&q=80" alt="Plumber at work">
        <img src="https://images.unsplash.com/photo-1558618666-fcd25c85cd64?w=500&q=80" alt="Copper pipes">
        <img src="https://images.unsplash.com/photo-1613323593608-abc90fec84ff?w=500&q=80" alt="Water heater">
    </div>

    <!-- Credentials Bar -->
    <div class="cred-bar">
        <div class="container">
            <div class="cred-item">
                <svg viewBox="0 0 24 24"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z"/></svg>
                State Licensed
            </div>
            <div class="cred-item">
                <svg viewBox="0 0 24 24"><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/></svg>
                Bonded & Insured
            </div>
            <div class="cred-item">
                <svg viewBox="0 0 24 24"><path d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"/></svg>
                REALTOR Recommended
            </div>
            <div class="cred-item">
                <svg viewBox="0 0 24 24"><path d="M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zM12 20c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8zm.5-13H11v6l5.25 3.15.75-1.23-4.5-2.67z"/></svg>
                Same-Day Service
            </div>
        </div>
    </div>

    <!-- Services -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-label">What We Do</div>
            <h2 class="section-title">Full-Service Plumbing</h2>
        </div>
        <div class="container">
            <div class="services-list">
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M17.66 8L12 2.35 6.34 8A8.02 8.02 0 0 0 4 13.64c0 2 .78 4.11 2.34 5.67a7.99 7.99 0 0 0 11.32 0c1.56-1.56 2.34-3.67 2.34-5.67S19.22 9.56 17.66 8z"/></svg>
                    </div>
                    <div>
                        <h3>Leak Detection & Repair</h3>
                        <p>Find and fix hidden leaks before they cause costly damage. Advanced equipment for fast results.</p>
                    </div>
                </div>
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M19 9h-4V3H9v6H5l7 7 7-7zM5 18v2h14v-2H5z"/></svg>
                    </div>
                    <div>
                        <h3>Whole Home Repiping</h3>
                        <p>Replace aging galvanized or polybutylene pipes with modern, reliable systems built to last.</p>
                    </div>
                </div>
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M12 3L2 12h3v8h6v-6h2v6h6v-8h3L12 3z"/></svg>
                    </div>
                    <div>
                        <h3>Water Heater Services</h3>
                        <p>Tank, tankless, gas, electric — installation, repair, and maintenance for all types.</p>
                    </div>
                </div>
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M19 14v3c0 .55-.45 1-1 1h-1v-4h2M6 14v4H5c-.55 0-1-.45-1-1v-3h2m7-11L4 10h3v7h4v-5h2v5h4v-7h3L13 3z"/></svg>
                    </div>
                    <div>
                        <h3>Drain Cleaning</h3>
                        <p>Clear stubborn clogs fast. Professional-grade equipment for the toughest blockages.</p>
                    </div>
                </div>
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M8 2c-1.1 0-2 .9-2 2v2H4v14h16V6h-2V4c0-1.1-.9-2-2-2H8zm8 2v2H8V4h8zM6 8h12v10H6V8z"/></svg>
                    </div>
                    <div>
                        <h3>Fixture Installation</h3>
                        <p>Faucets, toilets, sinks, showers — installed right the first time, every time.</p>
                    </div>
                </div>
                <div class="service-item">
                    <div class="service-icon">
                        <svg viewBox="0 0 24 24"><path d="M11.99 2C6.47 2 2 6.48 2 12s4.47 10 9.99 10C17.52 22 22 17.52 22 12S17.52 2 11.99 2zM12 20c-4.42 0-8-3.58-8-8s3.58-8 8-8 8 3.58 8 8-3.58 8-8 8zm.5-13H11v6l5.25 3.15.75-1.23-4.5-2.67z"/></svg>
                    </div>
                    <div>
                        <h3>Emergency Repairs</h3>
                        <p>Plumbing emergencies don't wait. Neither do we. Fast response when you need it most.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Split -->
    <section class="about-split">
        <div class="about-image"></div>
        <div class="about-content">
            <div class="section-label">About</div>
            <h2 class="section-title">Honest Work, Fair Prices</h2>
            <p>After 14 years with one of Tampa's largest plumbing companies, I started Luedke Plumbing to give homeowners what they deserve — skilled work, straight talk, and fair prices. No upsells, no surprises.</p>
            <ul class="about-list">
                <li>
                    <svg viewBox="0 0 24 24"><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/></svg>
                    Upfront pricing — know your cost before work starts
                </li>
                <li>
                    <svg viewBox="0 0 24 24"><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/></svg>
                    $3.2 million+ in completed projects
                </li>
                <li>
                    <svg viewBox="0 0 24 24"><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/></svg>
                    Top 8% of Florida contractors (BuildZoom)
                </li>
                <li>
                    <svg viewBox="0 0 24 24"><path d="M9 16.17L4.83 12l-1.42 1.41L9 19 21 7l-1.41-1.41z"/></svg>
                    Owner-operated — George is on every job
                </li>
            </ul>
        </div>
    </section>

    <!-- CTA -->
    <section class="cta" id="contact">
        <div class="container">
            <h2>Get a Free Estimate</h2>
            <p>No obligation, no pressure — just honest advice from a licensed pro.</p>
            <a href="tel:8135239534" class="cta-phone">
                <svg viewBox="0 0 24 24"><path d="M6.62 10.79c1.44 2.83 3.76 5.14 6.59 6.59l2.2-2.2c.27-.27.67-.36 1.02-.24 1.12.37 2.33.57 3.57.57.55 0 1 .45 1 1V20c0 .55-.45 1-1 1-9.39 0-17-7.61-17-17 0-.55.45-1 1-1h3.5c.55 0 1 .45 1 1 0 1.25.2 2.45.57 3.57.11.35.03.74-.25 1.02l-2.2 2.2z"/></svg>
                (813) 523-9534
            </a>
            <div class="cta-buttons">
                <a href="tel:8135239534" class="btn btn-dark">Call Now</a>
                <a href="mailto:beardboy76@gmail.com" class="btn btn-ghost">Email Us</a>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <div class="footer-brand">
                    <div class="logo-text">Luedke Plumbing</div>
                    <p>State licensed, bonded, and insured plumbing contractor serving Tampa and surrounding areas since 2014.</p>
                </div>
                <div>
                    <h4 class="footer-heading">Services</h4>
                    <ul class="footer-links">
                        <li><a href="#services">Leak Detection</a></li>
                        <li><a href="#services">Repiping</a></li>
                        <li><a href="#services">Water Heaters</a></li>
                        <li><a href="#services">Drain Cleaning</a></li>
                        <li><a href="#services">Emergency Repairs</a></li>
                    </ul>
                </div>
                <div>
                    <h4 class="footer-heading">Contact</h4>
                    <ul class="footer-links">
                        <li><a href="tel:8135239534">(813) 523-9534</a></li>
                        <li><a href="mailto:beardboy76@gmail.com">beardboy76@gmail.com</a></li>
                        <li>1310 Hilton Place</li>
                        <li>Tampa, FL 33604</li>
                    </ul>
                </div>
            </div>
            <div class="footer-bottom">
                <span>© 2024 Luedke Plumbing LLC</span>
                <span>Florida License #CFC1429117</span>
            </div>
        </div>
    </footer>
</body>
</html>#
