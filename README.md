<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lemnos Consulting | Marketing Infrastructure for SMBs</title>
  <meta name="description" content="Lemnos Consulting builds the marketing infrastructure SMBs actually need — CRM, email, paid media, automation, data, and reporting. Fractional marketing operations without the enterprise price tag.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Outfit:wght@100;300;400;500;600;700&display=swap" rel="stylesheet">
  <style>
    *,*::before,*::after{margin:0;padding:0;box-sizing:border-box}
    :root{
      --green:#4CBB17;--green-dark:#086108;--orange:#F28606;--purple:#8710D2;
      --black:#0B0B0B;--cream:#EAE8E4;--gray:#A0A0A0;--gray-mid:#888888;
      --gray-light:#CCCCCC;--white:#FFFFFF;
      --bg:var(--white);--bg-card:#F7F6F4;--bg-card-hover:var(--cream);
      --bg-dark:var(--black);--text:var(--black);--text-dim:var(--gray-mid);
      --accent:var(--green);--accent-dark:var(--green-dark);
      --border:rgba(11,11,11,0.08);--border-dark:rgba(255,255,255,0.08);
      --h1:61px;--h2:40px;--h3:37px;--h5:24px;--h6:22px;
      --p1:17px;--p2:15px;--p3:14px;
      --serif:'Bebas Neue',sans-serif;
      --sans:'Outfit',-apple-system,sans-serif;
      --max-w:1120px
    }
    html{scroll-behavior:smooth}
    body{font-family:var(--sans);background:var(--bg);color:var(--text);line-height:1.7;font-size:var(--p1);-webkit-font-smoothing:antialiased}
    ::selection{background:var(--green);color:var(--white)}
    a{color:var(--green-dark);text-decoration:none;transition:color .2s}
    a:hover{color:var(--green)}

    /* NAV */
    nav{position:fixed;top:0;left:0;right:0;z-index:100;padding:1.25rem 2rem;display:flex;justify-content:space-between;align-items:center;background:#FFFFFF;border-bottom:1px solid var(--border)}
    .nav-logo{display:flex;align-items:center}
    .nav-logo-img{height:48px;width:auto}
    .nav-logo span{color:var(--green)}
    .nav-links{display:flex;gap:2rem;align-items:center}
    .nav-links a{color:var(--gray-mid);font-size:var(--p3);letter-spacing:.05em;text-transform:uppercase;font-weight:500}
    .nav-links a:hover{color:var(--black)}
    .nav-cta{background:var(--green);color:var(--white)!important;padding:.5rem 1.25rem;font-size:.8rem;font-weight:600;letter-spacing:.05em;text-transform:uppercase;border:none;cursor:pointer;transition:all .2s}
    .nav-cta:hover{background:var(--green-dark);color:var(--white)!important}
    .hamburger{display:none;background:none;border:none;cursor:pointer;padding:.5rem}
    .hamburger span{display:block;width:22px;height:2px;background:var(--black);margin:5px 0;transition:all .3s}

    /* HERO */
    .hero{min-height:100vh;display:flex;flex-direction:column;justify-content:center;padding:8rem 2rem 6rem;background:var(--bg-dark);color:var(--cream);position:relative;overflow:hidden}
    .hero::before{content:'';position:absolute;top:-20%;right:-10%;width:600px;height:600px;background:radial-gradient(circle,rgba(76,187,23,0.06) 0%,transparent 70%);pointer-events:none}
    .hero-inner{max-width:var(--max-w);margin:0 auto;width:100%}
    .hero-eyebrow{font-size:var(--p3);letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:1.5rem;font-weight:500}
    .hero h1{font-family:var(--serif);font-size:clamp(2.8rem,6vw,var(--h1));line-height:1.1;font-weight:400;max-width:820px;margin-bottom:2rem;color:var(--cream)}
    .hero h1 em{font-style:italic;color:var(--green)}
    .hero-sub{font-size:1.15rem;color:var(--gray);max-width:620px;line-height:1.8;margin-bottom:3rem}
    .hero-links{display:flex;gap:1.5rem;flex-wrap:wrap;align-items:center}
    .btn-primary{display:inline-block;background:var(--green);color:var(--white);padding:.9rem 2.25rem;font-size:var(--p3);font-weight:600;letter-spacing:.08em;text-transform:uppercase;transition:all .2s;border:none;cursor:pointer}
    .btn-primary:hover{background:var(--green-dark);color:var(--white)}
    .btn-outline{display:inline-block;border:1px solid var(--gray-mid);color:var(--gray);padding:.85rem 2.25rem;font-size:var(--p3);font-weight:600;letter-spacing:.08em;text-transform:uppercase;transition:all .2s}
    .btn-outline:hover{border-color:var(--cream);color:var(--cream)}

    /* SECTIONS */
    section{padding:6rem 2rem}
    .section-inner{max-width:var(--max-w);margin:0 auto}
    .section-eyebrow{font-size:var(--p3);letter-spacing:.2em;text-transform:uppercase;color:var(--orange);margin-bottom:1rem;font-weight:600}
    .section-title{font-family:var(--serif);font-size:clamp(2rem,4vw,var(--h2));line-height:1.15;font-weight:400;margin-bottom:1.5rem;max-width:700px;color:var(--black)}
    .section-body{color:var(--gray-mid);max-width:640px;font-size:1.05rem;line-height:1.8}
    .section-body+.section-body{margin-top:1.25rem}
    .dark-section{background:var(--bg-dark);color:var(--cream)}
    .dark-section .section-title{color:var(--cream)}
    .dark-section .section-body{color:var(--gray)}
    .dark-section .section-eyebrow{color:var(--green)}
    .divider{max-width:var(--max-w);margin:0 auto;border:none;border-top:1px solid var(--border)}

    /* SERVICE CARDS */
    .service-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(320px,1fr));gap:1.5rem;margin-top:3rem}
    .service-card{background:var(--bg-card);border:1px solid var(--border);padding:2.5rem;transition:all .3s;position:relative}
    .service-card:hover{background:var(--bg-card-hover);border-color:rgba(76,187,23,0.2)}
    .service-number{font-size:.7rem;letter-spacing:.2em;text-transform:uppercase;color:var(--orange);margin-bottom:1rem;font-weight:700}
    .service-card h3{font-family:var(--serif);font-size:var(--h5);font-weight:400;margin-bottom:1rem;line-height:1.3;color:var(--black)}
    .service-card p{color:var(--gray-mid);font-size:var(--p2);line-height:1.7}
    .service-tools{margin-top:1.25rem;font-size:var(--p3);color:var(--green-dark);font-weight:500}

    /* DETAIL CARDS (smaller, for sub-capabilities) */
    .detail-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1rem;margin-top:2rem}
    .detail-card{background:rgba(255,255,255,0.03);border:1px solid var(--border-dark);padding:1.5rem;transition:border-color .3s}
    .detail-card:hover{border-color:rgba(76,187,23,0.2)}
    .detail-card .detail-label{font-size:.65rem;letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:.5rem;font-weight:700}
    .detail-card h4{font-family:var(--serif);font-size:1.15rem;color:var(--cream);margin-bottom:.5rem;font-weight:400}
    .detail-card p{font-size:var(--p3);color:var(--gray);line-height:1.6}

    /* HOW IT WORKS */
    .process-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:2rem;margin-top:3rem}
    .process-step{position:relative;padding-left:0}
    .process-num{font-family:var(--serif);font-size:3rem;color:var(--green);line-height:1;margin-bottom:.75rem;opacity:.4}
    .process-step h3{font-family:var(--serif);font-size:1.3rem;color:var(--black);margin-bottom:.75rem;font-weight:400}
    .process-step p{font-size:var(--p2);color:var(--gray-mid);line-height:1.7}

    /* EXPERIENCE */
    .exp-entry{margin-top:3rem;padding-bottom:3rem;border-bottom:1px solid var(--border-dark)}
    .exp-entry:last-child{border-bottom:none;padding-bottom:0}
    .exp-header{display:flex;justify-content:space-between;align-items:baseline;flex-wrap:wrap;gap:.5rem;margin-bottom:.5rem}
    .exp-title{font-family:var(--serif);font-size:var(--h5);color:var(--cream)}
    .exp-dates{font-size:var(--p3);color:var(--gray-mid);letter-spacing:.05em}
    .exp-company{font-size:var(--p2);color:var(--green);font-weight:500;margin-bottom:1rem}
    .exp-desc{color:var(--gray);font-size:var(--p2);line-height:1.8;margin-bottom:1rem}
    .exp-highlights{list-style:none;display:flex;flex-wrap:wrap;gap:.5rem}
    .exp-highlights li{font-size:var(--p3);color:var(--gray-mid);background:rgba(255,255,255,0.05);border:1px solid var(--border-dark);padding:.3rem .75rem}

    /* CREDENTIALS */
    .cred-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1.5rem;margin-top:2rem}
    .cred-card{background:var(--bg-card);border:1px solid var(--border);padding:1.75rem}
    .cred-card .cred-label{font-size:.7rem;letter-spacing:.2em;text-transform:uppercase;color:var(--orange);margin-bottom:.5rem;font-weight:700}
    .cred-card .cred-value{font-weight:600;font-size:var(--p1);color:var(--black)}
    .cred-card .cred-detail{font-size:var(--p3);color:var(--gray-mid);margin-top:.25rem}

    /* ABOUT */
    .about-layout{display:grid;grid-template-columns:1fr 1fr;gap:4rem;margin-top:2rem;align-items:start}
    .about-text p{color:var(--gray-mid);line-height:1.8;margin-bottom:1.25rem;font-size:1.05rem}
    .about-sidebar{display:flex;flex-direction:column;gap:1rem}
    .about-stat{padding:1.25rem;background:var(--bg-card);border:1px solid var(--border)}
    .about-stat .stat-label{font-size:.65rem;letter-spacing:.2em;text-transform:uppercase;color:var(--orange);font-weight:700}
    .about-stat .stat-value{font-family:var(--serif);font-size:1.75rem;color:var(--black);margin-top:.25rem}
    .about-stat .stat-detail{font-size:var(--p3);color:var(--gray-mid);margin-top:.15rem}

    /* CONTACT */
    .contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:4rem;margin-top:2rem}
    .contact-info p{color:var(--gray-mid);margin-bottom:2rem;line-height:1.8}
    .contact-detail{padding:1rem 0;border-top:1px solid var(--border);display:flex;justify-content:space-between;align-items:center}
    .contact-detail .label{font-size:var(--p3);letter-spacing:.15em;text-transform:uppercase;color:var(--gray)}
    .dual-cta{display:flex;flex-direction:column;gap:1.25rem}
    .cta-block{padding:2rem;border:1px solid var(--border);background:var(--bg-card);transition:all .3s}
    .cta-block:hover{border-color:rgba(76,187,23,0.2);background:var(--bg-card-hover)}
    .cta-block .cta-label{font-size:.65rem;letter-spacing:.2em;text-transform:uppercase;color:var(--orange);font-weight:700;margin-bottom:.5rem}
    .cta-block h3{font-family:var(--serif);font-size:1.3rem;color:var(--black);margin-bottom:.5rem;font-weight:400}
    .cta-block p{font-size:var(--p2);color:var(--gray-mid);line-height:1.7}
    .availability{display:inline-block;background:rgba(76,187,23,0.1);color:var(--green-dark);padding:.5rem 1rem;font-size:var(--p3);font-weight:600;letter-spacing:.05em;text-transform:uppercase;margin-bottom:2rem}

    /* FOOTER */
    footer{padding:3rem 2rem;background:var(--bg-dark)}
    .footer-inner{max-width:var(--max-w);margin:0 auto;display:flex;justify-content:space-between;align-items:center}
    .footer-copy{display:flex;align-items:center;gap:1rem;font-size:var(--p3);color:var(--gray-mid)}
    .footer-logo-img{height:60px;width:auto;clip-path:inset(0 0 3% 0)}
    .footer-links{display:flex;gap:2rem}
    .footer-links a{font-size:var(--p3);color:var(--gray-mid)}
    .footer-links a:hover{color:var(--cream)}

    /* RESPONSIVE */
    @media(max-width:768px){
      .nav-links{display:none}
      .hamburger{display:block}
      .nav-links.active{display:flex;flex-direction:column;position:absolute;top:100%;left:0;right:0;background:rgba(255,255,255,0.97);backdrop-filter:blur(20px);padding:2rem;gap:1.25rem;border-bottom:1px solid var(--border)}
      .contact-grid{grid-template-columns:1fr;gap:2rem}
      .about-layout{grid-template-columns:1fr;gap:2rem}
      .service-grid{grid-template-columns:1fr}
      .detail-grid{grid-template-columns:1fr}
      .process-grid{grid-template-columns:1fr;gap:1.5rem}
      .cred-grid{grid-template-columns:1fr}
      .exp-header{flex-direction:column}
      .footer-inner{flex-direction:column;gap:1rem;text-align:center}
      .hero-links{flex-direction:column;align-items:flex-start}
    }

    /* ANIMATIONS */
    .fade-in{opacity:0;transform:translateY(24px);transition:opacity .7s ease,transform .7s ease}
    .fade-in.visible{opacity:1;transform:translateY(0)}
  </style>
</head>
<body>

  <!-- NAV -->
  <nav>
    <!-- ▼▼▼ PASTE ORIGINAL LOGO BASE64 STRING IN SRC BELOW ▼▼▼ -->
    <a href="#" class="nav-logo"><img src="data:image/png;base64,PASTE_LEMNOS_LOGO_BASE64_HERE" alt="Lemnos Consulting" class="nav-logo-img"></a>
    <!-- ▲▲▲ END LOGO ▲▲▲ -->
    <div class="nav-links" id="navLinks">
      <a href="#services">Services</a>
      <a href="#how">How It Works</a>
      <a href="#track-record">Track Record</a>
      <a href="#about">About</a>
      <a href="#contact" class="nav-cta">Get In Touch</a>
    </div>
    <button class="hamburger" id="hamburger" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
  </nav>

  <!-- HERO -->
  <header class="hero">
    <div class="hero-inner">
      <div class="hero-eyebrow">Fractional Marketing Operations</div>
      <h1>The marketing infrastructure your team needs but doesn't have time to <em>build.</em></h1>
      <p class="hero-sub">CRM, email, paid media, automation, data enrichment, and the reporting that connects it all. Lemnos builds the systems layer so your marketing actually works — without hiring a full-time ops team.</p>
      <div class="hero-links">
        <a href="#contact" class="btn-primary">Start a conversation</a>
        <a href="#services" class="btn-outline">See services</a>
      </div>
    </div>
  </header>

  <!-- SERVICES -->
  <section id="services" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Services</div>
      <h2 class="section-title">Five systems. One partner. No gaps in the middle.</h2>
      <p class="section-body">Most SMBs don't need five agencies. They need one person who knows how all the pieces connect and can build them properly.</p>

      <div class="service-grid">

        <div class="service-card">
          <div class="service-number">01 — CRM & Marketing Ops</div>
          <h3>CRM Setup, Administration & Data Governance</h3>
          <p>HubSpot builds from scratch — custom properties, deal pipelines, lifecycle stages, segmentation frameworks. Plus platform migrations, database cleanup, deduplication, normalization, and the lead status definitions that keep marketing and sales aligned.</p>
          <div class="service-tools">HubSpot · Apollo · Clay · ZoomInfo</div>
        </div>

        <div class="service-card">
          <div class="service-number">02 — MarTech Stack Management</div>
          <h3>Full Marketing Technology Ecosystem</h3>
          <p>Configuring and integrating tools across CRM, email, paid, display, social, and enrichment platforms — including the API, webhook, GTM, and Apps Script work that connects systems where out-of-the-box integrations fall short. Vendor evaluation and procurement, contract negotiation, and making sure everything actually talks to each other.</p>
          <div class="service-tools">HubSpot · Mailchimp · Constant Contact · Google Ads · StackAdapt · Meta · LinkedIn</div>
        </div>

        <div class="service-card">
          <div class="service-number">03 — Demand Gen & Lead Flow</div>
          <h3>Lead Qualification, Routing & Nurture Infrastructure</h3>
          <p>The systems that connect marketing activity to qualified pipeline. Lead qualification logic, routing rules, automated nurture sequences, and lifecycle stage models. Includes AI-powered enrichment pipelines — like a Clay-built workflow processing ~8,000 D&amp;B records through automated normalization, dual email verification, person enrichment, and LinkedIn matching.</p>
          <div class="service-tools">HubSpot · Apollo · Clay · ZoomInfo · Instantly</div>
        </div>

        <div class="service-card">
          <div class="service-number">04 — Performance Marketing</div>
          <h3>Paid Search, Display & Social Campaign Infrastructure</h3>
          <p>Campaign setup and management across paid search, programmatic display, and paid social. Account structure, audience targeting, creative rotation, budget allocation, retargeting workflows, and the attribution reporting that shows what's working.</p>
          <div class="service-tools">Google Ads · StackAdapt · Meta · LinkedIn</div>
        </div>

        <div class="service-card">
          <div class="service-number">05 — Email Infrastructure</div>
          <h3>Email Operations, Deliverability & Automation</h3>
          <p>Platform setup across cold outreach and nurture. Automation workflows, list segmentation, send scheduling, deliverability monitoring, ISP reputation management, and campaign QA. Notable: rescued a client's domain reputation through DNS configuration (SPF, DKIM, DMARC) and template rebuilds — open rates went from 2% to 35%.</p>
          <div class="service-tools">Acoustic · Mailchimp · Constant Contact · Instantly · Lemlist · ActiveCampaign</div>
        </div>

      </div>
    </div>
  </section>

  <!-- ADDITIONAL CAPABILITIES -->
  <section class="dark-section fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Also Included</div>
      <h2 class="section-title" style="color:var(--cream)">The stuff that ties everything together.</h2>
      <p class="section-body">These aren't separate services — they run through everything above.</p>

      <div class="detail-grid">
        <div class="detail-card">
          <div class="detail-label">Reporting</div>
          <h4>Dashboards & Analytics</h4>
          <p>BI reporting in Looker Studio connecting cross-channel data into dashboards your team can actually use. GA4 and GTM implementation.</p>
        </div>
        <div class="detail-card">
          <div class="detail-label">Data</div>
          <h4>Enrichment & Hygiene</h4>
          <p>Database cleanup, deduplication, normalization, and enrichment workflows with smart exclusion filters.</p>
        </div>
        <div class="detail-card">
          <div class="detail-label">Vendors</div>
          <h4>Tool Evaluation & Procurement</h4>
          <p>MarTech assessment, contract negotiation, onboarding, and integration. The right tools, configured properly.</p>
        </div>
        <div class="detail-card">
          <div class="detail-label">Alignment</div>
          <h4>Marketing-to-Sales Handoff</h4>
          <p>Lifecycle stage design, lead status definitions, MQL/SQL criteria, and structured handoff processes across teams.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- HOW IT WORKS -->
  <section id="how" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">How It Works</div>
      <h2 class="section-title">Fractional ops means you get the expertise without the overhead.</h2>
      <p class="section-body">Lemnos works as a fractional marketing operations partner — embedded in your team, owning the systems layer, without a full-time salary and benefits line item.</p>

      <div class="process-grid">
        <div class="process-step">
          <div class="process-num">01</div>
          <h3>Audit & Scope</h3>
          <p>We look at what you have, what's broken, and what's missing. No 40-page deck — just a clear picture of the infrastructure gaps and a plan to close them.</p>
        </div>
        <div class="process-step">
          <div class="process-num">02</div>
          <h3>Build & Configure</h3>
          <p>Hands-on implementation. CRM setup, platform integrations, automation workflows, campaign infrastructure, reporting — built and configured to your sales process.</p>
        </div>
        <div class="process-step">
          <div class="process-num">03</div>
          <h3>Run & Optimize</h3>
          <p>Ongoing operations, monitoring, and iteration. Deliverability management, data hygiene, campaign QA, reporting, and the vendor management that keeps the stack healthy.</p>
        </div>
      </div>
    </div>
  </section>

  <hr class="divider">

  <!-- TRACK RECORD -->
  <section id="track-record" class="dark-section fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Track Record</div>
      <h2 class="section-title" style="color:var(--cream)">8+ years of building the systems behind the marketing.</h2>

      <div class="exp-entry">
        <div class="exp-header">
          <div class="exp-title">Marketing Operations Consultant</div>
          <div class="exp-dates">Sep 2022 &ndash; Present</div>
        </div>
        <div class="exp-company">Lemnos Consulting LLC</div>
        <p class="exp-desc">Fractional marketing technology partner for SMBs across insurance, benefits, and professional services. Built and managed the full martech ecosystem — CRM, email, paid media, display, social, automation, and reporting — for multiple concurrent clients. Led CRM builds from scratch, platform migrations, database cleanup, lead qualification and routing systems, ad campaign infrastructure, and cross-channel BI reporting.</p>
        <p class="exp-desc">Designed a lead qualification and routing system for an insurance underwriting client using vendor-hosted forms to capture criteria, automatically match and route qualified leads, and sell unmatched leads to secondary carriers. Set up warm call transfers and retargeting email campaigns to maximize lead value.</p>
        <ul class="exp-highlights">
          <li>HubSpot</li><li>Google Ads</li><li>StackAdapt</li>
          <li>Meta</li><li>LinkedIn</li><li>Apollo</li><li>Clay</li><li>ZoomInfo</li>
          <li>Mailchimp</li><li>Constant Contact</li><li>Instantly</li><li>Lemlist</li>
          <li>Acoustic</li><li>Looker Studio</li><li>GA4</li><li>GTM</li>
          <li>Apps Script</li><li>API/webhooks</li>
        </ul>
      </div>

      <div class="exp-entry">
        <div class="exp-header">
          <div class="exp-title">Director, Digital Marketing & Analytics</div>
          <div class="exp-dates">Aug 2018 &ndash; Aug 2022</div>
        </div>
        <div class="exp-company">Good2Go Auto Insurance</div>
        <p class="exp-desc">Led the marketing technology ecosystem and digital operations for a high-volume D2C insurance brand. Managed a direct report and vendor partnerships across email, paid media, display, and social. Ran a 100K+ contact database in Acoustic with data feeds via SFTP. Executed multi-channel remarketing campaigns targeting cancelled policyholders — 2 to 5 concurrent campaigns with email volumes exceeding 100K sends per month.</p>
        <p class="exp-desc">Identified a brand reputation gap and integrated Trustpilot into the website, automated review collection via email, and partnered with sales leadership on a recognition program that improved morale, service quality, and social proof contributing to increased sales.</p>
        <ul class="exp-highlights">
          <li>Acoustic</li><li>Google Ads</li><li>StackAdapt</li>
          <li>Meta</li><li>LinkedIn</li><li>Trustpilot</li>
          <li>100K+ contacts</li><li>100K+ emails/mo</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- CREDENTIALS -->
  <section id="credentials" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Credentials</div>
      <h2 class="section-title">Education & Certifications</h2>
      <div class="cred-grid">
        <div class="cred-card"><div class="cred-label">Education</div><div class="cred-value">MBA, Strategic Management & Leadership</div><div class="cred-detail">Gwynedd Mercy University, 2019</div></div>
        <div class="cred-card"><div class="cred-label">Education</div><div class="cred-value">BS, Marketing</div><div class="cred-detail">Gwynedd Mercy University, 2018</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">HubSpot Marketing Hub Software</div><div class="cred-detail">HubSpot Academy</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">HubSpot Revenue Operations</div><div class="cred-detail">HubSpot Academy</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">Google Analytics 4</div><div class="cred-detail">Google</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">Google Ads (4 certifications)</div><div class="cred-detail">AI-Powered Performance, Shopping, Creative, Apps</div></div>
        <div class="cred-card"><div class="cred-label">Experience</div><div class="cred-value">8+ Years</div><div class="cred-detail">Marketing Operations</div></div>
      </div>
    </div>
  </section>

  <hr class="divider">

  <!-- ABOUT -->
  <section id="about" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">About</div>
      <h2 class="section-title">One person. The full stack.</h2>
      <div class="about-layout">
        <div class="about-text">
          <p>Lemnos Consulting is run by Pete Delago — a marketing technology specialist who's spent the last 8+ years building the CRM, email, paid media, automation, and reporting infrastructure that marketing teams rely on but rarely have someone dedicated to managing.</p>
          <p>Before Lemnos, Pete led digital marketing and analytics for Good2Go Auto Insurance, managing a 100K+ contact database, multi-channel remarketing campaigns, and the full ad tech vendor stack for a high-volume D2C brand.</p>
          <p>The consultancy exists because most SMBs need someone who can build the whole system — not just one platform. And they need it at a price point that doesn't require enterprise budgets.</p>
          <p>Pete is also open to full-time roles in marketing technology, marketing operations, demand generation, or growth operations for the right organization. <a href="https://petedelago.com" target="_blank">View the personal site &rarr;</a></p>
        </div>
        <div class="about-sidebar">
          <div class="about-stat">
            <div class="stat-label">Experience</div>
            <div class="stat-value">8+ Years</div>
            <div class="stat-detail">Marketing operations</div>
          </div>
          <div class="about-stat">
            <div class="stat-label">Platforms</div>
            <div class="stat-value">20+</div>
            <div class="stat-detail">MarTech tools configured & managed</div>
          </div>
          <div class="about-stat">
            <div class="stat-label">Industries</div>
            <div class="stat-value">Insurance, Benefits, Professional Services</div>
            <div class="stat-detail">SMB-focused across verticals</div>
          </div>
          <div class="about-stat">
            <div class="stat-label">Based In</div>
            <div class="stat-value">Lafayette Hill, PA</div>
            <div class="stat-detail">Working remotely</div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <section id="contact" class="fade-in" style="padding-bottom:4rem">
    <div class="section-inner">
      <div class="section-eyebrow">Get In Touch</div>
      <h2 class="section-title">Two reasons to reach out.</h2>
      <div class="contact-grid">
        <div class="contact-info">
          <div class="availability">Available Now</div>
          <p>Whether you need a fractional marketing ops partner or you're hiring for a full-time role — either way, the conversation starts the same.</p>
          <div class="contact-detail"><span class="label">Email</span><a href="mailto:pete@lemnos.io">pete@lemnos.io</a></div>
          <div class="contact-detail"><span class="label">Phone</span><span>(856) 905-2166</span></div>
          <div class="contact-detail"><span class="label">LinkedIn</span><a href="https://linkedin.com/in/pete-delago" target="_blank">linkedin.com/in/pete-delago</a></div>
          <div class="contact-detail"><span class="label">Location</span><span>Lafayette Hill, PA (Remote)</span></div>
        </div>
        <div class="dual-cta">
          <div class="cta-block">
            <div class="cta-label">For Clients</div>
            <h3>Need marketing infrastructure built?</h3>
            <p>Fractional marketing ops for SMBs. CRM, email, paid media, automation, reporting — scoped to what you actually need, at a price that works.</p>
          </div>
          <div class="cta-block">
            <div class="cta-label">For Hiring Managers</div>
            <h3>Looking for marketing technology talent?</h3>
            <p>Open to full-time roles in marketing technology, marketing operations, demand generation, or growth operations. <a href="https://petedelago.com" target="_blank">View resume site &rarr;</a></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-inner">
      <div class="footer-copy">
        <!-- ▼▼▼ PASTE ORIGINAL LOGO BASE64 STRING IN SRC BELOW ▼▼▼ -->
        <img src="data:image/png;base64,PASTE_LEMNOS_LOGO_BASE64_HERE" alt="Lemnos Consulting" class="footer-logo-img">
        <!-- ▲▲▲ END LOGO ▲▲▲ -->
        <span>&copy; 2026 Lemnos Consulting LLC</span>
      </div>
      <div class="footer-links">
        <a href="mailto:pete@lemnos.io">Email</a>
        <a href="https://linkedin.com/in/pete-delago" target="_blank">LinkedIn</a>
        <a href="https://petedelago.com" target="_blank">Pete Delago</a>
      </div>
    </div>
  </footer>

  <script>
    document.getElementById('hamburger').addEventListener('click',()=>{document.getElementById('navLinks').classList.toggle('active')});
    document.querySelectorAll('.nav-links a').forEach(l=>{l.addEventListener('click',()=>document.getElementById('navLinks').classList.remove('active'))});
    const obs=new IntersectionObserver(e=>{e.forEach(x=>{if(x.isIntersecting)x.target.classList.add('visible')})},{threshold:.1});
    document.querySelectorAll('.fade-in').forEach(el=>obs.observe(el));
  </script>

</body>
</html>
