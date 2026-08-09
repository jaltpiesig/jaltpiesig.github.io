---
layout: default
title: About Us
permalink: /about/
---

<!-- Top Hero Black Box -->
<div class="hero-black-box">
  <div class="about-hero-text">
    <h2>About Us</h2>
    <p class="hero-intro-text">
      The mission of the Performance in Education SIG (formerly the Speech, Drama, and Debate SIG) is to provide a forum for teachers and academics to discuss research, and implement oral interpretation, speech, debate, drama and other forms of performance in language education. The main activities are the publication of a newsletter and the <em>Mask & Gavel</em> journal, as well as sponsoring conferences and workshops, including annual conferences in Okinawa and Sapporo. Other activities have included supporting chapter events and running local, regional, and national speech contests.
    </p>
    <p class="hero-intro-text">
      In the beginning, we created events by ourselves, which established our SIG as a vibrant entity. We started collaborative ventures by providing speakers to chapters upon request (Tokyo, Fukui, Fukuoka, Gifu, Nagoya, Okayama, Hiroshima, etc.). Many of these collaborations grew into co-sponsoring whole conferences, which we have done several times with Yokohama Chapter since 2015, Okinawa Chapter since 2015, and Hokkaido Chapter since 2019. Ever-evolving, these conferences have become annual.
    </p>
    <p class="hero-intro-text">
      We have also collaborated with other SIGs, such as the LLL SIG, the BRAIN SIG, and the Critical Thinking SIG. We do these projects to tap into the regional bases which attract many participants, but we also enjoy the synergy that comes from working with new colleagues with different skill sets.
    </p>
  </div>

  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<!-- Section Sub-Navigation Menu Bar -->
<nav class="pub-nav">
  <a href="#what-we-are">WHAT WE ARE</a>
  <a href="#what-we-do">WHAT WE DO</a>
  <a href="{{ '/officers/' | relative_url }}">PIE SIG OFFICERS</a>
  <a href="#">CONSTITUTION</a>
</nav>

<!-- WHAT WE ARE Section -->
<section id="what-we-are" class="about-card-section">
  <h2 class="section-title">WHAT WE ARE</h2>
  <p class="about-quote">
    "INTRODUCING, for Your Enlightenment and Entertainment... The Performance in Education SIG!" (Drumroll and trumpet fanfare)<br>
    A little too dramatic? Yes, well, that's who we are. Who are we, you ask?
  </p>

  <div class="about-grid">
    {% for item in site.data.about.what_we_are %}
      <div>
        <p><strong>{{ item.title }}</strong><br>
        {{ item.text }}</p>
      </div>
    {% endfor %}
  </div>
</section>

<!-- WHAT WE DO Section -->
<section id="what-we-do" class="about-card-section">
  <h2 class="section-title">WHAT WE DO</h2>
  <p class="about-intro-text">
    Organizationally speaking, we are a relatively young SIG, officially founded in 2012. We are also a small SIG with membership hovering in the low to mid-70s. However, we are also a very active SIG. Our main activities are:
  </p>

  <div class="about-grid">
    {% for item in site.data.about.what_we_do %}
      <div>
        <p><strong>{{ item.title }}</strong><br>
        {{ item.text }}</p>
      </div>
    {% endfor %}
  </div>
</section>