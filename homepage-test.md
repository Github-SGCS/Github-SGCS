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
<!-- Simple reset + Google fonts -->
<link href=https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700;800&display=swap rel="stylesheet">
<style>
 
    :root{
 
      --bg:#0b1220;
 
      --card:#0f1724;
 
      --muted:#a7b0c8;
 
      --accent:#17a2ff;
 
      --glass: rgba(255,255,255,0.03);
 
      --radius:12px;
 
      --maxWidth:1100px;
 
      color-scheme: dark;
 
    }
 
    *{box-sizing:border-box}
 
    html,body{height:100%}
 
    body{
 
      margin:0;
 
      font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
 
      background:linear-gradient(180deg,var(--bg) 0%, #071024 100%);
 
      color:#e6eef8;
 
      -webkit-font-smoothing:antialiased;
 
      -moz-osx-font-smoothing:grayscale;
 
      line-height:1.5;
 
      padding:32px;
 
    }
 
    .site{
 
      max-width:var(--maxWidth);
 
      margin:0 auto;
 
      display:block;
 
      gap:32px;
 
    }
 
    header{
 
      display:flex;
 
      align-items:center;
 
      justify-content:space-between;
 
      gap:16px;
 
      margin-bottom:28px;
 
    }
 
    .brand{
 
      display:flex;
 
      gap:12px;
 
      align-items:center;
 
      text-decoration:none;
 
      color:inherit;
 
    }
 
    .logo{
 
      width:48px;height:48px;border-radius:10px;background:linear-gradient(135deg,var(--accent),#00ffc9);
 
      display:flex;align-items:center;justify-content:center;font-weight:800;color:#061020;
 
      box-shadow:0 6px 20px rgba(0,0,0,0.6);
 
    }
 
    nav a{color:var(--muted);text-decoration:none;margin-left:18px;font-weight:600;font-size:14px}
 
    nav a:hover{color:var(--accent)}
 
    main{display:block;background:transparent}
 
    .hero{
 
      display:grid;
 
      grid-template-columns:1fr 420px;
 
      gap:28px;
 
      align-items:start;
 
      margin-bottom:28px;
 
    }
 
    .hero-card{
 
      background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
 
      padding:28px;border-radius:var(--radius);
 
      box-shadow: 0 8px 30px rgba(3,8,22,0.6);
 
      border: 1px solid rgba(255,255,255,0.03);
 
    }
 
    h1{font-size:28px;margin:0 0 10px 0;letter-spacing:-0.3px}
 
    .tag{color:var(--accent);font-weight:700;margin-bottom:12px;display:inline-block}
 
    p.lead{color:var(--muted);margin-top:6px;margin-bottom:18px}
 
    .cta{
 
      display:flex;gap:12px;margin-top:18px;
 
    }
 
    .btn{
 
      padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:700;font-size:14px;
 
      background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.04);color:inherit;
 
      transition:transform .12s ease, box-shadow .12s ease;
 
    }
 
    .btn:hover{transform:translateY(-3px);box-shadow:0 10px 30px rgba(23,162,255,0.08)}
 
    .btn.primary{background:linear-gradient(90deg,var(--accent),#00ffc9);color:#041025;border:0}
 
    .snapshot{display:flex;gap:12px;margin-top:16px}
 
    .stat{background:var(--glass);padding:12px;border-radius:10px;min-width:92px;text-align:center}
 
    .stat strong{display:block;font-size:18px}
 
    .right-profile{
 
      padding:24px;border-radius:var(--radius);background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
 
      border:1px solid rgba(255,255,255,0.03);box-shadow:0 6px 18px rgba(3,8,22,0.6)
 
    }
 
    .photo{width:100%;height:220px;background:linear-gradient(180deg,#071a2a,#072433);border-radius:10px;display:flex;align-items:center;justify-content:center;color:var(--muted);font-weight:700}
 
    .skills{margin-top:16px}
 
    .skill{display:flex;justify-content:space-between;font-size:13px;color:var(--muted);margin-top:8px}
 
    .bar{height:8px;background:rgba(255,255,255,0.03);border-radius:6px;margin-top:6px;overflow:hidden}
 
    .bar > i{display:block;height:100%;background:linear-gradient(90deg,var(--accent),#00ffc9)}
 
    /* Projects */
 
    .section{margin-top:28px}
 
    .section h2{margin:0 0 12px 0}
 
    .projects-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px}
 
    .project{
 
      background:var(--card);padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);
 
      transition:transform .12s ease, box-shadow .12s ease;
 
    }
 
    .project:hover{transform:translateY(-6px);box-shadow:0 14px 40px rgba(2,6,18,0.6)}
 
    .project .meta{color:var(--muted);font-size:13px;margin-bottom:8px}
 
    .project h3{margin:0 0 8px 0}
 
    .project p{color:var(--muted);margin:0 0 12px 0;font-size:14px}
 
    .project .tags{display:flex;gap:8px;flex-wrap:wrap}
 
    .tag-pill{background:rgba(255,255,255,0.025);padding:6px 8px;border-radius:8px;font-size:12px;color:var(--muted)}
 
    .project .more{margin-top:12px;display:flex;justify-content:space-between;align-items:center}
 
    .view-btn{font-size:13px;padding:8px 10px;border-radius:8px}
 
    /* modal / expanded case study */
 
    .modal{
 
      position:fixed;left:0;top:0;right:0;bottom:0;display:none;align-items:center;justify-content:center;background:linear-gradient(180deg,rgba(1,2,6,0.6),rgba(1,2,6,0.9));
 
      z-index:999;padding:28px;
 
    }
 
    .modal.open{display:flex}
 
    .modal-card{width:100%;max-width:920px;background:var(--card);padding:20px;border-radius:12px;border:1px solid rgba(255,255,255,0.04);overflow:auto;max-height:86vh}
 
    .modal .close{float:right;background:transparent;border:0;color:var(--muted);font-weight:700}
 
    /* blog grid */
 
    .blog-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:16px;margin-top:12px}
 
    .post{background:var(--card);padding:14px;border-radius:10px}
 
    .certs{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
 
    .cert{background:rgba(255,255,255,0.02);padding:8px 10px;border-radius:8px;font-size:13px;color:var(--muted)}
 
    /* contact */
 
    .contact-grid{display:grid;grid-template-columns:1fr 320px;gap:16px;margin-top:12px}
 
    .contact-card{background:var(--card);padding:16px;border-radius:12px}
 
    footer{margin-top:28px;color:var(--muted);font-size:13px;display:flex;justify-content:space-between;align-items:center}
 
    a.social{color:var(--muted);text-decoration:none;margin-left:12px}
 
    /* responsive */
 
    @media (max-width:980px){
 
      .hero{grid-template-columns:1fr}
 
      .projects-grid, .blog-grid{grid-template-columns:repeat(2,1fr)}
 
      .contact-grid{grid-template-columns:1fr}
 
    }
 
    @media (max-width:640px){
 
      body{padding:18px}
 
      .projects-grid, .blog-grid{grid-template-columns:1fr}
 
      nav a{display:none}
 
      header{align-items:flex-start;gap:8px}
 
    }
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
<!-- HERO -->
<section class="hero">
<div class="hero-card">
<div class="tag">Cybersecurity • Cloud • Incident Response</div>
<h1>Hi — I’m <span style="color:var(--accent)">SGCS</span>, a Cybersecurity Analyst building cloud security expertise.</h1>
<p class="lead">I design secure cloud environments, run incident response investigations, and build automation to reduce mean time to detect & respond. Below are redacted case studies, projects and resources illustrating my work.</p>
<div class="cta">
<a class="btn primary" href="#projects">See Projects</a>
<a class="btn" href=mailto:you@sgcs.uk?subject=Website%20enquiry>Contact</a>
<a class="btn" href="/sgcs-cv.pdf" target="_blank" rel="noopener">Download CV</a>
</div>
<div class="snapshot" aria-hidden="true">
<div class="stat">
<strong>6</strong>
 
              Case Studies
</div>
<div class="stat">
<strong>10+</strong>
 
              Certifications
</div>
<div class="stat">
<strong>5</strong>
 
              Open-source tools
</div>
</div>
<hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:18px 0">
<div>
<strong style="display:block">Featured project — Cloud Tenant Hardening</strong>
<p style="margin:6px 0;color:var(--muted)">Implemented a landing zone and guardrails in Azure using Terraform to reduce attack surface and enforce least privilege across subscriptions.</p>
<div style="display:flex;gap:8px;margin-top:10px">
<a class="btn" href="#project-1">Read case</a>
<a class="btn" href=https://github.com/yourusername target="_blank" rel="noopener">View code</a>
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
<div class="skill">
<div>Azure / IAM</div>
<div style="color:var(--muted)">Advanced</div>
</div>
<div class="bar"><i style="width:86%"></i></div>
<div class="skill">
<div>Incident Response</div>
<div style="color:var(--muted)">Mid</div>
</div>
<div class="bar"><i style="width:72%"></i></div>
<div class="skill">
<div>Python / Automation</div>
<div style="color:var(--muted)">Mid</div>
</div>
<div class="bar"><i style="width:65%"></i></div>
<div style="margin-top:10px;font-size:13px;color:var(--muted)">
 
                Open to roles: Cloud Security Engineer, Security Automation, IR
</div>
</div>
</div>
</aside>
</section>
<!-- PROJECTS -->
<section id="projects" class="section">
<h2>Projects & Case Studies</h2>
<div class="projects-grid">
<!-- Project 1 -->
<article class="project" data-case="project-1" id="project-1">
<div class="meta">Cloud • Terraform • Azure</div>
<h3>Tenant Hardening & Landing Zone</h3>
<p>Built a multi-subscription landing zone using IaC with automated policy enforcement, RBAC minimisation, and security baseline controls.</p>
<div class="tags">
<span class="tag-pill">Terraform</span>
<span class="tag-pill">Azure</span>
<span class="tag-pill">Policy</span>
</div>
<div class="more">
<small style="color:var(--muted)">3 weeks</small>
<button class="btn view-btn" data-open="project-1">View Case</button>
</div>
</article>
<!-- Project 2 -->
<article class="project" data-case="project-2" id="project-2">
<div class="meta">IR • SIEM • Detection</div>
<h3>Phishing Incident Response</h3>
<p>Performed triage on a targeted phishing campaign, produced IOC list and remediation playbook; improved detection rules in the SIEM.</p>
<div class="tags">
<span class="tag-pill">Splunk</span>
<span class="tag-pill">Playbooks</span>
<span class="tag-pill">IR</span>
</div>
<div class="more">
<small style="color:var(--muted)">2 days</small>
<button class="btn view-btn" data-open="project-2">View Case</button>
</div>
</article>
<!-- Project 3 -->
<article class="project" data-case="project-3" id="project-3">
<div class="meta">Tooling • Open Source</div>
<h3>Automated Asset Inventory</h3>
<p>Lightweight Python tool that inventories cloud assets and exports an asset register for risk scoring and remediation prioritisation.</p>
<div class="tags">
<span class="tag-pill">Python</span>
<span class="tag-pill">Open-source</span>
</div>
<div class="more">
<small style="color:var(--muted)">Repo</small>
<a class="btn view-btn" href=https://github.com/yourusername/repo target="_blank" rel="noopener">GitHub</a>
</div>
</article>
<!-- Add placeholders for more projects -->
<article class="project">
<div class="meta">Red Team / Blue Team</div>
<h3>Red Team Exercise (redacted)</h3>
<p>Summary of methodology and remediation recommendations (redacted for sensitivity).</p>
<div class="tags">
<span class="tag-pill">Testing</span>
<span class="tag-pill">Remediation</span>
</div>
<div class="more">
<small style="color:var(--muted)">Redacted</small>
<button class="btn view-btn" data-open="soon">View</button>
</div>
</article>
<article class="project">
<div class="meta">Cloud • CI/CD</div>
<h3>Secure Pipeline Proof-of-Concept</h3>
<p>Implemented secure build pipelines with signing and least privilege agent configuration.</p>
<div class="tags">
<span class="tag-pill">CI</span>
<span class="tag-pill">Security</span>
</div>
<div class="more">
<small style="color:var(--muted)">PoC</small>
<a class="btn view-btn" href=https://github.com/yourusername/pipeline target="_blank" rel="noopener">Repo</a>
</div>
</article>
<article class="project">
<div class="meta">Lab • Learning</div>
<h3>Home Lab — SIEM & Threat Hunting</h3>
<p>Design and docs for a low-cost home lab using ELK/OSSEC to simulate detection exercises.</p>
<div class="tags">
<span class="tag-pill">ELK</span>
<span class="tag-pill">Threat Hunting</span>
</div>
<div class="more">
<small style="color:var(--muted)">Guide</small>
<a class="btn view-btn" href="/lab-guide.pdf" target="_blank" rel="noopener">Download</a>
</div>
</article>
</div>
</section>
<!-- BLOG -->
<section id="blog" class="section">
<h2>Selected Blog & Writeups</h2>
<div class="blog-grid">
<article class="post">
<div style="font-size:13px;color:var(--muted)">Aug 2025 • Cloud</div>
<h3 style="margin-top:8px">Hardening Azure Subscriptions — Practical Steps</h3>
<p style="color:var(--muted);margin-top:8px">Short guide describing policy, RBAC & network baseline controls to apply to a tenant.</p>
<div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
<a class="btn" href="/blog/azure-hardening.html">Read</a>
<div style="color:var(--muted);font-size:13px">6 min</div>
</div>
</article>
<article class="post">
<div style="font-size:13px;color:var(--muted)">Jun 2025 • IR</div>
<h3 style="margin-top:8px">Phishing Triage Checklist</h3>
<p style="color:var(--muted);margin-top:8px">A concise checklist for SOC analysts during phishing investigations.</p>
<div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
<a class="btn" href="/blog/phish-triage.html">Read</a>
<div style="color:var(--muted);font-size:13px">3 min</div>
</div>
</article>
<article class="post">
<div style="font-size:13px;color:var(--muted)">May 2025 • Tools</div>
<h3 style="margin-top:8px">Building a Simple Asset Inventory with Python</h3>
<p style="color:var(--muted);margin-top:8px">Walkthrough and sample code for inventorying cloud resources from the API.</p>
<div style="display:flex;justify-content:space-between;align-items:center;margin-top:12px">
<a class="btn" href=https://github.com/yourusername/asset-inventory target="_blank" rel="noopener">View</a>
<div style="color:var(--muted);font-size:13px">Repo</div>
</div>
</article>
</div>
</section>
<!-- CERTIFICATIONS -->
<section id="certs" class="section">
<h2>Certifications & Skills</h2>
<div class="certs">
<div class="cert">CompTIA Security+</div>
<div class="cert">Microsoft SC-900</div>
<div class="cert">Azure Fundamentals</div>
<div class="cert">TryHackMe — Path: Blue Team</div>
<!-- Add verification links as needed -->
</div>
</section>
<!-- CONTACT -->
<section id="contact" class="section">
<h2>Contact</h2>
<div class="contact-grid">
<div class="contact-card">
<p style="color:var(--muted)">I'm happy to discuss collaboration, open roles, or give feedback on security projects. If you'd like to request a redacted case study or confirm certs, drop a message below or email me directly.</p>
<form id="contactForm" onsubmit="submitContact(event)" style="margin-top:12px">
<label style="font-size:13px;color:var(--muted)">Your name</label><br>
<input required name="name" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;margin-top:6px"><br>
<label style="font-size:13px;color:var(--muted);margin-top:8px;display:block">Email</label>
<input required type="email" name="email" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;margin-top:6px"><br>
<label style="font-size:13px;color:var(--muted);margin-top:8px;display:block">Message</label>
<textarea required name="message" rows="4" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;margin-top:6px"></textarea>
<div style="margin-top:12px;display:flex;gap:10px">
<button class="btn primary" type="submit">Send message</button>
<a class="btn" href=mailto:you@sgcs.uk?subject=Contact%20via%20site>Email directly</a>
</div>
<div id="formMsg" style="margin-top:10px;color:var(--muted);font-size:13px"></div>
</form>
</div>
<aside class="contact-card">
<div style="font-weight:700">Reach me</div>
<div style="color:var(--muted);margin-top:8px">Email: <a href=mailto:you@sgcs.uk style="color:var(--accent)">you@sgcs.uk</a></div>
<div style="color:var(--muted);margin-top:8px">LinkedIn: <a href=https://www.linkedin.com/in/yourprofile target="_blank" style="color:var(--accent)">yourprofile</a></div>
<div style="color:var(--muted);margin-top:8px">GitHub: <a href=https://github.com/yourusername target="_blank" style="color:var(--accent)">yourusername</a></div>
<hr style="border:none;border-top:1px solid rgba(255,255,255,0.03);margin:12px 0">
<div style="font-size:13px;color:var(--muted)">Availability: Open to work & contract engagements.</div>
<div style="margin-top:12px">
<div style="font-weight:700">Quick links</div>
<div style="margin-top:8px">
<a class="tag-pill" href="/sgcs-cv.pdf">Download CV</a>
</div>
</div>
</aside>
</div>
</section>
</main>
<footer>
<div>© <span id="year"></span> SGCS — sgcs.uk</div>
<div>
<a class="social" href=https://github.com/yourusername target="_blank">GitHub</a>
<a class="social" href=https://www.linkedin.com/in/yourprofile target="_blank">LinkedIn</a>
<a class="social" href=mailto:you@sgcs.uk>Email</a>
</div>
</footer>
</div>
<!-- Modal for expanded case studies -->
<div id="modal" class="modal" role="dialog" aria-hidden="true">
<div class="modal-card" id="modalCard" role="document">
<button class="close" onclick="closeModal()" aria-label="Close">Close ✕</button>
<div id="modalContent" style="clear:both"></div>
</div>
</div>
<script>
 
    // Basic interactive behaviors (no frameworks)
 
    document.getElementById('year').textContent = new Date().getFullYear();
 
    const modal = document.getElementById('modal');
 
    const modalContent = document.getElementById('modalContent');
 
    // Pre-populated case study content - replace or extend
 
    const cases = {
 
      "project-1": {
 
        title: "Tenant Hardening & Landing Zone",
 
        subtitle: "Azure • Terraform • Policy as Code",
 
        body: `
<p><strong>Summary</strong> — Designed and deployed a multi-subscription landing zone using Terraform modules, Azure Policy initiatives and RBAC reviews to reduce attack surface and provide consistent guardrails.</p>
<h4>Problem</h4>
<p>Inconsistent subscription configuration and permissive roles caused management complexity and elevated risk.</p>
<h4>Approach</h4>
<ul>
<li>Defined baseline subscriptions and tagging requirements</li>
<li>Implemented policy initiatives for allowed SKUs, NSG enforcement and diagnostic settings</li>
<li>Automated deployment with Terraform and a CI pipeline that enforces plan validation</li>
</ul>
<h4>Outcome</h4>
<p>Reduced misconfiguration risk, improved visibility in a centralised log subscription, and shortened onboarding time for new subscriptions.</p>
<p style="color:var(--muted)">Note: this case is redacted — links to code and full diagrams are available on request.</p>
 
        `
 
      },
 
      "project-2": {
 
        title: "Phishing Incident Response",
 
        subtitle: "SIEM • Playbooks • Detection",
 
        body: `
<p><strong>Summary</strong> — Rapid triage of a targeted phishing campaign; produced IOCs, updated detections and a remediation playbook for the SOC.</p>
<h4>Approach</h4>
<ol>
<li>Collected email headers and attachments for analysis</li>
<li>Pivoted through logs to identify lateral movement and suspicious authentications</li>
<li>Created detections in the SIEM and automated response steps</li>
</ol>
<h4>Result</h4>
<p>Containment within 8 hours; detections reduced recurrence and recovery time.</p>
 
        `
 
      },
 
      "project-3": {
 
        title: "Automated Asset Inventory",
 
        subtitle: "Python • Cloud APIs",
 
        body: `
<p><strong>Summary</strong> — A small Python CLI that interrogates cloud APIs to enumerate resources and produce a CSV asset register with tags for risk scoring.</p>
<h4>Why</h4>
<p>Many organisations struggle to maintain an authoritative asset list across multiple cloud accounts.</p>
<h4>How</h4>
<p>Script uses SDKs to fetch resources, normalises names, and exports metadata. Open-sourced under MIT — <a href=https://github.com/yourusername/asset-inventory target="_blank">repo</a>.</p>
 
        `
 
      },
 
      "soon": {
 
        title: "Coming soon",
 
        subtitle: "",
 
        body: "<p>This case study is not yet public — contact me for more information.</p>"
 
      }
 
    };
 
    // open modal with case content
 
    document.querySelectorAll('[data-open]').forEach(btn=>{
 
      btn.addEventListener('click', (e)=>{
 
        const id = btn.getAttribute('data-open');
 
        openCase(id);
 
      });
 
    });
 
    function openCase(id){
 
      const data = cases[id] || {title:"Case study", body:"<p>Not found</p>"};
 
      modalContent.innerHTML = '<h2 style="margin-top:0">'+(data.title||'')+'</h2>' + (data.subtitle?('<div style="color:var(--muted)">'+data.subtitle+'</div>'):'') + (data.body||'');
 
      modal.classList.add('open');
 
      modal.setAttribute('aria-hidden','false');
 
      document.body.style.overflow = 'hidden';
 
    }
 
    function closeModal(){
 
      modal.classList.remove('open');
 
      modal.setAttribute('aria-hidden','true');
 
      document.body.style.overflow = '';
 
    }
 
    // Escape to close modal
 
    document.addEventListener('keydown',(e)=>{
 
      if(e.key==='Escape') closeModal();
 
    });
 
    // Simple contact form handling (no backend) - opens mailto fallback
 
    function submitContact(e){
 
      e.preventDefault();
 
      const form = e.target;
 
      const name = encodeURIComponent(form.name.value.trim());
 
      const email = encodeURIComponent(form.email.value.trim());
 
      const msg = encodeURIComponent(form.message.value.trim());
 
      const subject = encodeURIComponent('Website contact from ' + (form.name.value.trim() || 'Website visitor'));
 
      const body = encodeURIComponent(`Name: ${form.name.value}\nEmail: ${form.email.value}\n\nMessage:\n${form.message.value}`);
 
      // Try to open mail client - users hosting with a server should replace this with a real POST endpoint
 
      window.location.href = `mailto:you@sgcs.uk?subject=${subject}&body=${body}`;
 
      document.getElementById('formMsg').textContent = "Opening your mail client... If nothing opens, please email you@sgcs.uk directly.";
 
    }
</script>
</body>
</html>