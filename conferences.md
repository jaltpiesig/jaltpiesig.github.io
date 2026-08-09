---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<div class="events-container">

  <!-- 1. LATEST EVENT -->
  <section class="events-section">
    <h2 class="events-heading">Latest Event</h2>

    {% assign latest_post = site.posts.first %}
    {% if latest_post %}
      <article class="latest-event-card">
        <header class="latest-event-header">
          <h1 class="latest-event-title"><a href="{{ latest_post.url }}">{{ latest_post.title }}</a></h1>
          <span class="latest-event-date">{{ latest_post.date | date: "%B %d, %Y" }}</span>
        </header>
        
        <div class="latest-event-content">
          {{ latest_post.content }}
        </div>
      </article>
    {% else %}
      <p class="no-events-text">No upcoming events listed at this time.</p>
    {% endif %}
  </section>

  <!-- 2. ALL EVENTS -->
  <section class="events-section">
    <h2 class="events-heading">All Events</h2>

    {% if site.posts.size > 0 %}
      <ul class="all-events-list">
        {% for post in site.posts %}
          <li class="event-list-item">
            <a href="{{ post.url }}" class="event-item-title">{{ post.title }}</a>
            <span class="event-item-date">{{ post.date | date: "%B %d, %Y" }}</span>
          </li>
        {% endfor %}
      </ul>
    {% else %}
      <p class="no-events-text">No events found.</p>
    {% endif %}
  </section>

  <!-- 3. ABOUT PIE SIG CONFERENCES & COLLABORATION INFO -->
  <section class="events-info-box">
    <p>
      The Performance In Education SIG of the Japan Association for Language Teaching (JALT) sponsors several conferences a year, usually in convenient and interesting locations, with workshops, presentations, and performances. Families are always welcome.
    </p>

    <blockquote class="events-quote">
      “We are always trying to grow and spread our message through collaboration with YOU.”
    </blockquote>

    <p>
      What draws many people to the PIE SIG are the amazing and effective activities described by SIG members, the creative talents of the teachers/performers, and most of all, the warm, friendly atmosphere that we work hard to create. We are useful and FUN.
    </p>

    <p class="events-contact-callout">
      Want to collaborate with us? Contact us at <a href="mailto:jaltpiesig@gmail.com">jaltpiesig@gmail.com</a> if you are in the collaborative mood or come and see for yourself what we are about at our annual Performance in Education Research & Practice Conference.
    </p>
  </section>

</div>