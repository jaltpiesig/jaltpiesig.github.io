---
layout: default
title: Home
permalink: /
---

<!-- Custom Styling matching publications.md & officers.md design system -->
<style>
  :root {
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink accent */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark boxes */
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped hero container matching publications.md / officers.md */
  .sloped-box-top {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 35px 25px 40px 25px;
    margin-bottom: 30px;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, var(--pie-heading-dark), var(--pie-purple-pink)) 1;
  }

  .home-card-wrapper {
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.18);
    border-radius: 8px;
    padding: 22px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .home-card-wrapper:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(138, 72, 184, 0.1);
    border-color: var(--pie-heading-dark);
  }

  .heading-serif {
    font-family: "Playfair Display", "Georgia", "Times New Roman", serif;
    color: var(--pie-heading-dark);
    font-size: 1.5rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .post-preview {
    padding-bottom: 15px;
    margin-bottom: 15px;
    border-bottom: 1px solid rgba(138, 72, 184, 0.12);
  }

  .post-preview:last-child {
    border-bottom: none;
    margin-bottom: 0;
    padding-bottom: 0;
  }
</style>

<!-- Top Hero Sloped Dark Box (Matching officers.md & publications.md layout) -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Text -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">WELCOME TO PIE SIG</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs.
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

<!-- Podcast Section -->
<div style="margin-bottom: 35px; padding: 10px 5px;">
  <h2 class="heading-serif" style="margin-bottom: 12px;">
    PODCAST
  </h2>
  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 20px;">
    Listen to conversations with educators, researchers, and performers in the field of language learning and performance-based education.
  </p>
  
  <!-- Buzzsprout Podcast Player -->
  <div id="buzzsprout-large-player"></div>
  <script type="text/javascript" charset="utf-8" src="https://www.buzzsprout.com/2520024.js?container_id=buzzsprout-large-player&amp;player=large"></script>
</div>

<!-- News Section (Jekyll Posts) -->
<div class="sloped-box-news">
  <h2 class="heading-serif" style="margin-bottom: 25px;">
    NEWS
  </h2>

  <div style="display: flex; flex-direction: column; gap: 20px;">
    {% for post in site.posts limit:4 %}
      <div style="border-bottom: 1px solid rgba(227, 218, 245, 0.2); padding-bottom: 15px;">
        <h3 style="margin: 0 0 6px 0; font-size: 1.15rem;">
          <a href="{{ post.url | relative_url }}" class="news-link">
            {{ post.title }}
          </a>
        </h3>
        <span style="font-size: 0.82rem; color: var(--pie-purple-pink); display: block; margin-bottom: 8px;">
          {{ post.date | date: "%B %d, %Y" }}
        </span>

        {% if forloop.first %}
          <p style="color: var(--pie-light-lilac); font-size: 0.92rem; line-height: 1.5; margin: 0;">
            {{ post.content | strip_html | truncatewords: 20 }}
          </p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</div>