---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<!-- Custom CSS matching index.md, about.md, and best-of-pie.md -->
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

  .event-link {
    color: var(--pie-heading-dark);
    font-weight: bold;
    text-decoration: underline;
    transition: color 0.2s ease;
  }

  .event-link:hover {
    color: var(--pie-purple-pink);
  }

  .event-title-link {
    color: var(--pie-heading-dark);
    text-decoration: none;
    font-weight: bold;
    transition: color 0.2s ease;
  }

  .event-title-link:hover {
    color: var(--pie-purple-pink);
  }
</style>

<!-- Top Hero Sloped Dark Box -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Text -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">CONFERENCES & EVENTS</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        Discover upcoming research gatherings, practical workshops, and performances sponsored by JALT PIE SIG.
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

<!-- 1. ABOUT PIE SIG CONFERENCES -->
<div style="margin-bottom: 45px; padding: 0 5px;">
  <h2 class="heading-serif" style="margin-bottom: 15px;">
    ABOUT PIE SIG CONFERENCES
  </h2>
  
  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 14px;">
    The Performance In Education SIG of the Japan Association for Language Teaching (JALT) sponsors several conferences a year, usually in convenient and interesting locations, with workshops, presentations, and performances. Families are always welcome.
  </p>

  <blockquote style="font-family: 'Playfair Display', 'Georgia', serif; font-style: italic; font-size: 1.1rem; color: var(--pie-heading-dark); border-left: 3px solid var(--pie-heading-dark); padding-left: 16px; margin: 20px 0; padding-top: 4px; padding-bottom: 4px;">
    “We are always trying to grow and spread our message through collaboration with YOU.”
  </blockquote>

  <p style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222); margin-bottom: 20px;">
    What draws many people to the PIE SIG are the amazing and effective activities described by SIG members, the creative talents of the teachers/performers, and most of all, the warm, friendly atmosphere that we work hard to create. We are useful and <strong>FUN</strong>.
  </p>

  <div style="border-bottom: 1px solid rgba(138, 72, 184, 0.2); padding-bottom: 20px; margin-top: 20px;">
    <strong style="color: var(--pie-heading-dark); font-size: 1.05rem; display: block; margin-bottom: 6px;">Want to collaborate with us?</strong>
    <p style="font-size: 0.92rem; line-height: 1.5; color: var(--text-dark, #222222); margin: 0;">
      Contact us at <a href="mailto:jaltpiesig@gmail.com" class="event-link">jaltpiesig@gmail.com</a> if you are in the collaborative mood or come and see for yourself what we are about at our annual Performance in Education Research & Practice Conference.
    </p>
  </div>
</div>

<!-- 2. LATEST EVENT -->
<div style="margin-bottom: 45px; padding: 0 5px;">
  <h2 class="heading-serif" style="margin-bottom: 20px;">
    LATEST EVENT
  </h2>

  {% assign latest_post = site.posts.first %}
  {% if latest_post %}
    <div style="border-bottom: 1px solid rgba(138, 72, 184, 0.2); padding-bottom: 20px;">
      <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; gap: 10px; margin-bottom: 12px;">
        <h3 style="font-size: 1.35rem; margin: 0;">
          <a href="{{ latest_post.url }}" class="event-title-link">{{ latest_post.title }}</a>
        </h3>
        <span style="font-size: 0.8rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 3px 10px; border-radius: 4px; font-weight: bold; display: inline-block;">{{ latest_post.date | date: "%B %d, %Y" }}</span>
      </div>
      
      <div style="font-size: 0.95rem; line-height: 1.6; color: var(--text-dark, #222222);">
        {{ latest_post.content }}
      </div>
    </div>
  {% else %}
    <p style="font-style: italic; color: #666;">No upcoming events listed at this time.</p>
  {% endif %}
</div>

<!-- 3. ALL EVENTS -->
<div style="margin-bottom: 35px; padding: 0 5px;">
  <h2 class="heading-serif" style="margin-bottom: 20px;">
    ALL EVENTS
  </h2>

  {% if site.posts.size > 0 %}
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px;">
      {% for post in site.posts %}
        <div style="border-bottom: 1px solid rgba(138, 72, 184, 0.2); padding-bottom: 15px; display: flex; flex-direction: column; justify-content: space-between;">
          <div>
            <span style="font-size: 0.8rem; background: var(--primary-navy, #1C2B36); color: #ffffff; padding: 2px 8px; border-radius: 4px; font-weight: bold; display: inline-block; margin-bottom: 8px;">{{ post.date | date: "%B %d, %Y" }}</span>
            <h3 style="font-size: 1.1rem; margin: 0 0 10px 0;">
              <a href="{{ post.url }}" class="event-title-link">{{ post.title }}</a>
            </h3>
          </div>
          <a href="{{ post.url }}" class="event-link" style="font-size: 0.88rem;">View Event Details &rarr;</a>
        </div>
      {% endfor %}
    </div>
  {% else %}
    <p style="font-style: italic; color: #666;">No events found.</p>
  {% endif %}
</div>