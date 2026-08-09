---
layout: default
title: Publications
permalink: /publications/
---

<!-- Top Hero Title Banner -->
<div class="hero-black-box" style="margin-bottom: 30px;">
  <div>
    <h1 style="color: #ffffff; font-size: 2rem; font-weight: bold;">PUBLICATIONS</h1>
    <p class="hero-intro-text" style="margin-top: 6px;">
      Explore our peer-reviewed journals, classroom resource collections, conference reviews, and collaborative works.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Intro & Submission Info Card -->
<div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px; margin-bottom: 35px;">
  <p style="font-size: 0.95rem; line-height: 1.6; color: #333; margin-bottom: 18px;">
    The PIE SIG publishes two main journals: <strong>Mask & Gavel</strong> is our official peer-reviewed journal and the <strong>PIE SIG Classroom Resources Journal</strong> which is a collection of My Share-type articles. Article submissions are accepted year-round, will be published online as they are finalized (with page numbers and DOIs for citation), and will be collected into full volumes that will be published as PDFs once we accumulate a sufficient number of articles.
  </p>

  <!-- Submission Details Box -->
  <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 18px;">
    <p style="font-size: 0.9rem; margin-bottom: 8px; color: #333;">
      <strong>Submission Guidelines:</strong> <a href="https://jalt-publications.org/tlt/submissions" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">View JALT Guidelines</a>
    </p>
    <p style="font-size: 0.9rem; margin-bottom: 12px; color: #333;">
      <strong>Send Submissions To:</strong> Philip Head (<a href="mailto:piesigpublications@gmail.com" style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">piesigpublications@gmail.com</a>)
    </p>
    <p style="font-size: 0.82rem; color: #666; line-height: 1.5; margin: 0; border-top: 1px dashed var(--border-subtle); padding-top: 10px;">
      Published by the Performance in Education Special Interest Group, The Japan Association for Language Teaching, JALT Central Office, Urban Edge Bldg 5F, 1-37-9 Taito, Taito-ku, Tokyo.
    </p>
  </div>
</div>

<!-- Category Navigation -->
<div style="display: flex; gap: 10px; flex-wrap: wrap; margin-bottom: 35px;">
  <a href="#mask-and-gavel" style="background: #ffffff; border: 1px solid var(--border-subtle); padding: 8px 16px; border-radius: 6px; color: var(--burgundy-accent); font-weight: bold; font-size: 0.88rem; text-decoration: none;">Mask & Gavel</a>
  <a href="#classroom-resources" style="background: #ffffff; border: 1px solid var(--border-subtle); padding: 8px 16px; border-radius: 6px; color: var(--burgundy-accent); font-weight: bold; font-size: 0.88rem; text-decoration: none;">Classroom Resources Journal</a>
  <a href="#pie-review" style="background: #ffffff; border: 1px solid var(--border-subtle); padding: 8px 16px; border-radius: 6px; color: var(--burgundy-accent); font-weight: bold; font-size: 0.88rem; text-decoration: none;">PIE Review</a>
  <a href="#collaborations" style="background: #ffffff; border: 1px solid var(--border-subtle); padding: 8px 16px; border-radius: 6px; color: var(--burgundy-accent); font-weight: bold; font-size: 0.88rem; text-decoration: none;">Collaborations</a>
</div>

<!-- 1. MASK & GAVEL -->
<section id="mask-and-gavel" style="margin-bottom: 35px;">
  {% assign mg = site.data.publications.mask_and_gavel %}
  <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px;">
    <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; border-bottom: 2px solid var(--border-subtle); padding-bottom: 8px; margin-bottom: 14px;">
      <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin: 0;">MASK & GAVEL</h2>
      {%- if mg.issn -%}
        <span style="font-size: 0.8rem; background: #f0f0f4; border: 1px solid var(--border-subtle); padding: 3px 8px; border-radius: 4px; font-weight: bold; color: #555;">ISSN {{ mg.issn }}</span>
      {%- endif -%}
    </div>

    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-bottom: 20px;">
      Mask & Gavel is the peer-reviewed academic journal of the Performance in Education SIG.
      <br><br>
      Article submissions are accepted year-round and published online as soon as they are finalized, before being collected into the full journal published online bi-annually. All articles are vetted by an editor, blinded, and peer-reviewed by two reviewers before publication. We welcome research-based, comment & opinion, interview, and review-based articles. Practical lesson resource articles should be submitted to the Classroom Resources journal. For submission guidelines please refer to the specifications outlined in The Language Teacher.
    </p>

    <!-- Volumes -->
    {%- if mg.volumes.size > 0 -%}
      {%- for vol in mg.volumes -%}
        <details style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 12px 16px; margin-bottom: 12px;">
          <summary style="font-weight: bold; color: var(--burgundy-accent); cursor: pointer; font-size: 0.95rem;">
            {{ vol.volume }}
          </summary>
          <div style="margin-top: 12px; padding-top: 10px; border-top: 1px solid var(--border-subtle); font-size: 0.88rem;">
            {%- if vol.doi -%}
              <p style="margin-bottom: 8px;"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold;">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p style="margin-bottom: 12px;">
                <a href="{{ vol.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong style="display: block; margin-bottom: 8px; color: #333;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-bottom: 1px dashed var(--border-subtle); padding: 8px 0;">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 10px;">
                      <strong style="color: #222;">{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: none;">[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 2px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #666; font-size: 0.82rem;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent);">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 2. CLASSROOM RESOURCES JOURNAL -->
<section id="classroom-resources" style="margin-bottom: 35px;">
  {% assign cr = site.data.publications.classroom_resources %}
  <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px;">
    <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; border-bottom: 2px solid var(--border-subtle); padding-bottom: 8px; margin-bottom: 14px;">
      <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin: 0;">PIE SIG CLASSROOM RESOURCES JOURNAL</h2>
      {%- if cr.issn -%}
        <span style="font-size: 0.8rem; background: #f0f0f4; border: 1px solid var(--border-subtle); padding: 3px 8px; border-radius: 4px; font-weight: bold; color: #555;">ISSN {{ cr.issn }}</span>
      {%- endif -%}
    </div>

    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-bottom: 20px;">
      The classroom resource journal of the Performance in Education SIG. PIE SIG has put together a new lesson resource online publication, and it is now available online. This is the publication for the sharing of practical lesson resources.
    </p>

    {%- if cr.volumes.size > 0 -%}
      {%- for vol in cr.volumes -%}
        <details style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 12px 16px; margin-bottom: 12px;">
          <summary style="font-weight: bold; color: var(--burgundy-accent); cursor: pointer; font-size: 0.95rem;">
            {{ vol.volume }}
          </summary>
          <div style="margin-top: 12px; padding-top: 10px; border-top: 1px solid var(--border-subtle); font-size: 0.88rem;">
            {%- if vol.doi -%}
              <p style="margin-bottom: 8px;"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold;">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p style="margin-bottom: 12px;">
                <a href="{{ vol.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong style="display: block; margin-bottom: 8px; color: #333;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-bottom: 1px dashed var(--border-subtle); padding: 8px 0;">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 10px;">
                      <strong style="color: #222;">{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: none;">[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 2px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #666; font-size: 0.82rem;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent);">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 3. PIE REVIEW -->
<section id="pie-review" style="margin-bottom: 35px;">
  {% assign pr = site.data.publications.pie_review %}
  <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px;">
    <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; border-bottom: 2px solid var(--border-subtle); padding-bottom: 8px; margin-bottom: 14px;">
      <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin: 0;">PERFORMANCE IN EDUCATION REVIEW</h2>
      {%- if pr.issn -%}
        <span style="font-size: 0.8rem; background: #f0f0f4; border: 1px solid var(--border-subtle); padding: 3px 8px; border-radius: 4px; font-weight: bold; color: #555;">ISSN {{ pr.issn }}</span>
      {%- endif -%}
    </div>

    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-bottom: 20px;">
      Some of PIE SIG’s amazing conference presenters have been kind enough to write scholarly articles on their presentations, workshops, and performances. The Performance in Education Review presents some of these notable articles previously presented at PIE SIG conferences. The intention of this journal is to create a montage of the year in PIE conferences, but some volumes may cover multiple years due to the time needed to gather all proposals.
    </p>

    {%- if pr.volumes.size > 0 -%}
      {%- for vol in pr.volumes -%}
        <details style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 12px 16px; margin-bottom: 12px;">
          <summary style="font-weight: bold; color: var(--burgundy-accent); cursor: pointer; font-size: 0.95rem;">
            {{ vol.volume }}
          </summary>
          <div style="margin-top: 12px; padding-top: 10px; border-top: 1px solid var(--border-subtle); font-size: 0.88rem;">
            {%- if vol.doi -%}
              <p style="margin-bottom: 8px;"><strong>Volume DOI:</strong> <a href="{{ vol.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold;">{{ vol.doi }}</a></p>
            {%- endif -%}
            {%- if vol.pdf -%}
              <p style="margin-bottom: 12px;">
                <a href="{{ vol.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">📄 Download Full {{ vol.volume }} PDF</a>
              </p>
            {%- endif -%}

            {%- if vol.chapters -%}
              <strong style="display: block; margin-bottom: 8px; color: #333;">Table of Contents</strong>
              <ul style="list-style: none; padding: 0; margin: 0;">
                {%- for chapter in vol.chapters -%}
                  <li style="border-bottom: 1px dashed var(--border-subtle); padding: 8px 0;">
                    <div style="display: flex; justify-content: space-between; align-items: flex-start; gap: 10px;">
                      <strong style="color: #222;">{{ chapter.title }}</strong>
                      {%- if chapter.pdf -%}
                        <a href="{{ chapter.pdf }}" target="_blank" download style="color: var(--burgundy-accent); font-weight: bold; text-decoration: none;">[PDF]</a>
                      {%- endif -%}
                    </div>
                    {%- if chapter.author -%}
                      <span style="display: block; color: #666; font-size: 0.82rem; margin-top: 2px;">By {{ chapter.author }}</span>
                    {%- endif -%}
                    {%- if chapter.doi -%}
                      <span style="display: block; color: #666; font-size: 0.82rem;">DOI: <a href="{{ chapter.doi }}" target="_blank" rel="noopener" style="color: var(--burgundy-accent);">{{ chapter.doi }}</a></span>
                    {%- endif -%}
                  </li>
                {%- endfor -%}
              </ul>
            {%- endif -%}
          </div>
        </details>
      {%- endfor -%}
    {%- else -%}
      <p style="font-style: italic; color: #666; font-size: 0.9rem;">Volume details coming soon.</p>
    {%- endif -%}
  </div>
</section>

<!-- 4. COLLABORATIONS -->
<section id="collaborations" style="margin-bottom: 35px;">
  <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px;">
    <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; border-bottom: 2px solid var(--border-subtle); padding-bottom: 8px; margin-bottom: 14px;">
      COLLABORATION PUBLICATIONS
    </h2>
    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-bottom: 20px;">
      PIE SIG also co-publishes issues centered around PIE’s focal areas, including on Debate, Discussion, and Drama. Below, you can find a list of these Collaboration Publications.
    </p>

    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 15px;">
      
      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">August 2025</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Public Speaking in the Language Classroom</p>
        </div>
        <a href="https://www.mindbrained.org/august-2025-public-speaking/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">March 2025</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Teaching Speech and Presentation in the Language Classroom</p>
        </div>
        <a href="https://www.mindbrained.org/march-2025-speech-presentation/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">February 2025</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Integrating Music and Performance in the Language Classroom</p>
        </div>
        <a href="https://www.mindbrained.org/february-2025-music/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">December 2024</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Setting Up Discussions in the Language Classroom</p>
        </div>
        <a href="https://www.mindbrained.org/december-2024-discussion/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">November 2024</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Debate</p>
        </div>
        <a href="https://www.mindbrained.org/november-2024-debate/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

      <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; display: flex; flex-direction: column; justify-content: space-between;">
        <div>
          <strong style="color: var(--burgundy-accent); display: block; font-size: 0.95rem;">Mind, Brain, Education SIG</strong>
          <span style="font-size: 0.8rem; color: #666; font-weight: bold;">December 2021</span>
          <p style="font-size: 0.9rem; color: #333; margin: 8px 0 14px 0;">Drama</p>
        </div>
        <a href="https://www.mindbrained.org/december-2021-drama/" target="_blank" rel="noopener" style="color: var(--burgundy-accent); font-weight: bold; font-size: 0.85rem; text-decoration: none;">View Collaboration &rarr;</a>
      </div>

    </div>
  </div>
</section>