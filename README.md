# devesh.github.io

<style>
@import url('https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500&display=swap');
*{box-sizing:border-box;margin:0;padding:0}
body{font-family:'DM Sans',sans-serif;color:var(--color-text-primary);background:transparent}
.port{max-width:860px;margin:0 auto;padding:1.5rem 1rem 3rem}
.hero{display:grid;grid-template-columns:1fr auto;gap:2rem;align-items:center;padding:2.5rem 2rem;background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);margin-bottom:1.5rem}
.hero-name{font-family:'DM Serif Display',serif;font-size:2.4rem;line-height:1.1;margin-bottom:.5rem}
.hero-title{font-size:1rem;font-weight:500;color:var(--color-text-info);margin-bottom:.75rem;letter-spacing:.04em}
.hero-bio{font-size:.9rem;color:var(--color-text-secondary);line-height:1.7;max-width:480px;margin-bottom:1.25rem}
.hero-tags{display:flex;flex-wrap:wrap;gap:8px}
.tag{font-size:.75rem;padding:4px 12px;border-radius:100px;background:var(--color-background-secondary);border:0.5px solid var(--color-border-tertiary);color:var(--color-text-secondary)}
.avatar{width:100px;height:100px;border-radius:50%;background:#185FA5;display:flex;align-items:center;justify-content:center;font-family:'DM Serif Display',serif;font-size:2rem;color:#E6F1FB;flex-shrink:0}
.metrics-row{display:grid;grid-template-columns:repeat(4,1fr);gap:12px;margin-bottom:1.5rem}
.m-card{background:var(--color-background-secondary);border-radius:var(--border-radius-md);padding:1rem;text-align:center}
.m-num{font-family:'DM Serif Display',serif;font-size:1.8rem;color:var(--color-text-primary);display:block}
.m-label{font-size:.75rem;color:var(--color-text-secondary);margin-top:4px;display:block}
.sec-title{font-family:'DM Serif Display',serif;font-size:1.25rem;margin-bottom:1rem;padding-bottom:.5rem;border-bottom:0.5px solid var(--color-border-tertiary)}
.sec{margin-bottom:2rem}
.case-grid{display:grid;grid-template-columns:1fr 1fr;gap:1rem}
.case-card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1.25rem;display:flex;flex-direction:column}
.case-tag{font-size:.7rem;font-weight:500;padding:3px 10px;border-radius:100px;display:inline-block;margin-bottom:.75rem;width:fit-content}
.tag-pm{background:#E6F1FB;color:#0C447C}
.tag-ba{background:#EAF3DE;color:#27500A}
.tag-data{background:#FAEEDA;color:#633806}
.case-title{font-family:'DM Serif Display',serif;font-size:1.05rem;margin-bottom:.5rem;line-height:1.3}
.case-prob{font-size:.82rem;color:var(--color-text-secondary);margin-bottom:.75rem;line-height:1.6}
.star-row{display:grid;grid-template-columns:1fr 1fr;gap:6px;margin-bottom:.75rem}
.star-item{font-size:.75rem;padding:6px 8px;background:var(--color-background-secondary);border-radius:var(--border-radius-md)}
.star-label{font-weight:500;color:var(--color-text-secondary);display:block;font-size:.68rem;text-transform:uppercase;letter-spacing:.06em;margin-bottom:2px}
.star-val{color:var(--color-text-primary)}
.impact-pill{margin-top:auto;padding-top:.75rem;border-top:0.5px solid var(--color-border-tertiary)}
.impact-num{font-family:'DM Serif Display',serif;font-size:1.4rem;color:#185FA5}
.impact-desc{font-size:.75rem;color:var(--color-text-secondary);margin-top:2px}
.artefacts{display:flex;flex-wrap:wrap;gap:6px;margin-top:.75rem}
.art-chip{font-size:.7rem;padding:3px 9px;border:0.5px solid var(--color-border-tertiary);border-radius:100px;color:var(--color-text-secondary)}
.skills-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
.skill-group{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1rem}
.sg-title{font-size:.8rem;font-weight:500;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:.08em;margin-bottom:.75rem}
.skill-pill{font-size:.78rem;padding:5px 10px;background:var(--color-background-secondary);border-radius:var(--border-radius-md);display:inline-block;margin:3px 3px 3px 0;color:var(--color-text-primary)}
.cert-row{display:grid;grid-template-columns:repeat(3,1fr);gap:1rem}
.cert-card{background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);padding:1rem;display:flex;align-items:center;gap:.75rem}
.cert-icon{width:36px;height:36px;border-radius:var(--border-radius-md);background:#E6F1FB;display:flex;align-items:center;justify-content:center;flex-shrink:0}
.cert-name{font-size:.82rem;font-weight:500;line-height:1.3}
.cert-body{font-size:.72rem;color:var(--color-text-secondary);margin-top:2px}
.contact-bar{display:flex;gap:1rem;align-items:center;padding:1.5rem 2rem;background:var(--color-background-primary);border:0.5px solid var(--color-border-tertiary);border-radius:var(--border-radius-lg);flex-wrap:wrap}
.contact-item{font-size:.85rem;color:var(--color-text-info);text-decoration:none;display:flex;align-items:center;gap:6px}
.resume-btn{margin-left:auto;font-size:.82rem;font-weight:500;padding:8px 20px;background:#185FA5;color:#E6F1FB;border:none;border-radius:var(--border-radius-md);cursor:pointer}
.dot{width:4px;height:4px;border-radius:50%;background:var(--color-border-secondary);flex-shrink:0}
@media(max-width:600px){
.case-grid,.skills-grid,.cert-row,.metrics-row{grid-template-columns:1fr}
.hero{grid-template-columns:1fr;text-align:center}.hero-tags{justify-content:center}.avatar{margin:0 auto}
}
</style>
<div class="port">
  <div class="hero">
    <div>
      <div style="font-size:.75rem;font-weight:500;color:var(--color-text-secondary);text-transform:uppercase;letter-spacing:.1em;margin-bottom:.5rem">Portfolio · Business Analyst & Product Manager</div>
      <div class="hero-name">Alex Morgan</div>
      <div class="hero-title">Senior BA / Associate PM · Open to new opportunities</div>
      <p class="hero-bio">Results-driven Business Analyst and Product Manager with 5+ years delivering digital transformation, data-driven insights, and customer-centric product experiences. Expert in bridging business needs and technical teams to ship products that matter.</p>
      <div class="hero-tags">
        <span class="tag">Agile / Scrum</span>
        <span class="tag">Product Roadmaps</span>
        <span class="tag">SQL & Power BI</span>
        <span class="tag">Stakeholder Management</span>
        <span class="tag">User Story Mapping</span>
        <span class="tag">JIRA · Confluence</span>
      </div>
    </div>
    <div class="avatar">AM</div>
  </div>

  <div class="metrics-row">
    <div class="m-card"><span class="m-num">5+</span><span class="m-label">Years experience</span></div>
    <div class="m-card"><span class="m-num">12</span><span class="m-label">Projects delivered</span></div>
    <div class="m-card"><span class="m-num">£2.4M</span><span class="m-label">Value generated</span></div>
    <div class="m-card"><span class="m-num">94%</span><span class="m-label">Stakeholder sat.</span></div>
  </div>

  <div class="sec">
    <div class="sec-title">Case studies</div>
    <div class="case-grid">

      <div class="case-card">
        <span class="case-tag tag-pm">Product Management</span>
        <div class="case-title">Customer Onboarding Portal Redesign</div>
        <p class="case-prob">Legacy portal drove 35% drop-off rate causing £600K annual churn. Tasked with full product discovery to launch.</p>
        <div class="star-row">
          <div class="star-item"><span class="star-label">Situation</span><span class="star-val">35% user drop-off, high support costs</span></div>
          <div class="star-item"><span class="star-label">Task</span><span class="star-val">Own discovery, prioritisation & roadmap</span></div>
          <div class="star-item"><span class="star-label">Action</span><span class="star-val">User interviews, journey mapping, MVP scoping</span></div>
          <div class="star-item"><span class="star-label">Result</span><span class="star-val">Launched in 3 sprints, measurable uplift</span></div>
        </div>
        <div class="artefacts">
          <span class="art-chip">PRD</span><span class="art-chip">Figma Prototype</span><span class="art-chip">Roadmap</span><span class="art-chip">OKRs</span>
        </div>
        <div class="impact-pill">
          <div class="impact-num">-40% drop-off</div>
          <div class="impact-desc">Onboarding completion rate up to 91% within 60 days of launch</div>
        </div>
      </div>

      <div class="case-card">
        <span class="case-tag tag-ba">Business Analysis</span>
        <div class="case-title">Supply Chain Process Re-engineering</div>
        <p class="case-prob">Manual procurement process causing 3-day delays and data inconsistencies across 4 regional teams.</p>
        <div class="star-row">
          <div class="star-item"><span class="star-label">Situation</span><span class="star-val">Manual, error-prone procurement workflow</span></div>
          <div class="star-item"><span class="star-label">Task</span><span class="star-val">Document AS-IS, design TO-BE process</span></div>
          <div class="star-item"><span class="star-label">Action</span><span class="star-val">Swimlane mapping, requirements, UAT</span></div>
          <div class="star-item"><span class="star-label">Result</span><span class="star-val">Automated end-to-end, £380K saved/yr</span></div>
        </div>
        <div class="artefacts">
          <span class="art-chip">BRD</span><span class="art-chip">Swimlane Diagram</span><span class="art-chip">UAT Plan</span><span class="art-chip">Gap Analysis</span>
        </div>
        <div class="impact-pill">
          <div class="impact-num">£380K saved/yr</div>
          <div class="impact-desc">Cycle time reduced from 72hrs to 8hrs across all regions</div>
        </div>
      </div>

      <div class="case-card">
        <span class="case-tag tag-data">Data & Analytics</span>
        <div class="case-title">Executive KPI Dashboard — Power BI</div>
        <p class="case-prob">C-suite relied on weekly Excel reports compiled manually, leading to 2-day data lag in strategic decisions.</p>
        <div class="star-row">
          <div class="star-item"><span class="star-label">Situation</span><span class="star-val">No real-time visibility for leadership team</span></div>
          <div class="star-item"><span class="star-label">Task</span><span class="star-val">Define KPIs, design self-serve dashboard</span></div>
          <div class="star-item"><span class="star-label">Action</span><span class="star-val">SQL data model, Power BI, stakeholder workshops</span></div>
          <div class="star-item"><span class="star-label">Result</span><span class="star-val">Live data for 200+ users, 0 manual reports</span></div>
        </div>
        <div class="artefacts">
          <span class="art-chip">SQL Model</span><span class="art-chip">Power BI</span><span class="art-chip">KPI Framework</span><span class="art-chip">Data Dictionary</span>
        </div>
        <div class="impact-pill">
          <div class="impact-num">200+ users</div>
          <div class="impact-desc">Eliminated 8hrs/week of manual reporting; real-time data latency</div>
        </div>
      </div>

      <div class="case-card">
        <span class="case-tag tag-pm">Product Management</span>
        <div class="case-title">B2B SaaS Feature Prioritisation & Launch</div>
        <p class="case-prob">Product backlog had 200+ items with no clear priority framework. Engineering team blocked by conflicting stakeholder demands.</p>
        <div class="star-row">
          <div class="star-item"><span class="star-label">Situation</span><span class="star-val">Unranked backlog, no delivery cadence</span></div>
          <div class="star-item"><span class="star-label">Task</span><span class="star-val">Build prioritisation framework & quarterly plan</span></div>
          <div class="star-item"><span class="star-label">Action</span><span class="star-val">RICE scoring, MoSCoW, sprint ceremonies</span></div>
          <div class="star-item"><span class="star-label">Result</span><span class="star-val">3 features shipped, NPS +22 points</span></div>
        </div>
        <div class="artefacts">
          <span class="art-chip">Roadmap</span><span class="art-chip">RICE Matrix</span><span class="art-chip">User Stories</span><span class="art-chip">Release Notes</span>
        </div>
        <div class="impact-pill">
          <div class="impact-num">NPS +22 pts</div>
          <div class="impact-desc">3 high-value features shipped in Q3; velocity up 30%</div>
        </div>
      </div>

    </div>
  </div>

  <div class="sec">
    <div class="sec-title">Skills & tools</div>
    <div class="skills-grid">
      <div class="skill-group">
        <div class="sg-title">BA Methods</div>
        <span class="skill-pill">Requirements Elicitation</span>
        <span class="skill-pill">BRD / FRD Writing</span>
        <span class="skill-pill">Gap Analysis</span>
        <span class="skill-pill">Process Mapping</span>
        <span class="skill-pill">UAT Planning</span>
        <span class="skill-pill">Use Case Modelling</span>
      </div>
      <div class="skill-group">
        <div class="sg-title">PM Methods</div>
        <span class="skill-pill">Agile / Scrum</span>
        <span class="skill-pill">Product Roadmaps</span>
        <span class="skill-pill">OKR Framework</span>
        <span class="skill-pill">RICE / MoSCoW</span>
        <span class="skill-pill">User Story Mapping</span>
        <span class="skill-pill">A/B Testing</span>
      </div>
      <div class="skill-group">
        <div class="sg-title">Tools & tech</div>
        <span class="skill-pill">JIRA & Confluence</span>
        <span class="skill-pill">Figma</span>
        <span class="skill-pill">Power BI</span>
        <span class="skill-pill">SQL</span>
        <span class="skill-pill">Miro</span>
        <span class="skill-pill">Excel / Sheets</span>
        <span class="skill-pill">Salesforce</span>
      </div>
    </div>
  </div>

  <div class="sec">
    <div class="sec-title">Certifications</div>
    <div class="cert-row">
      <div class="cert-card">
        <div class="cert-icon">
          <svg width="18" height="18" viewBox="0 0 18 18" fill="none"><circle cx="9" cy="9" r="8" stroke="#185FA5" stroke-width="1.5"/><path d="M6 9l2 2 4-4" stroke="#185FA5" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
        <div><div class="cert-name">CBAP — Certified BA Professional</div><div class="cert-body">IIBA · 2023</div></div>
      </div>
      <div class="cert-card">
        <div class="cert-icon">
          <svg width="18" height="18" viewBox="0 0 18 18" fill="none"><circle cx="9" cy="9" r="8" stroke="#185FA5" stroke-width="1.5"/><path d="M6 9l2 2 4-4" stroke="#185FA5" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
        <div><div class="cert-name">Professional Scrum Master I</div><div class="cert-body">Scrum.org · 2022</div></div>
      </div>
      <div class="cert-card">
        <div class="cert-icon">
          <svg width="18" height="18" viewBox="0 0 18 18" fill="none"><circle cx="9" cy="9" r="8" stroke="#185FA5" stroke-width="1.5"/><path d="M6 9l2 2 4-4" stroke="#185FA5" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/></svg>
        </div>
        <div><div class="cert-name">Google PM Certificate</div><div class="cert-body">Coursera · 2023</div></div>
      </div>
    </div>
  </div>

  <div class="contact-bar">
    <a class="contact-item" href="#">
      <svg width="14" height="14" viewBox="0 0 16 16" fill="currentColor"><path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z"/></svg>
      linkedin.com/in/alexmorgan
    </a>
    <div class="dot"></div>
    <a class="contact-item" href="#">
      <svg width="14" height="14" viewBox="0 0 16 16" fill="currentColor"><path d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555zM0 4.697v7.104l5.803-3.558L0 4.697zM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757zm3.436-.586L16 11.801V4.697l-5.803 3.546z"/></svg>
      alex.morgan@email.com
    </a>
    <div class="dot"></div>
    <a class="contact-item" href="#">
      <svg width="14" height="14" viewBox="0 0 16 16" fill="currentColor"><path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"/></svg>
      github.com/alexmorgan
    </a>
    <button class="resume-btn" onclick="sendPrompt('Help me create a PDF version of this portfolio')">Download CV ↗</button>
  </div>
</div>
