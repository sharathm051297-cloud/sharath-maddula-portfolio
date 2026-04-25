<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>Sharath Maddula | Portfolio</title>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet"/>
    <style>
        :root {
            --primary: #007acc;
            --secondary: #004f7c;
            --accent: #00ff96;
            --bg: #f8f9fa;
            --text: #333;
            --white: #ffffff;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; scroll-behavior: smooth; }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--bg);
            color: var(--text);
            line-height: 1.6;
        }

        /* 🌌 Animated Engineering Background */
        body::before {
            content: "";
            position: fixed;
            width: 100%; height: 100%;
            background: radial-gradient(circle, rgba(0,122,204,0.05) 1px, transparent 1px);
            background-size: 30px 30px;
            z-index: -1;
        }

        /* Navigation */
        nav {
            position: sticky; top: 0;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            display: flex; justify-content: center;
            padding: 1rem;
            box-shadow: 0 2px 15px rgba(0,0,0,0.05);
            z-index: 1000;
        }

        nav a {
            margin: 0 1.5rem;
            text-decoration: none;
            color: var(--secondary);
            font-weight: 600;
            transition: 0.3s;
        }

        nav a:hover { color: var(--primary); }

        /* Header */
        header {
            text-align: center;
            padding: 5rem 1rem 3rem;
            background: linear-gradient(180deg, #fff 0%, var(--bg) 100%);
        }

        header h1 { font-size: 3rem; color: var(--secondary); margin-bottom: 0.5rem; }
        .subtitle { font-size: 1.2rem; color: var(--primary); font-weight: 400; margin-bottom: 1.5rem; }

        .contact-bar {
            display: flex; justify-content: center; gap: 20px; flex-wrap: wrap;
            font-size: 0.9rem;
        }

        /* Sections */
        section {
            max-width: 1000px;
            margin: 3rem auto;
            padding: 2rem;
            background: var(--white);
            border-radius: 16px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.05);
        }

        h2 {
            font-size: 1.8rem;
            color: var(--secondary);
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        h2::after {
            content: "";
            height: 3px;
            flex-grow: 1;
            background: linear-gradient(90deg, var(--primary), transparent);
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }

        .skill-category h3 { font-size: 1rem; color: var(--primary); margin-bottom: 0.5rem; }
        .skill-tag {
            display: inline-block;
            background: #eef2f7;
            padding: 4px 12px;
            border-radius: 20px;
            margin: 3px;
            font-size: 0.85rem;
        }

        /* Experience & Projects */
        .item { margin-bottom: 2rem; }
        .item-header { display: flex; justify-content: space-between; align-items: baseline; }
        .item-header h3 { color: var(--secondary); }
        .date { font-size: 0.9rem; color: #777; }

        /* Image Gallery */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 15px;
            margin-top: 1.5rem;
        }

        .gallery-item {
            border-radius: 8px;
            overflow: hidden;
            border: 1px solid #ddd;
            transition: transform 0.3s;
        }

        .gallery-item:hover { transform: scale(1.03); }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            display: block;
        }

        .img-caption {
            padding: 8px;
            font-size: 0.8rem;
            text-align: center;
            background: #f1f1f1;
        }

        @media (max-width: 768px) {
            header h1 { font-size: 2.2rem; }
            section { margin: 1rem; padding: 1.5rem; }
        }
    </style>
</head>
<body>

<nav>
    <a href="#summary">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#experience">Experience</a>
</nav>

<header>
    <h1>Sharath Maddula</h1>
    <p class="subtitle">Manufacturing Design Engineer</p>
    <div class="contact-bar">
        <span>📍 Texas, USA</span>
        <span>📞 832-966-6447</span>
        <span>✉️ sharathmaddula12@gmail.com</span>
        <span>🔗 <a href="https://linkedin.com/in/maddulasharath" target="_blank" style="color: inherit;">LinkedIn</a></span>
    </div>
</header>

<section id="summary">
    <h2>Professional Summary</h2>
    <p>
        Manufacturing Engineer with 5+ years of experience in automotive design, specializing in drivetrain systems and Electronic Control Units (ECUs). 
        Expert in leveraging <strong>MATLAB</strong> and <strong>Excel</strong> for data-driven optimizations. Proficient in applying <strong>DFM/DFA</strong> 
        principles to streamline production and implementing Failure Modes and Effects Analysis (FMEA) to ensure product durability.
    </p>
</section>

<section id="skills">
    <h2>Technical Expertise</h2>
    <div class="skills-grid">
        <div class="skill-category">
            <h3>CAD & Design</h3>
            <span class="skill-tag">Siemens NX</span>
            <span class="skill-tag">SolidWorks</span>
            <span class="skill-tag">CATIA V5</span>
            <span class="skill-tag">Creo</span>
            <span class="skill-tag">AutoCAD</span>
        </div>
        <div class="skill-category">
            <h3>Simulation & Analysis</h3>
            <span class="skill-tag">ANSYS Fluent</span>
            <span class="skill-tag">FEA/CFD</span>
            <span class="skill-tag">MATLAB</span>
            <span class="skill-tag">FMEA</span>
        </div>
        <div class="skill-category">
            <h3>Manufacturing</h3>
            <span class="skill-tag">DFM/DFA</span>
            <span class="skill-tag">GD&T</span>
            <span class="skill-tag">Value Stream Mapping</span>
            <span class="skill-tag">Tooling Design</span>
        </div>
    </div>
</section>

<section id="projects">
    <h2>Key Projects</h2>
    <div class="item">
        <div class="item-header">
            <h3>Next-Generation ECU Design & Optimization</h3>
            <span class="date">Automotive Platform</span>
        </div>
        <p>Designed a compact, thermally efficient ECU enclosure, optimizing performance for real-world operating conditions.</p>
        <ul>
            <li>Reduced unit size by 15% while improving thermal dissipation by 20%.</li>
            <li>Utilized <strong>Siemens NX</strong> and <strong>ANSYS</strong> for structural and thermal validation.</li>
            <li>Implemented cost reduction strategies, saving $1.2M in annual production costs.</li>
        </ul>
        
        <div class="gallery">
            <div class="gallery-item">
                <img src="WhatsApp Image 2026-04-24 at 20.22.42.jpeg" alt="Project Part">
                <div class="img-caption">CAD Part Modeling</div>
            </div>
            <div class="gallery-item">
                <img src="WhatsApp Image 2026-04-24 at 20.22.43.jpeg" alt="Technical Drawing">
                <div class="img-caption">Drafting & GD&T</div>
            </div>
            <div class="gallery-item">
                <img src="WhatsApp Image 2026-04-24 at 20.22.43 (1).jpeg" alt="Design Analysis">
                <div class="img-caption">Design Analysis</div>
            </div>
        </div>
    </div>
</section>

<section id="experience">
    <h2>Professional Experience</h2>
    <div class="item">
        <div class="item-header">
            <h3>Manufacturing Engineer</h3>
            <span class="date">2024 — Present</span>
        </div>
        <p><em>GE Healthcare / Automotive Projects</em></p>
        <ul>
            <li>Leading end-to-end mechanical design and production scaling.</li>
            <li>Collaborating with cross-functional teams to define constraints like 50G shock loads.</li>
        </ul>
    </div>

    <div class="item">
        <div class="item-header">
            <h3>Mechanical Design Engineer</h3>
            <span class="date">2019 — 2023</span>
        </div>
        <p><em>Ashok Leyland / JBM Group</em></p>
        <ul>
            <li>Optimized sheet metal nesting, reducing material waste by 12%.</li>
            <li>Conducted formability studies and trim line analysis for precision tooling.</li>
        </ul>
    </div>
</section>

<section id="education">
    <h2>Education</h2>
    <div class="item">
        <div class="item-header">
            <h3>Master of Science in Engineering Management</h3>
            <span class="date">Houston, TX</span>
        </div>
        <p>University of Houston-Clear Lake</p>
    </div>
    <div class="item">
        <div class="item-header">
            <h3>Bachelor of Engineering in Mechanical Engineering</h3>
            <span class="date">Hyderabad, India</span>
        </div>
        <p>Malla Reddy College of Engineering & Technology</p>
    </div>
</section>

</body>
</html>
