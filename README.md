<!DOCTYPE html>
<html lang="en" style="scroll-behavior: smooth;">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Tarek Rajab | Developer & Data Enthusiast</title>
  <meta name="description" content="Portfolio of Tarek Rajab - From Biomedical Science to Full Stack Engineering and Data Science.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap" rel="stylesheet">
  <style>
    *{box-sizing:border-box;margin:0;padding:0}
    html,body{height:100%}
    body{font-family:"Inter",system-ui,-apple-system,BlinkMacSystemFont,sans-serif;background:#020617;color:#e5e7eb;line-height:1.6}
    a{text-decoration:none;color:inherit;transition:color .2s,background .2s,transform .2s}
    img{max-width:100%;display:block}
    ul{list-style:none}
    h1,h2,h3,h4{line-height:1.2}
    .container{max-width:1120px;margin:0 auto;padding:0 1.25rem}
    .section{padding:5rem 0}
    .section-header{text-align:center;margin-bottom:3rem}
    .pill{display:inline-flex;align-items:center;gap:.4rem;border-radius:999px;padding:.25rem .9rem;font-size:.75rem;font-weight:600;text-transform:uppercase;letter-spacing:.08em;background:rgba(15,23,42,.8);color:#38bdf8;border:1px solid rgba(56,189,248,.35);backdrop-filter:blur(16px)}
    .pill-dot{width:.4rem;height:.4rem;border-radius:999px;background:#22c55e}
    .headline{font-size:2.4rem;font-weight:800;color:#f9fafb;margin-top:1rem}
    .headline span{background:linear-gradient(120deg,#22d3ee,#38bdf8,#a855f7);-webkit-background-clip:text;background-clip:text;color:transparent}
    .subhead{margin-top:1rem;font-size:1.05rem;color:#9ca3af;max-width:36rem}
    .btn-row{display:flex;flex-wrap:wrap;gap:.75rem;margin-top:2rem}
    .btn{display:inline-flex;align-items:center;justify-content:center;padding:.75rem 1.6rem;border-radius:.75rem;font-size:.95rem;font-weight:600;border:1px solid transparent;cursor:pointer}
    .btn-primary{background:#38bdf8;color:#020617;box-shadow:0 18px 50px rgba(56,189,248,.25)}
    .btn-primary:hover{transform:translateY(-1px);box-shadow:0 20px 60px rgba(56,189,248,.35)}
    .btn-ghost{background:rgba(15,23,42,.85);border-color:rgba(148,163,184,.4);color:#e5e7eb}
    .btn-ghost:hover{background:rgba(15,23,42,1);border-color:#38bdf8}
    .chip-row{display:flex;flex-wrap:wrap;gap:.5rem;margin-top:1.75rem}
    .chip{font-size:.75rem;padding:.35rem .85rem;border-radius:999px;background:rgba(15,23,42,.9);border:1px solid rgba(148,163,184,.35);color:#9ca3af}
    .chip strong{color:#e5e7eb;font-weight:600}
    .layout-2{display:flex;flex-direction:column;gap:3rem}
    .hero-media{display:flex;justify-content:center;align-items:center}
    .profile-shell{position:relative;width:260px;height:260px;border-radius:999px;background:radial-gradient(circle at 0 0,rgba(56,189,248,.3),transparent 55%),radial-gradient(circle at 100% 100%,rgba(168,85,247,.4),transparent 55%),#020617;padding:4px;box-shadow:0 24px 80px rgba(15,23,42,.9)}
    .profile-inner{width:100%;height:100%;border-radius:inherit;background:radial-gradient(circle at 30% 0%,rgba(248,250,252,.15),transparent 55%),#020617;display:flex;align-items:center;justify-content:center;overflow:hidden;position:relative}
    .profile-inner img{width:100%;height:100%;object-fit:cover}
    .ring{position:absolute;inset:-16px;border-radius:999px;border:1px dashed rgba(148,163,184,.4);opacity:.7}
    .ring:nth-child(2){transform:scale(.88);opacity:.45}
    .floating-card{position:absolute;bottom:-14px;left:50%;transform:translateX(-50%);background:rgba(15,23,42,.92);border-radius:999px;padding:.4rem .9rem;display:flex;align-items:center;gap:.5rem;font-size:.75rem;border:1px solid rgba(148,163,184,.35);backdrop-filter:blur(14px)}
    .dot-green{width:.4rem;height:.4rem;border-radius:999px;background:#22c55e}
    .nav-shell{position:sticky;top:0;z-index:40;background:rgba(2,6,23,.92);backdrop-filter:blur(18px);border-bottom:1px solid rgba(15,23,42,.9)}
    .nav{display:flex;align-items:center;justify-content:space-between;height:4.2rem}
    .nav-brand{font-weight:800;font-size:1.15rem;letter-spacing:.05em;text-transform:uppercase;background:linear-gradient(120deg,#38bdf8,#a855f7);-webkit-background-clip:text;background-clip:text;color:transparent}
    .nav-links{display:none;align-items:center;gap:1.5rem;font-size:.9rem}
    .nav-links a{color:#9ca3af}
    .nav-links a:hover{color:#e5e7eb}
    .nav-cta{padding:.5rem 1.05rem;border-radius:999px;background:#38bdf8;color:#020617;font-weight:600;font-size:.85rem}
    .nav-cta:hover{background:#0ea5e9}
    .nav-toggle{display:inline-flex;align-items:center;justify-content:center;width:2.35rem;height:2.35rem;border-radius:.9rem;border:1px solid rgba(51,65,85,.9);background:rgba(15,23,42,.9);color:#e5e7eb;cursor:pointer}
    .nav-toggle svg{width:1.35rem;height:1.35rem}
    .nav-mobile{display:none;flex-direction:column;padding:.75rem 1.25rem 1.3rem;border-bottom:1px solid rgba(15,23,42,.9);background:rgba(2,6,23,.98);gap:.35rem;font-size:.95rem}
    .nav-mobile a{padding:.5rem 0;color:#9ca3af}
    .nav-mobile a:hover{color:#e5e7eb}
    .nav-mobile .nav-mobile-cta{margin-top:.4rem;padding:.6rem .95rem;border-radius:.9rem;background:#38bdf8;color:#020617;font-weight:600;text-align:center}
    .pill-section-label{font-size:.8rem;font-weight:600;text-transform:uppercase;letter-spacing:.1em;color:#38bdf8;margin-bottom:.25rem}
    .section-title{font-size:1.7rem;font-weight:700;color:#f9fafb}
    .section-lead{margin-top:.75rem;color:#9ca3af;font-size:.98rem;max-width:36rem}
    .card{border-radius:1.25rem;background:radial-gradient(circle at 0 0,rgba(56,189,248,.15),transparent 60%),radial-gradient(circle at 100% 100%,rgba(168,85,247,.12),transparent 60%),#020617;border:1px solid rgba(31,41,55,.9);box-shadow:0 22px 60px rgba(15,23,42,.9);padding:1.8rem}
    .card-muted{background:rgba(15,23,42,.9);border:1px solid rgba(31,41,55,.95)}
    .two-col{display:flex;flex-direction:column;gap:2rem;margin-top:2.2rem}
    .stacked{display:flex;flex-direction:column;gap:1.5rem;margin-top:1.5rem}
    .label{font-size:.8rem;font-weight:600;letter-spacing:.12em;text-transform:uppercase;color:#64748b}
    .text-muted{color:#9ca3af;font-size:.95rem}
    .highlight{color:#f9fafb;font-weight:600}
    .badge-row{display:flex;flex-wrap:wrap;gap:.4rem;margin-top:.7rem}
    .badge{font-size:.7rem;padding:.25rem .65rem;border-radius:999px;background:rgba(15,23,42,1);border:1px solid rgba(51,65,85,1);color:#cbd5f5}
    .badge-accent{border-color:#38bdf8;color:#e0f2fe;background:rgba(8,47,73,.8)}
    .project-shell{display:grid;grid-template-columns:minmax(0,1.2fr) minmax(0,1fr);gap:0;border-radius:1.5rem;overflow:hidden;border:1px solid rgba(31,41,55,1);background:linear-gradient(135deg,rgba(15,23,42,1),rgba(15,23,42,.98))}
    .project-left{padding:2rem}
    .project-right{padding:2rem;background:radial-gradient(circle at 0 0,rgba(56,189,248,.15),transparent 55%),#020617;display:flex;align-items:center;justify-content:center}
    .project-title{font-size:1.35rem;font-weight:700;color:#f9fafb;margin-top:.4rem}
    .project-meta{display:flex;flex-wrap:wrap;gap:.6rem;margin-top:.9rem}
    .project-tag{font-size:.75rem;padding:.25rem .75rem;border-radius:999px;background:rgba(15,23,42,1);border:1px solid rgba(51,65,85,1);color:#cbd5f5}
    .project-tag strong{color:#e5e7eb}
    .project-list{display:flex;flex-direction:column;gap:.9rem;margin-top:1.4rem}
    .project-item{display:flex;gap:.7rem;font-size:.93rem;color:#cbd5f5}
    .bullet{margin-top:.25rem;width:.48rem;height:.48rem;border-radius:999px;background:#38bdf8;flex-shrink:0}
    .code-shell{width:100%;max-width:420px;border-radius:1rem;overflow:hidden;background:rgba(2,6,23,1);border:1px solid rgba(31,41,55,1);box-shadow:0 18px 50px rgba(15,23,42,.95)}
    .code-header{display:flex;align-items:center;justify-content:space-between;padding:.55rem .85rem;border-bottom:1px solid rgba(31,41,55,1);font-size:.7rem;color:#64748b;background:linear-gradient(135deg,rgba(15,23,42,1),rgba(15,23,42,.98))}
    .code-dots{display:flex;align-items:center;gap:.25rem}
    .code-dot{width:.55rem;height:.55rem;border-radius:999px}
    .code-dot:nth-child(1){background:#f97373}
    .code-dot:nth-child(2){background:#facc15}
    .code-dot:nth-child(3){background:#22c55e}
    .code-body{padding:1.05rem;font-family:ui-monospace,Menlo,Monaco,Consolas,"Liberation Mono","Courier New",monospace;font-size:.77rem;color:#e5e7eb;overflow-x:auto;white-space:pre}
    .code-kw{color:#38bdf8}
    .code-type{color:#facc15}
    .code-str{color:#22c55e}
    .code-fn{color:#a855f7}
    .code-anno{color:#f97316}
    .skills-grid{display:grid;grid-template-columns:repeat(1,minmax(0,1fr));gap:1.3rem;margin-top:2rem}
    .skill-card{border-radius:1.2rem;background:rgba(15,23,42,.98);border:1px solid rgba(31,41,55,1);padding:1.5rem;display:flex;flex-direction:column;gap:.65rem}
    .skill-title{font-size:1rem;font-weight:600;color:#f9fafb}
    .skill-meta{font-size:.8rem;text-transform:uppercase;letter-spacing:.14em;color:#64748b}
    .skill-text{font-size:.95rem;color:#9ca3af}
    .skill-footer{margin-top:.35rem;font-size:.8rem;color:#e5e7eb}
    .timeline{margin-top:1.9rem;display:flex;flex-direction:column;gap:1.4rem}
    .timeline-item{display:flex;gap:1rem}
    .timeline-line{width:1.2rem;display:flex;flex-direction:column;align-items:center}
    .timeline-dot-outer{width:.85rem;height:.85rem;border-radius:999px;border:2px solid rgba(37,99,235,1);display:flex;align-items:center;justify-content:center;background:#020617}
    .timeline-dot-inner{width:.4rem;height:.4rem;border-radius:999px;background:#38bdf8}
    .timeline-connector{flex:1;width:1px;background:linear-gradient(to bottom,rgba(30,64,175,1),transparent)}
    .timeline-content{flex:1}
    .timeline-label{font-size:.75rem;letter-spacing:.12em;text-transform:uppercase;color:#64748b}
    .timeline-title{font-size:.97rem;font-weight:600;color:#e5e7eb;margin-top:.2rem}
    .timeline-text{font-size:.9rem;color:#9ca3af;margin-top:.3rem}
    .pill-soft{display:inline-flex;align-items:center;border-radius:999px;padding:.2rem .6rem;font-size:.7rem;background:rgba(8,47,73,1);color:#e0f2fe;border:1px solid rgba(56,189,248,.7);margin-top:.55rem}
    .ethics-grid{display:flex;flex-direction:column;gap:1.6rem;margin-top:2rem}
    .ethics-card-title{font-size:1.05rem;font-weight:600;color:#f9fafb}
    .ethics-text{font-size:.95rem;color:#9ca3af;margin-top:.35rem}
    .ethics-list{margin-top:.7rem;display:flex;flex-direction:column;gap:.5rem;font-size:.93rem;color:#cbd5f5}
    .ethics-bullet{display:flex;gap:.5rem}
    .ethics-bullet span{margin-top:.2rem;width:.35rem;height:.35rem;border-radius:999px;background:#a855f7;flex-shrink:0}
    .footer-shell{padding:3rem 0 2.2rem;border-top:1px solid rgba(15,23,42,1);margin-top:2rem}
    .footer-main{display:flex;flex-direction:column;gap:2.2rem}
    .footer-title{font-size:1.45rem;font-weight:700;color:#f9fafb}
    .footer-sub{margin-top:.4rem;color:#9ca3af;font-size:.95rem;max-width:30rem}
    .footer-actions{display:flex;flex-wrap:wrap;gap:.75rem;margin-top:1.5rem}
    .social-row{display:flex;flex-wrap:wrap;gap:.75rem;font-size:.9rem;color:#9ca3af}
    .social-link{display:inline-flex;align-items:center;gap:.35rem;padding:.45rem .9rem;border-radius:.9rem;background:rgba(2,6,23,1);border:1px solid rgba(31,41,55,1)}
    .social-link:hover{border-color:#38bdf8;color:#e5e7eb}
    .dot-muted{width:.45rem;height:.45rem;border-radius:999px;background:#38bdf8}
    .footer-meta{display:flex;flex-wrap:wrap;gap:.6rem;font-size:.78rem;color:#6b7280}
    @media (min-width:768px){
      .headline{font-size:3rem}
      .layout-2{flex-direction:row;align-items:center}
      .hero-text{flex:1}
      .hero-media{flex:1;justify-content:flex-end}
      .two-col{flex-direction:row}
      .two-col>div{flex:1}
      .skills-grid{grid-template-columns:repeat(3,minmax(0,1fr))}
      .ethics-grid{flex-direction:row}
      .ethics-grid>div{flex:1}
      .footer-main{flex-direction:row;justify-content:space-between;align-items:flex-start}
    }
    @media (min-width:900px){
      .nav-links{display:flex}
      .nav-toggle{display:none}
    }
    @media (max-width:899px){
      .project-shell{grid-template-columns:minmax(0,1fr)}
    }
  </style>
</head>
<body>
  <header class="nav-shell">
    <div class="container">
      <nav class="nav">
        <a href="#home" class="nav-brand">Tarek Rajab</a>
        <div class="nav-links">
          <a href="#home">Home</a>
          <a href="#intro">Introduction</a>
          <a href="#projects">Projects</a>
          <a href="#skills">Skills</a>
          <a href="#future">Future</a>
          <a href="#ethics">Ethics</a>
          <a href="#conclusion">Conclusion</a>
          <a href="#resume" class="nav-cta">Resume</a>
        </div>
        <button id="navToggle" class="nav-toggle" aria-label="Toggle navigation">
          <svg id="iconMenu" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none">
            <path d="M4 7h16M4 12h16M4 17h10" stroke="currentColor" stroke-width="1.7" stroke-linecap="round"/>
          </svg>
          <svg id="iconClose" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" style="display:none">
            <path d="M6 6l12 12M18 6l-12 12" stroke="currentColor" stroke-width="1.7" stroke-linecap="round"/>
          </svg>
        </button>
      </nav>
    </div>
    <div id="navMobile" class="nav-mobile">
      <a href="#home">Home</a>
      <a href="#intro">Introduction</a>
      <a href="#projects">Projects</a>
      <a href="#skills">Skills</a>
      <a href="#future">Future</a>
      <a href="#ethics">Ethics</a>
      <a href="#conclusion">Conclusion</a>
      <a href="#resume" class="nav-mobile-cta">View Resume</a>
    </div>
  </header>

  <main>
    <section id="home" class="section">
      <div class="container layout-2">
        <div class="hero-text">
          <div class="pill">
            <span class="pill-dot"></span>
            Open to internships · Backend & Data
          </div>
          <h1 class="headline">
            From biomedical science
            <span>to full-stack engineering & data</span>
          </h1>
          <p class="subhead">
            I’m a Computer Science student (class of 2027) who transitioned from Biomedical Engineering.
            I build robust backend systems with Java & Spring, and I’m steadily moving toward a future in
            Data Science and AI.
          </p>
          <div class="btn-row">
            <a href="mailto:eliosrajab@gmail.com" class="btn btn-primary">Contact me</a>
            <a href="#projects" class="btn btn-ghost">See my work</a>
          </div>
          <div class="chip-row">
            <span class="chip"><strong>Backend:</strong> Java, Spring Boot, REST APIs</span>
            <span class="chip"><strong>Data:</strong> Python, Pandas, ML basics</span>
            <span class="chip"><strong>Domain:</strong> Healthcare, clinical data</span>
          </div>
        </div>
        <div class="hero-media">
          <div class="profile-shell">
            <div class="ring"></div>
            <div class="ring"></div>
            <div class="profile-inner">
              <img src="image.jpg" alt="Portrait of Tarek Rajab">
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="intro" class="section">
      <div class="container">
        <div class="two-col">
          <div>
            <div class="pill-section-label">Introduction</div>
            <h2 class="section-title">Learning philosophy</h2>
            <p class="section-lead">
              My path from Biomedical Engineering to Computer Science was driven by curiosity about how systems work,
              both biological and digital. That shift clarified what motivates me: solving real problems with logic,
              data, and code.
            </p>
            <div class="stacked">
              <div>
                <div class="label">Core pillars</div>
                <p class="text-muted">
                  I learn best by building, breaking, and fixing. I value:
                  curiosity about how and why things work,
                  persistence when they don’t, and
                  practical application that turns theory into something tangible.
                </p>
              </div>
              <div>
                <div class="label">How I approach new tech</div>
                <p class="text-muted">
                  When I explore a new concept, I usually move from documentation to small experiments, then to a
                  project that forces me to combine multiple ideas. This helps me build a mental model that is
                  deeper than just syntax or surface-level patterns.
                </p>
              </div>
            </div>
          </div>
          <div>
            <div class="card card-muted">
              <div class="label">Collaboration & empathy</div>
              <h3 class="section-title" style="font-size:1.2rem;margin-top:.3rem">Experience in patient-centered work</h3>
              <p class="text-muted" style="margin-top:.75rem">
                During my internship at a physiotherapy centre, I acted as the link between staff and patients.
                I assisted clients, managed patient flow, and supported a smooth rehabilitation process.
              </p>
              <p class="text-muted" style="margin-top:.75rem">
                This strengthened my communication, organisational, and interpersonal skills in a real-world,
                high-pressure environment. Today, I bring the same empathy and clarity when collaborating with
                teammates, stakeholders, or non-technical audiences.
              </p>
              <div class="badge-row">
                <span class="badge badge-accent">Patient-facing experience</span>
                <span class="badge">Stakeholder communication</span>
                <span class="badge">High-pressure environments</span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="projects" class="section">
      <div class="container">
        <div class="section-header">
          <div class="pill">
            <span class="pill-dot"></span>
            Featured work
          </div>
          <h2 class="headline" style="font-size:2rem;margin-top:1rem">Interdisciplinary projects</h2>
          <p class="subhead" style="margin-inline:auto">
            I enjoy building systems where reliability and clarity matter. Below is a full-stack hospital
            application that brings together my interest in healthcare and backend engineering.
          </p>
        </div>
        <div class="project-shell">
          <div class="project-left">
            <div class="label">Full-stack project</div>
            <h3 class="project-title">Hospital management web application</h3>
            <p class="text-muted" style="margin-top:.6rem">
              A web platform that combines a public-facing hospital website with a secure backend application for managing
              patients, appointments, and doctors.
            </p>
            <div class="project-meta">
              <span class="project-tag"><strong>Backend:</strong> Java · Spring Boot · Spring Security</span>
              <span class="project-tag"><strong>Frontend:</strong> HTML · CSS · JavaScript</span>
              <span class="project-tag"><strong>Focus:</strong> Robust APIs · Clean domain model</span>
            </div>
            <div class="project-list">
              <div class="project-item">
                <span class="bullet"></span>
                <p>Designed and implemented REST APIs to manage patients, appointments, and doctor schedules with proper validation.</p>
              </div>
              <div class="project-item">
                <span class="bullet"></span>
                <p>Integrated Spring Security and role-based access control to protect sensitive medical and scheduling data.</p>
              </div>
              <div class="project-item">
                <span class="bullet"></span>
                <p>Built a responsive public website so patients can explore services, doctors, and contact information easily.</p>
              </div>
            </div>
            <div style="margin-top:1.7rem">
              <a href="https://github.com/TarekRajab0" target="_blank" class="btn btn-ghost" style="padding:.6rem 1.2rem;font-size:.9rem">
                View repository
              </a>
            </div>
          </div>
          <div class="project-right">
            <div class="code-shell">
              <div class="code-header">
                <div class="code-dots">
                  <span class="code-dot"></span>
                  <span class="code-dot"></span>
                  <span class="code-dot"></span>
                </div>
                <span>PatientController.java</span>
              </div>
              <pre class="code-body"><code><span class="code-anno">@RestController</span>
<span class="code-anno">@RequestMapping</span>(<span class="code-str">"/api/patients"</span>)
<span class="code-kw">public class</span> <span class="code-type">PatientController</span> {

    <span class="code-anno">@Autowired</span>
    <span class="code-type">PatientService</span> patientService;

    <span class="code-anno">@GetMapping</span>(<span class="code-str">"/{id}"</span>)
    <span class="code-type">ResponseEntity</span>&lt;<span class="code-type">Patient</span>&gt;
    <span class="code-fn">getPatientById</span>(<span class="code-anno">@PathVariable</span> <span class="code-type">Long</span> id) {
        <span class="code-type">Patient</span> patient =
            patientService.<span class="code-fn">findPatientById</span>(id);

        <span class="code-kw">return</span>
            <span class="code-type">ResponseEntity</span>.<span class="code-fn">ok</span>(patient);
    }

    <span class="code-anno">@PostMapping</span>
    <span class="code-type">ResponseEntity</span>&lt;<span class="code-type">Patient</span>&gt;
    <span class="code-fn">createPatient</span>(
        <span class="code-anno">@RequestBody</span> <span class="code-type">Patient</span> patient
    ) {
        <span class="code-type">Patient</span> saved =
            patientService.<span class="code-fn">savePatient</span>(patient);

        <span class="code-kw">return new</span> <span class="code-type">ResponseEntity</span>&lt;&gt;(
            saved,
            <span class="code-type">HttpStatus</span>.<span class="code-type">CREATED</span>
        );
    }
}</code></pre>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="skills" class="section">
      <div class="container">
        <div class="pill-section-label">Core competencies</div>
        <h2 class="section-title">What I’m actively strengthening</h2>
        <p class="section-lead">
          I’m building depth in backend engineering while developing strong foundations in data science and
          communication skills that translate across domains.
        </p>
        <div class="skills-grid">
          <div class="skill-card">
            <div class="skill-meta">Engineering</div>
            <h3 class="skill-title">Backend with Java & Spring</h3>
            <p class="skill-text">
              Ability to design and build secure, maintainable, and scalable backend services with Spring Boot,
              RESTful APIs, and clean separation between layers.
            </p>
            <p class="skill-footer">
              Artefact: Hospital management application source code.
            </p>
          </div>
          <div class="skill-card">
            <div class="skill-meta">Computer science</div>
            <h3 class="skill-title">Problem solving & data structures</h3>
            <p class="skill-text">
              Strong grasp of core CS fundamentals, using data structures and algorithms to write efficient,
              predictable code rather than relying on trial and error.
            </p>
            <p class="skill-footer">
              Artefact: DSA coursework and problem-solving certifications.
            </p>
          </div>
          <div class="skill-card">
            <div class="skill-meta">Human skills</div>
            <h3 class="skill-title">Communication & collaboration</h3>
            <p class="skill-text">
              Experience explaining complex ideas to people from non-technical backgrounds and collaborating with
              diverse teams under time pressure.
            </p>
            <p class="skill-footer">
              Artefact: Internship evaluation from physiotherapy centre.
            </p>
          </div>
        </div>
      </div>
    </section>

    <section id="future" class="section">
      <div class="container">
        <div class="two-col">
          <div>
            <div class="pill-section-label">Future horizon</div>
            <h2 class="section-title">Path toward data science</h2>
            <p class="section-lead">
              My long-term goal is to become a data scientist who can move from raw information to clear,
              actionable insights, especially in healthcare and high-impact domains.
            </p>
            <div class="stacked">
              <div>
                <div class="label">Current focus</div>
                <p class="text-muted">
                  I am strengthening my Python fundamentals and working through data science tools such as
                  Pandas, NumPy, scikit-learn, and introductory deep learning libraries.
                </p>
              </div>
              <div>
                <div class="label">How I like to work with data</div>
                <p class="text-muted">
                  I enjoy the process from data cleaning to feature selection, building simple baseline models,
                  and then iterating thoughtfully instead of jumping straight to complex solutions.
                </p>
              </div>
            </div>
          </div>
          <div>
            <div class="card">
              <div class="label">Featured data project</div>
              <h3 class="section-title" style="font-size:1.2rem;margin-top:.3rem">
                Leukemia clinical data analysis (research paper contribution)
              </h3>
              <p class="text-muted" style="margin-top:.7rem">
                Contributed to a research conference paper by analysing clinical trial data to identify patterns
                and possible markers of treatment efficacy for leukemia patients.
              </p>
              <div class="badge-row">
                <span class="badge badge-accent">Python · Pandas</span>
                <span class="badge">Exploratory data analysis</span>
                <span class="badge">Matplotlib · Seaborn</span>
              </div>
              <div class="timeline">
                <div class="timeline-item">
                  <div class="timeline-line">
                    <div class="timeline-dot-outer">
                      <div class="timeline-dot-inner"></div>
                    </div>
                    <div class="timeline-connector"></div>
                  </div>
                  <div class="timeline-content">
                    <div class="timeline-label">Data preparation</div>
                    <div class="timeline-title">Cleaning and structuring datasets</div>
                    <p class="timeline-text">
                      Used Python and Pandas to clean raw clinical data, handle missing values, and construct
                      consistent features for downstream analysis.
                    </p>
                  </div>
                </div>
                <div class="timeline-item">
                  <div class="timeline-line">
                    <div class="timeline-dot-outer">
                      <div class="timeline-dot-inner" style="background:#a855f7"></div>
                    </div>
                    <div class="timeline-connector" style="background:linear-gradient(to bottom,rgba(147,51,234,1),transparent)"></div>
                  </div>
                  <div class="timeline-content">
                    <div class="timeline-label">Insight</div>
                    <div class="timeline-title">Visualising trends and responses</div>
                    <p class="timeline-text">
                      Visualised patient responses over time using Matplotlib and Seaborn, helping the team
                      quickly spot emerging patterns and potential efficacy markers.
                    </p>
                    <div class="pill-soft">
                      Data used responsibly with anonymisation in mind.
                    </div>
                  </div>
                </div>
              </div>
              <div style="margin-top:1.6rem">
                <a href="https://github.com/TarekRajab0" target="_blank" class="btn btn-ghost" style="padding:.55rem 1.1rem;font-size:.85rem">
                  View data-related work
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="ethics" class="section">
      <div class="container">
        <div class="pill-section-label">Ethics & global awareness</div>
        <h2 class="section-title">Building systems that should exist</h2>
        <p class="section-lead">
          My interest in healthcare software naturally exposed me to one of the most sensitive types of data:
          patient information. That experience shaped how I think about security, privacy, and impact.
        </p>
        <div class="ethics-grid">
          <div class="card card-muted">
            <h3 class="ethics-card-title">Healthcare data case study</h3>
            <p class="ethics-text">
              When handling patient records, the impact of a single mistake is not theoretical. A small bug,
              misconfigured endpoint, or weak access rule can expose deeply sensitive information and break
              patient trust.
            </p>
            <div class="ethics-list">
              <div class="ethics-bullet">
                <span></span>
                <p>
                  Recognising that security is not an optional feature but a basic requirement for any system
                  working with real people and real consequences.
                </p>
              </div>
              <div class="ethics-bullet">
                <span></span>
                <p>
                  Being careful with logging, error messages, and data access patterns so that sensitive details
                  aren’t leaked unnecessarily.
                </p>
              </div>
            </div>
          </div>
          <div class="card card-muted">
            <h3 class="ethics-card-title">Personal principles</h3>
            <p class="ethics-text">
              Working with healthcare data made me more aware of how technology can both help and harm. A
              well-designed system can support better decisions and outcomes. A careless one can amplify
              inequality or cause real damage.
            </p>
            <div class="ethics-list">
              <div class="ethics-bullet">
                <span></span>
                <p>
                  I treat user data with the assumption that someone I care about could be directly affected by
                  how it is handled.
                </p>
              </div>
              <div class="ethics-bullet">
                <span></span>
                <p>
                  I aim to work on projects where I can stand behind both the technical quality and the impact
                  they have on people’s lives.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="conclusion" class="section">
      <div class="container">
        <div class="two-col">
          <div>
            <div class="pill-section-label">Summary</div>
            <h2 class="section-title">Where I am right now</h2>
            <p class="section-lead">
              I am a Computer Science student with a background in biomedical studies, building a foundation in
              backend development and growing steadily into data science and AI.
            </p>
            <div class="stacked">
              <div>
                <div class="label">What I bring</div>
                <p class="text-muted">
                  A mix of healthcare context, solid backend fundamentals, and a strong interest in data-driven
                  decision-making. I care about robustness, clarity, and the human impact behind the systems I
                  help build.
                </p>
              </div>
              <div>
                <div class="label">What I’m looking for</div>
                <p class="text-muted">
                  Opportunities to work on backend or data-oriented projects where I can learn from experienced
                  engineers, contribute meaningfully, and continue merging my technical skills with real-world
                  domains like healthcare.
                </p>
              </div>
            </div>
          </div>
          <div id="resume">
            <div class="card card-muted">
              <div class="label">Resume</div>
              <h3 class="section-title" style="font-size:1.15rem;margin-top:.3rem">Want the full story?</h3>
              <p class="text-muted" style="margin-top:.75rem">
                You can view or download my resume for a concise overview of my education, projects, and experience.
              </p>
              <div class="badge-row">
                <span class="badge">CS student · Class of 2027</span>
                <span class="badge">Backend · Java & Spring</span>
                <span class="badge">Data science in progress</span>
              </div>
              <div style="margin-top:1.3rem;display:flex;flex-wrap:wrap;gap:.75rem">
                <a href="resume.pdf" class="btn btn-primary" style="padding:.6rem 1.3rem;font-size:.9rem" target="_blank">
                  Open resume
                </a>
                <a href="mailto:eliosrajab@gmail.com" class="btn btn-ghost" style="padding:.6rem 1.3rem;font-size:.9rem">
                  Request updated copy
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer-shell">
    <div class="container">
      <div class="footer-main">
        <div>
          <h2 class="footer-title">Let’s build something useful</h2>
          <p class="footer-sub">
            I’m happy to discuss internships, junior roles, or collaborations where backend reliability
            and data thinking matter.
          </p>
          <div class="footer-actions">
            <a href="mailto:eliosrajab@gmail.com" class="btn btn-primary" style="padding:.65rem 1.4rem;font-size:.9rem">
              Email me
            </a>
            <a href="https://github.com/TarekRajab0" target="_blank" class="btn btn-ghost" style="padding:.65rem 1.4rem;font-size:.9rem">
              GitHub profile
            </a>
          </div>
        </div>
        <div style="display:flex;flex-direction:column;gap:1.2rem">
          <div class="social-row">
            <a href="https://www.linkedin.com/in/tarek-rajab" target="_blank" class="social-link">
              <span class="dot-muted"></span>
              <span>LinkedIn</span>
            </a>
            <a href="https://github.com/TarekRajab0" target="_blank" class="social-link">
              <span class="dot-muted"></span>
              <span>GitHub</span>
            </a>
          </div>
          <div class="footer-meta">
            <span>© <span id="year"></span> Tarek Rajab</span>
            <span>Built with HTML, CSS and a bit of JS</span>
          </div>
        </div>
      </div>
    </div>
  </footer>

  <script>
    const navToggle=document.getElementById("navToggle");
    const navMobile=document.getElementById("navMobile");
    const iconMenu=document.getElementById("iconMenu");
    const iconClose=document.getElementById("iconClose");
    navToggle.addEventListener("click",function(){
      const isOpen=navMobile.style.display==="flex";
      navMobile.style.display=isOpen?"none":"flex";
      iconMenu.style.display=isOpen?"block":"none";
      iconClose.style.display=isOpen?"none":"block";
    });
    navMobile.querySelectorAll("a").forEach(function(link){
      link.addEventListener("click",function(){
        navMobile.style.display="none";
        iconMenu.style.display="block";
        iconClose.style.display="none";
      });
    });
    document.getElementById("year").textContent=new Date().getFullYear();
  </script>
</body>
</html>
