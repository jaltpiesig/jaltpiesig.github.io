---
layout: default
title: Publications
permalink: /publications/
---

<div class="publications-container">

  <!-- Intro Paragraph -->
  <p class="publications-intro">
    The PIE SIG publishes two main journals: <strong>Mask & Gavel</strong> is our official peer-reviewed journal and the <strong>PIE SIG Classroom Resources Journal</strong> which is a collection of My Share-type articles. Article submissions are accepted year-round, will be published online as they are finalized (with page numbers and DOIs for citation), and will be collected into full volumes that will be published as PDFs once we accumulate a sufficient number of articles.
  </p>

  <!-- Global Submission & Publisher Info Box -->
  <div class="submission-info-box">
    <p><strong>Submission Guidelines:</strong> <a href="https://jalt-publications.org/tlt/submissions" target="_blank" rel="noopener">View JALT Guidelines</a></p>
    <p><strong>Send Submissions To:</strong> Philip Head (<a href="mailto:head.philip@gmail.com">head.philip@gmail.com</a>)</p>
    <p class="publisher-info">Published by the Performance in Education Special Interest Group, The Japan Association for Language Teaching, JALT Central Office, Urban Edge Bldg 5F, 1-37-9 Taito, Taito-ku, Tokyo.</p>
  </div>

  <!-- Category Navigation Bar -->
  <nav class="pub-nav">
    <a href="#mask-and-gavel">Mask & Gavel</a>
    <a href="#classroom-resources">Classroom Resources Journal</a>
    <a href="#collaborations">Collaborations</a>
  </nav>

  <!-- 1. MASK & GAVEL -->
  <section id="mask-and-gavel" class="pub-section">
    {% assign mg = site.data.publications.mask_and_gavel %}
    <h2>Mask & Gavel</h2>
    {%- if mg.issn -%}<span class="issn-badge">ISSN {{ mg.issn }}</span>{%- endif -%}
    <p class="pub-description">{{ mg.description }}</p>

    <div class="volumes-list">
      {%- if mg.volumes.size > 0 -%}
        {%- for vol in mg.volumes -%}
          <details class="publication-volume">
            <summary class="volume-header">
              <span class="volume-title">{{ vol.volume }}</span>
            </summary>
            <div class="volume-content">
              {%- if vol.doi -%}
                <p class="volume-doi"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
              {%- endif -%}

              {%- if vol.pdf -%}
                <div class="volume-download-bar">
                  <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>
                    📄 Download Full {{ vol.volume }} PDF
                  </a>
                </div>
              {%- endif -%}

              {%- if vol.chapters -%}
                <h3 class="chapters-heading">Table of Contents</h3>
                <ul class="chapter-list">
                  {%- for chapter in vol.chapters -%}
                    <li class="chapter-item">
                      <div class="chapter-header-line">
                        <strong class="chapter-title">{{ chapter.title }}</strong>
                        <div class="chapter-actions">
                          {%- if chapter.pdf -%}
                            <a href="{{ chapter.pdf }}" class="chapter-pdf-link" target="_blank" download>[PDF]</a>
                          {%- endif -%}
                        </div>
                      </div>
                      
                      {%- if chapter.author -%}
                        <span class="chapter-author">By {{ chapter.author }}</span>
                      {%- endif -%}

                      {%- if chapter.doi -%}
                        <div class="chapter-doi-block">
                          <strong>DOI:</strong> <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="doi-link">{{ chapter.doi }}</a>
                        </div>
                      {%- endif -%}
                    </li>
                  {%- endfor -%}
                </ul>
              {%- endif -%}
            </div>
          </details>
        {%- endfor -%}
      {%- else -%}
        <p class="no-volumes">Volume details coming soon.</p>
      {%- endif -%}
    </div>
  </section>

  <!-- 2. CLASSROOM RESOURCES JOURNAL -->
  <section id="classroom-resources" class="pub-section">
    {% assign cr = site.data.publications.classroom_resources %}
    <h2>PIE SIG Classroom Resources Journal</h2>
    {%- if cr.issn -%}<span class="issn-badge">ISSN {{ cr.issn }}</span>{%- endif -%}
    <p class="pub-description">{{ cr.description }}</p>

    <div class="volumes-list">
      {%- if cr.volumes.size > 0 -%}
        {%- for vol in cr.volumes -%}
          <details class="publication-volume">
            <summary class="volume-header">
              <span class="volume-title">{{ vol.volume }}</span>
            </summary>
            <div class="volume-content">
              {%- if vol.doi -%}
                <p class="volume-doi"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
              {%- endif -%}

              {%- if vol.pdf -%}
                <div class="volume-download-bar">
                  <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>
                    📄 Download Full {{ vol.volume }} PDF
                  </a>
                </div>
              {%- endif -%}

              {%- if vol.chapters -%}
                <h3 class="chapters-heading">Table of Contents</h3>
                <ul class="chapter-list">
                  {%- for chapter in vol.chapters -%}
                    <li class="chapter-item">
                      <div class="chapter-header-line">
                        <strong class="chapter-title">{{ chapter.title }}</strong>
                        <div class="chapter-actions">
                          {%- if chapter.pdf -%}
                            <a href="{{ chapter.pdf }}" class="chapter-pdf-link" target="_blank" download>[PDF]</a>
                          {%- endif -%}
                        </div>
                      </div>

                      {%- if chapter.author -%}
                        <span class="chapter-author">By {{ chapter.author }}</span>
                      {%- endif -%}

                      {%- if chapter.doi -%}
                        <div class="chapter-doi-block">
                          <strong>DOI:</strong> <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="doi-link">{{ chapter.doi }}</a>
                        </div>
                      {%- endif -%}
                    </li>
                  {%- endfor -%}
                </ul>
              {%- endif -%}
            </div>
          </details>
        {%- endfor -%}
      {%- else -%}
        <p class="no-volumes">Volume details coming soon.</p>
      {%- endif -%}
    </div>
  </section>

  <!-- 3. COLLABORATIONS -->
  <section id="collaborations" class="pub-section">
    <h2>Collaboration Publications</h2>
    <p class="pub-description">
      PIE SIG also co-publishes issues centered around PIE’s focal areas, including on Debate, Discussion, and Drama. Below, you can find a list of these Collaboration Publications.
    </p>

    <ul class="collaboration-list">
      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (August 2025)</div>
        <p class="collab-desc">Public Speaking in the Language Classroom</p>
        <a href="https://www.mindbrained.org/august-2025-public-speaking/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>

      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (March 2025)</div>
        <p class="collab-desc">Teaching Speech and Presentation in the Language Classroom</p>
        <a href="https://www.mindbrained.org/march-2025-speech-presentation/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>

      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (February 2025)</div>
        <p class="collab-desc">Integrating Music and Performance in the Language Classroom</p>
        <a href="https://www.mindbrained.org/february-2025-music/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>

      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (December 2024)</div>
        <p class="collab-desc">Setting Up Discussions in the Language Classroom</p>
        <a href="https://www.mindbrained.org/december-2024-discussion/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>

      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (November 2024)</div>
        <p class="collab-desc">Debate</p>
        <a href="https://www.mindbrained.org/november-2024-debate/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>

      <li class="collab-item">
        <div class="collab-title"><strong>Mind, Brain, Education SIG</strong> (December 2021)</div>
        <p class="collab-desc">Drama</p>
        <a href="https://www.mindbrained.org/december-2021-drama/" class="collab-link" target="_blank" rel="noopener">View Collaboration &rarr;</a>
      </li>
    </ul>
  </section>

</div>