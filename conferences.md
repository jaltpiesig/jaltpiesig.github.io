---
layout: default
title: Conferences & Events
permalink: /conferences/
---

<!-- Top Hero Title Banner -->
<div class="hero-black-box" style="margin-bottom: 30px;">
  <div>
    <h1 style="color: #ffffff; font-size: 2rem; font-weight: bold;">CONFERENCES & EVENTS</h1>
    <p class="hero-intro-text" style="margin-top: 6px;">
      Discover upcoming research gatherings, practical workshops, and performances sponsored by JALT PIE SIG.
    </p>
  </div>
  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- 1. ABOUT PIE SIG CONFERENCES (MOVED TO TOP) -->
<div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px; margin-bottom: 35px;">
  <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin-bottom: 12px; border-bottom: 2px solid var(--border-subtle); padding-bottom: 6px;">
    ABOUT PIE SIG CONFERENCES
  </h2>
  
  <p style="font-size: 0.92rem; line-height: 1.6; color: #333; margin-bottom: 14px;">
    The Performance In Education SIG of the Japan Association for Language Teaching (JALT) sponsors several conferences a year, usually in convenient and interesting locations, with workshops, presentations, and performances. Families are always welcome.
  </p>

  <blockquote style="font-family: 'Georgia', serif; font-style: italic; font-size: 1.05rem; color: var(--burgundy-accent); border-left: 3px solid var(--burgundy-accent); padding-left: 14px; margin: 18px 0; background: #fdfbfb; padding-top: 8px; padding-bottom: 8px;">
    “We are always trying to grow and spread our message through collaboration with YOU.”
  </blockquote>

  <p style="font-size: 0.92rem; line-height: 1.6; color: #333; margin-bottom: 16px;">
    What draws many people to the PIE SIG are the amazing and effective activities described by SIG members, the creative talents of the teachers/performers, and most of all, the warm, friendly atmosphere that we work hard to create. We are useful and <strong>FUN</strong>.
  </p>

  <div style="background: #f9f9fb; border: 1px solid var(--border-subtle); border-radius: 6px; padding: 16px; margin-top: 18px;">
    <strong style="color: var(--burgundy-accent); font-size: 0.95rem; display: block; margin-bottom: 4px;">Want to collaborate with us?</strong>
    <p style="font-size: 0.9rem; line-height: 1.5; color: #333; margin: 0;">
      Contact us at <a href="mailto:jaltpiesig@gmail.com" style="color: var(--burgundy-accent); font-weight: bold; text-decoration: underline;">jaltpiesig@gmail.com</a> if you are in the collaborative mood or come and see for yourself what we are about at our annual Performance in Education Research & Practice Conference.
    </p>
  </div>
</div>

<!-- 2. LATEST EVENT -->
<div style="margin-bottom: 35px;">
  <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin-bottom: 16px; border-bottom: 2px solid var(--border-subtle); padding-bottom: 6px;">
    LATEST EVENT
  </h2>

  {% assign latest_post = site.posts.first %}
  {% if latest_post %}
    <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 25px;">
      <div style="display: flex; justify-content: space-between; align-items: baseline; flex-wrap: wrap; border-bottom: 1px solid var(--border-subtle); padding-bottom: 12px; margin-bottom: 18px;">
        <h3 style="font-size: 1.35rem; margin: 0;">
          <a href="{{ latest_post.url }}" style="color: var(--burgundy-accent); text-decoration: none; font-weight: bold;">{{ latest_post.title }}</a>
        </h3>
        <span style="font-size: 0.85rem; color: #666; font-weight: bold; margin-top: 4px;">{{ latest_post.date | date: "%B %d, %Y" }}</span>
      </div>
      
      <div style="font-size: 0.92rem; line-height: 1.6; color: #333;">
        {{ latest_post.content }}
      </div>
    </div>
  {% else %}
    <p style="font-style: italic; color: #666;">No upcoming events listed at this time.</p>
  {% endif %}
</div>

<!-- 3. ALL EVENTS -->
<div style="margin-bottom: 35px;">
  <h2 style="color: var(--burgundy-accent); font-size: 1.3rem; font-weight: bold; margin-bottom: 16px; border-bottom: 2px solid var(--border-subtle); padding-bottom: 6px;">
    ALL EVENTS
  </h2>

  {% if site.posts.size > 0 %}
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 15px;">
      {% for post in site.posts %}
        <div style="background: #ffffff; border: 1px solid var(--border-subtle); border-radius: 8px; padding: 18px; display: flex; flex-direction: column; justify-content: space-between;">
          <div>
            <span style="font-size: 0.8rem; color: #777; font-weight: bold; display: block; margin-bottom: 6px;">{{ post.date | date: "%B %d, %Y" }}</span>
            <h3 style="font-size: 1.05rem; margin: 0 0 12px 0;">
              <a href="{{ post.url }}" style="color: var(--burgundy-accent); text-decoration: none; font-weight: bold;">{{ post.title }}</a>
            </h3>
          </div>
          <a href="{{ post.url }}" style="font-size: 0.85rem; color: var(--burgundy-accent); font-weight: bold; text-decoration: none;">View Event Details &rarr;</a>
        </div>
      {% endfor %}
    </div>
  {% else %}
    <p style="font-style: italic; color: #666;">No events found.</p>
  {% endif %}
</div>