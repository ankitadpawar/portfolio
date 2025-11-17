# portfolio
this web site all about my brief introduction with the tech touch to showcase my self to world ...
<!-- Portfolio Website for Ankit Adpawar (Data Analyst) -->
<!-- Theme: Clean + Modern Premium Hybrid (A + C + D) -->

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Ankit Adpawar | Data Analyst Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        html {
            scroll-behavior: smooth;
        }
         body {
            background: #0f0f0f;
            color: #d0d0d0;
            overflow-x: hidden;
        }
        a {
            text-decoration: none;
        }
        /* HEADER / NAVBAR */
        header {
            width: 100%;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(10, 26, 47, 0.95);
            position: sticky;
            top: 0;
            z-index: 100;
            backdrop-filter: blur(10px);
        }
        header h1 {
            color: #4c8dff;
            font-size: 24px;
            font-weight: 700;
            letter-spacing: 0.5px;
        }
        .nav-links {
            display: flex;
            align-items: center;
            gap: 24px;
        }
        .nav-links a {
            color: #d0d0d0;
            font-size: 14px;
            font-weight: 400;
        }
        .nav-links a:hover {
            color: #4c8dff;
        }
        .nav-btn {
            padding: 8px 18px;
            border-radius: 999px;
            border: 1px solid #4c8dff;
            color: #ffffff;
            font-size: 13px;
        }
        .nav-btn:hover {
            background: #4c8dff;
        }
        .menu-toggle {
            display: none;
            flex-direction: column;
            gap: 4px;
            cursor: pointer;
        }
        .menu-toggle span {
            width: 20px;
            height: 2px;
            background: #ffffff;
        }
        /* LAYOUT */
        section {
            padding: 80px 8%;
            max-width: 1200px;
            margin: 0 auto;
        }
        .section-title {
            font-size: 28px;
            margin-bottom: 16px;
            color: #4c8dff;
            font-weight: 600;
        }
        .section-subtitle {
            font-size: 14px;
            color: #9a9a9a;
            margin-bottom: 32px;
        }
        /* HERO */
        .hero {
            min-height: 80vh;
            display: grid;
            grid-template-columns: minmax(0, 2.2fr) minmax(0, 1.4fr);
            gap: 40px;
            align-items: center;
            background: radial-gradient(circle at top left, #1c3c5c 0, #0f0f0f 55%);
        }
        .hero-heading {
            font-size: 40px;
            font-weight: 700;
            color: #ffffff;
            line-height: 1.25;
            margin-bottom: 18px;
        }
        .hero-highlight {
            color: #00d4ff;
        }
        .hero-tag {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            padding: 4px 10px;
            border-radius: 999px;
            background: rgba(12, 27, 52, 0.9);
            border: 1px solid rgba(76, 141, 255, 0.4);
            font-size: 11px;
            color: #c0d7ff;
            margin-bottom: 12px;
        }
        .hero-tag span {
            width: 6px;
            height: 6px;
            border-radius: 50%;
            background: #00d4ff;
        }
        .hero-text {
            font-size: 15px;
            color: #c4c4c4;
            max-width: 520px;
            margin-bottom: 24px;
        }
        .hero-meta {
            display: flex;
            flex-wrap: wrap;
            gap: 16px;
            margin-top: 12px;
            font-size: 12px;
            color: #a7a7a7;
        }
        .hero-actions {
            display: flex;
            flex-wrap: wrap;
            gap: 14px;
            margin-top: 18px;
        }
        .btn-primary {
            padding: 10px 22px;
            border-radius: 999px;
            border: none;
            background: linear-gradient(135deg, #4c8dff, #00d4ff);
            color: #ffffff;
            font-size: 14px;
            cursor: pointer;
        }
        .btn-primary:hover {
            opacity: 0.92;
        }
        .btn-ghost {
            padding: 10px 22px;
            border-radius: 999px;
            border: 1px solid #3a3a3a;
            background: transparent;
            color: #d0d0d0;
            font-size: 14px;
            cursor: pointer;
        }
        .btn-ghost:hover {
            border-color: #4c8dff;
        }
        .hero-right {
            justify-self: center;
        }
        .hero-card {
            width: 100%;
            max-width: 340px;
            border-radius: 24px;
            padding: 22px 20px;
            background: radial-gradient(circle at top, #1f2937 0, #050608 70%);
            border: 1px solid rgba(76, 141, 255, 0.4);
            box-shadow: 0 18px 45px rgba(0, 0, 0, 0.7);
        }
        .hero-card-title {
            font-size: 16px;
            font-weight: 600;
            margin-bottom: 4px;
        }
        .hero-card-sub {
            font-size: 12px;
            color: #9a9a9a;
            margin-bottom: 16px;
        }
        .hero-metrics {
            display: grid;
            grid-template-columns: repeat(2, minmax(0, 1fr));
            gap: 14px;
            margin-bottom: 16px;
        }
        .metric-box {
            padding: 10px;
            border-radius: 12px;
            background: rgba(12, 20, 35, 0.9);
            border: 1px solid rgba(76, 141, 255, 0.25);
        }
        .metric-label {
            font-size: 11px;
            color: #9babc5;
            margin-bottom: 4px;
        }
        .metric-value {
            font-size: 16px;
            font-weight: 600;
            color: #ffffff;
        }
        .hero-tools {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 8px;
        }
        .tool-pill {
            padding: 4px 10px;
            border-radius: 999px;
            background: rgba(15, 23, 42, 0.9);
            border: 1px solid rgba(148, 163, 184, 0.4);
            font-size: 11px;
            color: #cbd5f5;
        }
        /* ABOUT */
        .about-grid {
            display: grid;
            grid-template-columns: minmax(0, 1.7fr) minmax(0, 1.3fr);
            gap: 32px;
        }
        .about-text {
            font-size: 14px;
            color: #c4c4c4;
            line-height: 1.7;
        }
        .about-list {
            margin-top: 18px;
            display: grid;
            gap: 8px;
            font-size: 13px;
            color: #b8b8b8;
        }
        .tag-row {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 10px;
        }
        .tag {
            padding: 4px 10px;
            border-radius: 999px;
            background: #141414;
            font-size: 11px;
            color: #d0d0d0;
            border: 1px solid #252525;
        }
        .about-card {
            border-radius: 18px;
            background: #111827;
            border: 1px solid #1f2937;
            padding: 18px 18px 16px;
        }
        .about-card-title {
            font-size: 13px;
            color: #9ca3af;
            margin-bottom: 6px;
        }
        .about-card-value {
            font-size: 22px;
            font-weight: 600;
            color: #e5e7eb;
        }
        .about-card-note {
            font-size: 11px;
            color: #9ca3af;
            margin-top: 4px;
        }
        /* EXPERIENCE */
        .timeline {
            display: grid;
            gap: 18px;
        }
        .exp-item {
            padding: 16px 18px;
            border-radius: 14px;
            background: #111111;
            border: 1px solid #1f1f1f;
        }
        .exp-role {
            font-size: 15px;
            font-weight: 600;
            color: #ffffff;
        }
        .exp-meta {
            font-size: 12px;
            color: #9a9a9a;
            margin: 2px 0 10px;
        }
        .exp-bullets {
            font-size: 13px;
            color: #c4c4c4;
            list-style: none;
        }
        .exp-bullets li {
            margin-bottom: 4px;
        }
        /* SKILLS */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 18px;
        }
        .skills-card {
            padding: 16px 18px;
            border-radius: 16px;
            background: #101010;
            border: 1px solid #1f1f1f;
        }
        .skills-card h3 {
            font-size: 15px;
            margin-bottom: 8px;
            color: #ffffff;
        }
        .skills-list {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }
        .skill-pill {
            padding: 4px 9px;
            border-radius: 999px;
            border: 1px solid #262626;
            font-size: 11px;
            color: #d0d0d0;
        }
        /* PROJECTS */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 22px;
        }
        .project-card {
            background: #111111;
            padding: 18px 18px 16px;
            border-radius: 16px;
            border: 1px solid #1f1f1f;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
       }
        .project-label {
            font-size: 11px;
            color: #9ca3af;
            margin-bottom: 4px;
        }
        .project-title {
            font-size: 17px;
            font-weight: 600;
            color: #ffffff;
            margin-bottom: 6px;
        }
        .project-desc {
            font-size: 13px;
            color: #c4c4c4;
            margin-bottom: 10px;
        }
        .project-meta {
            font-size: 11px;
            color: #9a9a9a;
            margin-bottom: 10px;
        }
        .project-actions {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 6px;
        }
        .btn-link {
            font-size: 11px;
            padding: 6px 11px;
            border-radius: 999px;
            border: 1px solid #2a2a2a;
            color: #e5e5e5;
            background: #151515;
        }
        .btn-link:hover {
            border-color: #4c8dff;
        }
        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 6px;
            margin-top: 8px;
        }
        .tech-tag {
            font-size: 10px;
            padding: 3px 8px;
            border-radius: 999px;
            background: #1a1a1a;
            color: #cbd5f5;
            border: 1px solid #262626;
        }
        /* GITHUB SECTION */
        .github-box {
            border-radius: 18px;
            background: #020617;
            border: 1px solid #1f2937;
            padding: 22px 20px;
            display: flex;
            flex-wrap: wrap;
            gap: 18px;
            align-items: center;
            justify-content: space-between;
        }
        .github-box h3 {
            font-size: 18px;
            color: #e5e7eb;
        }
        .github-box p {
            font-size: 13px;
            color: #9ca3af;
            max-width: 420px;
        }
        /* CONTACT */
        .contact-grid {
            display: grid;
            grid-template-columns: minmax(0, 1.4fr) minmax(0, 1.6fr);
            gap: 28px;
        }
        .contact-card {
            padding: 18px 18px 16px;
            border-radius: 16px;
            background: #020617;
            border: 1px solid #1f2937;
        }
        .contact-card h3 {
            font-size: 16px;
            margin-bottom: 6px;
        }
        .contact-line {
            font-size: 13px;
            color: #9ca3af;
            margin-bottom: 4px;
        }
        form {
            display: grid;
            gap: 10px;
        }
        label {
            font-size: 12px;
            color: #9ca3af;
        }
        input, textarea {
            width: 100%;
            padding: 8px 10px;
            border-radius: 8px;
            border: 1px solid #262626;
            background: #020617;
            color: #e5e7eb;
            font-size: 13px;
        }
        textarea {
            min-height: 90px;
            resize: vertical;
        }
        input:focus, textarea:focus {
            outline: none;
            border-color: #4c8dff;
        }
        /* FOOTER */
        footer {
            text-align: center;
            padding: 30px 8% 40px;
            background: #020617;
            color: #9ca3af;
            font-size: 12px;
            border-top: 1px solid #111827;
        }
        footer a {
            color: #cbd5f5;
        }
        footer a:hover {
            color: #4c8dff;
        }
        /* RESPONSIVE */
        @media (max-width: 900px) {
            .hero {
                grid-template-columns: minmax(0, 1fr);
                padding-top: 90px;
            }
            .hero-right {
                order: -1;
            }
            .hero-heading {
                font-size: 30px;
            }
            .about-grid,
            .contact-grid {
                grid-template-columns: minmax(0, 1fr);
            }
        }
        @media (max-width: 768px) {
            header {
                padding-inline: 6%;
            }
            .nav-links {
                position: absolute;
                top: 60px;
                right: 6%;
                background: #020617;
                border-radius: 14px;
                border: 1px solid #1f2937;
                padding: 10px 16px;
                flex-direction: column;
                align-items: flex-start;
                gap: 12px;
                display: none;
            }
            .nav-links.show {
                display: flex;
            }
            .menu-toggle {
                display: flex;
            }
            .nav-btn {
                width: 100%;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Ankit Adpawar</h1>
        <nav class="nav-links" id="navLinks">
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#experience">Experience</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
            <a href="ANKIT_ADPAWAR_CV.pdf" class="nav-btn" download>Download CV</a>
        </nav>
        <div class="menu-toggle" id="menuToggle">
            <span></span>
            <span></span>
            <span></span>
        </div>
    </header>
    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="hero-left">
            <div class="hero-tag">
                <span></span>
                <p>Data Analyst • Python • SQL • BI Dashboards</p>
            </div>
            <h2 class="hero-heading">
                Turning <span class="hero-highlight">messy data</span> into clear, actionable
                business insights.
            </h2>
            <p class="hero-text">
                I’m a Data Analyst with a focus on transforming raw datasets into dashboards,
                models, and metrics that actually support decision-making. Skilled in Python,
                SQL, Tableau, and Power BI with hands-on experience in EDA, forecasting,
                and churn analysis.
            </p>
            <div class="hero-actions">
                <button class="btn-primary" onclick="document.getElementById('projects').scrollIntoView()">
                    View My Projects
                </button>
                <button class="btn-ghost" onclick="window.location.href='mailto:ankitadpawar898@gmail.com'">
                    Email Me
                </button>
            </div>
            <div class="hero-meta">
                <span>📍 Nagpur, India</span>
                <span>🎓 B.Tech CSE (Data Science)</span>
                <span>📊 Data Analyst Intern @ Coreline Solutions</span>
            </div>
        </div>
        <div class="hero-right">
            <div class="hero-card">
                <p class="hero-card-title">Snapshot</p>
                <p class="hero-card-sub">What I bring to a data team</p>
                <div class="hero-metrics">
                    <div class="metric-box">
                        <p class="metric-label">Tools</p>
                        <p class="metric-value">Python, SQL, BI</p>
                    </div>
                    <div class="metric-box">
                        <p class="metric-label">Focus</p>
                        <p class="metric-value">EDA & Dashboards</p>
                    </div>
                    <div class="metric-box">
                        <p class="metric-label">Strength</p>
                        <p class="metric-value">Problem Solving</p>
                    </div>
                    <div class="metric-box">
                        <p class="metric-label">Experience</p>
                        <p class="metric-value">Internship + Projects</p>
                    </div>
                </div>
                <p style="font-size: 12px; color: #9ca3af; margin-bottom: 6px;">Comfortable with:</p>
                <div class="hero-tools">
                    <span class="tool-pill">Python (Pandas, NumPy)</span>
                    <span class="tool-pill">SQL (Joins, CTEs)</span>
                    <span class="tool-pill">Power BI</span>
                    <span class="tool-pill">Tableau</span>
                    <span class="tool-pill">Excel</span>
                </div>
            </div>
        </div>
    </section>
    <!-- ABOUT SECTION -->
    <section id="about">
        <h2 class="section-title">About</h2>
        <p class="section-subtitle">Who I am beyond the buzzwords.</p>
        <div class="about-grid">
            <div>
                <p class="about-text">
                    I’m currently pursuing a B.Tech in Computer Science (Data Science) at
                    JD College of Engineering & Management, Nagpur. I enjoy working on
                    end-to-end analytics workflows: from cleaning and exploring data,
                    to building dashboards and simple predictive models that tell a clear story.
                </p>
                <div class="about-list">
                    <span>• Strong foundation in statistics, EDA, and business-focused insights.</span>
                    <span>• Experience building dashboards for sales, e-commerce, and COVID-19 trends.</span>
                    <span>• Comfortable collaborating in agile teams and communicating results clearly.</span>
                </div>
                <div class="tag-row">
                    <span class="tag">B.Tech CSE (Data Science) — 2022–2026</span>
                    <span class="tag">GPA: 8.50 / 10</span>
                </div>
            </div>
            <div>
                <div class="about-card">
                    <p class="about-card-title">Education</p>
                    <p class="about-card-value">Data Science Major</p>
                    <p class="about-card-note">JD College of Engineering & Management, Nagpur</p>
                </div>
                <div style="height: 10px;"></div>
                <div class="about-card">
                    <p class="about-card-title">Languages</p>
                    <p class="about-card-value">EN • HI • MR • TE</p>
                    <p class="about-card-note">Comfortable working in multilingual teams.</p>
                </div>
            </div>
        </div>
    </section>
    <!-- EXPERIENCE SECTION -->
    <section id="experience">
        <h2 class="section-title">Experience</h2>
        <p class="section-subtitle">Practical work I’ve done so far.</p>
        <div class="timeline">
            <div class="exp-item">
                <p class="exp-role">Data Analyst Intern</p>
                <p class="exp-meta">Coreline Solutions Pvt Ltd, Pune • Jul 2025 – Sep 2025</p>
                <ul class="exp-bullets">
                    <li>Performed data cleaning and exploratory analysis on business datasets to support reporting and decision-making.</li>
                    <li>Helped automate recurring reporting workflows using Python, reducing manual effort for the team.</li>
                    <li>Contributed to predictive modelling experiments for basic business forecasting tasks.</li>
                </ul>
            </div>
        </div>
    </section>
    <!-- SKILLS SECTION -->
    <section id="skills">
        <h2 class="section-title">Skills</h2>
        <p class="section-subtitle">Tools and techniques I actually use.</p>
        <div class="skills-grid">
            <div class="skills-card">
                <h3>Programming & Databases</h3>
                <div class="skills-list">
                    <span class="skill-pill">Python</span>
                    <span class="skill-pill">SQL</span>
                    <span class="skill-pill">R (Basics)</span>
                    <span class="skill-pill">Pandas</span>
                    <span class="skill-pill">NumPy</span>
                    <span class="skill-pill">Jupyter Notebook</span>
                </div>
            </div>
            <div class="skills-card">
                <h3>Data Visualization & BI</h3>
                <div class="skills-list">
                    <span class="skill-pill">Tableau</span>
                    <span class="skill-pill">Power BI</span>
                    <span class="skill-pill">Excel</span>
                    <span class="skill-pill">Google Sheets</span>
                    <span class="skill-pill">Dashboard Design</span>
                </div>
            </div>
            <div class="skills-card">
                <h3>Soft Skills</h3>
                <div class="skills-list">
                    <span class="skill-pill">Problem Solving</span>
                    <span class="skill-pill">Teamwork</span>
                    <span class="skill-pill">Agile Ways of Working</span>
                    <span class="skill-pill">Communication</span>
                </div>
            </div>
        </div>
    </section>
    <!-- PROJECTS SECTION -->
    <section id="projects">
        <h2 class="section-title">Projects</h2>
        <p class="section-subtitle">Case studies that show how I work with data.</p>
        <div class="projects-grid">
            <div class="project-card">
                <p class="project-label">Machine Learning</p>
                <h3 class="project-title">Customer Churn Prediction</h3>
                <p class="project-desc">
                    Built a classification model to identify customers likely to churn based on
                    usage patterns, demographics, and account features. Included EDA,
                    feature engineering, and model comparison.
                </p>
                <p class="project-meta">Goal: Help the business focus retention efforts on high-risk customers.</p>
                <div class="tech-tags">
                    <span class="tech-tag">Python</span>
                    <span class="tech-tag">Pandas</span>
                    <span class="tech-tag">Scikit-learn</span>
                    <span class="tech-tag">Matplotlib</span>
                </div>
                <div class="project-actions">
                    <a class="btn-link" href="https://github.com/ankitadpawar/customer-churn-prediction" target="_blank">View Code</a>
                    <a class="btn-link" href="#" target="_blank">Read Case Study</a>
                </div>
            </div>
            <div class="project-card">
                <p class="project-label">Business Analytics</p>
                <h3 class="project-title">Sales Data Analysis</h3>
                <p class="project-desc">
                    Explored sales data to understand revenue trends, seasonality, and product
                    performance. Used Python & Excel to create summary tables and visuals.
                </p>
                <p class="project-meta">Outcome: Identified top-performing segments and time periods for targeted campaigns.</p>
                <div class="tech-tags">
                    <span class="tech-tag">Python</span>
                    <span class="tech-tag">Excel</span>
                    <span class="tech-tag">EDA</span>
                </div>
                <div class="project-actions">
                    <a class="btn-link" href="https://github.com/ankitadpawar/sales-data-analysis" target="_blank">View Code</a>
                    <a class="btn-link" href="#" target="_blank">View Report</a>
                </div>
            </div>
            <div class="project-card">
                <p class="project-label">BI Dashboard</p>
                <h3 class="project-title">E-commerce Business Dashboard</h3>
                <p class="project-desc">
                    Designed an interactive Power BI dashboard to track orders, revenue,
                    customer segments, and product performance for an e-commerce scenario.
                </p>
                <p class="project-meta">Focus: Clean layout, key KPIs, and drill-down views for decision-makers.</p>
                <div class="tech-tags">
                    <span class="tech-tag">Power BI</span>
                    <span class="tech-tag">DAX</span>
                    <span class="tech-tag">Data Modelling</span>
                </div>
                <div class="project-actions">
                    <a class="btn-link" href="#" target="_blank">View Dashboard</a>
                    <a class="btn-link" href="https://github.com/ankitadpawar/ecommerce-dashboard" target="_blank">View Files</a>
                </div>
            </div>
            <div class="project-card">
                <p class="project-label">Data Exploration</p>
                <h3 class="project-title">COVID-19 Data Analysis</h3>
                <p class="project-desc">
                    Analyzed COVID-19 case data to understand trends across regions,
                    growth rates, and the impact of different phases.
                </p>
                <p class="project-meta">Built visuals in Python and Tableau to make trends easy to understand.</p>
                <div class="tech-tags">
                    <span class="tech-tag">Python</span>
                    <span class="tech-tag">Tableau</span>
                    <span class="tech-tag">Time-series</span>
                </div>
                <div class="project-actions">
                    <a class="btn-link" href="https://github.com/ankitadpawar/covid19-data-analysis" target="_blank">View Code</a>
                </div>
            </div>
        </div>
    </section>
    <!-- GITHUB SECTION -->
    <section>
        <div class="github-box">
            <div>
                <h3>See more on GitHub</h3>
                <p>
                    I keep all my active notebooks, experiments, and small analysis scripts on GitHub.
                    You can explore how I structure code, document work, and iterate on ideas.
                </p>
            </div>
            <button class="btn-primary" onclick="window.open('https://github.com/ankitadpawar', '_blank')">
                Open GitHub Profile
            </button>
        </div>
    </section>
    <!-- CONTACT SECTION -->
    <section id="contact">
        <h2 class="section-title">Let’s Connect</h2>
        <p class="section-subtitle">Open to internships, entry-level data roles, and project collaborations.</p>
        <div class="contact-grid">
            <div class="contact-card">
                <h3>Contact Details</h3>
                <p class="contact-line">📧 Email: <a href="mailto:ankitadpawar898@gmail.com">ankitadpawar898@gmail.com</a></p>
                <p class="contact-line">📱 Phone: +91-8080705756</p>
                <p class="contact-line">🔗 LinkedIn: <a href="https://linkedin.com/in/ankit-adpawar-078332238" target="_blank">linkedin.com/in/ankit-adpawar-078332238</a></p>
                <p class="contact-line">💻 GitHub: <a href="https://github.com/ankitadpawar" target="_blank">github.com/ankitadpawar</a></p>
                <p class="contact-line" style="margin-top: 8px;">If you’d like to discuss an opportunity or project, feel free to mail me directly or use the form.</p>
            </div>
            <div class="contact-card">
                <h3>Quick Message</h3>
                <form onsubmit="event.preventDefault(); alert('This form is a front-end demo. Use email to contact directly.');">
                    <div>
                        <label for="name">Your Name</label>
                        <input id="name" type="text" placeholder="Enter your name" required />
                    </div>
                    <div>
                        <label for="email">Your Email</label>
                        <input id="email" type="email" placeholder="Enter your email" required />
                    </div>
                    <div>
                        <label for="message">Message</label>
                        <textarea id="message" placeholder="Write a short message" required></textarea>
                    </div>
                    <button class="btn-primary" type="submit">Send Message</button>
                </form>
            </div>
        </div>
    </section>
    <footer>
        <p>© <span id="year"></span> Ankit Adpawar · Data Analyst Portfolio · Built with HTML, CSS & a focus on clean data stories.</p>
    </footer>
    <script>
        // mobile nav toggle
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');
        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('show');
        });
        // dynamic year
        document.getElementById('year').textContent = new Date().getFullYear();
    </script>
</body>
</html>
