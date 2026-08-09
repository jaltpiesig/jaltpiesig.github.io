---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<div class="conferences-container">

  <!-- Intro Paragraph -->
  <p class="conferences-intro">
    The Performance In Education SIG sponsors conferences throughout the year featuring practical workshops, research presentations, and creative performances. Explore our featured event below or browse past gatherings.
  </p>

  <!-- 1. LATEST EVENT FEATURED CARD -->
  <section class="conf-section">
    <h2 class="conf-heading">Latest Event</h2>

    {% assign latest_post = site.posts.first %}
    {% if latest_post %}
      <article class="featured-event-card">
        <div class="featured-badge">Featured Event</div>
        <header class="featured-event-header">
          <h1 class="featured-event-title">
            <a href="{{ latest_post.url }}">{{ latest_post.title }}</a>
          </h1>
          <time class="featured-event-date">
            <span class="icon">📅</span> {{ latest_post.date | date: "%B %d, %Y" }}
          </time>
        </header>

        <div class="featured-event-body">
          {{ latest_post.content }}
        </div>
      </article>
    {% else %}
      <p class="no-events">No upcoming events listed at this time.</p>
    {% endif %}
  </section>

  <!-- 2. ALL EVENTS LIST -->
  <section class="conf-section">
    <h2 class="conf-heading">All Events</h2>

    {% if site.posts.size > 0 %}
      <div class="events-grid">
        {% for post in site.posts %}
          <div class="event-card">
            <div class="event-card-content">
              <span class="event-date-badge">{{ post.date | date: "%b %d, %Y" }}</span>
              <h3 class="event-card-title">
                <a href="{{ post.url }}">{{ post.title }}</a>
              </h3>
            </div>
            <a href="{{ post.url }}" class="event-card-link" aria-label="Read more about {{ post.title }}">Read Details &rarr;</a>
          </div>
        {% endfor %}
      </div>
    {% else %}
      <p class="no-events">No events found.</p>
    {% endif %}
  </section>

  <!-- 3. ABOUT & COLLABORATION CALLOUT BOX -->
  <section class="conf-info-box">
    <div class="info-box-header">
      <h2>About PIE SIG Conferences</h2>
    </div>
    
    <p>
      The Performance In Education SIG of the Japan Association for Language Teaching (JALT) sponsors several conferences a year, usually in convenient and interesting locations, with workshops, presentations, and performances. Families are always welcome.
    </p>

    <blockquote class="conf-quote">
      “We are always trying to grow and spread our message through collaboration with YOU.”
    </blockquote>

    <p>
      What draws many people to the PIE SIG are the amazing and effective activities described by SIG members, the creative talents of the teachers/performers, and most of all, the warm, friendly atmosphere that we work hard to create. We are useful and <strong>FUN</strong>.
    </p>

    <div class="conf-collab-card">
      <div class="collab-icon">🤝</div>
      <div class="collab-text">
        <strong>Want to collaborate with us?</strong>
        <p>
          Contact us at <a href="mailto:jaltpiesig@gmail.com">jaltpiesig@gmail.com</a> if you are in the collaborative mood or come and see for yourself what we are about at our annual Performance in Education Research & Practice Conference.
        </p>
      </div>
    </div>
  </section>

</div>