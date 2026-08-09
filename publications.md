---
layout: default
title: Publications
---

<div class="publications-container">
  <h1 class="section-title">Publications</h1>

  <!-- Introductory Paragraph -->
  <p class="publications-intro">
    The PIE SIG publishes two main journals: Mask & Gavel is our official peer-reviewed journal and the PIE SIG Classroom Resources Journal which is a collection of My Share-type articles. Article submissions are accepted year-round, will be published online as they are finalized (with page numbers and DOIs for citation), and will be collected into full volumes that will be published as PDFs once we accumulate a sufficient number of articles.
  </p>

  <!-- Category Navigation Bar -->
  <nav class="pub-nav">
    <a href="#mask-and-gavel">Mask & Gavel</a>
    <a href="#classroom-resources">Classroom Resources</a>
    <a href="#pie-review">PIE Review</a>
    <a href="#collaborations">Collaborations</a>
    <a href="#pre-publication">Pre-Publication</a>
  </nav>

  <!-- 1. MASK & GAVEL -->
  <section id="mask-and-gavel" class="pub-section">
    {% assign mg = site.data.publications.mask_and_gavel %}
    <h2>Mask & Gavel</h2>
    <span class="issn-badge">ISSN {{ mg.issn }}</span>
    <p class="pub-description">{{ mg.description }}</p>

    <div class="submission-info-box">
      <p><strong>Submission Guidelines:</strong> <a href="{{ mg.submission_guidelines_url }}" target="_blank">View JALT Guidelines</a></p>
      <p><strong>Send submissions to:</strong> {{ mg.contact_person }} (<a href="mailto:{{ mg.contact_email }}">{{ mg.contact_email }}</a>)</p>
      <p class="publisher-info">{{ mg.publisher_info }}</p>
    </div>

    <!-- Collapsible Volumes Container -->
    <div class="volumes-list">
      {% if mg.volumes.size > 0 %}
        {% for vol in mg.volumes %}
          <details class="publication-volume">
            <summary class="volume-header">
              <span class="volume-title">{{ vol.volume }}</span>
              {% if vol.subtitle %}<span class="volume-subtitle">{{ vol.subtitle }}</span>{% endif %}
            </summary>
            <div class="volume-content">
              {% if vol.pdf %}
                <div class="volume-download-bar">
                  <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>📄 Download Full Issue PDF</a>
                </div>
              {% endif %}
              {% if vol.chapters %}
                <ul class="chapter-list">
                  {% for chapter in vol.chapters %}
                    <li class="chapter-item">
                      <div class="chapter-header-line">
                        <strong class="chapter-title">{{ chapter.title }}</strong>
                        {% if chapter.pdf %}<a href="{{ chapter.pdf }}" class="chapter-pdf-link" target="_blank" download>[ Download PDF ]</a>{% endif %}
                      </div>
                      {% if chapter.author %}<span class="chapter-author">By {{ chapter.author }}</span>{% endif %}
                      {% if chapter.abstract %}<p class="chapter-abstract">{{ chapter.abstract }}</p>{% endif %}
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

  <!-- 2. PIE SIG CLASSROOM RESOURCES JOURNAL -->
  <section id="classroom-resources" class="pub-section">
    {% assign cr = site.data.publications.classroom_resources %}
    <h2>PIE SIG Classroom Resources Journal</h2>
    <span class="issn-badge">ISSN {{ cr.issn }}</span>
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
              {% if vol.subtitle %}<span class="volume-subtitle">{{ vol.subtitle }}</span>{% endif %}
            </summary>
            <div class="volume-content">
              {% if vol.pdf %}
                <div class="volume-download-bar">
                  <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>📄 Download Full Issue PDF</a>
                </div>
              {% endif %}
              {% if vol.chapters %}
                <ul class="chapter-list">
                  {% for chapter in vol.chapters %}
                    <li class="chapter-item">
                      <div class="chapter-header-line">
                        <strong class="chapter-title">{{ chapter.title }}</strong>
                        {% if chapter.pdf %}<a href="{{ chapter.pdf }}" class="chapter-pdf-link" target="_blank" download>[ Download PDF ]</a>{% endif %}
                      </div>
                      {% if chapter.author %}<span class="chapter-author">By {{ chapter.author }}</span>{% endif %}
                      {% if chapter.abstract %}<p class="chapter-abstract">{{ chapter.abstract }}</p>{% endif %}
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
      {% if pr.volumes.size > 0 %}
        {% for vol in pr.volumes %}
          <details class="publication-volume">
            <summary class="volume-header">
              <span class="volume-title">{{ vol.volume }}</span>
            </summary>
            <div class="volume-content">
              {% if vol.pdf %}
                <div class="volume-download-bar">
                  <a href="{{ vol.pdf }}" class="download-pdf-btn" target="_blank" download>📄 Download Full Issue PDF</a>
                </div>
              {% endif %}
            </div>
          </details>
        {% endfor %}
      {% else %}
        <p class="no-volumes">Volume details coming soon.</p>
      {% endif %}
    </div>
  </section>

  <!-- 4. COLLABORATION PUBLICATIONS -->
  <section id="collaborations" class="pub-section">
    {% assign col = site.data.publications.collaboration_publications %}
    <h2>Collaboration Publications</h2>
    <p class="pub-description">{{ col.description }}</p>

    <ul class="collaboration-list">
      {% for item in col.links %}
        <li class="collab-item">
          <strong>{{ item.organization }} ({{ item.date }}):</strong>
          <a href="{{ item.url }}" target="_blank" rel="noopener">{{ item.title }} ↗</a>
        </li>
      {% endfor %}
    </ul>
  </section>

  <!-- 5. PRE-PUBLICATION PAGES -->
  <section id="pre-publication" class="pub-section">
    {% assign prep = site.data.publications.pre_publication %}
    <h2>Pre-Publication Pages</h2>
    <p class="pub-description">{{ prep.description }}</p>
    <a href="{{ prep.url }}" target="_blank" rel="noopener" class="external-link-btn">
      🌐 Visit Pre-Publication Pages Site ↗
    </a>
  </section>
</div>