---
layout: default
title: Resources
permalink: /resources/
---

<!-- Custom CSS matching site aesthetic -->
<style>
  :root {
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink accent */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark hero */
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped hero banner */
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
    font-size: 1.6rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }

  /* Responsive Video Container (16:9 Aspect Ratio) */
  .video-container {
    position: relative;
    padding-bottom: 56.25%; /* 16:9 aspect ratio */
    height: 0;
    overflow: hidden;
    border-radius: 8px;
    background-color: #000000;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
  }

  .video-container iframe {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    border: 0;
  }

  .resource-link-placeholder {
    color: var(--pie-heading-dark);
    font-weight: bold;
    text-decoration: underline;
  }
</style>

<!-- Top Hero Banner -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Title -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">RESOURCES</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        Here you can find various educational/instructional resources created by PIE SIG members.
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

<!-- Main Content Area -->
<div style="padding: 0 5px; margin-bottom: 40px;">
  
  <!-- Presentation Design Section -->
  <section style="margin-bottom: 40px; border-bottom: 1px solid rgba(138, 72, 184, 0.2); padding-bottom: 25px;">
    <h2 class="heading-serif" style="margin-bottom: 12px;">PRESENTATION DESIGN 101</h2>
    <p style="font-size: 1rem; color: var(--text-dark, #222222); margin: 0;">
      By Marc Helgesen — <a href="#" onclick="return false;" class="resource-link-placeholder">Presentation Design 101 Link (Coming Soon)</a>
    </p>
  </section>

  <!-- Video Library Section -->
  <section>
    <h2 class="heading-serif" style="margin-bottom: 20px;">INSTRUCTIONAL VIDEOS</h2>

    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 25px;">
      
      <!-- Video 1 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/djaVfFDS28g" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 2 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/QpULv6Fxvm0" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 3 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/r0YFjjaEP5Q" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 4 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/sWl5-zibZG4" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 5 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VGHId_rs2Uc" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 6 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/0FGHjqOSRcA" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 7 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/Vm-WO9JluzQ" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

      <!-- Video 8 -->
      <div class="video-container">
        <iframe src="https://www.youtube.com/embed/aNa-3XSvFEM" title="YouTube video player" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
      </div>

    </div>
  </section>

</div>