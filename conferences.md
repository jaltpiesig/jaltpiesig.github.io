---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<!-- Top Hero Title Banner -->
<div class="hero-black-box mb-30">
  <div>
    <h2>CONFERENCES & EVENTS</h2>
    <p class="hero-intro-text">
      Discover upcoming research gatherings, practical workshops, and performances sponsored by JALT PIE SIG.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- 1. ABOUT PIE SIG CONFERENCES -->
<section class="events-about-card">
  <h2 class="events-section-title">ABOUT PIE SIG CONFERENCES</h2>
  
  <p class="events-body-text">
    The Performance In Education SIG of the Japan Association for Language Teaching (JALT) sponsors several conferences a year, usually in convenient and interesting locations, with workshops, presentations, and performances. Families are always welcome.
  </p>

  <blockquote class="events-quote">
    “We are always trying to grow and spread our message through collaboration with YOU.”
  </blockquote>

  <p class="events-body-text">
    What draws many people to the PIE SIG are the amazing and effective activities described by SIG members, the creative talents of the teachers/performers, and most of all, the warm, friendly atmosphere that we work hard to create. We are useful and <strong>FUN</strong>.
  </p>

  <div class="events-callout-box">
    <strong>Want to collaborate with us?</strong>
    <p>
      Contact us at <a href="mailto:jaltpiesig@gmail.com">jaltpiesig@gmail.com</a> if you are in the collaborative mood or come and see for yourself what we are about at our annual Performance in Education Research & Practice Conference.
    </p>
  </div>
</section>

<!-- 2. LATEST EVENT -->
<section class="events-section">
  <h2 class="events-section-title">LATEST EVENT</h2>

  {% assign latest_post = site.posts.first %}
  {% if latest_post %}
    <article class="latest-event-card">
      <header class="latest-event-header">
        <h3 class="latest-event-title">
          <a href="{{ latest_post.url }}">{{ latest_post.title }}</a>
        </h3>
        <span class="event-date">{{ latest_post.date | date: "%B %d, %Y" }}</span>
      </header>
      
      <div class="latest-event-content">
        {{ latest_post.content }}
      </div>
    </article>
  {% else %}
    <p class="no-events-text">No upcoming events listed at this time.</p>
  {% endif %}
</section>

<!-- 3. ALL EVENTS -->
<section class="events-section">
  <h2 class="events-section-title">ALL EVENTS</h2>

  {% if site.posts.size > 0 %}
    <div class="all-events-grid">
      {% for post in site.posts %}
        <article class="event-mini-card">
          <div>
            <span class="event-date">{{ post.date | date: "%B %d, %Y" }}</span>
            <h3 class="event-card-title">
              <a href="{{ post.url }}">{{ post.title }}</a>
            </h3>
          </div>
          <a href="{{ post.url }}" class="event-card-link">View Event Details &rarr;</a>
        </article>
      {% endfor %}
    </div>
  {% else %}
    <p class="no-events-text">No events found.</p>
  {% endif %}
</section>