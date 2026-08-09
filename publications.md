---
layout: default
title: Publications
permalink: /publications/
---

<!-- Custom CSS matching index.md, about.md, best-of-pie.md, and conference.md -->
<style>
  :root {
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink accent */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark boxes */
    --pie-lilac-hover: #ffffff;
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped hero container matching index.md */
  .sloped-box-top {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 35px 25px 40px 25px;
    margin-bottom: 30px;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, var(--pie-heading-dark), var(--pie-purple-pink)) 1;
  }

  .heading-serif {
    font-family: "Playfair Display", "Georgia", "Times New Roman", serif;
    color: var(--pie-heading-dark);
    font-size: 1.8rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  /* Navigation Pills matching dark style */
  .category-nav-btn {
    background-color: var(--primary-navy, #1C2B36);
    color: #ffffff;
    padding: 10px 18px;
    border-radius: 4px;
    text-decoration: none;
    font-weight: bold;
    font-size: 0.85rem;
    transition: background-color 0.2s ease, color 0.2s ease, transform 0.2s ease;
    display: inline-block;
  }

  .category-nav-btn:hover {
    background-color: var(--burgundy-accent, #7A0C2E);
    color: #ffffff;
    transform: translateY(-1px);
  }

  .pub-link {
    color: var(--pie-heading-dark);
    font-weight: bold;
    text-decoration: underline;
    transition: color 0.2s ease;
  }

  .pub-link:hover {
    color: var(--pie-purple-pink);
  }

  /* Volume Card Collapsible Details */
  details.volume-card {
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.2);
    border-radius: 8px;
    margin-bottom: 14px;
    overflow: hidden;
    box-shadow: 0 2px 5px rgba(0,0,0,0.03);
    transition: box-shadow 0.2s ease, border-color 0.2s ease;
  }

  details.volume-card[open] {
    border-color: var(--pie-heading-dark);
    box-shadow: 0 4px 12px rgba(138, 72, 184, 0.1);
  }

  details.volume-card summary {
    font-weight: 700;
    color: var(--primary-navy, #1C2B36);
    cursor: pointer;
    font-size: 1.05rem;
    padding: 16px 20px;
    background-color: #ffffff;
    list-style: none;
    display: flex;
    justify-content: space-between;
    align-items: center;
    transition: background-color 0.2s ease, color 0.2s ease;
    user-select: none;
  }

  details.volume-card summary::-webkit-details-marker {
    display: none;
  }

  details.volume-card summary:hover {
    background-color: #faf8fc;
    color: var(--pie-heading-dark);
  }

  details.volume-card summary::after {
    content: "▼";
    font-size: 0.75rem;
    color: var(--pie-heading-dark);
    transition: transform 0.2s ease;
  }

  details.volume-card[open] summary::after {
    transform: rotate(180deg);
  }

  .volume-content {
    padding: 0 20px 20px 20px;
    border-top: 1px solid rgba(138, 72, 184, 0.1);
    background-color: #ffffff;
  }

  /* Full Volume PDF Button */
  .dl-btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: linear-gradient(135deg, var(--primary-navy, #1C2B36), #2a3e4e);
    color: #ffffff !important;
    padding: 10px 20px;
    border-radius: 6px;
    font-weight: 600;
    font-size: 0.88rem;
    text-decoration: none !important;
    box-shadow: 0 3px 8px rgba(28, 43, 54, 0.2);
    transition: all 0.2s ease;
  }

  .dl-btn:hover {
    background: linear-gradient(135deg, var(--pie-heading-dark), #6c3293);
    color: #ffffff !important;
    transform: translateY(-2px);
    box-shadow: 0 5px 12px rgba(138, 72, 184, 0.3);
  }

  /* Chapter Specific PDF Button */
  .chapter-pdf-btn {
    display: inline-flex;
    align-items: center;
    gap: 4px;
    background-color: rgba(138, 72, 184, 0.08);
    color: var(--pie-heading-dark) !important;
    border: 1px solid rgba(138, 72, 184, 0.25);
    padding: 4px 10px;
    border-radius: 4px;
    font-weight: 700;
    font-size: 0.78rem;
    text-decoration: none !important;
    transition: all 0.2s ease;
  }

  .chapter-pdf-btn:hover {
    background-color: var(--pie-heading-dark);
    color: #ffffff !important;
    border-color: var(--pie-heading-dark);
  }

  /* Collaboration Cards */
  .collab-card {
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.18);
    border-radius: 8px;
    padding: 20px;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .collab-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 6px 16px rgba(138, 72, 184, 0.12);
    border-color: var(--pie-heading-dark);
  }
</style>

<!-- Top Hero Sloped Dark Box -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Text -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">PUBLICATIONS</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        Explore our peer-reviewed journals, classroom resource collections, conference reviews, and collaborative works.
      </p>
    </div>

    <!-- Right Brand Graphic -->
    <div class="hero-brand-graphic" style="text-align: right; flex: 0 0 auto;">
      <h1 style="font-size: 2.2rem; margin: 0; font-weight: bold;">
        <span style="color: var(--pie-heading-dark);">PIE</span> <span style="color: var(--pie-purple-pink);">sig</span>
      </h1>
      <p style="color: #b0b5c0; font-size: 0.75rem; letter-spacing: 1px; margin-top: 4px; margin-bottom: 0;">PERFORMANCE IN EDUCATION</p>
    </div>
  </div>
</div>

<!-- Intro & Submission Info -->
<div style="margin-bottom: 35px; padding: 0 5px;">
  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 20px;">
    The PIE SIG publishes two main journals: <strong>Mask & Gavel</strong> is our official peer-reviewed journal and the <strong>PIE SIG Classroom Resources Journal</strong> which is a collection of My Share-type articles. Article submissions are accepted year-round, will be published online as they are finalized (with page numbers and DOIs for citation), and will be collected into full volumes that will be published as PDFs once we accumulate a sufficient number of articles.
  </p>

  <!-- Submission Details -->
  <div style="border-bottom: 1px solid rgba(138, 72, 184, 0.2); padding-bottom: 20px;">
    <p style="font-size: 0.92rem; margin-bottom: 8px; color: var(--text-dark, #222222);">
      <strong>Submission Guidelines:</strong> <a href="https://jalt-publications.org/tlt/submissions" target="_blank" rel="noopener" class="pub-link">View JALT Guidelines</a>
    </p>
    <p style="font-size: 0.92rem; margin-bottom: 12px; color: var(--text-dark, #222222);">
      <strong>Send Submissions To:</strong> Philip Head (<a href="mailto:piesigpublications@gmail.com" class="pub-link">piesigpublications@gmail.com</a>)
    </p>
    <p style="font-size: 0.82rem; color: #666; line-height: 1.5; margin: 0; padding-top: 6px;">
      Published by the Performance in Education Special Interest Group, The Japan Association for Language Teaching, JALT Central Office, Urban Edge Bldg 5F, 1-37-9 Taito, Taito-ku, Tokyo.
    </p>
  </div>
</div>

<!-- Category Navigation -->
<div style="display: flex; gap: 12px; flex-wrap: wrap; margin-bottom: 35px;">
  <a href="#mask-and-gavel" class="category-nav-btn">Mask & Gavel</a>
  <a href="#classroom-resources" class="category-nav-btn">Classroom Resources Journal</a>
  <a href="#pie-review" class="category-nav-btn">PIE Review</a>
  <a href="#collaborations" class="category-nav-btn">Collaborations</a>
</div>

<!-- 1. MASK & GAVEL -->
<section id="mask-and-gavel" style="margin-bottom: 45px; padding: 0 5px;">
  {% assign mg = site.data.publications.mask_and_gavel %}
  <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; gap: 10px; margin-bottom: 15px;">
    <h2 class="heading-serif" style="margin: 0;">MASK & GAVEL</h2>
    {%- if mg.issn -%}
      <span style="font-size: 0.8rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold;">ISSN {{ mg.issn }}</span>
    {%- endif -%}
  </div>

  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 25px;">
    Mask & Gavel is the peer-reviewed academic journal of the Performance in Education SIG.
    <br><br>
    Article submissions are accepted year-round and published online as soon as they are finalized, before being collected into the full journal published online bi-annually. All articles are vetted by an editor, blinded, and peer-reviewed by two reviewers before publication. We welcome research-based, comment & opinion, interview, and review-based articles. Practical lesson resource articles should be submitted to the Classroom Resources journal. For submission guidelines please refer to the specifications outlined in The Language Teacher.
  </p>

  <!-- Volumes -->
  {%- if mg.volumes.size > 0 -%}
    {%- for vol in mg.volumes -%}
      <details class="volume-card">
        <summary>
          <span>{{ vol.volume }}</span>
        </summary>
        <div class="volume-content">
          <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 15px; margin: 15px 0 20px 0;">
            {%- if vol.doi -%}
              <span style="font-size: 0.88rem; color: #555;"><strong>DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" class="pub-link">{{ vol.doi }}</a></span>
            {%- else -%}
              <span></span>
            {%- endif -%}
            {%- if vol.pdf -%}
              <a href="{{ vol.pdf }}" target="_blank" download class="dl-btn">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                Download {{ vol.volume }} PDF
              </a>
            {%- endif -%}
          </div>

          {%- if vol.chapters -%}
            <div style="background: #faf8fc; border-radius: 6px; padding: 15px 18px; border: 1px solid rgba(138, 72, 184, 0.1);">
              <strong style="display: block; margin-bottom: 12px; color: var(--pie-heading-dark); font-size: 0.85rem; text-transform: uppercase; letter-spacing: 0.5px;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-top: 1px solid rgba(138, 72, 184, 0.12); padding: 10px 0; {% if forloop.first %}border-top: none; padding-top: 0;{% endif %}">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 12px;">
                      <span style="color: var(--text-dark, #222222); font-weight: 600; font-size: 0.92rem; line-height: 1.4;">{{ chapter.title }}</span>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download class="chapter-pdf-btn">
                          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                          PDF
                        </a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 3px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #777; font-size: 0.8rem; margin-top: 2px;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="pub-link">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            </div>
          {%- endif -%}
        </div>
      </details>
    {%- endfor -%}
  {%- else -%}
    <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
  {%- endif -%}
</section>

<!-- 2. CLASSROOM RESOURCES JOURNAL -->
<section id="classroom-resources" style="margin-bottom: 45px; padding: 0 5px;">
  {% assign cr = site.data.publications.classroom_resources %}
  <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; gap: 10px; margin-bottom: 15px;">
    <h2 class="heading-serif" style="margin: 0;">PIE SIG CLASSROOM RESOURCES JOURNAL</h2>
    {%- if cr.issn -%}
      <span style="font-size: 0.8rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold;">ISSN {{ cr.issn }}</span>
    {%- endif -%}
  </div>

  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 25px;">
    The classroom resource journal of the Performance in Education SIG. PIE SIG has put together a new lesson resource online publication, and it is now available online. This is the publication for the sharing of practical lesson resources.
  </p>

  {%- if cr.volumes.size > 0 -%}
    {%- for vol in cr.volumes -%}
      <details class="volume-card">
        <summary>
          <span>{{ vol.volume }}</span>
        </summary>
        <div class="volume-content">
          <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 15px; margin: 15px 0 20px 0;">
            {%- if vol.doi -%}
              <span style="font-size: 0.88rem; color: #555;"><strong>DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" class="pub-link">{{ vol.doi }}</a></span>
            {%- else -%}
              <span></span>
            {%- endif -%}
            {%- if vol.pdf -%}
              <a href="{{ vol.pdf }}" target="_blank" download class="dl-btn">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                Download {{ vol.volume }} PDF
              </a>
            {%- endif -%}
          </div>

          {%- if vol.chapters -%}
            <div style="background: #faf8fc; border-radius: 6px; padding: 15px 18px; border: 1px solid rgba(138, 72, 184, 0.1);">
              <strong style="display: block; margin-bottom: 12px; color: var(--pie-heading-dark); font-size: 0.85rem; text-transform: uppercase; letter-spacing: 0.5px;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-top: 1px solid rgba(138, 72, 184, 0.12); padding: 10px 0; {% if forloop.first %}border-top: none; padding-top: 0;{% endif %}">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 12px;">
                      <span style="color: var(--text-dark, #222222); font-weight: 600; font-size: 0.92rem; line-height: 1.4;">{{ chapter.title }}</span>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download class="chapter-pdf-btn">
                          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                          PDF
                        </a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 3px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #777; font-size: 0.8rem; margin-top: 2px;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="pub-link">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            </div>
          {%- endif -%}
        </div>
      </details>
    {%- endfor -%}
  {%- else -%}
    <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
  {%- endif -%}
</section>

<!-- 3. PIE REVIEW -->
<section id="pie-review" style="margin-bottom: 45px; padding: 0 5px;">
  {% assign pr = site.data.publications.pie_review %}
  <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; gap: 10px; margin-bottom: 15px;">
    <h2 class="heading-serif" style="margin: 0;">PERFORMANCE IN EDUCATION REVIEW</h2>
    {%- if pr.issn -%}
      <span style="font-size: 0.8rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold;">ISSN {{ pr.issn }}</span>
    {%- endif -%}
  </div>

  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 25px;">
    Some of PIE SIG’s amazing conference presenters have been kind enough to write scholarly articles on their presentations, workshops, and performances. The Performance in Education Review presents some of these notable articles previously presented at PIE SIG conferences. The intention of this journal is to create a montage of the year in PIE conferences, but some volumes may cover multiple years due to the time needed to gather all proposals.
  </p>

  {%- if pr.volumes.size > 0 -%}
    {%- for vol in pr.volumes -%}
      <details class="volume-card">
        <summary>
          <span>{{ vol.volume }}</span>
        </summary>
        <div class="volume-content">
          <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 15px; margin: 15px 0 20px 0;">
            {%- if vol.doi -%}
              <span style="font-size: 0.88rem; color: #555;"><strong>DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" class="pub-link">{{ vol.doi }}</a></span>
            {%- else -%}
              <span></span>
            {%- endif -%}
            {%- if vol.pdf -%}
              <a href="{{ vol.pdf }}" target="_blank" download class="dl-btn">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                Download {{ vol.volume }} PDF
              </a>
            {%- endif -%}
          </div>

          {%- if vol.chapters -%}
            <div style="background: #faf8fc; border-radius: 6px; padding: 15px 18px; border: 1px solid rgba(138, 72, 184, 0.1);">
              <strong style="display: block; margin-bottom: 12px; color: var(--pie-heading-dark); font-size: 0.85rem; text-transform: uppercase; letter-spacing: 0.5px;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-top: 1px solid rgba(138, 72, 184, 0.12); padding: 10px 0; {% if forloop.first %}border-top: none; padding-top: 0;{% endif %}">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 12px;">
                      <span style="color: var(--text-dark, #222222); font-weight: 600; font-size: 0.92rem; line-height: 1.4;">{{ chapter.title }}</span>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download class="chapter-pdf-btn">
                          <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path><polyline points="7 10 12 15 17 10"></polyline><line x1="12" y1="15" x2="12" y2="3"></line></svg>
                          PDF
                        </a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 3px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #777; font-size: 0.8rem; margin-top: 2px;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="pub-link">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            </div>
          {%- endif -%}
        </div>
      </details>
    {%- endfor -%}
  {%- else -%}
    <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
  {%- endif -%}
</section>

<!-- 4. COLLABORATIONS -->
<section id="collaborations" style="margin-bottom: 35px; padding: 0 5px;">
  <h2 class="heading-serif" style="margin-bottom: 15px;">
    COLLABORATION PUBLICATIONS
  </h2>
  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 25px;">
    PIE SIG also co-publishes issues centered around PIE’s focal areas, including on Debate, Discussion, and Drama. Below, you can find a list of these Collaboration Publications.
  </p>

  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px;">
    
    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">August 2025</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Public Speaking in the Language Classroom</p>
      </div>
      <a href="https://www.mindbrained.org/august-2025-public-speaking/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">March 2025</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Teaching Speech and Presentation in the Language Classroom</p>
      </div>
      <a href="https://www.mindbrained.org/march-2025-speech-presentation/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">February 2025</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Integrating Music and Performance in the Language Classroom</p>
      </div>
      <a href="https://www.mindbrained.org/february-2025-music/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">December 2024</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Setting Up Discussions in the Language Classroom</p>
      </div>
      <a href="https://www.mindbrained.org/december-2024-discussion/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">November 2024</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Debate</p>
      </div>
      <a href="https://www.mindbrained.org/november-2024-debate/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

    <div class="collab-card">
      <div>
        <strong style="color: var(--pie-heading-dark); display: block; font-size: 1.05rem;">Mind, Brain, Education SIG</strong>
        <span style="font-size: 0.78rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block; margin: 8px 0 10px 0;">December 2021</span>
        <p style="font-size: 0.92rem; color: var(--text-dark, #222222); margin: 0 0 15px 0; line-height: 1.4;">Drama</p>
      </div>
      <a href="https://www.mindbrained.org/december-2021-drama/" target="_blank" rel="noopener" class="pub-link" style="font-size: 0.88rem;">View Collaboration &rarr;</a>
    </div>

  </div>
</section>