<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>SGCS — Cybersecurity Portfolio</title>
<meta name="description" content="SGCS — Cybersecurity Analyst | Cloud Security Engineer in progress. Case studies, projects, blog and contact."/>
<meta property="og:title" content="SGCS — Cybersecurity Portfolio" />
<meta property="og:description" content="Case studies, projects, cloud security, incident response and open source tools." />
<meta name="theme-color" content="#0b1220" />
<link rel="icon" href="data:;base64,iVBORw0KGgo=">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap" rel="stylesheet">
<style>
  :root {
    --bg:#0b1220;
    --card:#0f1724;
    --muted:#a7b0c8;
    --accent:#17a2ff;
    --glass: rgba(255,255,255,0.03);
    --radius:12px;
    --maxWidth:1100px;
    color-scheme: dark;
  }
  *{box-sizing:border-box;}
  html,body{height:100%;margin:0;font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;background:linear-gradient(180deg,var(--bg) 0%, #071024 100%);color:#e6eef8;line-height:1.5;padding:32px;-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale;}
  .site{max-width:var(--maxWidth);margin:0 auto;display:block;gap:32px;}
  header{display:flex;align-items:center;justify-content:space-between;gap:16px;margin-bottom:28px;}
  .brand{display:flex;gap:12px;align-items:center;text-decoration:none;color:inherit;}
  .logo{width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#00ffc9);display:flex;align-items:center;justify-content:center;font-weight:800;color:#061020;box-shadow:0 6px 20px rgba(0,0,0,0.6);}
  nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600;font-size:14px;}
  nav a:hover{color:var(--accent);}
  main{display:block;background:transparent;}
  /* Hero */
  .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:start;margin-bottom:28px;}
  .hero-card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:28px;border-radius:var(--radius);box-shadow:0 8px 30px rgba(3,8,22,0.6);border:1px solid rgba(255,255,255,0.03);}
  h1{font-size:28px;margin:0 0 10px 0;letter-spacing:-0.3px;}
  .tag{color:var(--accent);font-weight:700;margin-bottom:12px;display:inline-block;}
  p.lead{color:var(--muted);margin-top:6px;margin-bottom:18px;}
  .cta{display:flex;gap:12px;margin-top:18px;}
  .btn{padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:700;font-size:14px;background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.04);color:inherit;transition:transform .12s ease, box-shadow .12s ease;}
  .btn:hover{transform:translateY(-3px);box-shadow:0 10px 30px rgba(23,162,255,0.08);}
  .btn.primary{background:linear-gradient(90deg,var(--accent),#00ffc9);color:#041025;border:0;}
  .snapshot{display:flex;gap:12px;margin-top:16px;}
  .stat{background:var(--glass);padding:12px;border-radius:10px;min-width:92px;text-align:center;}
  .stat strong{display:block;font-size:18px;}
  .right-profile{padding:24px;border-radius:var(--radius);background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border:1px solid rgba(255,255,255,0.03);box-shadow:0 6px 18px rgba(3,8,22,0.6);}
  .photo{width:100%;height:220px;background:linear-gradient(180deg,#071a2a,#072433);border-radius:10px;display:flex;align-items:center;justify-content:center;color:var(--muted);font-weight:700;}
  .skills{margin-top:16px;}
  .skill{display:flex;justify-content:space-between;font-size:13px;color:var(--muted);margin-top:8px;}
  .bar{height:8px;background:rgba(255,255,255,0.03);border-radius:6px;margin-top:6px;overflow:hidden;}
  .bar > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent),#00ffc9);}
  /* Projects */
  .section{margin-top:28px;}
  .projects-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;}
  .project{background:var(--card);padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);transition:transform .12s ease, box-shadow .12s ease;}
  .project:hover{transform:translateY(-6px);box-shadow:0 14px 40px rgba(2,6,18,0.6);}
  .project .meta{color:var(--muted);font-size:13px;margin-bottom:8px;}
  .project h3{margin:0 0 8px 0;}
  .project p{color:var(--muted);margin:0 0 12px 0;font-size:14px;}
  .project .tags{display:flex;gap:8px;flex-wrap:wrap;}
  .tag-pill{background:rgba(255,255,255,0.025);padding:6px 8px;border-radius:8px;font-size:12px;color:var(--muted);}
  .project .more{margin-top:12px;display:flex;justify-content:space-between;align-items:center;}
  .view-btn{font-size:13px;padding:8px 10px;border-radius:8px;}
  /* modal */
  .modal{position:fixed;left:0;top:0;right:0;bottom:0;display:none;align-items:center;justify-content:center;background:linear-gradient(180deg,rgba(1,2,6,0.6),rgba(1,2,6,0.9));z-index:999;padding:28px;}
  .modal.open{display:flex;}
  .modal-card{width:100%;max-width:920px;background:var(--card);padding:20px;border-radius:12px;border:1px solid rgba(255,255,255,0.04);overflow:auto;max-height:86vh;}
  .modal .close{float:right;background:transparent;border:0;color:var(--muted);font-weight:700;}
  /* Responsive */
  @media (max-width:980px){.hero{grid-template-columns:1fr}.projects-grid{grid-template-columns:repeat(2,1fr);}}
  @media (max-width:640px){body{padding:18px}.projects-grid{grid-template-columns:1fr}nav a{display:none}header{align-items:flex-start;gap:8px}}
</style>
</head>
<body>
<div class="site">
<header>
<a class="brand" href="#">
<div class="logo">SG</div>
<div>
<div style="font-weight:800">SGCS</div>
<div style="font-size:12px;color:var(--muted)">Cybersecurity Portfolio</div>
</div>
</a>
<nav>
<a href="#projects">Projects</a>
<a href="#blog">Blog</a>
<a href="#certs">Certs</a>
<a href="#contact">Contact</a>
</nav>
</header>
<main>
<section class="hero">
<div class="hero-card">
<div class="tag">Cybersecurity • Cloud • Incident Response</div>
<h1>Hi — I’m <span style="color:var(--accent)">SGCS</span>, a Cybersecurity Analyst building cloud security expertise.</h1>
<p class="lead">I design secure cloud environments, run incident response investigations, and build automation to reduce mean time to detect & respond. Below are redacted case studies, projects and resources illustrating my work.</p>
<div class="cta">
<a class="btn primary" href="#projects">See Projects</a>
<a class="btn" href="mailto:you@sgcs.uk?subject=Website%20enquiry">Contact</a>
<a class="btn" href="/sgcs-cv.pdf" target="_blank" rel="noopener">Download CV</a>
</div>
<div class="snapshot" aria-hidden="true">
<div class="stat"><strong>6</strong> Case Studies</div>
<div class="stat"><strong>10+</strong> Certifications</div>
<div class="stat"><strong>5</strong> Open-source tools</div>
</div>
<hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:18px 0">
<div>
<strong style="display:block">Featured project — Cloud Tenant Hardening</strong>
<p style="margin:6px 0;color:var(--muted)">Implemented a landing zone and guardrails in Azure using Terraform to reduce attack surface and enforce least privilege across subscriptions.</p>
<div style="display:flex;gap:8px;margin-top:10px">
<a class="btn" href="#project-1">Read case</a>
<a class="btn" href="https://github.com/yourusername" target="_blank" rel="noopener">View code</a>
</div>
</div>
</div>
<aside class="right-profile">
<div class="photo">Your Photo / Avatar</div>
<div style="margin-top:12px">
<div style="display:flex;justify-content:space-between;align-items:center">
<div>
<div style="font-weight:700">SGCS</div>
<div style="color:var(--muted);font-size:13px">Junior Cybersecurity Analyst ➜ Cloud Security</div>
</div>
<div style="text-align:right;color:var(--muted);font-size:13px">Based in: London, UK</div>
</div>
<div class="skills">
<div style="font-weight:700;margin-top:10px">Core skills</div>
<div class="skill"><div>Azure / IAM</div><div style="color:var(--muted)">Advanced</div></div>
<div class="bar"><i style="width:86%"></i></div>
<div class="skill"><div>Incident Response</div><div style="color:var(--muted)">Mid</div></div>
<div class="bar"><i style="width:72%"></i></div>
<div class="skill"><div>Python / Automation</div><div style="color:var(--muted)">Mid</div></div>
<div class="bar"><i style="width:65%"></i></div>
<div style="margin-top:10px;font-size:13px;color:var(--muted)">
Open to roles: Cloud Security Engineer, Security Automation, IR
</div>
</div>
</div>
</aside>
</section>
<!-- Projects, blog, certs, contact sections remain unchanged -->
<footer>
<div>© <span id="year"></span> SGCS — sgcs.uk</div>
<div>
<a class="social" href="https://github.com/yourusername" target="_blank">GitHub</a>
<a class="social" href="https://www.linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
<a class="social" href="mailto:you@sgcs.uk">Email</a>
</div>
</footer>
</div>
<script>
document.getElementById('year').textContent = new Date().getFullYear();
</script>
</body>
</html>