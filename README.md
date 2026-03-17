<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Omar Ben Fathallah — GitHub README</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;500;600;700&family=Fira+Code:wght@400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
body{background:#ffffff;color:#1a1a1a;font-family:'Space Grotesk',sans-serif;}
:root{
  --color-text-primary:#1a1a1a;
  --color-text-secondary:#6b7280;
  --color-background-primary:#ffffff;
  --color-background-secondary:#f9fafb;
  --color-border-tertiary:rgba(0,0,0,0.1);
  --color-border-secondary:rgba(0,0,0,0.2);
  --border-radius-md:8px;
  --border-radius-lg:12px;
}
.rm{font-family:'Space Grotesk',sans-serif;max-width:780px;margin:0 auto;padding:2rem 1.25rem;color:#1a1a1a;}
@keyframes fadeUp{from{opacity:0;transform:translateY(16px)}to{opacity:1;transform:translateY(0)}}
@keyframes pulse{0%,100%{opacity:1}50%{opacity:.4}}
@keyframes barGrow{from{width:0}to{width:var(--w)}}
@keyframes spin{to{transform:rotate(360deg)}}
.hero{display:flex;align-items:flex-start;gap:1.5rem;margin-bottom:2rem;animation:fadeUp .5s ease both;}
.av-wrap{position:relative;flex-shrink:0;}
.avatar{width:76px;height:76px;border-radius:50%;background:linear-gradient(135deg,#085041,#1D9E75,#5DCAA5);display:flex;align-items:center;justify-content:center;font-size:24px;font-weight:700;color:#fff;letter-spacing:-1px;}
.av-ring{position:absolute;inset:-5px;border-radius:50%;border:1.5px dashed #5DCAA5;animation:spin 14s linear infinite;}
.av-dot{position:absolute;bottom:4px;right:4px;width:12px;height:12px;border-radius:50%;background:#1D9E75;border:2px solid #fff;}
.av-dot::after{content:'';position:absolute;inset:-3px;border-radius:50%;background:#1D9E7540;animation:pulse 2s ease infinite;}
.hero-text h1{font-size:30px;font-weight:700;letter-spacing:-1px;line-height:1.1;margin-bottom:5px;}
.hero-text h1 em{color:#1D9E75;font-style:normal;}
.role{font-size:13px;color:#6b7280;margin-bottom:10px;display:flex;align-items:center;gap:7px;font-family:'Fira Code',monospace;}
.role-sep{color:#d1d5db;}
.badges{display:flex;flex-wrap:wrap;gap:5px;}
.badge{font-family:'Fira Code',monospace;font-size:10px;padding:3px 9px;border-radius:20px;font-weight:500;border:1px solid;}
.bg-teal{background:#E1F5EE;border-color:#5DCAA5;color:#085041;}
.bg-blue{background:#E6F1FB;border-color:#85B7EB;color:#0C447C;}
.bg-purple{background:#EEEDFE;border-color:#AFA9EC;color:#3C3489;}
.bg-amber{background:#FAEEDA;border-color:#FAC775;color:#633806;}
.bg-coral{background:#FAECE7;border-color:#F0997B;color:#712B13;}
.divider{height:.5px;background:rgba(0,0,0,0.1);margin:1.75rem 0;}
.sec{margin-bottom:1.75rem;animation:fadeUp .5s ease both;}
.sec-hd{display:flex;align-items:center;gap:9px;margin-bottom:1rem;}
.sec-ic{width:26px;height:26px;border-radius:7px;display:flex;align-items:center;justify-content:center;flex-shrink:0;}
.sec-ic svg{width:13px;height:13px;}
.sec-lbl{font-size:11px;font-weight:600;letter-spacing:2px;text-transform:uppercase;color:#6b7280;}
.about-p{font-size:14.5px;line-height:1.85;margin-bottom:1rem;}
.hl-list{display:flex;flex-direction:column;gap:7px;}
.hl{display:flex;align-items:baseline;gap:8px;font-size:13px;}
.hl-k{color:#6b7280;flex-shrink:0;}
.hl-v{font-weight:500;}
.hl::before{content:'▸';color:#1D9E75;font-size:10px;flex-shrink:0;}
.tabs{display:flex;gap:5px;flex-wrap:wrap;margin-bottom:1rem;}
.tab{font-family:'Fira Code',monospace;font-size:11px;padding:5px 11px;border-radius:6px;border:.5px solid rgba(0,0,0,0.2);cursor:pointer;color:#6b7280;background:transparent;transition:all .18s;}
.tab.on{background:#1D9E75;border-color:#1D9E75;color:#fff;}
.tab:hover:not(.on){background:#f9fafb;}
.sp{display:none;flex-direction:column;gap:7px;}
.sp.show{display:flex;}
.sr{display:flex;align-items:center;gap:10px;}
.sn{font-family:'Fira Code',monospace;font-size:12px;width:140px;flex-shrink:0;color:#1a1a1a;}
.sb-bg{flex:1;height:4px;border-radius:2px;background:#f3f4f6;border:.5px solid rgba(0,0,0,0.1);overflow:hidden;}
.sb{height:100%;border-radius:2px;animation:barGrow .75s ease both;}
.sb.g{background:linear-gradient(90deg,#085041,#1D9E75,#5DCAA5);}
.sb.b{background:linear-gradient(90deg,#0C447C,#378ADD);}
.sb.p{background:linear-gradient(90deg,#3C3489,#7F77DD);}
.sb.a{background:linear-gradient(90deg,#633806,#EF9F27);}
.sb.c{background:linear-gradient(90deg,#712B13,#D85A30);}
.sp-pct{font-family:'Fira Code',monospace;font-size:11px;color:#6b7280;width:30px;text-align:right;}
.exp-list{display:flex;flex-direction:column;gap:10px;}
.ec{background:#fff;border:.5px solid rgba(0,0,0,0.1);border-radius:12px;padding:14px 16px 12px;position:relative;overflow:hidden;transition:border-color .2s,transform .15s;}
.ec::before{content:'';position:absolute;top:0;left:0;width:3px;height:100%;border-radius:0;}
.ec.teal::before{background:linear-gradient(180deg,#1D9E75,#5DCAA5);}
.ec.blue::before{background:linear-gradient(180deg,#185FA5,#378ADD);}
.ec.purple::before{background:linear-gradient(180deg,#534AB7,#7F77DD);}
.ec.coral::before{background:linear-gradient(180deg,#993C1D,#D85A30);}
.ec:hover{border-color:rgba(0,0,0,0.2);transform:translateX(2px);}
.ec-top{display:flex;justify-content:space-between;align-items:flex-start;gap:8px;margin-bottom:4px;flex-wrap:wrap;}
.ec-title{font-size:14px;font-weight:600;}
.ec-org{font-family:'Fira Code',monospace;font-size:10px;padding:2px 8px;border-radius:4px;white-space:nowrap;font-weight:500;}
.ec-org.teal{background:#E1F5EE;color:#085041;}
.ec-org.blue{background:#E6F1FB;color:#0C447C;}
.ec-org.purple{background:#EEEDFE;color:#3C3489;}
.ec-org.coral{background:#FAECE7;color:#712B13;}
.ec-date{font-family:'Fira Code',monospace;font-size:10px;color:#6b7280;}
.ec-desc{font-size:12.5px;color:#6b7280;line-height:1.6;margin:6px 0 8px;}
.ec-tags{display:flex;flex-wrap:wrap;gap:4px;}
.ec-tag{font-family:'Fira Code',monospace;font-size:10px;padding:2px 6px;background:#f9fafb;border:.5px solid rgba(0,0,0,0.1);border-radius:3px;color:#6b7280;}
.proj-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:10px;}
.pj{background:#fff;border:.5px solid rgba(0,0,0,0.1);border-radius:12px;padding:12px 14px;transition:border-color .2s;}
.pj:hover{border-color:rgba(0,0,0,0.2);}
.pj-title{font-size:13px;font-weight:600;margin-bottom:4px;}
.pj-desc{font-size:12px;color:#6b7280;line-height:1.55;margin-bottom:8px;}
.contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;}
.cc{background:#fff;border:.5px solid rgba(0,0,0,0.1);border-radius:12px;padding:12px 14px;display:flex;align-items:center;gap:10px;text-decoration:none;color:#1a1a1a;transition:border-color .18s,background .18s;}
.cc:hover{border-color:rgba(0,0,0,0.2);background:#f9fafb;}
.cc-ic{width:34px;height:34px;border-radius:8px;display:flex;align-items:center;justify-content:center;flex-shrink:0;}
.cc-ic svg{width:15px;height:15px;}
.cc-lbl{font-size:10px;color:#6b7280;margin-bottom:2px;}
.cc-val{font-size:12px;font-weight:500;font-family:'Fira Code',monospace;}
.footer{margin-top:1.5rem;padding-top:1rem;border-top:.5px solid rgba(0,0,0,0.1);display:flex;align-items:center;gap:8px;font-family:'Fira Code',monospace;font-size:11px;color:#6b7280;}
.f-pulse{width:6px;height:6px;border-radius:50%;background:#1D9E75;animation:pulse 2.5s ease infinite;flex-shrink:0;}
</style>
</head>
<body>
<div class="rm">

<div class="hero">
  <div class="av-wrap">
    <div class="avatar">OB</div>
    <div class="av-ring"></div>
    <div class="av-dot"></div>
  </div>
  <div class="hero-text">
    <h1>Omar <em>Ben Fathallah</em></h1>
    <div class="role">
      <span>Software Engineer</span><span class="role-sep">·</span>
      <span>Backend &amp; Full-Stack</span><span class="role-sep">·</span>
      <span>El Aouina, Tunisia</span>
    </div>
    <div class="badges">
      <span class="badge bg-teal">Spring Boot</span>
      <span class="badge bg-blue">Angular · React · Vite</span>
      <span class="badge bg-coral">FastAPI · Python</span>
      <span class="badge bg-purple">DevOps · CI/CD</span>
      <span class="badge bg-amber">Microservices</span>
      <span class="badge bg-teal">Open to work</span>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.05s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#E1F5EE"><svg viewBox="0 0 16 16" fill="none" stroke="#1D9E75" stroke-width="1.5" stroke-linecap="round"><circle cx="8" cy="5" r="3"/><path d="M2 14c0-3.3 2.7-6 6-6s6 2.7 6 6"/></svg></div>
    <span class="sec-lbl">About</span>
  </div>
  <p class="about-p">Software Engineering graduate from ESPRIT (Aug 2025) with a strong focus on backend architecture, REST API design, and full-stack development. Experienced in DevOps practices and microservices. Currently building AI-powered features with FastAPI and React Vite.</p>
  <div class="hl-list">
    <div class="hl"><span class="hl-k">Currently building</span><span class="hl-v">FastAPI + React Vite project · dynamic backend systems</span></div>
    <div class="hl"><span class="hl-k">Interests</span><span class="hl-v">system design · APIs · AI integration · performance</span></div>
    <div class="hl"><span class="hl-k">Languages</span><span class="hl-v">Arabic (native) · French (professional) · English (intermediate)</span></div>
    <div class="hl"><span class="hl-k">Status</span><span class="hl-v">open to opportunities &amp; collaboration</span></div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.1s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#E6F1FB"><svg viewBox="0 0 16 16" fill="none" stroke="#378ADD" stroke-width="1.5" stroke-linecap="round"><rect x="1" y="3" width="14" height="10" rx="2"/><path d="M5 7l2 2 4-4"/></svg></div>
    <span class="sec-lbl">Tech stack</span>
  </div>
  <div class="tabs">
    <button class="tab on" onclick="sw('backend',this)">Backend</button>
    <button class="tab" onclick="sw('frontend',this)">Frontend</button>
    <button class="tab" onclick="sw('devops',this)">DevOps</button>
    <button class="tab" onclick="sw('database',this)">Database</button>
    <button class="tab" onclick="sw('ai',this)">AI &amp; Data</button>
  </div>
  <div id="sp-backend" class="sp show">
    <div class="sr"><span class="sn">Spring Boot</span><div class="sb-bg"><div class="sb g" style="--w:92%;width:92%;animation-delay:.05s"></div></div><span class="sp-pct">92%</span></div>
    <div class="sr"><span class="sn">Java</span><div class="sb-bg"><div class="sb g" style="--w:90%;width:90%;animation-delay:.1s"></div></div><span class="sp-pct">90%</span></div>
    <div class="sr"><span class="sn">REST APIs</span><div class="sb-bg"><div class="sb g" style="--w:90%;width:90%;animation-delay:.15s"></div></div><span class="sp-pct">90%</span></div>
    <div class="sr"><span class="sn">FastAPI</span><div class="sb-bg"><div class="sb c" style="--w:75%;width:75%;animation-delay:.2s"></div></div><span class="sp-pct">75%</span></div>
    <div class="sr"><span class="sn">Node.js / Express</span><div class="sb-bg"><div class="sb g" style="--w:72%;width:72%;animation-delay:.25s"></div></div><span class="sp-pct">72%</span></div>
    <div class="sr"><span class="sn">JPA / Hibernate</span><div class="sb-bg"><div class="sb g" style="--w:85%;width:85%;animation-delay:.3s"></div></div><span class="sp-pct">85%</span></div>
    <div class="sr"><span class="sn">Spring Security</span><div class="sb-bg"><div class="sb g" style="--w:80%;width:80%;animation-delay:.35s"></div></div><span class="sp-pct">80%</span></div>
  </div>
  <div id="sp-frontend" class="sp">
    <div class="sr"><span class="sn">Angular</span><div class="sb-bg"><div class="sb b" style="--w:87%;width:87%"></div></div><span class="sp-pct">87%</span></div>
    <div class="sr"><span class="sn">React.js + Vite</span><div class="sb-bg"><div class="sb b" style="--w:82%;width:82%"></div></div><span class="sp-pct">82%</span></div>
    <div class="sr"><span class="sn">TypeScript</span><div class="sb-bg"><div class="sb b" style="--w:80%;width:80%"></div></div><span class="sp-pct">80%</span></div>
    <div class="sr"><span class="sn">TailwindCSS</span><div class="sb-bg"><div class="sb b" style="--w:85%;width:85%"></div></div><span class="sp-pct">85%</span></div>
    <div class="sr"><span class="sn">JavaScript</span><div class="sb-bg"><div class="sb b" style="--w:83%;width:83%"></div></div><span class="sp-pct">83%</span></div>
  </div>
  <div id="sp-devops" class="sp">
    <div class="sr"><span class="sn">Docker</span><div class="sb-bg"><div class="sb p" style="--w:82%;width:82%"></div></div><span class="sp-pct">82%</span></div>
    <div class="sr"><span class="sn">Jenkins / CI-CD</span><div class="sb-bg"><div class="sb p" style="--w:78%;width:78%"></div></div><span class="sp-pct">78%</span></div>
    <div class="sr"><span class="sn">GitHub Actions</span><div class="sb-bg"><div class="sb p" style="--w:75%;width:75%"></div></div><span class="sp-pct">75%</span></div>
    <div class="sr"><span class="sn">Microservices</span><div class="sb-bg"><div class="sb p" style="--w:74%;width:74%"></div></div><span class="sp-pct">74%</span></div>
    <div class="sr"><span class="sn">Prometheus / Grafana</span><div class="sb-bg"><div class="sb p" style="--w:65%;width:65%"></div></div><span class="sp-pct">65%</span></div>
    <div class="sr"><span class="sn">SonarQube</span><div class="sb-bg"><div class="sb p" style="--w:70%;width:70%"></div></div><span class="sp-pct">70%</span></div>
  </div>
  <div id="sp-database" class="sp">
    <div class="sr"><span class="sn">MySQL</span><div class="sb-bg"><div class="sb a" style="--w:88%;width:88%"></div></div><span class="sp-pct">88%</span></div>
    <div class="sr"><span class="sn">PostgreSQL</span><div class="sb-bg"><div class="sb a" style="--w:84%;width:84%"></div></div><span class="sp-pct">84%</span></div>
    <div class="sr"><span class="sn">MongoDB</span><div class="sb-bg"><div class="sb a" style="--w:65%;width:65%"></div></div><span class="sp-pct">65%</span></div>
    <div class="sr"><span class="sn">Dynamic schemas</span><div class="sb-bg"><div class="sb a" style="--w:85%;width:85%"></div></div><span class="sp-pct">85%</span></div>
  </div>
  <div id="sp-ai" class="sp">
    <div class="sr"><span class="sn">Python</span><div class="sb-bg"><div class="sb c" style="--w:78%;width:78%"></div></div><span class="sp-pct">78%</span></div>
    <div class="sr"><span class="sn">FastAPI</span><div class="sb-bg"><div class="sb c" style="--w:75%;width:75%"></div></div><span class="sp-pct">75%</span></div>
    <div class="sr"><span class="sn">Data Mining</span><div class="sb-bg"><div class="sb c" style="--w:60%;width:60%"></div></div><span class="sp-pct">60%</span></div>
    <div class="sr"><span class="sn">Hadoop / Big Data</span><div class="sb-bg"><div class="sb c" style="--w:55%;width:55%"></div></div><span class="sp-pct">55%</span></div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.15s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#EEEDFE"><svg viewBox="0 0 16 16" fill="none" stroke="#7F77DD" stroke-width="1.5" stroke-linecap="round"><rect x="2" y="2" width="12" height="12" rx="2"/><path d="M5 8h6M8 5v6"/></svg></div>
    <span class="sec-lbl">Professional experience</span>
  </div>
  <div class="exp-list">
    <div class="ec teal">
      <div class="ec-top"><span class="ec-title">Document Management System (DMS)</span><span class="ec-org teal">Sharing Technologies · BH Bank</span></div>
      <div class="ec-date">Dec 2024 – Jun 2025 · Final Year Internship</div>
      <p class="ec-desc">Led end-to-end development of a DMS web app. Integrated Alfresco via CMIS protocol. Built a dynamic database system enabling automated table/entity creation through an admin interface.</p>
      <div class="ec-tags"><span class="ec-tag">Spring Boot</span><span class="ec-tag">Angular</span><span class="ec-tag">PostgreSQL</span><span class="ec-tag">Docker</span><span class="ec-tag">JWT</span><span class="ec-tag">TailwindCSS</span><span class="ec-tag">REST API</span></div>
    </div>
    <div class="ec blue">
      <div class="ec-top"><span class="ec-title">Aircraft Maintenance Management App</span><span class="ec-org blue">Sharing Technologies · Tunisair</span></div>
      <div class="ec-date">Jul 2024 – Aug 2024 · Summer Internship</div>
      <p class="ec-desc">Developed an application for managing aircraft maintenance operations, records tracking and automated technical report generation.</p>
      <div class="ec-tags"><span class="ec-tag">Spring Boot</span><span class="ec-tag">Angular</span><span class="ec-tag">REST API</span><span class="ec-tag">MySQL</span></div>
    </div>
    <div class="ec purple">
      <div class="ec-top"><span class="ec-title">Back-Office Data Management System</span><span class="ec-org purple">ESPRIT · Information Systems</span></div>
      <div class="ec-date">Jul 2023 – Aug 2023 · Immersion Internship</div>
      <p class="ec-desc">Designed and implemented CRUD features and a complete back-office system for efficient data management.</p>
      <div class="ec-tags"><span class="ec-tag">ReactJS</span><span class="ec-tag">Spring Boot</span><span class="ec-tag">MySQL</span></div>
    </div>
    <div class="ec coral">
      <div class="ec-top"><span class="ec-title">Attack of Zombie — 3D Mobile Game</span><span class="ec-org coral">CGI Studio</span></div>
      <div class="ec-date">Feb 2022 – Jun 2022 · Final Year Project</div>
      <p class="ec-desc">Designed and developed a full 3D mobile game including 3D modeling, animation, and immersive gameplay mechanics.</p>
      <div class="ec-tags"><span class="ec-tag">C#</span><span class="ec-tag">Unity</span><span class="ec-tag">Blender</span><span class="ec-tag">3D Animation</span></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.2s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#FAEEDA"><svg viewBox="0 0 16 16" fill="none" stroke="#BA7517" stroke-width="1.5" stroke-linecap="round"><path d="M3 3h10v4a5 5 0 01-10 0V3z"/><path d="M8 10v3M5 13h6"/></svg></div>
    <span class="sec-lbl">Academic projects</span>
  </div>
  <div class="proj-grid">
    <div class="pj">
      <div class="pj-title">DevOps CI/CD Microservices Pipeline</div>
      <p class="pj-desc">Full CI/CD pipeline with Jenkins, Docker, GitHub webhooks, Grafana monitoring and SonarQube code quality.</p>
      <div class="ec-tags"><span class="ec-tag">Jenkins</span><span class="ec-tag">Docker</span><span class="ec-tag">GitHub Actions</span><span class="ec-tag">Grafana</span><span class="ec-tag">Prometheus</span></div>
    </div>
    <div class="pj">
      <div class="pj-title">Internship Management Platform</div>
      <p class="pj-desc">Full CRUD platform with Spring Security auth, user roles, access control and admin dashboard.</p>
      <div class="ec-tags"><span class="ec-tag">Spring Boot</span><span class="ec-tag">Spring Security</span><span class="ec-tag">Angular</span><span class="ec-tag">TailwindCSS</span></div>
    </div>
    <div class="pj">
      <div class="pj-title">Municipal Recycling Platform</div>
      <p class="pj-desc">Offer management and purchasing flow for a municipal recycling initiative with JavaFX UI.</p>
      <div class="ec-tags"><span class="ec-tag">JavaFX</span><span class="ec-tag">Symfony</span><span class="ec-tag">PHP</span><span class="ec-tag">Bootstrap</span></div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.25s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#E1F5EE"><svg viewBox="0 0 16 16" fill="none" stroke="#1D9E75" stroke-width="1.5" stroke-linecap="round"><path d="M8 2v4M8 10v4M2 8h4M10 8h4"/><circle cx="8" cy="8" r="2"/></svg></div>
    <span class="sec-lbl">Currently learning</span>
  </div>
  <div style="display:flex;flex-direction:column;gap:8px;">
    <div class="hl"><span>FastAPI advanced patterns &amp; async Python for production APIs</span></div>
    <div class="hl"><span>React Vite architecture with modern state management</span></div>
    <div class="hl"><span>AI &amp; LLM integration in enterprise applications</span></div>
    <div class="hl"><span>Microservices &amp; advanced system design at scale</span></div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.3s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#FAECE7"><svg viewBox="0 0 16 16" fill="none" stroke="#D85A30" stroke-width="1.5" stroke-linecap="round"><circle cx="8" cy="8" r="6"/><path d="M8 5v3l2 2"/></svg></div>
    <span class="sec-lbl">Education</span>
  </div>
  <div class="exp-list">
    <div class="ec teal">
      <div class="ec-top"><span class="ec-title">National Engineering Degree — Software Engineering</span><span class="ec-org teal">ESPRIT, Tunis</span></div>
      <div class="ec-date">2022 – 2025</div>
    </div>
    <div class="ec blue">
      <div class="ec-top"><span class="ec-title">Bachelor's Degree — Information Technology</span><span class="ec-org blue">ISET Siliana</span></div>
      <div class="ec-date">2019 – 2022</div>
    </div>
  </div>
</div>

<div class="divider"></div>

<div class="sec" style="animation-delay:.35s">
  <div class="sec-hd">
    <div class="sec-ic" style="background:#E6F1FB"><svg viewBox="0 0 16 16" fill="none" stroke="#378ADD" stroke-width="1.5" stroke-linecap="round"><path d="M13 2H3a1 1 0 00-1 1v2h12V3a1 1 0 00-1-1zM2 5v8a1 1 0 001 1h10a1 1 0 001-1V5H2z"/></svg></div>
    <span class="sec-lbl">Contact</span>
  </div>
  <div class="contact-grid">
    <a href="https://www.linkedin.com/in/ben-fathallah-omar/" class="cc">
      <div class="cc-ic" style="background:#E6F1FB"><svg viewBox="0 0 16 16" fill="#378ADD"><path d="M3 2a1 1 0 100 2 1 1 0 000-2zM2 5h2v7H2V5zm4 0h1.9v1h.03c.26-.5 1-1 2.07-1C12 5 12 7 12 8.5V12h-2V9c0-.75 0-1.71-1.04-1.71-1.05 0-1.21.82-1.21 1.66V12H6V5z"/></svg></div>
      <div><div class="cc-lbl">LinkedIn</div><div class="cc-val">ben-fathallah-omar</div></div>
    </a>
    <a href="mailto:benfathallah.omar@gmail.com" class="cc">
      <div class="cc-ic" style="background:#E1F5EE"><svg viewBox="0 0 16 16" fill="none" stroke="#1D9E75" stroke-width="1.5" stroke-linecap="round"><rect x="2" y="4" width="12" height="9" rx="1.5"/><path d="M2 6l6 4 6-4"/></svg></div>
      <div><div class="cc-lbl">Email</div><div class="cc-val" style="font-size:11px">benfathallah.omar@gmail.com</div></div>
    </a>
    <a href="https://github.com/omarbenfathallah" class="cc">
      <div class="cc-ic" style="background:#F1EFE8"><svg viewBox="0 0 16 16" fill="#1a1a1a"><path d="M8 1C4.13 1 1 4.13 1 8c0 3.09 2.01 5.72 4.79 6.64.35.06.48-.15.48-.34v-1.2c-1.95.42-2.36-.94-2.36-.94-.32-.81-.78-1.03-.78-1.03-.64-.43.05-.42.05-.42.7.05 1.07.72 1.07.72.62 1.07 1.63.76 2.03.58.06-.45.24-.76.44-.94-1.55-.18-3.19-.78-3.19-3.46 0-.76.27-1.39.72-1.88-.07-.18-.31-.89.07-1.85 0 0 .59-.19 1.93.72A6.7 6.7 0 018 4.79c.6 0 1.2.08 1.76.23 1.34-.91 1.93-.72 1.93-.72.38.96.14 1.67.07 1.85.45.49.72 1.12.72 1.88 0 2.69-1.64 3.28-3.2 3.45.25.22.48.65.48 1.31v1.94c0 .19.13.4.48.34A7.003 7.003 0 0015 8c0-3.87-3.13-7-7-7z"/></svg></div>
      <div><div class="cc-lbl">GitHub</div><div class="cc-val">omarbenfathallah</div></div>
    </a>
    <a href="tel:+21627351545" class="cc">
      <div class="cc-ic" style="background:#FAEEDA"><svg viewBox="0 0 16 16" fill="none" stroke="#BA7517" stroke-width="1.5" stroke-linecap="round"><path d="M3 2h3l1.5 3.5-1.5 1a8 8 0 004 4l1-1.5L14.5 10V13A1.5 1.5 0 0113 14.5C6.1 14.5 1.5 9.9 1.5 3A1.5 1.5 0 013 1.5V2z"/></svg></div>
      <div><div class="cc-lbl">Phone</div><div class="cc-val">+216 27 351 545</div></div>
    </a>
  </div>
</div>

<div class="footer">
  <span class="f-pulse"></span>
  <span>available for opportunities · open to remote &amp; international roles</span>
</div>

</div>
<script>
function sw(id,btn){
  document.querySelectorAll('.sp').forEach(p=>p.classList.remove('show'));
  document.querySelectorAll('.tab').forEach(b=>b.classList.remove('on'));
  document.getElementById('sp-'+id).classList.add('show');
  btn.classList.add('on');
  document.querySelectorAll('#sp-'+id+' .sb').forEach((b,i)=>{
    b.style.animation='none';
    setTimeout(()=>{b.style.animation='barGrow .7s ease '+(i*.08)+'s both';},10);
  });
}
</script>
</body>
</html>
