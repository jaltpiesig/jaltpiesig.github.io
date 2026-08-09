---
layout: default
title: Home
permalink: /
---

<!-- Custom CSS for Styles, Colors, Slopes, and Hover Effects -->
<style>
  :root {
    --pie-bg-purple: #f4effa;       /* Very light purple tint between boxes */
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink color for 'sig' */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark boxes */
    --pie-lilac-hover: #ffffff;      /* Hover color for news links */
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped boxes using exact primary navy footer background color (#1C2B36) */
  .sloped-box-top {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 30px 25px 40px 25px;
    margin-bottom: 30px;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, var(--pie-heading-dark), var(--pie-purple-pink)) 1;
  }

  .sloped-box-news {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 35px 25px 40px 25px;
    margin-bottom: 30px;
    border-top: 4px solid #6c757d;
    border-bottom: 4px solid #6c757d;
  }

  .heading-serif {
    font-family: "Playfair Display", "Georgia", "Times New Roman", serif;
    color: var(--pie-heading-dark);
    font-size: 1.8rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  .news-link {
    color: var(--pie-light-lilac);
    text-decoration: underline;
    font-weight: bold;
    transition: color 0.2s ease-in-out;
  }

  .news-link:hover {
    color: var(--pie-lilac-hover);
  }
</style>

<!-- Hero / Intro Box -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 20px;">
    <!-- Left Paragraph -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <p style="color: #ffffff; font-size: 1.05rem; line-height: 1.7; margin: 0;">
        Welcome to the JALT Performance in Education Special Interest Group (PIE SIG). We support language educators through speech, drama, debate, music, and performance-based pedagogical approaches.
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