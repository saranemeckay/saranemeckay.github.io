# saranemeckay.github.io
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sara Rose Nemeckay | Marketing Portfolio</title>
    <style>
        /* Rutgers Scarlet Brand Colors */
        :root {
            --rutgers-red: #CC0033;
            --dark-gray: #222222;
            --light-bg: #F8F9FA;
            --border-color: #E0E0E0;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: var(--dark-gray);
            background-color: var(--light-bg);
            margin: 0;
            padding: 0;
        }

        /* Navigation Bar */
        header {
            background-color: #ffffff;
            border-bottom: 3px solid var(--rutgers-red);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.2rem;
            font-weight: bold;
            color: var(--rutgers-red);
            text-decoration: none;
        }

        nav a {
            margin-left: 1.5rem;
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 600;
            transition: color 0.2s;
        }

        nav a:hover {
            color: var(--rutgers-red);
        }

        /* Main Container */
        .container {
            max-width: 1000px;
            margin: 2rem auto;
            padding: 0 2rem;
        }

        section {
            background: #ffffff;
            padding: 2rem;
            margin-bottom: 2rem;
            border-radius: 8px;
            border: 1px solid var(--border-color);
        }

        h1, h2 {
            color: var(--rutgers-red);
            margin-top: 0;
        }

        /* Personal Statement Section */
        .personal-statement {
            font-size: 1.2rem;
            font-weight: 500;
            line-height: 1.8;
            color: #333333;
            border-left: 4px solid var(--rutgers-red);
            padding-left: 1rem;
            margin: 1rem 0 0 0;
        }

        /* Skills Showcase Section */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 1rem;
        }

        .skill-category {
            background-color: var(--light-bg);
            padding: 1.2rem;
            border-radius: 6px;
            border: 1px solid #EAEAEA;
        }

        .skill-category h3 {
            margin-top: 0;
            font-size: 1rem;
            color: var(--dark-gray);
            border-bottom: 2px solid var(--rutgers-red);
            padding-bottom: 0.3rem;
            display: inline-block;
        }

        .skill-category ul {
            list-style-type: none;
            padding-left: 0;
            margin-bottom: 0;
        }

        .skill-category li {
            padding: 0.3rem 0;
            color: #555555;
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
            border-radius: 6px;
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            background-color: #ffffff;
        }

        .project-card h3 {
            margin-top: 0;
            color: var(--dark-gray);
        }

        .project-card p {
            color: #555555;
            font-size: 0.95rem;
        }

        .project-link {
            display: inline-block;
            margin-top: 1rem;
            color: var(--rutgers-red);
            text-decoration: none;
            font-weight: bold;
        }

        .project-link:hover {
            text-decoration: underline;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 2rem 0;
            color: #666666;
            font-size: 0.9rem;
        }

        /* Mobile Responsive Adjustments */
        @media (max-width: 600px) {
            .nav-container {
                flex-direction: column;
                gap: 0.5rem;
            }
            nav a {
                margin: 0 0.5rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation Header -->
    <header>
        <div class="nav-container">
            <a href="#" class="logo">Sara Rose Nemeckay | RBS Marketing</a>
            <nav>
                <a href="#about">About</a>
                <a href="#skills">Skills</a>
                <a href="#projects">Projects</a>
            </nav>
        </div>
    </header>

    <div class="container">

        <!-- Header / Personal Statement Section -->
        <section id="about">
            <h1>Rutgers Business School Portfolio</h1>
            <!-- One-Sentence Personal Statement tailored to marketing + creative production/retail management -->
            <p class="personal-statement">
                I am a Rutgers Business School Marketing major combining hands-on retail management experience, inventory analytics, and creative media production background to drive impactful brand marketing and operational execution.
            </p>
        </section>

        <!-- Skills Showcase Section -->
        <section id="skills">
            <h2>Skills & Capabilities</h2>
            <div class="skills-grid">
                <div class="skill-category">
                    <h3>Marketing & Management</h3>
                    <ul>
                        <li>Inventory Analytics & Demand Tracking</li>
                        <li>Retail Merchandise Planning & Planograms</li>
                        <li>Team Supervision & Employee Training</li>
                        <li>Customer Experience & Event Execution</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Technical & Software Skills</h3>
                    <ul>
                        <li>HTML Web Development</li>
                        <li>ZBrush Digital Sculpting (Certified)</li>
                        <li>Loss Prevention Analysis</li>
                        <li>Sanitation & Organization (Certified)</li>
                    </ul>
                </div>
                <div class="skill-category">
                    <h3>Creative & Production</h3>
                    <ul>
                        <li>Special Effects (SFX) Makeup & Design</li>
                        <li>Airbrushing (Single & Dual Action)</li>
                        <li>Character Makeup Continuity & Rigging</li>
                        <li>Event Internship & Industry Production</li>
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
                        <h3>Retail Operations & Inventory Strategy</h3>
                        <p>
                            Managed business operations at Dunellen Bagel, overseeing staff training, opening/closing procedures, and weekly inventory monitoring based on historical sales trends and demand forecasting.
                        </p>
                    </div>
                    <a href="https://github.com" target="_blank" class="project-link">View Management Details &rarr;</a>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <div>
                        <h3>Visual Merchandising & Planograms</h3>
                        <p>
                            Led store resets and new-hire training at Ulta Beauty, auditing inventory discrepancies for loss prevention and executing promotional in-store event launches to drive brand engagement.
                        </p>
                    </div>
                    <a href="https://github.com" target="_blank" class="project-link">View Retail Operations Overview &rarr;</a>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <div>
                        <h3>Film Production FX & Continuity</h3>
                        <p>
                            Served as Key Makeup Artist for "The Translator" (premiered at Warner Bros. Studios via New York Film Academy), directing SFX character makeup continuity and managing specialized FX rigs.
                        </p>
                    </div>
                    <a href="https://github.com" target="_blank" class="project-link">View Production Details &rarr;</a>
                </div>

            </div>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Sara Rose Nemeckay | Rutgers Business School, Major in Marketing</p>
    </footer>

</body>
</html>
