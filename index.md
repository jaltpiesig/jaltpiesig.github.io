---
layout: default
title: Home
permalink: /
---

<!-- Custom Sloped Bounding Box Styles -->
<style>
  .sloped-box {
    position: relative;
    background: #111111;
    clip-path: polygon(0 0, 100% 0, 100% calc(100% - 15px), 0 100%);
    padding: 30px 25px 45px 25px;
    margin-bottom: 35px;
  }

  .sloped-box-news {
    position: relative;
    background: #111111;
    clip-path: polygon(0 15px, 100% 0, 100% calc(100% - 15px), 0 100%);
    padding: 40px 25px 45px 25px;
    margin-bottom: 35px;
  }

  .gradient-border-bottom {
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, #d8b4fe, #ec4899) 1;
  }

  .gradient-border-top-bottom {
    border-top: 4px solid;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, #6b7280, #9ca3af) 1;
  }

  .text-lilac {
    color: #c084fc !important;
  }

  .text-purple-pink {
    color: #f472b6 !important;
  }

  .text-light-lilac {
    color: #e9d5ff !important;
  }
</style>

<!-- Hero / Intro Box -->
<div class="sloped-box gradient-border-bottom">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <div style="max-width: 650px;">
      <p style="color: #ffffff; font-size: 1.05rem; line-height: 1.7; margin: 0;">
        Welcome to the JALT Performance in Education Special Interest Group (PIE SIG). We support language educators through speech, drama, debate, music, and performance-based pedagogical approaches.
      </p>
    </div>
    <div class="hero-brand-graphic">
      <h1 style="font-size: 2.2rem; margin: 0; font-weight: bold;">
        <span class="text-lilac">PIE</span> <span class="text-purple-pink">sig</span>
      </h1>
      <p style="color: #aaa; font-size: 0.75rem; letter-spacing: 1px; margin-top: 4px;">PERFORMANCE IN EDUCATION</p>
    </div>
  </div>
</div>

<!-- News Section (Jekyll Posts) -->
<div class="sloped-box-news gradient-border-top-bottom">
  <h2 class="text-lilac" style="font-size: 1.8rem; font-weight: bold; margin-bottom: 25px; text-transform: uppercase;">
    NEWS
  </h2>

  <div style="display: flex; flex-direction: column; gap: 20px;">
    {% for post in site.posts limit:4 %}
      <div style="border-bottom: 1px solid rgba(233, 213, 255, 0.2); padding-bottom: 15px;">
        <h3 style="margin: 0 0 6px 0; font-size: 1.15rem;">
          <a href="{{ post.url | relative_url }}" class="text-light-lilac" style="text-decoration: underline; font-weight: bold;">
            {{ post.title }}
          </a>
        </h3>
        <span style="font-size: 0.82rem; color: #a855f7; display: block; margin-bottom: 8px;">
          {{ post.date | date: "%B %d, %Y" }}
        </span>

        {% if forloop.first %}
          <p class="text-light-lilac" style="font-size: 0.92rem; line-height: 1.5; margin: 0;">
            {{ post.content | strip_html | truncatewords: 20 }}
          </p>
        {% endif %}
      </div>
    {% endfor %}
  </div>
</div>

<!-- Podcast Section -->
<div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px; margin-bottom: 35px;">
  <h2 class="text-lilac" style="font-size: 1.8rem; font-weight: bold; margin-bottom: 15px; text-transform: uppercase;">
    PODCAST
  </h2>
  <p style="font-size: 0.95rem; line-height: 1.6; color: #333; margin: 0;">
    Listen to conversations with educators, researchers, and performers in the field of language learning and performance-based education.
  </p>
</div>