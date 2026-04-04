---
permalink: /
title: "Home"
author_profile: true
layout: homepage
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* ===== General ===== */
.homepage-section {
  margin-bottom: 2.8em;
}
.homepage-section h2 {
  font-size: 1.5em;
  padding-bottom: 0.35em;
  margin-bottom: 1em;
  border-bottom: 2px solid var(--global-base-color, #11999e);
  display: flex;
  align-items: center;
  gap: 0.4em;
}
.homepage-section h2 i {
  font-size: 0.85em;
  opacity: 0.7;
}

/* ===== About ===== */
.about-text {
  font-size: 0.96em;
  line-height: 1.75;
}
.contact-row {
  margin-top: 0.8em;
  display: flex;
  flex-wrap: wrap;
  gap: 0.5em;
}
.contact-pill {
  display: inline-flex;
  align-items: center;
  gap: 0.35em;
  padding: 0.3em 0.75em;
  border-radius: 20px;
  font-size: 0.85em;
  font-weight: 600;
  text-decoration: none;
  background: var(--global-code-background-color, #f5f5f5);
  color: var(--global-text-color, #333);
  border: 1px solid var(--global-border-color, #ddd);
  transition: all 0.2s;
}
.contact-pill:hover {
  background: var(--global-base-color, #11999e);
  color: #fff;
  border-color: var(--global-base-color, #11999e);
  text-decoration: none;
}

/* ===== News ===== */
.news-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.news-list li {
  padding: 0.5em 0;
  font-size: 0.92em;
  border-bottom: 1px solid var(--global-border-color, #eee);
}
.news-list li:last-child {
  border-bottom: none;
}
.news-date {
  font-weight: 700;
  color: var(--global-base-color, #11999e);
  margin-right: 0.6em;
  display: inline-block;
  min-width: 85px;
}

/* ===== Publications ===== */
.pub-entry {
  display: flex;
  gap: 1.5em;
  margin-bottom: 2em;
  padding: 1.2em;
  border-radius: 10px;
  background: var(--global-code-background-color, #fafafa);
  border: 1px solid var(--global-border-color, #e8e8e8);
  transition: box-shadow 0.2s;
}
.pub-entry:hover {
  box-shadow: 0 4px 16px rgba(0,0,0,0.08);
}
.pub-img {
  flex-shrink: 0;
  width: 240px;
  min-height: 150px;
  overflow: hidden;
  border-radius: 8px;
  border: 1px solid var(--global-border-color, #e0e0e0);
  display: flex;
  align-items: center;
  justify-content: center;
  background: var(--global-border-color, #f0f0f0);
}
.pub-img img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.pub-text {
  flex: 1;
  display: flex;
  flex-direction: column;
  gap: 0.3em;
}
.pub-title {
  font-size: 1.1em;
  font-weight: 700;
  line-height: 1.35;
  color: var(--global-text-color, #333);
}
.pub-authors {
  font-size: 0.9em;
  color: var(--global-text-color-light, #666);
  line-height: 1.5;
}
.pub-authors .me {
  font-weight: 700;
  text-decoration: underline;
  color: var(--global-text-color, #333);
}
.pub-venue {
  font-size: 0.9em;
  margin-top: 0.15em;
}
.pub-venue-name {
  font-weight: 600;
}
.pub-badge {
  display: inline-block;
  background: var(--global-base-color, #11999e);
  color: #fff;
  font-size: 0.75em;
  padding: 0.2em 0.6em;
  border-radius: 4px;
  margin-right: 0.4em;
  font-weight: 700;
  letter-spacing: 0.02em;
}
.pub-badge.preprint {
  background: #e67e22;
}
.pub-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.4em;
  margin-top: 0.5em;
}
.pub-pill {
  display: inline-flex;
  align-items: center;
  gap: 0.3em;
  padding: 0.25em 0.7em;
  border-radius: 20px;
  font-size: 0.8em;
  font-weight: 600;
  text-decoration: none;
  background: var(--global-bg-color, #fff);
  color: var(--global-text-color, #555);
  border: 1px solid var(--global-border-color, #ddd);
  transition: all 0.2s;
}
.pub-pill:hover {
  background: var(--global-base-color, #11999e);
  color: #fff;
  border-color: var(--global-base-color, #11999e);
  text-decoration: none;
}
.pub-note {
  font-size: 0.82em;
  color: var(--global-text-color-light, #888);
  line-height: 1.5;
  margin-top: 0.2em;
}
.equal-note {
  font-size: 0.82em;
  color: var(--global-text-color-light, #999);
}

/* ===== Experience ===== */
.exp-entry {
  display: flex;
  gap: 1em;
  margin-bottom: 1.5em;
  padding: 1em;
  border-radius: 10px;
  background: var(--global-code-background-color, #fafafa);
  border: 1px solid var(--global-border-color, #e8e8e8);
  transition: box-shadow 0.2s;
}
.exp-entry:hover {
  box-shadow: 0 2px 12px rgba(0,0,0,0.06);
}
.exp-logo {
  flex-shrink: 0;
  width: 48px;
  height: 48px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 800;
  font-size: 0.7em;
  color: #fff;
  margin-top: 0.1em;
}
.exp-logo.openai { background: #000; }
.exp-logo.microsoft { background: #00a4ef; }
.exp-logo.celestra { background: #6c5ce7; }
.exp-logo.judgment { background: #e17055; }
.exp-body {
  flex: 1;
}
.exp-header {
  display: flex;
  justify-content: space-between;
  align-items: baseline;
  flex-wrap: wrap;
  gap: 0.3em;
}
.exp-company {
  font-weight: 700;
  font-size: 1.02em;
}
.exp-date {
  font-size: 0.82em;
  color: var(--global-text-color-light, #999);
  font-style: italic;
}
.exp-role {
  font-size: 0.88em;
  color: var(--global-text-color-light, #666);
  margin-top: 0.1em;
}
.exp-desc {
  font-size: 0.86em;
  margin-top: 0.35em;
  line-height: 1.55;
  color: var(--global-text-color-light, #555);
}

/* ===== Education ===== */
.edu-entry {
  display: flex;
  gap: 1em;
  padding: 1em;
  border-radius: 10px;
  background: var(--global-code-background-color, #fafafa);
  border: 1px solid var(--global-border-color, #e8e8e8);
}
.edu-logo {
  flex-shrink: 0;
  width: 48px;
  height: 48px;
  border-radius: 10px;
  background: #2774AE;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 800;
  font-size: 0.65em;
  color: #FFD100;
}
.edu-body {
  flex: 1;
}
.edu-school {
  font-weight: 700;
  font-size: 1.02em;
}
.edu-degree {
  font-size: 0.9em;
  margin-top: 0.15em;
}
.edu-date {
  font-size: 0.82em;
  color: var(--global-text-color-light, #999);
  font-style: italic;
}
.edu-courses {
  font-size: 0.82em;
  color: var(--global-text-color-light, #777);
  margin-top: 0.3em;
  line-height: 1.5;
}

/* ===== Responsive ===== */
@media (max-width: 600px) {
  .pub-entry {
    flex-direction: column;
  }
  .pub-img {
    width: 100%;
    height: 180px;
  }
  .exp-header {
    flex-direction: column;
  }
}
</style>

<!-- ==================== ABOUT ==================== -->
<div class="homepage-section" id="about">
<h2><i class="fas fa-user"></i> About</h2>
<div class="about-text">

I am a student at <b>UCLA</b> studying Computer Science and Applied Mathematics. I am currently an <b>Applied Scientist Intern at Microsoft</b>, working on similarity-preserving hashing (SimHash) for biometric authentication and model quantization for efficient CPU deployment.

My research interests span <b>AI agents</b>, <b>mechanistic interpretability</b>, <b>reinforcement learning</b>, and <b>efficient ML systems</b>. I have worked on multi-agent system design, LLM evaluation with RL-tuned rewards, and understanding the internal mechanisms of instruction-tuned language models.

Previously, I worked at <b><a href="https://celestra.com/">Celestra</a></b> and <b><a href="https://www.judgmentlabs.ai/">Judgment Labs</a></b>. I will be joining <b>OpenAI</b> as a Member of Technical Staff Intern in Summer 2026.

<div class="contact-row">
  <a class="contact-pill" href="mailto:yifanz1207@gmail.com"><i class="fas fa-envelope"></i> Email</a>
  <a class="contact-pill" href="https://scholar.google.com/citations?user=tUNPDm8AAAAJ"><i class="ai ai-google-scholar"></i> Google Scholar</a>
  <a class="contact-pill" href="https://github.com/yifan1207"><i class="fab fa-github"></i> GitHub</a>
  <a class="contact-pill" href="https://www.linkedin.com/in/yifan-zhou127"><i class="fab fa-linkedin"></i> LinkedIn</a>
</div>

</div>
</div>

<!-- ==================== NEWS ==================== -->
<div class="homepage-section" id="news">
<h2><i class="fas fa-newspaper"></i> News</h2>
<ul class="news-list">
  <li><span class="news-date">Apr 2026</span> Our paper <i>"Investigating Component Contributions in Multi-Agent ML Systems"</i> is accepted at <b>ICML 2026</b>!</li>
  <li><span class="news-date">Jan 2026</span> Started as Applied Scientist Intern at <b>Microsoft</b>.</li>
</ul>
</div>

<!-- ==================== PUBLICATIONS ==================== -->
<div class="homepage-section" id="publications">
<h2><i class="fas fa-book"></i> Publications</h2>

<p class="equal-note">* equal contribution</p>

<div class="pub-entry">
  <div class="pub-img">
    <img src="/images/component_contribution.png" alt="Component Contributions in Multi-Agent ML Systems">
  </div>
  <div class="pub-text">
    <div class="pub-title">Investigating Component Contributions in Multi-Agent ML Systems</div>
    <div class="pub-authors">
      Junsung Kim*, Ilia Mireskandari*, Seungwan Son*, <span class="me">Yifan Zhou*</span>, Khizer Shahid*, Dylan Yihan Dai*
    </div>
    <div class="pub-venue">
      <span class="pub-badge">ICML 2026</span>
      <span class="pub-venue-name">International Conference on Machine Learning, 2026</span>
    </div>
    <div class="pub-links">
      <a class="pub-pill" href="https://openreview.net/pdf?id=FOfvTwBGUX"><i class="fas fa-file-pdf"></i> Paper</a>
    </div>
  </div>
</div>

</div>

<!-- ==================== PREPRINTS ==================== -->
<div class="homepage-section" id="preprints">
<h2><i class="fas fa-file-lines"></i> Preprints</h2>

<div class="pub-entry">
  <div class="pub-img">
    <i class="fas fa-file-alt" style="font-size:3em;color:var(--global-text-color-light,#bbb);"></i>
  </div>
  <div class="pub-text">
    <div class="pub-title">Instruction Tuning Delays Prediction Commitment</div>
    <div class="pub-authors">
      <span class="me">Yifan Zhou</span>
    </div>
    <div class="pub-venue">
      <span class="pub-badge preprint">Preprint</span>
      <span class="pub-venue-name">2025</span>
    </div>
    <div class="pub-note">A mechanistic interpretability study showing instruction tuning restructures LLM computation by delaying token commitment ~6 layers, expanding late-layer dimensionality, and implementing a localized "corrective stage" for output style. Validated across 6 architectures.</div>
    <div class="pub-links">
      <a class="pub-pill" href="https://github.com/yifan1207/PT-IT-Model-Differences"><i class="fab fa-github"></i> Code</a>
    </div>
  </div>
</div>

</div>

<!-- ==================== EXPERIENCE ==================== -->
<div class="homepage-section" id="experience">
<h2><i class="fas fa-briefcase"></i> Industry Experience</h2>

<div class="exp-entry">
  <div class="exp-logo openai">OAI</div>
  <div class="exp-body">
    <div class="exp-header">
      <span class="exp-company">OpenAI</span>
      <span class="exp-date">Jun 2026 -- Sep 2026</span>
    </div>
    <div class="exp-role">Member of Technical Staff Intern, Integrity Team</div>
    <div class="exp-desc">Incoming summer 2026.</div>
  </div>
</div>

<div class="exp-entry">
  <div class="exp-logo microsoft">MS</div>
  <div class="exp-body">
    <div class="exp-header">
      <span class="exp-company">Microsoft</span>
      <span class="exp-date">Jan 2026 -- Apr 2026</span>
    </div>
    <div class="exp-role">Applied Scientist Intern</div>
    <div class="exp-desc">Research on SimHash for biometric auth and model quantization for CPU deployment (60% size reduction, 2.3x speedup).</div>
  </div>
</div>

<div class="exp-entry">
  <div class="exp-logo celestra">CEL</div>
  <div class="exp-body">
    <div class="exp-header">
      <span class="exp-company">Celestra</span>
      <span class="exp-date">Sep 2025 -- Dec 2025</span>
    </div>
    <div class="exp-role">Research Scientist Intern</div>
    <div class="exp-desc">Co-authored agent scaffolding research (4,000+ ablations; ICML 2026) and deployed agent stack achieving top-3 on MLE-Bench.</div>
  </div>
</div>

<div class="exp-entry">
  <div class="exp-logo judgment">JL</div>
  <div class="exp-body">
    <div class="exp-header">
      <span class="exp-company">Judgment Labs</span>
      <span class="exp-date">Jan 2025 -- Sep 2025</span>
    </div>
    <div class="exp-role">Member of Technical Staff</div>
    <div class="exp-desc">First hire; led RL-tuned LLM evaluations (+40-45% alignment over LLM-as-judge baselines) and agent SFT optimization.</div>
  </div>
</div>

</div>

<!-- ==================== EDUCATION ==================== -->
<div class="homepage-section" id="education">
<h2><i class="fas fa-graduation-cap"></i> Education</h2>

<div class="edu-entry">
  <div class="edu-logo">UCLA</div>
  <div class="edu-body">
    <div class="edu-school">University of California, Los Angeles</div>
    <div class="edu-degree">B.S. in Computer Science and Applied Mathematics -- GPA: 3.92/4.0</div>
    <div class="edu-date">Sep 2024 -- Jun 2027 (Expected)</div>
    <div class="edu-courses">Reinforcement Learning, NLP, Foundations of Machine Learning, Algorithms, Database Systems, Probability Theory, Complex Analysis, Linear Algebra</div>
  </div>
</div>

</div>
