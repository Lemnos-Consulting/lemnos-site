<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Pete Delago | Marketing Technology & Operations</title>
  <meta name="description" content="Pete Delago — marketing technology specialist with 8+ years building martech infrastructure from scratch for SMBs. Deep HubSpot, custom integrations and code, data architecture, AI-powered workflows, and the lifecycle systems that feed pipeline.">
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
      --serif: 'Bebas Neue', sans-serif;
      --sans: 'Outfit', -apple-system, sans-serif;
      --max-w:1120px
    }
    html{scroll-behavior:smooth}
    body{font-family:var(--sans);background:var(--bg);color:var(--text);line-height:1.7;font-size:var(--p1);-webkit-font-smoothing:antialiased}
    ::selection{background:var(--green);color:var(--white)}
    a{color:var(--green-dark);text-decoration:none;transition:color .2s}
    a:hover{color:var(--green)}

    nav{position:fixed;top:0;left:0;right:0;z-index:100;padding:1.25rem 2rem;display:flex;justify-content:space-between;align-items:center;background:rgba(255,255,255,0.9);backdrop-filter:blur(20px);border-bottom:1px solid var(--border)}
    .nav-logo{font-family:var(--sans);font-weight:700;font-size:1.1rem;letter-spacing:.08em;color:var(--black)}
    .nav-logo span{color:var(--green)}
    .nav-links{display:flex;gap:2rem;align-items:center}
    .nav-links a{color:var(--black);font-size:var(--p3);letter-spacing:.05em;text-transform:uppercase;font-weight:500}
    .nav-links a:hover{color:var(--black)}
    .nav-cta{background:var(--green);color:var(--white);padding:.5rem 1.25rem;font-size:.8rem;font-weight:600;letter-spacing:.05em;text-transform:uppercase;border:none;cursor:pointer;transition:all .2s}
    .nav-cta:hover{background:var(--green-dark);color:var(--white)}
    .hamburger{display:none;background:none;border:none;cursor:pointer;padding:.5rem}
    .hamburger span{display:block;width:22px;height:2px;background:var(--black);margin:5px 0;transition:all .3s}

    .hero{min-height:100vh;display:flex;flex-direction:column;justify-content:center;padding:8rem 2rem 6rem;background:var(--bg-dark);color:var(--cream)}
    .hero-inner{max-width:var(--max-w);margin:0 auto;width:100%}
    .hero-eyebrow{font-size:var(--p3);letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:1.5rem;font-weight:500}
    .hero h1{font-family:var(--serif);font-size:clamp(2.8rem,6vw,var(--h1));line-height:1.1;font-weight:400;max-width:820px;margin-bottom:2rem;color:var(--cream)}
    .hero h1 em{font-style:italic;color:var(--green)}
    .hero-sub{font-size:1.15rem;color:var(--gray);max-width:640px;line-height:1.8;margin-bottom:3rem}
    .hero-links{display:flex;gap:1.5rem;flex-wrap:wrap;align-items:center}
    .btn-primary{display:inline-block;background:var(--green);color:var(--white);padding:.9rem 2.25rem;font-size:var(--p3);font-weight:600;letter-spacing:.08em;text-transform:uppercase;transition:all .2s;border:none;cursor:pointer}
    .btn-primary:hover{background:var(--green-dark);color:var(--white)}
    .btn-outline{display:inline-block;border:1px solid var(--gray-mid);color:var(--gray);padding:.85rem 2.25rem;font-size:var(--p3);font-weight:600;letter-spacing:.08em;text-transform:uppercase;transition:all .2s}
    .btn-outline:hover{border-color:var(--cream);color:var(--cream)}

    section{padding:6rem 2rem}
    .section-inner{max-width:var(--max-w);margin:0 auto}
    .section-eyebrow{font-size:var(--p3);letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:1rem;font-weight:600}
    .section-title{font-family:var(--serif);font-size:clamp(2rem,4vw,var(--h2));line-height:1.15;font-weight:400;margin-bottom:1.5rem;max-width:700px;color:var(--black)}
    .section-body{color:var(--gray-mid);max-width:640px;font-size:1.05rem;line-height:1.8}
    .section-body+.section-body{margin-top:1.25rem}
    .dark-section{background:var(--bg-dark);color:var(--cream)}
    .dark-section .section-title{color:var(--cream)}
    .dark-section .section-body{color:var(--gray)}
    .dark-section .section-eyebrow{color:var(--green)}
    .divider{max-width:var(--max-w);margin:0 auto;border:none;border-top:1px solid var(--border)}

    .card-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:1.5rem;margin-top:3rem}
    .card{background:var(--bg-card);border:1px solid var(--border);padding:2.25rem;transition:all .3s}
    .card:hover{background:var(--bg-card-hover);border-color:rgba(76,187,23,0.2)}
    .card-label{font-size:.7rem;letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:.75rem;font-weight:700}
    .card h3{font-family:var(--serif);font-size:var(--h5);font-weight:400;margin-bottom:1rem;line-height:1.3;color:var(--black)}
    .card p{color:var(--gray-mid);font-size:var(--p2);line-height:1.7}
    .card .tools{margin-top:1.25rem;font-size:var(--p3);color:var(--green-dark);font-weight:500}

    .exp-entry{margin-top:3rem;padding-bottom:3rem;border-bottom:1px solid var(--border-dark)}
    .exp-entry:last-child{border-bottom:none;padding-bottom:0}
    .exp-header{display:flex;justify-content:space-between;align-items:baseline;flex-wrap:wrap;gap:.5rem;margin-bottom:.5rem}
    .exp-title{font-family:var(--serif);font-size:var(--h5);color:var(--cream)}
    .exp-dates{font-size:var(--p3);color:var(--gray-mid);letter-spacing:.05em}
    .exp-company{font-size:var(--p2);color:var(--green);font-weight:500;margin-bottom:1rem}
    .exp-desc{color:var(--gray);font-size:var(--p2);line-height:1.8;margin-bottom:1rem}
    .exp-highlights{list-style:none;display:flex;flex-wrap:wrap;gap:.5rem}
    .exp-highlights li{font-size:var(--p3);color:var(--gray-mid);background:rgba(255,255,255,0.05);border:1px solid var(--border-dark);padding:.3rem .75rem}

    .cred-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:1.5rem;margin-top:2rem}
    .cred-card{background:var(--bg-card);border:1px solid var(--border);padding:1.75rem}
    .cred-card .cred-label{font-size:.7rem;letter-spacing:.2em;text-transform:uppercase;color:var(--green);margin-bottom:.5rem;font-weight:700}
    .cred-card .cred-value{font-weight:600;font-size:var(--p1);color:var(--black)}
    .cred-card .cred-detail{font-size:var(--p3);color:var(--gray-mid);margin-top:.25rem}

    .contact-grid{display:grid;grid-template-columns:1fr 1fr;gap:4rem;margin-top:2rem}
    .contact-info p{color:var(--gray-mid);margin-bottom:2rem;line-height:1.8}
    .contact-detail{padding:1rem 0;border-top:1px solid var(--border);display:flex;justify-content:space-between;align-items:center}
    .contact-detail .label{font-size:var(--p3);letter-spacing:.15em;text-transform:uppercase;color:var(--gray)}
    .availability{display:inline-block;background:rgba(76,187,23,0.1);color:var(--green-dark);padding:.5rem 1rem;font-size:var(--p3);font-weight:600;letter-spacing:.05em;text-transform:uppercase;margin-bottom:2rem}
    .role-card{padding:1rem 1.25rem;background:var(--bg-card);border:1px solid var(--border)}
    .role-card .role-title{font-weight:600;color:var(--black)}
    .role-card .role-desc{font-size:var(--p3);color:var(--gray-mid);margin-top:.25rem}
    .role-list{display:flex;flex-direction:column;gap:.75rem}
    .role-list-heading{font-size:var(--p1);font-weight:600;color:var(--black);margin-bottom:1rem}

    footer{padding:3rem 2rem;background:var(--bg-dark);border-top:1px solid var(--border-dark)}
    .footer-inner{max-width:var(--max-w);margin:0 auto;display:flex;justify-content:space-between;align-items:center}
    .footer-copy{font-size:var(--p3);color:var(--gray-mid)}
    .footer-links{display:flex;gap:2rem}
    .footer-links a{font-size:var(--p3);color:var(--gray-mid)}
    .footer-links a:hover{color:var(--cream)}

    @media(max-width:768px){
      .nav-links{display:none}
      .hamburger{display:block}
      .nav-links.active{display:flex;flex-direction:column;position:absolute;top:100%;left:0;right:0;background:rgba(255,255,255,0.97);backdrop-filter:blur(20px);padding:2rem;gap:1.25rem;border-bottom:1px solid var(--border)}
      .contact-grid{grid-template-columns:1fr;gap:2rem}
      .card-grid{grid-template-columns:1fr}
      .cred-grid{grid-template-columns:1fr}
      .exp-header{flex-direction:column}
      .footer-inner{flex-direction:column;gap:1rem;text-align:center}
      .hero-links{flex-direction:column;align-items:flex-start}
    }

    .fade-in{opacity:0;transform:translateY(24px);transition:opacity .7s ease,transform .7s ease}
    .fade-in.visible{opacity:1;transform:translateY(0)}
  </style>
</head>
<body>

  <!-- NAV -->
  <nav>
    <a href="#" class="nav-logo">Pete <span>Delago</span></a>
    <div class="nav-links" id="navLinks">
      <a href="#expertise">Expertise</a>
      <a href="#experience">Experience</a>
      <a href="#credentials">Credentials</a>
      <a href="#contact" class="nav-cta">Get In Touch</a>
    </div>
    <button class="hamburger" id="hamburger" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
  </nav>

  <!-- HERO -->
  <header class="hero">
    <div class="hero-inner">
      <div class="hero-eyebrow">Marketing Technology & Operations</div>
      <h1>I build the marketing <em>infrastructure</em> that makes everything else work.</h1>
      <p class="hero-sub">8+ years walking into fragmented or nonexistent martech stacks and standing them up from zero. Deep HubSpot, custom API/webhook/Apps Script integrations, data architecture, AI-powered workflows, and the lifecycle systems that feed pipeline.</p>
      <div class="hero-links">
        <a href="#contact" class="btn-primary">Get in touch</a>
        <a href="https://linkedin.com/in/pete-delago" target="_blank" class="btn-outline">LinkedIn</a>
      </div>
    </div>
  </header>

  <!-- WHAT I DO -->
  <section id="expertise" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">What I Do</div>
      <h2 class="section-title">Build it from scratch. Operate it day-to-day.</h2>
      <p class="section-body">Most teams don't need someone to operate an existing stack — they need someone who can build what isn't there yet, write the custom code where out-of-the-box falls short, and run it. That's the work.</p>

      <div class="card-grid">

        <div class="card">
          <div class="card-label">Build</div>
          <h3>Building Martech From Scratch</h3>
          <p>I walk into fragmented or nonexistent stacks and stand up the architecture from zero. HubSpot rebuilds across Marketing Hub and Sales Hub — custom properties, deal pipelines, lifecycle stages, governance frameworks. Plus the documentation and operating models that let the system survive after I'm gone.</p>
          <div class="tools">HubSpot Marketing Hub + Sales Hub, system architecture</div>
        </div>

        <div class="card">
          <div class="card-label">Code</div>
          <h3>Custom Integrations & Automation</h3>
          <p>Where out-of-the-box integrations fall short, I write the connection. API integrations, webhooks, custom GTM events, and Apps Script automations to wire HubSpot up to enrichment platforms, ad networks, third-party sales tools, and analytics.</p>
          <div class="tools">API, Webhooks, GTM, Apps Script, GitHub</div>
        </div>

        <div class="card">
          <div class="card-label">Data</div>
          <h3>Data Architecture & Governance</h3>
          <p>Property design, deduplication, normalization, validation logic, and enrichment pipelines with smart exclusion filters. The discipline behind segmentation that actually targets and reporting that's trustworthy.</p>
          <div class="tools">Clay, Apollo, ZoomInfo</div>
        </div>

        <div class="card">
          <div class="card-label">AI</div>
          <h3>AI-Powered Marketing Workflows</h3>
          <p>AI agents and LLM-powered workflows integrated into daily operations to eliminate manual work and scale output. Including a Clay-built enrichment pipeline that processed ~8,000 D&amp;B records through automated normalization, dual email verification, person enrichment, and LinkedIn matching.</p>
          <div class="tools">Clay, LLM workflows, AI agents</div>
        </div>

        <div class="card">
          <div class="card-label">Funnel</div>
          <h3>Lifecycle, Lead Scoring & Routing</h3>
          <p>Lifecycle stage models with scoring criteria and MQL/SQL handoff SLAs. Routing rules that get the right leads to the right people at the right time. Nurture programs tied to behavior and lifecycle stage.</p>
          <div class="tools">HubSpot workflows, scoring frameworks</div>
        </div>

        <div class="card">
          <div class="card-label">Email</div>
          <h3>Email Deliverability & Operations</h3>
          <p>DNS configuration (SPF, DKIM, DMARC), template hygiene, list segmentation, ISP reputation management, automation logic. Notable: rescued a client's domain reputation through DNS config and template rebuilds — open rates went from 2% to 35%.</p>
          <div class="tools">Acoustic, Mailchimp, Constant Contact, Instantly, Lemlist</div>
        </div>

        <div class="card">
          <div class="card-label">Reporting</div>
          <h3>Campaign Ops & Pipeline Attribution</h3>
          <p>UTM governance, CRM campaign structure, multi-channel campaign infrastructure across paid search, display, paid social, and email. GA4 built from scratch, Looker Studio dashboards giving leadership the pipeline visibility they can act on.</p>
          <div class="tools">Google Ads, Meta, LinkedIn, StackAdapt, GA4, GTM, Looker Studio</div>
        </div>

      </div>
    </div>
  </section>

  <hr class="divider">

  <!-- EXPERIENCE -->
  <section id="experience" class="dark-section fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Where I've Done It</div>
      <h2 class="section-title" style="color:var(--cream)">8+ years building the systems behind the marketing.</h2>

      <div class="exp-entry">
        <div class="exp-header">
          <div class="exp-title">Marketing Technology & Operations Consultant</div>
          <div class="exp-dates">Sep 2022 &ndash; Present</div>
        </div>
        <div class="exp-company">Lemnos Consulting LLC</div>
        <p class="exp-desc">Fractional marketing operations partner for SMBs — building marketing technology infrastructure from scratch, owning systems and data governance, and operating the full stack day-to-day to connect marketing activity to pipeline. Stood up HubSpot CRM instances from zero across Marketing Hub and Sales Hub. Wrote API integrations, webhooks, and custom GTM/Apps Script code to connect HubSpot to third-party tools. Designed lifecycle and lead scoring models, deployed AI-powered enrichment pipelines, and trained client teams on HubSpot ops.</p>
        <ul class="exp-highlights">
          <li>HubSpot</li><li>API/webhooks</li><li>Apps Script</li><li>GTM</li>
          <li>Clay</li><li>Apollo</li><li>ZoomInfo</li>
          <li>Google Ads</li><li>StackAdapt</li><li>Meta</li><li>LinkedIn</li>
          <li>Mailchimp</li><li>Constant Contact</li><li>Instantly</li><li>Lemlist</li>
          <li>GA4</li><li>Looker Studio</li>
        </ul>
      </div>

      <div class="exp-entry">
        <div class="exp-header">
          <div class="exp-title">Director, Digital Marketing & Analytics</div>
          <div class="exp-dates">Aug 2018 &ndash; Aug 2022</div>
        </div>
        <div class="exp-company">Good2Go Auto Insurance</div>
        <p class="exp-desc">Led digital marketing operations, data infrastructure, and analytics for a high-volume D2C insurance brand. Managed a direct report and external vendor partnerships across email, paid media, display, and social. Ran a 100K+ contact database in Acoustic with Salesforce data feeds via SFTP. Executed multi-channel remarketing campaigns targeting cancelled policyholders at 100K+ monthly email sends. Built GA4 from scratch and centralized cross-channel reporting in Looker Studio. Integrated Trustpilot to solve a brand reputation gap, automated review collection, and partnered with sales on a recognition program that improved morale, social proof, and service quality.</p>
        <ul class="exp-highlights">
          <li>Acoustic</li><li>Salesforce (SFTP)</li>
          <li>Google Ads</li><li>StackAdapt</li><li>Meta</li><li>LinkedIn</li>
          <li>Trustpilot</li><li>GA4</li><li>Looker Studio</li>
          <li>100K+ contacts</li><li>100K+ emails/mo</li>
        </ul>
      </div>
    </div>
  </section>

  <!-- CREDENTIALS -->
  <section id="credentials" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Background</div>
      <h2 class="section-title">Education & Certifications</h2>
      <div class="cred-grid">
        <div class="cred-card"><div class="cred-label">Education</div><div class="cred-value">MBA, Strategic Management & Leadership</div><div class="cred-detail">Gwynedd Mercy University, 2019</div></div>
        <div class="cred-card"><div class="cred-label">Education</div><div class="cred-value">BS, Marketing</div><div class="cred-detail">Gwynedd Mercy University, 2018</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">HubSpot Marketing Hub Software</div><div class="cred-detail">HubSpot Academy</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">HubSpot Revenue Operations</div><div class="cred-detail">HubSpot Academy</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">Google Analytics 4</div><div class="cred-detail">Google</div></div>
        <div class="cred-card"><div class="cred-label">Certification</div><div class="cred-value">Google Ads (4 certifications)</div><div class="cred-detail">AI-Powered Performance, Shopping, Creative, Apps</div></div>
        <div class="cred-card"><div class="cred-label">Experience</div><div class="cred-value">8+ Years</div><div class="cred-detail">Marketing Technology & Operations</div></div>
      </div>
    </div>
  </section>

  <hr class="divider">

  <!-- CONTACT -->
  <section id="contact" class="fade-in">
    <div class="section-inner">
      <div class="section-eyebrow">Let's Connect</div>
      <h2 class="section-title">Looking for my next role.</h2>
      <div class="contact-grid">
        <div class="contact-info">
          <div class="availability">Open to Opportunities</div>
          <p>I'm looking for a full-time role where I can own the martech function — ideally for an organization with an immature or fragmented stack that needs someone to build, integrate, and operate the whole system. Remote preferred. If you're hiring for marketing technology, marketing operations, demand generation, or campaign/growth operations, I'd like to hear about it.</p>
          <div class="contact-detail"><span class="label">Email</span><a href="mailto:pete@lemnos.io">pete@lemnos.io</a></div>
          <div class="contact-detail"><span class="label">Phone</span><span>(856) 905-2166</span></div>
          <div class="contact-detail"><span class="label">LinkedIn</span><a href="https://linkedin.com/in/pete-delago" target="_blank">linkedin.com/in/pete-delago</a></div>
          <div class="contact-detail"><span class="label">Location</span><span>Lafayette Hill, PA (Remote)</span></div>
        </div>
        <div>
          <div class="role-list-heading">Target roles:</div>
          <div class="role-list">
            <div class="role-card">
              <div class="role-title">Marketing Technology Manager</div>
              <div class="role-desc">Full-stack martech ownership across CRM, email, paid, display, automation</div>
            </div>
            <div class="role-card">
              <div class="role-title">Demand Generation Operations</div>
              <div class="role-desc">Lead flow, enrichment, nurture, routing, multi-channel pipeline</div>
            </div>
            <div class="role-card">
              <div class="role-title">Campaign Operations Manager</div>
              <div class="role-desc">Campaign execution, infrastructure, QA, and tracking across email, paid, and lifecycle programs</div>
            </div>
            <div class="role-card">
              <div class="role-title">Growth Operations Manager</div>
              <div class="role-desc">Growth systems, experimentation, funnel optimization, lifecycle programs</div>
            </div>
            <div class="role-card">
              <div class="role-title">Digital Marketing Manager</div>
              <div class="role-desc">Multi-channel digital execution: paid search, display, social, email, web</div>
            </div>
            <div class="role-card">
              <div class="role-title">Marketing Operations Manager</div>
              <div class="role-desc">CRM administration, workflows, lifecycle design, data governance</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <footer>
    <div class="footer-inner">
      <div class="footer-copy">&copy; 2026 Pete Delago</div>
      <div class="footer-links">
        <a href="mailto:pete@lemnos.io">Email</a>
        <a href="https://linkedin.com/in/pete-delago" target="_blank">LinkedIn</a>
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
