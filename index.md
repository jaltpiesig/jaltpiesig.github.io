---
layout: default
title: Home
---

<!-- 1. Black Box: Intro Text (White) on Left + PIE SIG Graphic on Right -->
<div class="hero-black-box">
  <p class="hero-intro-text">
    The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs.
  </p>

  <div class="hero-brand-graphic">
    <h1>PIE <span>sig</span></h1>
    <p>PERFORMANCE IN EDUCATION</p>
  </div>
</div>

<h2 class="section-title">Podcast</h2>

<!-- Podcast Grid: Player Card Left + Intro Text & PIE pod Logo Right -->
<div class="podcast-grid">
  <div class="podcast-player-card">
    <p><strong>PIE SIG Podcast Episode 12</strong></p>
    <p style="font-size:0.85rem; color:#555; margin-bottom:10px;">Why Settle for Student Participation When You Can Have Student Engagement?</p>
    <a href="https://open.spotify.com" target="_blank" style="display:inline-block; background:#1db954; color:#fff; padding:6px 14px; border-radius:15px; text-decoration:none; font-size:0.8rem; font-weight:bold;">Listen on Spotify</a>
  </div>

  <div class="podcast-info-side">
    <p>The PIE SIG Podcast features conversations with educators who use performance to make language teaching more engaging, creative, and effective. New episodes are released monthly.</p>
    <p>Listen on the PIE SIG website or Spotify, and follow along so you never miss one!</p>
    
    <div class="pie-pod-text-logo">
      PIE
      <span>pod</span>
      <sub>PODCAST IN EDUCATION</sub>
    </div>
  </div>
</div>

<!-- 2. Black Box: News Section with Lilac Posts on Left + Social Links on Right -->
<div class="news-black-box">
  <div class="news-box-header">
    <h2>NEWS</h2>
  </div>

  <div class="news-box-grid">
    <div class="news-posts-column">
      {% for post in site.posts limit:5 %}
        <div class="news-post-item">
          <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
          <span class="news-post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
          <p class="news-post-excerpt">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
        </div>
      {% endfor %}
    </div>

    <!-- Vertical Social Icons on Right Side inside News Box -->
    <div class="news-social-column">
      <a href="#" class="social-circle-btn" title="Facebook">f</a>
      <a href="#" class="social-circle-btn" title="YouTube">yt</a>
      <a href="#" class="social-circle-btn" title="X / Twitter">x</a>
      <a href="#" class="social-circle-btn" title="LinkedIn">in</a>
    </div>
  </div>
</div>

<!-- 3. Partner Banners Row -->
<div class="partner-logos-row">
  <div class="partner-card">
    <img src="/assets/images/beyond-classroom-logo.png" alt="Beyond the Classroom" onerror="this.parentNode.innerHTML='BEYOND THE CLASSROOM';">
  </div>
  <div class="partner-card">
    <img src="/assets/images/pansig-logo.png" alt="PanSIG Chukyo University" onerror="this.parentNode.innerHTML='PanSIG CHUKYO UNIVERSITY';">
  </div>
  <div class="partner-card">
    <img src="/assets/images/jalt-logo.png" alt="JALT" onerror="this.parentNode.innerHTML='JALT';">
  </div>
</div>

<!-- 4. Black Footer Bar: Socials Bottom-Left + PIE SIG & JALT Logos Bottom-Right -->
<footer class="site-black-footer">
  <div class="footer-social-links">
    <a href="#" class="social-circle-btn" title="Facebook">f</a>
    <a href="#" class="social-circle-btn" title="YouTube">yt</a>
    <a href="#" class="social-circle-btn" title="X / Twitter">x</a>
    <a href="#" class="social-circle-btn" title="LinkedIn">in</a>
  </div>

  <div class="footer-brand-logos">
    <span>PIE sig</span> | <span>JALT</span>
  </div>
</footer>