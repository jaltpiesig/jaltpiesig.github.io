---
layout: default
title: Publications
permalink: /publications/
---

<div class="publications-header">
  <h1>PIE SIG Publications</h1>
  <p class="lead-text">
    Explore scholarly journals, classroom resources, and conference proceedings published by the Performance in Education Special Interest Group of JALT.
  </p>
</div>

<!-- 1. MASK & GAVEL -->
<section id="mask-and-gavel" class="pub-section">
  {% assign mg = site.data.publications.mask_and_gavel %}
  <h2>Mask & Gavel</h2>
  {%- if mg.issn -%}<span class="issn-badge">ISSN {{ mg.issn }}</span>{%- endif -%}
  <p class="pub-description">{{ mg.description }}</p>

  <div class="submission-info-box">
    <p><strong>Submission Guidelines:</strong> <a href="{{ mg.submission_guidelines_url }}" target="_blank">View JALT Guidelines</a></p>
    <p><strong>Send submissions to:</strong> {{ mg.contact_person }} (<a href="mailto:{{ mg.contact_email }}">{{ mg.contact_email }}</a>)</p>
    <p class="publisher-info">{{ mg.publisher_info }}</p>
  </div>

  <div class="volumes-list">
    {%- if mg.volumes.size > 0 -%}
      {%- for vol in mg.volumes -%}
        <details class="publication-volume">
          <summary class="volume-header">
            <span class="volume-title">{{ vol.volume }}</span>
          </summary>
          <div class="volume-content">
            {%- if vol.doi -%}
              <p class="volume-doi"><strong>DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener">{{ vol.doi }}</a></p>
            {%- endif -%}

            {%- if vol.pdf -%}
              <div class="volume-download-bar">
                <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>
                  📄 Download Full {{ vol.volume }} PDF
                </a>
              </div>
            {%- endif -%}

            {%- if vol.chapters -%}
              <h3 class="chapters-heading" style="margin-top: 15px; margin-bottom: 10px; font-size: 0.95rem;">Table of Contents</h3>
              <ul class="chapter-list">
                {%- for chapter in vol.chapters -%}
                  <li class="chapter-item" style="margin-bottom: 12px; padding-bottom: 8px; border-bottom: 1px dotted rgba(255,255,255,0.15);">
                    <div class="chapter-header-line" style="display: flex; justify-content: space-between; align-items: baseline; gap: 10px;">
                      <strong class="chapter-title" style="font-size: 0.95rem; color: #ffffff;">{{ chapter.title }}</strong>
                      <div class="chapter-actions" style="white-space: nowrap; font-size: 0.85rem;">
                        {%- if chapter.doi -%}
                          <a href="{{ chapter.doi }}" target="_blank" rel="noopener" class="doi-link" style="margin-right: 8px;">DOI</a>
                        {%- endif -%}
                        {%- if chapter.pdf -%}
                          <a href="{{ chapter.pdf }}" class="chapter-pdf-link" target="_blank" download>[PDF]</a>
                        {%- endif -%}
                      </div>
                    </div>
                    {%- if chapter.author -%}
                      <span class="chapter-author" style="display: block; font-size: 0.85rem; opacity: 0.8; margin-top: 2px;">By {{ chapter.author }}</span>
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

<!-- 2. PIE SIG CLASSROOM RESOURCES JOURNAL -->
<section id="classroom-resources" class="pub-section">
  {% assign cr = site.data.publications.classroom_resources %}
  <h2>PIE SIG Classroom Resources Journal</h2>
  {% if cr.issn %}<span class="issn-badge">ISSN {{ cr.issn }}</span>{% endif %}
  <p class="pub-description">{{ cr.description }}</p>

  <div class="submission-info-box">
    <p><strong>Submission Guidelines:</strong> <a href="{{ cr.submission_guidelines_url }}" target="_blank">View JALT Guidelines</a> (Use JALT’s <em>My Share</em> column guidelines)</p>
    <p><strong>Send submissions to:</strong> {{ cr.contact_person }} (<a href="mailto:{{ cr.contact_email }}">{{ cr.contact_email }}</a>)</p>
    <p class="publisher-info">{{ cr.publisher_info }}</p>
  </div>

  <div class="volumes-list">
    {% if cr.volumes.size > 0 %}
      {% for vol in cr.volumes %}
        <details class="publication-volume">
          <summary class="volume-header">
            <span class="volume-title">{{ vol.volume }}</span>
          </summary>
          <div class="volume-content">
            {% if vol.pdf %}
              <div class="volume-download-bar">
                <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>
                  📄 Download Full {{ vol.volume }} PDF
                </a>
              </div>
            {% endif %}

            {% if vol.chapters %}
              <h3 class="chapters-heading">Table of Contents</h3>
              <ul class="chapter-list">
                {% for chapter in vol.chapters %}
                  <li class="chapter-item">
                    <div class="chapter-header-line">
                      <strong class="chapter-title">{{ chapter.number }}. {{ chapter.title }}</strong>
                    </div>
                    <span class="chapter-author">By {{ chapter.author }}</span>
                  </li>
                {% endfor %}
              </ul>
            {% endif %}
          </div>
        </details>
      {% endfor %}
    {% else %}
      <p class="no-volumes">Volume details coming soon.</p>
    {% endif %}
  </div>
</section>

<!-- 3. PERFORMANCE IN EDUCATION REVIEW -->
<section id="pie-review" class="pub-section">
  {% assign pr = site.data.publications.pie_review %}
  <h2>Performance in Education Review</h2>
  <p class="pub-description">{{ pr.description }}</p>

  <div class="submission-info-box">
    <p><strong>Submission Guidelines:</strong> <a href="{{ pr.submission_guidelines_url }}" target="_blank">View JALT Guidelines</a></p>
    <p><strong>Send submissions to:</strong> {{ pr.contact_person }} (<a href="mailto:{{ pr.contact_email }}">{{ pr.contact_email }}</a>)</p>
    <p class="publisher-info">{{ pr.publisher_info }}</p>
  </div>

  <div class="volumes-list">
    {%- if pr.volumes.size > 0 -%}
      {%- for vol in pr.volumes -%}
        <details class="publication-volume">
          <summary class="volume-header">
            <span class="volume-title">{{ vol.volume }}</span>
          </summary>
          <div class="volume-content">
            {%- if vol.pdf -%}
              <div class="volume-download-bar">
                <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>
                  📄 Download Full {{ vol.volume }} PDF
                </a>
              </div>
            {%- endif -%}

            {%- if vol.sections -%}
              <h3 class="chapters-heading">Table of Contents</h3>
              {%- for sec in vol.sections -%}
                <div class="toc-category-group">
                  <h4 class="toc-category-title">{{ sec.category | strip }}</h4>
                  <ul class="chapter-list">
                    {%- for item in sec.items -%}
                      <li class="chapter-item">
                        <div class="chapter-header-line">
                          <strong class="chapter-title">{{ item.title | strip }}</strong>
                          {%- if item.page -%}<span class="chapter-page-no">({{ item.page | strip }})</span>{%- endif -%}
                        </div>
                        {%- if item.author -%}<span class="chapter-author">By {{ item.author | strip }}</span>{%- endif -%}
                      </li>
                    {%- endfor -%}
                  </ul>
                </div>
              {%- endfor -%}
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p class="no-volumes">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 4. Black Footer Bar: Socials Bottom-Left + PIE SIG & JALT Logos Bottom-Right -->
<footer class="site-black-footer">
  <div class="footer-social-links">
    <a href="#" class="social-circle-btn" title="Facebook">f</a>
    <a href="#" class="social-circle-btn" title="YouTube">yt</a>
    <a href="#" class="social-circle-btn" title="X / Twitter">x</a>
    <a href="#" class="social-circle-btn" title="LinkedIn">in</a>
  </div>

  <div class="footer-brand-logos">
    <span>PIE sig</span> | <span>JALT</span>
  </div>
</footer>