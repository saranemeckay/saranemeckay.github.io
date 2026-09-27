<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sara Rose Nemeckay | Marketing & SFX Portfolio</title>
    <style>
        /* Rutgers Scarlet & Modern Color Palette */
        :root {
            --rutgers-red: #CC0033;
            --rutgers-red-hover: #A00028;
            --dark-gray: #1E2022;
            --medium-gray: #4A4A4A;
            --light-bg: #F4F6F8;
            --card-bg: #FFFFFF;
            --border-color: #E2E8F0;
            --accent-glow: rgba(204, 0, 51, 0.08);
            --shadow-sm: 0 2px 4px rgba(0,0,0,0.04);
            --shadow-md: 0 10px 25px -5px rgba(0, 0, 0, 0.08), 0 8px 10px -6px rgba(0, 0, 0, 0.04);
        }

        * {
            box-sizing: border-box;
        }

        body {
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: var(--light-bg);
            margin: 0;
            padding: 0;
            -webkit-font-smoothing: antialiased;
        }

        /* Navigation Header */
        header {
            background-color: #ffffff;
            border-bottom: 3px solid var(--rutgers-red);
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: var(--shadow-sm);
        }

        .nav-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1.1rem 2rem;
        }

        .logo {
            font-size: 1.25rem;
            font-weight: 800;
            color: var(--rutgers-red);
            text-decoration: none;
            letter-spacing: -0.3px;
        }

        .logo span {
            color: var(--dark-gray);
            font-weight: 400;
        }

        nav {
            display: flex;
            align-items: center;
            gap: 1.2rem;
        }

        nav a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 600;
            font-size: 0.95rem;
            transition: color 0.2s ease;
        }

        nav a:hover {
            color: var(--rutgers-red);
        }

        .nav-resume-btn {
            background-color: var(--rutgers-red);
            color: #ffffff !important;
            padding: 0.4rem 0.8rem;
            border-radius: 6px;
            font-size: 0.85rem;
            transition: background-color 0.2s ease;
        }

        .nav-resume-btn:hover {
            background-color: var(--rutgers-red-hover);
        }

        /* Main Container */
        .container {
            max-width: 1000px;
            margin: 2.5rem auto;
            padding: 0 1.5rem;
        }

        section {
            background: var(--card-bg);
            padding: 2.5rem;
            margin-bottom: 2rem;
            border-radius: 12px;
            border: 1px solid var(--border-color);
            box-shadow: var(--shadow-sm);
            transition: box-shadow 0.3s ease;
        }

        h1 {
            font-size: 1.8rem;
            color: var(--rutgers-red);
            margin-top: 0;
            margin-bottom: 1rem;
            font-weight: 800;
            letter-spacing: -0.5px;
        }

        h2 {
            font-size: 1.4rem;
            color: var(--dark-gray);
            margin-top: 0;
            margin-bottom: 1.5rem;
            border-bottom: 2px solid var(--border-color);
            padding-bottom: 0.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        h2::before {
            content: "";
            display: inline-block;
            width: 8px;
            height: 18px;
            background-color: var(--rutgers-red);
            border-radius: 2px;
        }

        /* Personal Statement Banner */
        .personal-statement {
            font-size: 1.2rem;
            font-weight: 400;
            line-height: 1.85;
            color: #2D3748;
            background-color: var(--accent-glow);
            border-left: 5px solid var(--rutgers-red);
            padding: 1.5rem 1.8rem;
            border-radius: 0 8px 8px 0;
            margin: 0;
        }

        /* Dual Resume Cards Layout */
        .resumes-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .resume-card {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            background-color: var(--light-bg);
            border: 1px solid var(--border-color);
            padding: 1.8rem;
            border-radius: 10px;
        }

        .resume-info h3 {
            margin: 0 0 0.5rem 0;
            color: var(--dark-gray);
            font-size: 1.15rem;
        }

        .resume-info p {
            margin: 0 0 1.2rem 0;
            color: #4A5568;
            font-size: 0.95rem;
            line-height: 1.5;
        }

        .btn-primary {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            background-color: var(--rutgers-red);
            color: #ffffff;
            padding: 0.75rem 1.2rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 700;
            font-size: 0.9rem;
            transition: background-color 0.2s ease, transform 0.2s ease;
            box-shadow: var(--shadow-sm);
            width: fit-content;
        }

        .btn-primary:hover {
            background-color: var(--rutgers-red-hover);
            transform: translateY(-1px);
        }

        .btn-secondary {
            background-color: var(--dark-gray);
        }

        .btn-secondary:hover {
            background-color: #000000;
        }

        /* Skills Section */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(270px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .skill-category {
            background-color: var(--light-bg);
            padding: 1.5rem;
            border-radius: 8px;
            border: 1px solid var(--border-color);
            transition: transform 0.2s ease, box-shadow 0.2s ease;
        }

        .skill-category:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-sm);
        }

        .skill-category h3 {
            margin-top: 0;
            font-size: 1.05rem;
            color: var(--rutgers-red);
            border-bottom: 2px solid var(--rutgers-red);
            padding-bottom: 0.4rem;
            display: inline-block;
            margin-bottom: 1rem;
        }

        .skill-category ul {
            list-style-type: none;
            padding-left: 0;
            margin: 0;
        }

        .skill-category li {
            padding: 0.4rem 0;
            color: #4A5568;
            font-size: 0.95rem;
            display: flex;
            align-items: center;
        }

        .skill-category li::before {
            content: "•";
            color: var(--rutgers-red);
            font-weight: bold;
            display: inline-block;
            width: 1rem;
            font-size: 1.2rem;
        }

        /* Projects Section */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .project-card {
            border: 1px solid var(--border-color);
            border-radius: 10px;
            padding: 1.8rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            background-color: var(--card-bg);
            transition: all 0.3s ease;
            position: relative;
            top: 0;
        }

        .project-card:hover {
            top: -4px;
            box-shadow: var(--shadow-md);
            border-color: #CBD5E0;
        }

        .badge {
            display: inline-block;
            background-color: var(--accent-glow);
            color: var(--rutgers-red);
            font-size: 0.75rem;
            font-weight: 700;
            padding: 0.25rem 0.6rem;
            border-radius: 20px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 0.8rem;
            width: fit-content;
        }

        .project-card h3 {
            margin-top: 0;
            margin-bottom: 0.8rem;
            color: var(--dark-gray);
            font-size: 1.15rem;
        }

        .project-card p {
            color: #4A5568;
            font-size: 0.95rem;
            line-height: 1.6;
            margin-bottom: 1.2rem;
        }

        .project-link {
            display: inline-flex;
            align-items: center;
            color: var(--rutgers-red);
            text-decoration: none;
            font-weight: 700;
            font-size: 0.9rem;
            transition: color 0.2s;
        }

        .project-link:hover {
            color: var(--rutgers-red-hover);
            text-decoration: underline;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2.5rem 0;
            color: #718096;
            font-size: 0.9rem;
            border-top: 1px solid var(--border-color);
            background-color: #ffffff;
            margin-top: 3rem;
        }

        /* Responsive Design */
        @media (max-width: 650px) {
            .nav-container {
                flex-direction: column;
                gap: 0.8rem;
                padding: 1rem;
            }
            nav {
                flex-wrap: wrap;
                justify-content: center;
            }
            section {
                padding: 1.5rem;
            }
            .personal-statement {
                font-size: 1.05rem;
                padding: 1.2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation Header -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">Sara Rose Nemeckay <span>| RBS Marketing</span></a>
            <nav>
                <a href="#about">About</a>
                <a href="#resumes">Resumes</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
                <a href="Sara_Rose_Nemeckay_Business_Resume.pdf" target="_blank" class="nav-resume-btn">Business Resume</a>
                <a href="Sara_Rose_Nemeckay_Film_Resume.pdf" target="_blank" class="nav-resume-btn">TV/Film Resume</a>
            </nav>
        </div>
    </header>

    <div class="container">

        <!-- About / Personal Statement Section -->
        <section id="about">
            <h1>Rutgers Business School Portfolio</h1>
            <p class="personal-statement">
                While studying marketing at Rutgers Business School, I am also a full-time makeup and special effects artist for TV and Film, looking forward to seamlessly combining the world of business with my world of creativity.
            </p>
        </section>

        <!-- Dedicated Dual Resume Section -->
        <section id="resumes">
            <h2>Professional Resumes</h2>
            <div class="resumes-grid">
                
                <!-- Business Resume Card -->
                <div class="resume-card">
                    <div class="resume-info">
                        <h3>Business & Marketing Resume</h3>
                        <p>Focuses on Rutgers marketing degree coursework, retail management, inventory analytics, and administrative skill sets.</p>
                    </div>
                    <a href="Sara_Rose_Nemeckay_Business_Resume.pdf" target="_blank" class="btn-primary">
                        📄 Open Business Resume &rarr;
                    </a>
                </div>

                <!-- TV/Film Resume Card -->
                <div class="resume-card">
                    <div class="resume-info">
                        <h3>TV & Film SFX Resume</h3>
                        <p>Highlights feature film credits (<em>Men of Granite</em>, <em>Words From the Oven</em>), music videos, theatrical productions, and SFX shop work at Gotham FX Lab.</p>
                    </div>
                    <a href="Sara_Rose_Nemeckay_Film_Resume.pdf" target="_blank" class="btn-primary btn-secondary">
                        🎬 Open TV/Film Resume &rarr;
                    </a>
                </div>

            </div>
        </section>

        <!-- Skills Showcase Section -->
        <section id="skills">
            <h2>Skills & Capabilities</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Marketing & Management</h3>
                    <ul>
                        <li>Inventory Analytics & Demand Tracking</li>
                        <li>Retail Merchandise Planning</li>
                        <li>Team Supervision & Leadership</li>
                        <li>Customer Experience & Event Execution</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Technical & Digital</h3>
                    <ul>
                        <li>HTML Web Development</li>
                        <li>ZBrush & Nomad Sculpting (Certified)</li>
                        <li>Loss Prevention Analysis</li>
                        <li>Sanitation & Organization Certified</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Creative & Film Production</h3>
                    <ul>
                        <li>Special Effects (SFX) Makeup & Design</li>
                        <li>Single & Dual Action Airbrushing</li>
                        <li>Character Continuity & FX Rigging</li>
                        <li>Gotham FX Lab & Cinema Makeup Track</li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- Featured Projects / Experience Section -->
        <section id="projects">
            <h2>Featured Projects & Leadership</h2>
            <div class="projects-grid">
                
                <!-- Project 1 -->
                <div class="project-card">
                    <div>
                        <span class="badge">Business Operations</span>
                        <h3>Retail Operations & Demand Forecasting</h3>
                        <p>
                            Managed store operations at Dunellen Bagel, supervising staff, executing standard opening/closing protocols, and auditing weekly inventory based on historical sales trends and demand forecasting.
                        </p>
                    </div>
                    <a href="Sara_Rose_Nemeckay_Business_Resume.pdf" target="_blank" class="project-link">View Business Resume &rarr;</a>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <div>
                        <span class="badge">Merchandising</span>
                        <h3>Visual Merchandising & Event Execution</h3>
                        <p>
                            Trained retail associates on weekly planogram store resets at Ulta Beauty, tracked inventory discrepancies for loss prevention, and executed promotional in-store event launches to drive brand engagement.
                        </p>
                    </div>
                    <a href="Sara_Rose_Nemeckay_Business_Resume.pdf" target="_blank" class="project-link">View Business Resume &rarr;</a>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <div>
                        <span class="badge">Film Production</span>
                        <h3>Film Production FX & Character Continuity</h3>
                        <p>
                            Key Makeup Artist and SFX Artist on feature films (<em>Men of Granite</em>, <em>Mercury 1938</em>, <em>The Translator</em>) managing character continuity, blood rigs, and prosthetic applications.
                        </p>
                    </div>
                    <a href="Sara_Rose_Nemeckay_Film_Resume.pdf" target="_blank" class="project-link">View TV/Film Resume &rarr;</a>
                </div>

            </div>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Sara Rose Nemeckay | Rutgers Business School & Film Industry Portfolio</p>
    </footer>

</body>
</html>
