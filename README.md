
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Eric John N. Cruz - Portfolio</title>
  <meta name="description" content="Portfolio of Eric John N. Cruz. Junior Electrical Engineer, Digital Marketing Specialist, General Virtual Assistant.">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Poppins:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#141a20;
      --card:#151b24;
      --text:#e6edf3;
      --muted:#9da7b3;
      --accent:#7c5cff;
      --accent2:#22d3ee;
      --chip:#232a33;
      --ok:#10b981;
      --warn:#f59e0b;
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:var(--bg);color:var(--text);font-family:Poppins,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif;line-height:1.6}
    a{color:var(--accent);text-decoration:none}
    a:hover{text-decoration:underline}
    .container{max-width:1200px;margin:0 auto;padding:24px}
    header{position:sticky;top:0;z-index:50;background:rgba(13,17,23,.7);backdrop-filter:saturate(160%) blur(6px);border-bottom:1px solid #222}
    nav{display:flex;align-items:center;justify-content:space-between;gap:16px}
    .brand{display:flex;align-items:center;gap:10px;font-weight:700;font-family:Montserrat,system-ui}
    .brand .dot{width:10px;height:10px;background:linear-gradient(135deg,var(--accent),var(--accent2));border-radius:50%}
    .navlinks{display:flex;gap:18px;flex-wrap:wrap}
    .navlinks a {display:inline-flex; align-items:center; line-height:1; font-weight:600; color:var(--text); opacity: 9;}
    .navlinks a:hover{opacity:1}
    .cta{background:linear-gradient(135deg,var(--accent),var(--accent2));color:#000;font-weight:700;padding:10px 22px;border-radius:999px;line-height:1.2; display: inline-flex; align-items: center;}
    .hero{display:grid;grid-template-columns:1fr;gap:28px;align-items:center;padding:28px 0}  
    .hero-card{display:grid; grid-template-columns:230px 1fr; gap:18px; align-items:start;}
    .profile-picture{grid-row:1 / span 2;} @media (max-width:640px){.hero-card{grid-template-columns:1fr;} .profile-picture{grid-row:auto;}} h1{margin:0 0 10px;font-size: clamp(28px, 4vw, 42px);font-family:Montserrat,system-ui;font-weight:800;letter-spacing:.4px;background:linear-gradient(90deg,var(--text),#b6c2ce);-webkit-background-clip:text;background-clip:text;-webkit-text-fill-color:transparent}
    .tagline{color:var(--muted);font-size:clamp(14px,1.8vw,16px)}
    .quick{margin-top:16px;display:flex;flex-wrap:wrap;gap:10px}
    .chip{display:inline-flex;align-items:center;gap:8px;background:var(--chip);border:1px solid #262e38;padding:8px 12px;border-radius:999px;font-size:13px}
    .stats{display:grid;grid-template-columns:repeat(3,1fr);gap:12px;margin-top:18px}
    .stat{background:var(--card);border:1px solid #262e38;border-radius:14px;padding:14px;text-align:center}
    .stat .big{font-family:Montserrat,system-ui;font-weight:800;font-size:20px}
    .muted{color:var(--muted)}
    /* Sections */
    section{padding:28px 0}
    .section-title{display:flex;align-items:center;justify-content:space-between;margin-bottom:14px}
    .section-title h2{margin:0;font-family:Montserrat,system-ui;font-weight:800;font-size:clamp(20px,2.8vw,26px)}
    /* Cards grid */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
    @media (max-width: 980px){.hero{grid-template-columns:1fr}.grid{grid-template-columns:repeat(2,1fr)}}
    @media (max-width: 640px){.navlinks{display:none}.grid{grid-template-columns:1fr}}
    .card{background:var(--card);border:1px solid #262e38;border-radius:16px;padding:16px;display:flex;flex-direction:column;gap:10px;box-shadow:0 10px 24px rgba(0,0,0,.18)}
    .card h3{margin:0;font-family:Montserrat,system-ui;font-weight:700;font-size:18px}
    .pill{display:inline-block;background:#1f2430;border:1px solid #2a3240;border-radius:10px;padding:4px 8px;font-size:12px;color:var(--muted);margin-right:6px}
    .list{margin:0 0 0 16px;padding:0}
    .list li{margin:6px 0}
    .skills-wrap{display:flex;flex-wrap:wrap;gap:10px}
    .skill{background:#1b2130;border:1px solid #2a3240;border-radius:10px;padding:8px 10px;font-size:13px}
    .footer{border-top:1px solid #20262f;margin-top:28px;padding:24px 0;color:var(--muted);text-align:center}
    /* Buttons */
    .btn{display:inline-flex;align-items:center;gap:8px;border:1px solid #2a3240;background:#151a23;border-radius:12px;padding:10px 14px;color:var(--text);font-weight:600}
    .btn:hover{border-color:#3a4354}
    .btn.small{padding:8px 10px;font-size:13px}
    /* Contact icons */
    .icons{display:flex;gap:12px;flex-wrap:wrap}
    .icon{width:42px;height:42px;border-radius:12px;display:inline-flex;align-items:center;justify-content:center;border:1px solid #2a3240;background:#151a23}
    /* Badge colors */
    .ok{background:rgba(16,185,129,.12);border-color:rgba(16,185,129,.35);color:#86efac}
    .warn{background:rgba(245,158,11,.12);border-color:rgba(245,158,11,.35);color:#fde68a}
    .accent{background:rgba(124,92,255,.14);border-color:rgba(124,92,255,.4);color:#c7b8ff}
    .profile-picture {width: 230px; height: 230px; border-radius: 50%; object-fit: cover; margin-bottom: 16px; border: 4px solid #2a3240;box-shadow: 0 6px 18px rgba(0,0,0,.45);} 
    .skills-wrap {display: flex; flex-wrap: wrap; gap: 10px;}

/* HERO as a proper card section */
.hero { padding: 0; }
.hero-card-wrap { background: var(--card); border:1px solid #262e38; border-radius:16px; padding:18px; box-shadow:0 10px 24px rgba(0,0,0,.18); }

/* Two-column layout with a left profile column */
.hero-card { display:grid; grid-template-columns:240px 1fr; gap:18px; align-items:start; }

/* Left column stacks photo, chips, and CTAs */
.profile-col { display:flex; flex-direction:column; gap:12px; }

/* Chip row for the four requested chips */
.quick { display:flex; flex-wrap:wrap; gap:10px; }
.chip { display:inline-flex; align-items:center; gap:8px; background:var(--chip); border:1px solid #262e38; padding:8px 12px; border-radius:999px; font-size:13px; line-height:1; }

/* Buttons under the chips, full width on mobile */
.hero-actions { display:flex; gap:10px; flex-wrap:wrap; }
.hero-actions .btn { flex:0 0 auto; }

/* Responsive */
@media (max-width: 820px){
  .hero-card { grid-template-columns:1fr; }
  .profile-col { order:1; }
}

/* tighten the hero */
.hero { padding: 0; }
.hero-card-wrap { background: var(--card); border:1px solid #262e38; border-radius:16px; padding:18px; box-shadow:0 10px 24px rgba(0,0,0,.18); }
.hero-card { display:grid; grid-template-columns:260px 1fr; gap:22px; align-items:center; }

/* right column content width + rows */
.hero-content { max-width: 84ch; }
.meta-row { display:flex; flex-wrap:wrap; gap:10px 12px; margin:10px 0 8px; }
.meta-row .chip { line-height:1; }
.meta-row .btn { padding:8px 12px; border-radius:999px; }

/* make the photo visually centered */
.profile-col { display:flex; justify-content:center; }
.profile-picture{ width:240px;height:240px;border-radius:50%;object-fit:cover;margin:0; }

/* responsive */
@media (max-width: 860px){
  .hero-card { grid-template-columns:1fr; align-items:start; }
  .profile-col { order:1; }
}

.skill {
  display: inline-flex;
  align-items: center;
  gap: 6px;
  padding: 6px 10px;
  background: #232a33;
  border-radius: 6px;
  margin: 5px;
  font-size: 13px;
}

.skill .logo {
  width: 20px;   
  height: auto;
  object-fit: contain;
}

/* Dropdown */
.dropdown {
  position: relative;
  display: inline-block;
}

.dropdown .dropbtn {
  cursor: pointer;
  font-weight: 600;
  color: var(--text);
  padding: 8px 0;
}

.dropdown-content {
  display: none;
  position: absolute;
  background: var(--card);
  border: 1px solid #262e38;
  border-radius: 8px;
  min-width: 180px;
  box-shadow: 0 8px 16px rgba(0,0,0,.2);
  z-index: 100;
}

.dropdown-content a {
  display: block;
  padding: 10px 14px;
  color: var(--text);
  text-decoration: none;
  font-weight: 500;
}

.dropdown-content a:hover {
  background: var(--chip);
}

.dropdown:hover .dropdown-content {
  display: block;
}

/* Fix dropdown alignment */
.dropdown {
  position: relative;
  display: inline-flex; /* inline-flex instead of inline-block */
  align-items: center;  /* vertically align with other nav items */
}

.dropdown .dropbtn {
  display: inline-flex;
  align-items: center;
  gap: 4px;
  font-weight: 600;
  color: var(--text);
  line-height: 1;
  padding: 0; /* remove extra padding */
}

.dropdown-content {
  display: none;
  position: absolute;
  top: 100%; /* align directly under "Projects" */
  left: 0;
  background: var(--card);
  border: 1px solid #262e38;
  border-radius: 8px;
  min-width: 180px;
  box-shadow: 0 8px 16px rgba(0,0,0,.2);
  z-index: 100;
}

.dropdown-content a {
  display: block;
  padding: 10px 14px;
  color: var(--text);
  font-weight: 500;
}

.dropdown-content a:hover {
  background: var(--chip);
}

.dropdown:hover .dropdown-content {
  display: block;
}

.card h3 a::after {
  content: "↗"; /* Unicode arrow pointing NE */
  margin-left: 6px;
  font-size: 14px;
  color: var(--accent); /* matches your theme */
}

</style>
</head>

<script>
  function scrollToHeading(id) {
    const headerOffset = document.querySelector('header').offsetHeight;
    const section = document.querySelector(id);
    if (!section) return;

    // Look for h2 inside the section, otherwise use section itself
    const target = section.querySelector('h2') || section;
    const y = target.getBoundingClientRect().top + window.scrollY - headerOffset - 10; // adjust -10 if needed
    window.scrollTo({ top: y, behavior: 'smooth' });
  }

  // Handle clicks on nav links
  document.querySelectorAll('nav .navlinks a[href^="#"]').forEach(link => {
    link.addEventListener('click', e => {
      const id = link.getAttribute('href');
      if (id && id.length > 1) {
        e.preventDefault();
        scrollToHeading(id);
        history.replaceState(null, '', id);
      }
    });
  });

  // Handle page load with hash
  window.addEventListener('load', () => {
    if (location.hash) scrollToHeading(location.hash);
  });

  // Handle hash changes
  window.addEventListener('hashchange', () => {
    if (location.hash) scrollToHeading(location.hash);
  });
</script>

<body>
  <header>
    <div class="container">
      <nav>
        <div class="brand"><span class="dot"></span> <span>Eric John N. Cruz</span></div>
<div class="navlinks">
  <a href="#about">About</a>
  <a href="#skills">Services</a>
  <a href="#experience">Experience</a>

  <div class="dropdown">
    <a href="#projects" class="dropbtn">Projects ▾</a>
    <div class="dropdown-content">
      <a href="Engineering.html">Engineering</a>
      <a href="Marketing.html">Marketing</a>
      <a href="Programming.html">Programming</a>
    </div>
  </div>

  <a href="#tools">Tools</a>
  <a href="#education">Education</a>
  <a href="#certs">Licenses</a>
  <a href="#contact" class="cta">Contact</a>
</div>
      </nav>
    </div>
  </header>

  <main class="container">
    <!-- HERO -->
<!-- ABOUT / HERO -->
<section id="about" class="hero">
  <div class="hero-card-wrap">
    <div class="hero-card">
      <!-- LEFT: photo only -->
      <div class="profile-col">
        <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/Profile.jpg" alt="Eric John N. Cruz" class="profile-picture">
      </div>
      <div class="hero-content">
        <h1>Engineer, Entrepreneur, & Operations Support</h1>
        <div class="meta-row">
        </div>
        <p class="tagline">
          Hi, I’m Eric. I help entrepreneurs and businesses by creating smoother operations, stronger online visibility, and organized workflows that keep projects moving forward. My aim is to lighten the load for teams so they can focus on growth while knowing the details are handled with care.
          Whether it’s guiding a project to completion or boosting digital presence through SEO, content, and email campaigns, I focus on delivering results that save time, reduce stress, and open new opportunities. My role is to be a trusted partner who helps businesses work smarter and achieve lasting success.
        </p>
      </div>
    </div>
  </div>
</section>
    <!-- SKILLS -->
    <section id="skills">
      <div class="section-title"><h2>Services</h2></div>
      <div class="skills-wrap">
        <span class="skill">AutoCAD 2D Electrical Design</span>
        <span class="skill">BOM and Takeoffs</span>
        <span class="skill">Data Entry & Management</span>
        <span class="skill">Email Campaigns, Automation & A/B Testing</span>
        <span class="skill">Graphic Design & Branded Content Creation</span>
        <span class="skill">Google Analytics (Traffic Analysis, Conversion Tracking, Reporting)</span>
        <span class="skill">Image Editing & Marketing Graphics</span>
        <span class="skill">Keyword Research & Competitor Analysis</span>
        <span class="skill">MATLAB Simulink Power Systems Simulation</span>
        <span class="skill">Project Coordination and Management</span>
        <span class="skill">Protective Devices Testing</span>
        <span class="skill">Python Basic Automation and Coding</span>
        <span class="skill">QA/QC Reviews</span>
        <span class="skill">SEO (On-Page, Off-Page, Local, Keyword Strategy)</span>
        <span class="skill">SEO Audits & Site Optimization</span>
        <span class="skill">Task Management</span>
        <span class="skill">Video Editing (Promotional Content, Reels & Ads)</span>
        <span class="skill">Website Management & Customization</span>
      </div>
    </section>

    <!-- EXPERIENCE -->
    <section id="experience">
      <div class="section-title">
        <h2>Experience</h2>
      </div>
      <div class="grid">

        <article class="card">
          <h3>Technical Encoder</h3>
          <span class="pill">Rapid Care Manpower Services</span>
          <div class="muted">Mar 2025 - Jun 2025</div>
          <ul class="list">
            <li>Supported electrical project design and document approvals.</li>
            <li>Logged maintenance activities and updated system records.</li>
            <li>Coordinated with field crews and assisted test planning.</li>
            <li>Prepared preventive maintenance checklists and inventory updates.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Digital Operations Manager</h3>
          <span class="pill">Freelance</span>
          <div class="muted">Feb 2024 - Jul 2025</div>
          <ul class="list">
            <li>Managed citations, backlinks, and press releases to improve visibility.</li>
            <li>Owned email marketing cadence and weekly stats reporting.</li>
            <li>Updated website content and coordinated monthly reviews.</li>
            <li>Handled data entry, report generation, and meeting coordination.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Electrical Engineer</h3>
          <span class="pill">Freelance</span>
          <div class="muted">June 2024 - Present</div>
          <ul class="list">
            <li>Designed and installed building wiring and panel boards.</li>
            <li>Coordinated with contractors and reviewed costs.</li>
            <li>Supervised site work and ensured standards compliance.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Marketing and Sales Specialist</h3>
          <span class="pill">Freelance</span>
          <div class="muted">Feb 2023 - Jan 2024</div>
          <ul class="list">
            <li>Keyword research, content audits, and on-page refinements.</li>
            <li>Link building with high quality citations and PR.</li>
            <li>Lead generation and monthly performance reports.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Trainee Engineer</h3>
          <span class="pill">Office of the Municipal Engineer</span>
          <div class="muted">Jun 2022 - Aug 2022</div>
          <ul class="list">
            <li>Produced CAD drawings, redlines, and as-builts to reduce rework.</li>
            <li>Prepared BOMs and load schedules to streamline procurement.</li>
            <li>Drafted test procedures and acceptance criteria.</li>
            <li>Coordinated stakeholders and tracked dependencies.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Subject Matter Expert</h3>
          <span class="pill">Foundever</span>
          <div class="muted">Apr 2021 - Mar 2023</div>
          <ul class="list">
            <li>Coached agents, monitored quality, and ensured compliance.</li>
            <li>Handled escalations and performance analytics.</li>
            <li>Prepared reports and supported training programs.</li>
          </ul>
        </article>

        <article class="card">
          <h3>CSR Inbound 1</h3>
          <span class="pill">Foundever</span>
          <div class="muted">August 2020 - Mar 2021</div>
          <ul class="list">
            <li>Assisted customers with accounts, orders, refunds, and memberships.</li>
            <li>Troubleshot devices, content, and security issues.</li>
            <li>Supported billing, delivery, gift cards, and general inquiries.</li>
          </ul>
        </article>

        <article class="card">
          <h3>Electrician</h3>
          <span class="pill">AP Cruz Trading and Services</span>
          <div class="muted">Jan 2020 - Mar 2021</div>
          <ul class="list">
            <li>Building Wiring Installation</li>
            <li>System Troubleshooting Installation</li>
            <li>Panel Board Installation</li>
          </ul>
        </article>

        <article class="card">
          <h3>Admin Assistant (OJT)</h3>
          <span class="pill">Palawan Governors Office</span>
          <div class="muted">Jan 2020 - Mar 2021</div>
          <ul class="list">
            <li>Assisted in office management and administrative tasks.</li>
            <li>Supported document preparation and filing systems.</li>
            <li>Coordinated schedules and organized meetings.</li>
          </ul>
        </article>
      </div>
    </section>

    <!-- PROJECTS -->
    <section id="projects">
  <div class="section-title">
    <h2>Projects</h2>
  </div>
  <div class="grid">
    <article class="card">
      <h3><a href="Engineering.html">Engineering</a></h3>
      <div class="muted">Electrical Design and Estimation</div>
      <ul class="list">
        <li>Created SLD and load schedules for a rehabilitation project.</li>
        <li>Applied standards and coordinated field updates.</li>
      </ul>
    </article>

    <article class="card">
      <h3><a href="Marketing.html">Marketing</a></h3>
      <div class="muted">Digital marketing operations</div>
      <ul class="list">
        <li>Managed citations, backlinks, and PR for multiple clients.</li>
        <li>Drafted, sent, and reported on weekly email campaigns.</li>
      </ul>
    </article>

    <article class="card">
      <h3><a href="Programming.html">Programming</a></h3>
      <div class="muted">Automation</div>
      <div class="muted">Web design & Development</div>
      <ul class="list">
        <li>Built and customized WordPress websites with pages, forms, and media integration.</li>
        <li>Applied HTML and CSS to create clen layouts and improve design styling.</li>
      </ul>
    </article>
  </div>
</section>

        <!-- TOOLS -->
    <section id="tools">
          <div class="section-title"><h2>Tools</h2></div>
          <div class="skills-wrap">
            <span class="skill">Adobe Dreamweaver
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/dreamweaver.png" alt="Adobe Dreamweaver" class="logo">
            </span>
            <span class="skill">Adobe Photoshop
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/photoshop.png" alt="Adobe Photoshop" class="logo">
            </span>
            <span class="skill">Adobe Premiere
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/premiere.png" alt="Premiere" class="logo">
            </span>
            <span class="skill">AutoCAD
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/autocad.png" alt="AutoCAD" class="logo">
            </span>
            <span class="skill">Brevo
              <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/brevo.png" alt="Brevo" class="logo">
            </span>
            <span class="skill">Canva
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/Canva.png" alt="Canva" class="logo">
            </span>
            <span class="skill">ClickUp
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/clickup.png" alt="ClickUp" class="logo">
            </span>
            <span class="skill">Google Analytics
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/google-analytics.png" alt="Google Analytics" class="logo">
            </span>
            <span class="skill">Google Workspace
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/google-workspace.png" alt="Google Workspace" class="logo">
            </span>
            <span class="skill">MATLAB Simulink
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/matlab.png" alt="MATLAB Simulink" class="logo">
            </span>
            <span class="skill">Microsoft 365
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/microsoft-365.png" alt="Microsoft 365" class="logo">
            </span>
            <span class="skill">Microsoft Studio Code
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/microsoft-studio-code.png" alt="Microsoft Studio Code" class="logo">
            </span>
            <span class="skill">Python
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/python.png" alt="Python" class="logo">
            </span>
            <span class="skill">Ubersuggest
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/ubersuggest.webp" alt="Ubersuggest" class="logo">
            </span>
            <span class="skill">Vegas Pro
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/vegas-pro.png" alt="Vegas Pro" class="logo">
            </span>
            <span class="skill">WordPress
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/wordpress.png" alt="WordPress" class="logo">
            </span>
            <span class="skill">Woorank
            <img src="https://raw.githubusercontent.com/engineericjohncruz/portfolio/refs/heads/main/woorank.png" alt="Woorank" class="logo">
            </span>
          </div>
    </section>

    <!-- EDUCATION -->
    <section id="education">
      <div class="section-title"><h2>Education</h2></div>
      <div class="grid">
        <article class="card">
          <h3>BS in Electrical Engineering</h3>
          <div class="muted">Palawan State University</div>
          <div class="muted">2018 - 2023</div>
        </article>
        <article class="card">
          <h3>General Academics - High School</h3>
          <div class="muted">Seminario de San Jose</div>
          <div class="muted">2012 - 2018</div>
          <div class="muted">With High Honors, Outstanding in Research</div>
        </article>
      </div>
    </section>

    <!-- LICENSES & CERTS -->
    <section id="certs">
      <div class="section-title"><h2>Licenses and Certificates</h2></div>
      <div class="grid">
        <article class="card">
          <h3>Registered Electrical Engineer</h3>
          <div class="muted">Professional Regulation Commission</div>
        </article>
        <article class="card">
          <h3>Safety Officer 2</h3>
          <div class="muted">Mastery Consultancy OPC</div>
        </article>
        <article class="card">
          <h3>NC II - Electrical Installation & Maintenance</h3>
          <div class="muted">TESDA</div>
        </article>
        <article class="card">
          <h3>Preparing Computer-Aided Drawings</h3>
          <div class="muted">TESDA</div>
        </article>
        <article class="card">
          <h3>MATLAB Simulink: Power Systems Simulation</h3>
          <div class="muted">MathWorks</div>
        </article>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact">
      <div class="section-title"><h2>Get in touch</h2></div>
      <div class="card">
        <p class="muted">Available for engineering roles, digital operations, or hybrid positions.</p>
        <div class="icons" style="margin-top:10px">
          <a class="icon" href="mailto:cruzericjohn@gmail.com" title="Email (Gmail)" aria-label="Email (Gmail)">
            <svg width="20" height="20" viewBox="0 0 24 24" role="img" xmlns="http://www.w3.org/2000/svg" aria-hidden="false" focusable="false">
              <!-- white envelope body -->
              <rect x="2" y="5" width="20" height="14" rx="2" fill="#ffffff" />
              <!-- red flap (Gmail-like accent without using the trademark) -->
              <path d="M3 7l9 6 9-6v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V7z" fill="#D44638" />
              <!-- envelope outline -->
              <path d="M3 7l9 6 9-6" fill="none" stroke="#ffffff" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </a>
          <a class="icon" href="https://www.linkedin.com/in/eric-john-cruz-ree/" target="_blank" rel="noopener" title="LinkedIn" aria-label="LinkedIn">
            <svg width="20" height="20" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg" role="img" aria-hidden="false">
              <!-- blue rounded square background -->
              <rect x="0" y="0" width="24" height="24" rx="4" ry="4" fill="#0A66C2"/>
              <!-- white "in" glyph -->
              <path d="M6.8 8.7h2.3V18H6.8V8.7zM7.95 7.3a1.2 1.2 0 1 0 0-2.4 1.2 1.2 0 0 0 0 2.4zM10.9 8.7h2.2v1.3h.03c.31-.6 1.05-1.3 2.28-1.3 2.44 0 2.88 1.6 2.88 3.7V18h-2.3v-4.1c0-1-.02-2.3-1.4-2.3-1.4 0-1.6 1.1-1.6 2.2V18h-2.3V8.7z" fill="#fff"/>
            </svg>
          </a>
        </div>
        <div style="margin-top:12px;display:flex;gap:10px;flex-wrap:wrap">
          <a class="btn small" href="#experience">View experience</a>
          <a class="btn small" href="#projects">See projects</a>
          <a class="btn small" href="https://www.canva.com/design/DAGvmKyqc20/o9_zFYjW8ZK_NO515k3OfQ/view?utm_content=DAGvmKyqc20&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h204abdc4bb">Resume</a>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <div>© 2025 Eric John N. Cruz</div>
      <div style="margin-top:6px">Coded from scratch using HTML, CSS, and JavaScript.</div>
    </div>
  </footer>
</body>

</html>


