---
layout: default
title: Home
---

<p class="intro-text">
  The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs.
</p>

<h2 class="section-title">Podcast</h2>

<!-- Podcast Player & PIE Pod Logo Side-by-Side -->
<div class="podcast-grid">
  <div class="podcast-player">
    <iframe style="border-radius:12px" src="https://open.spotify.com/embed/show/3vU4S1oGkQ4Y9Z2H2eU7Gg?utm_source=generator" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
  </div>
  <div class="podcast-logo">
    <img src="/assets/images/pie-pod-logo.png" alt="PIE Pod Logo" class="pie-pod-logo-img" onerror="this.style.display='none'">
  </div>
</div>

<p>The PIE SIG Podcast features conversations with educators who use performance to make language teaching more engaging, creative, and effective. New episodes are released monthly.</p>

<p>Listen on the PIE SIG website or Spotify, and follow along so you never miss one!</p>

<h2 class="section-title">News</h2>

<div class="news-section">
  {% for post in site.posts limit:5 %}
    <div class="news-item">
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span class="news-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    </div>
  {% endfor %}
</div>

<!-- Bottom Banner Grid: 3 Logos Side-by-Side + Social Icons below -->
<div class="footer-banner-section">
  <div class="banner-logo-row">
    <img src="/assets/images/beyond-classroom-logo.png" alt="Beyond the Classroom" onerror="this.style.display='none'">
    <img src="/assets/images/pansig-logo.png" alt="PanSIG Chukyo University" onerror="this.style.display='none'">
    <img src="/assets/images/jalt-logo.png" alt="JALT" onerror="this.style.display='none'">
  </div>
  
  <div class="social-icons-row">
    <a href="#" class="social-icon-circle">fb</a>
    <a href="#" class="social-icon-circle">yt</a>
    <a href="#" class="social-icon-circle">x</a>
    <a href="#" class="social-icon-circle">in</a>
  </div>
</div>