<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&family=DM+Sans:wght@300;400;500;600&display=swap');
  * { box-sizing: border-box; margin: 0; padding: 0; }
  :root {
    --accent: #E63946;
    --accent2: #FF9F1C;
    --bg: #0D0D0D;
    --surface: #161616;
    --surface2: #1F1F1F;
    --border: rgba(255,255,255,0.08);
    --text: #F0EDE8;
    --muted: #888580;
    --mono: 'Space Mono', monospace;
    --sans: 'DM Sans', sans-serif;
  }
  body, .root { background: var(--bg); color: var(--text); font-family: var(--sans); }
  .root { padding: 2rem 1.5rem; max-width: 720px; margin: 0 auto; }

  .header { margin-bottom: 2.5rem; position: relative; }
  .name-row { display: flex; align-items: baseline; gap: 12px; flex-wrap: wrap; }
  .name { font-family: var(--mono); font-size: clamp(1.6rem, 5vw, 2.4rem); font-weight: 700; color: var(--text); letter-spacing: -0.02em; }
  .tag { font-family: var(--mono); font-size: 11px; background: var(--accent); color: #fff; padding: 3px 8px; border-radius: 3px; letter-spacing: 0.08em; text-transform: uppercase; vertical-align: middle; }
  .tagline { font-size: 14px; color: var(--muted); margin-top: 6px; font-weight: 300; letter-spacing: 0.03em; }
  .meta { display: flex; gap: 16px; flex-wrap: wrap; margin-top: 10px; }
  .meta-item { font-size: 12px; color: var(--muted); font-family: var(--mono); }
  .meta-item span { color: var(--accent2); }

  .divider { height: 1px; background: var(--border); margin: 0 0 2rem; }

  .section { margin-bottom: 2rem; }
  .section-label { font-family: var(--mono); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; color: var(--accent); margin-bottom: 12px; }
  .bio { font-size: 14px; line-height: 1.75; color: #C8C5BF; font-weight: 300; }
  .bio strong { color: var(--text); font-weight: 500; }

  .focus-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(160px, 1fr)); gap: 8px; margin-top: 10px; }
  .focus-chip { background: var(--surface); border: 0.5px solid var(--border); border-radius: 6px; padding: 10px 12px; font-size: 12px; color: #C8C5BF; font-family: var(--mono); }
  .focus-chip::before { content: '→ '; color: var(--accent); }

  .project-list { display: flex; flex-direction: column; gap: 10px; }
  .project-card { background: var(--surface); border: 0.5px solid var(--border); border-radius: 8px; padding: 14px 16px; border-left: 2px solid var(--accent); }
  .project-card:nth-child(2) { border-left-color: var(--accent2); }
  .project-card:nth-child(3) { border-left-color: #5BC0BE; }
  .project-title { font-family: var(--mono); font-size: 13px; font-weight: 700; color: var(--text); margin-bottom: 5px; }
  .project-desc { font-size: 12px; color: var(--muted); line-height: 1.6; }
  .project-tags { display: flex; gap: 6px; flex-wrap: wrap; margin-top: 8px; }
  .ptag { font-size: 10px; font-family: var(--mono); background: var(--surface2); border: 0.5px solid var(--border); border-radius: 3px; padding: 2px 7px; color: #888; }

  .stack-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(100px, 1fr)); gap: 8px; }
  .stack-item { background: var(--surface); border: 0.5px solid var(--border); border-radius: 6px; padding: 8px 12px; font-family: var(--mono); font-size: 11px; color: #C8C5BF; text-align: center; }

  .ach-list { display: flex; flex-direction: column; gap: 8px; }
  .ach-item { display: flex; align-items: center; gap: 10px; font-size: 13px; color: #C8C5BF; }
  .ach-dot { width: 6px; height: 6px; border-radius: 50%; background: var(--accent2); flex-shrink: 0; }

  .connect-row { display: flex; gap: 10px; flex-wrap: wrap; margin-top: 8px; }
  .connect-btn { font-family: var(--mono); font-size: 11px; border: 0.5px solid var(--border); border-radius: 5px; padding: 7px 14px; color: var(--muted); background: var(--surface); text-decoration: none; cursor: pointer; }
  .connect-btn:hover { border-color: var(--accent); color: var(--accent); }

  .racing-bar { background: linear-gradient(90deg, var(--accent) 0%, var(--accent2) 100%); height: 2px; border-radius: 1px; margin-bottom: 2rem; }
</style>

<div class="root">
  <div class="racing-bar"></div>

  <div class="header">
    <div class="name-row">
      <span class="name">Naval Agarwal</span>
      <span class="tag">2nd Year</span>
    </div>
    <div class="tagline">CSE (AI/ML) · Autonomous Systems Engineer · ML & Systems Builder</div>
    <div class="meta">
      <span class="meta-item"><span>@</span> VIT Vellore</span>
      <span class="meta-item"><span>⚡</span> Team Ojas Racing — Formula Student EV</span>
      <span class="meta-item"><span>📍</span> Mumbai, India</span>
    </div>
  </div>

  <div class="divider"></div>

  <div class="section">
    <div class="section-label">About</div>
    <p class="bio">
      I build systems that <strong>make decisions</strong> — not just interfaces. My work sits at the intersection of <strong>autonomous systems</strong>, machine learning, and real-time C++ engineering. Currently developing perception and decision pipelines for a Formula Student EV at <strong>Team Ojas Racing</strong>.
    </p>
    <div class="focus-grid" style="margin-top:14px;">
      <div class="focus-chip">Autonomous Systems</div>
      <div class="focus-chip">Explainable AI</div>
      <div class="focus-chip">Systems C++</div>
      <div class="focus-chip">Decision Models</div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Autonomous Engineering @ Ojas Racing</div>
    <div class="focus-grid">
      <div class="focus-chip">ROS2 Architecture</div>
      <div class="focus-chip">Sensor Fusion</div>
      <div class="focus-chip">Perception Pipelines</div>
      <div class="focus-chip">Safety-Critical RT</div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Selected Projects</div>
    <div class="project-list">
      <div class="project-card">
        <div class="project-title">Internal Data Leak Risk Detector</div>
        <div class="project-desc">ML-based behavioral prediction system evaluating insider threat likelihood using behavioral baselines, psychometric features, and multi-factor risk scoring.</div>
        <div class="project-tags">
          <span class="ptag">behavioral-ml</span>
          <span class="ptag">risk-scoring</span>
          <span class="ptag">psychometrics</span>
        </div>
      </div>
      <div class="project-card">
        <div class="project-title">Scrape-Krunch</div>
        <div class="project-desc">Real-time multi-domain news scraper feeding structured data into a locally hosted LLM (Ollama) for contextual summarization and analysis.</div>
        <div class="project-tags">
          <span class="ptag">web-scraping</span>
          <span class="ptag">ollama</span>
          <span class="ptag">llm-pipeline</span>
        </div>
      </div>
      <div class="project-card">
        <div class="project-title">Adaptive Loan Repayment Scheduler</div>
        <div class="project-desc">Dynamic priority-based loan optimization engine in C++ — evaluates multiple loans simultaneously using multi-factor decision logic for optimal repayment sequencing.</div>
        <div class="project-tags">
          <span class="ptag">c++</span>
          <span class="ptag">optimization</span>
          <span class="ptag">decision-systems</span>
        </div>
      </div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Tech Stack</div>
    <div class="stack-grid">
      <div class="stack-item">Python</div>
      <div class="stack-item">C++</div>
      <div class="stack-item">C</div>
      <div class="stack-item">JavaScript</div>
      <div class="stack-item">PyTorch</div>
      <div class="stack-item">TensorFlow</div>
      <div class="stack-item">scikit-learn</div>
      <div class="stack-item">ROS2</div>
      <div class="stack-item">Linux</div>
      <div class="stack-item">React</div>
      <div class="stack-item">Git</div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Achievements</div>
    <div class="ach-list">
      <div class="ach-item"><div class="ach-dot"></div>Gold Badge Problem Solver — CodeChef</div>
      <div class="ach-item"><div class="ach-dot"></div>IEEE-VIT Member</div>
      <div class="ach-item"><div class="ach-dot"></div>Autonomous Software Developer & Ops — Team Ojas Racing (Formula Student EV)</div>
    </div>
  </div>

  <div class="section">
    <div class="section-label">Connect</div>
    <div class="connect-row">
      <a class="connect-btn" href="https://www.linkedin.com/in/naval-agarwal-48b678205/" target="_blank">LinkedIn ↗</a>
      <a class="connect-btn" href="https://github.com/NavalAgarwal" target="_blank">GitHub ↗</a>
    </div>
  </div>
</div>

