---
layout: default
title: Publications
permalink: /publications/
---

<!-- Top Hero Title Banner -->
<div class="hero-black-box mb-30">
  <div>
    <h2>PUBLICATIONS</h2>
    <p class="hero-intro-text">
      Explore our peer-reviewed journals, classroom resource collections, conference reviews, and collaborative works.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Intro & Submission Info Card -->
<div class="pub-intro-card">
  <p class="pub-intro-text">
    The PIE SIG publishes two main journals: <strong>Mask & Gavel</strong> is our official peer-reviewed journal and the <strong>PIE SIG Classroom Resources Journal</strong> which is a collection of My Share-type articles. Article submissions are accepted year-round, will be published online as they are finalized (with page numbers and DOIs for citation), and will be collected into full volumes that will be published as PDFs once we accumulate a sufficient number of articles.
  </p>

  <!-- Submission Details Box -->
  <div class="pub-submission-box">
    <p class="pub-submission-line">
      <strong>Submission Guidelines:</strong> <a href="https://jalt-publications.org/tlt/submissions" target="_blank" rel="noopener">View JALT Guidelines</a>
    </p>
    <p class="pub-submission-line">
      <strong>Send Submissions To:</strong> Philip Head (<a href="mailto:piesigpublications@gmail.com">piesigpublications@gmail.com</a>)
    </p>
    <p class="pub-publisher-footnote">
      Published by the Performance in Education Special Interest Group, The Japan Association for Language Teaching, JALT Central Office, Urban Edge Bldg 5F, 1-37-9 Taito, Taito-ku, Tokyo.
    </p>
  </div>
</div>

<!-- Category Navigation -->
<nav class="pub-category-nav">
  <a href="#mask-and-gavel">Mask & Gavel</a>
  <a href="#classroom-resources">Classroom Resources Journal</a>
  <a href="#pie-review">PIE Review</a>
  <a href="#collaborations">Collaborations</a>
</nav>

<!-- 1. MASK & GAVEL -->
<section id="mask-and-gavel" class="pub-section">
  {% assign mg = site.data.publications.mask_and_gavel %}
  <div class="pub-card">
    <div class="pub-card-header">
      <h2>MASK & GAVEL</h2>
      {%- if mg.issn -%}
        <span class="pub-issn-badge">ISSN {{ mg.issn }}</span>
      {%- endif -%}
    </div>

    <p class="pub-journal-desc">
      Mask & Gavel is the peer-reviewed academic journal of the Performance in Education SIG.
      <br><br>
      Article submissions are accepted year-round and published online as soon as they are finalized, before being collected into the full journal published online bi-annually. All articles are vetted by an editor, blinded, and peer-reviewed by two reviewers before publication. We welcome research-based, comment & opinion, interview, and review-based articles. Practical lesson resource articles should be submitted to the Classroom Resources journal. For submission guidelines please refer to the specifications outlined in The Language Teacher.
    </p>

    <!-- Volumes -->
    {%- if mg.volumes.size > 0 -%}
      {%- for vol in mg.volumes -%}
        <details class="pub-volume-details">
          <summary>{{ vol.volume }}</summary>
          <div class="pub-volume-content">
            {%- if vol.doi -%}
              <p class="pub-meta-line"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p class="pub-meta-line">
                <a href="{{ vol.pdf }}" target="_blank" download class="pub-pdf-download">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong class="pub-toc-heading">Table of Contents</strong>
              <ul class="pub-toc-list">
                {%- for chapter in vol.chapters -%}
                  <li>
                    <div class="pub-toc-row">
                      <strong>{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download>[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span class="pub-chapter-author">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span class="pub-chapter-doi">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p class="pub-empty-text">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 2. CLASSROOM RESOURCES JOURNAL -->
<section id="classroom-resources" class="pub-section">
  {% assign cr = site.data.publications.classroom_resources %}
  <div class="pub-card">
    <div class="pub-card-header">
      <h2>PIE SIG CLASSROOM RESOURCES JOURNAL</h2>
      {%- if cr.issn -%}
        <span class="pub-issn-badge">ISSN {{ cr.issn }}</span>
      {%- endif -%}
    </div>

    <p class="pub-journal-desc">
      The classroom resource journal of the Performance in Education SIG. PIE SIG has put together a new lesson resource online publication, and it is now available online. This is the publication for the sharing of practical lesson resources.
    </p>

    {%- if cr.volumes.size > 0 -%}
      {%- for vol in cr.volumes -%}
        <details class="pub-volume-details">
          <summary>{{ vol.volume }}</summary>
          <div class="pub-volume-content">
            {%- if vol.doi -%}
              <p class="pub-meta-line"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p class="pub-meta-line">
                <a href="{{ vol.pdf }}" target="_blank" download class="pub-pdf-download">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong class="pub-toc-heading">Table of Contents</strong>
              <ul class="pub-toc-list">
                {%- for chapter in vol.chapters -%}
                  <li>
                    <div class="pub-toc-row">
                      <strong>{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download>[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span class="pub-chapter-author">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span class="pub-chapter-doi">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p class="pub-empty-text">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 3. PIE REVIEW -->
<section id="pie-review" class="pub-section">
  {% assign pr = site.data.publications.pie_review %}
  <div class="pub-card">
    <div class="pub-card-header">
      <h2>PERFORMANCE IN EDUCATION REVIEW</h2>
      {%- if pr.issn -%}
        <span class="pub-issn-badge">ISSN {{ pr.issn }}</span>
      {%- endif -%}
    </div>

    <p class="pub-journal-desc">
      Some of PIE SIG’s amazing conference presenters have been kind enough to write scholarly articles on their presentations, workshops, and performances. The Performance in Education Review presents some of these notable articles previously presented at PIE SIG conferences. The intention of this journal is to create a montage of the year in PIE conferences, but some volumes may cover multiple years due to the time needed to gather all proposals.
    </p>

    {%- if pr.volumes.size > 0 -%}
      {%- for vol in pr.volumes -%}
        <details class="pub-volume-details">
          <summary>{{ vol.volume }}</summary>
          <div class="pub-volume-content">
            {%- if vol.doi -%}
              <p class="pub-meta-line"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p class="pub-meta-line">
                <a href="{{ vol.pdf }}" target="_blank" download class="pub-pdf-download">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong class="pub-toc-heading">Table of Contents</strong>
              <ul class="pub-toc-list">
                {%- for chapter in vol.chapters -%}
                  <li>
                    <div class="pub-toc-row">
                      <strong>{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download>[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span class="pub-chapter-author">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span class="pub-chapter-doi">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p class="pub-empty-text">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 4. COLLABORATIONS -->
<section id="collaborations" class="pub-section">
  <div class="pub-card">
    <h2 class="pub-section-heading">COLLABORATION PUBLICATIONS</h2>
    <p class="pub-journal-desc">
      PIE SIG also co-publishes issues centered around PIE’s focal areas, including on Debate, Discussion, and Drama. Below, you can find a list of these Collaboration Publications.
    </p>

    <div class="pub-collab-grid">
      {% for collab in site.data.publications.collaborations %}
        <div class="pub-collab-card">
          <div>
            <strong class="pub-collab-partner">{{ collab.partner }}</strong>
            <span class="pub-collab-date">{{ collab.date }}</span>
            <p class="pub-collab-title">{{ collab.title }}</p>
          </div>
          <a href="{{ collab.url }}" target="_blank" rel="noopener" class="pub-collab-link">View Collaboration &rarr;</a>
        </div>
      {% endfor %}
    </div>
  </div>
</section>