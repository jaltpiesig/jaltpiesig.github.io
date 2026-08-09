---
layout: default
title: Home
permalink: /
---

<!-- Custom Styling matching publications.md & officers.md design system -->
<style>
  :root {
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink accent */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark boxes */
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped hero container matching publications.md / officers.md */
  .sloped-box-top {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 35px 25px 40px 25px;
    margin-bottom: 30px;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, var(--pie-heading-dark), var(--pie-purple-pink)) 1;
  }

  .home-card-wrapper {
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.18);
    border-radius: 8px;
    padding: 22px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .home-card-wrapper:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(138, 72, 184, 0.1);
    border-color: var(--pie-heading-dark);
  }

  .heading-serif {
    font-family: "Playfair Display", "Georgia", "Times New Roman", serif;
    color: var(--pie-heading-dark);
    font-size: 1.5rem;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 0.5px;
  }
</style>

<!-- Top Hero Sloped Dark Box (Matching officers.md & publications.md layout) -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Text -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">WELCOME TO PIE SIG</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        Exploring the intersections of performance, drama, music, speech, and art in language education.
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

<!-- Main Content Section -->
<div style="display: grid; grid-template-columns: 1fr; gap: 20px; margin-bottom: 35px;">

  <div class="home-card-wrapper">
    <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">About the Performance in Education SIG</h2>
    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
      The JALT Performance in Education (PIE) Special Interest Group is a community of educators, artists, and researchers dedicated to integrating performance arts—such as drama, music, storytelling, public speaking, and creative movement—into foreign language teaching and learning environments.
    </p>
    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
      Whether you are an experienced practitioner or just beginning to explore performance-based pedagogy, PIE provides a welcoming platform for professional development, collaborative research, and sharing practical classroom ideas.
    </p>
  </div>

  <div class="home-card-wrapper">
    <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">Get Involved</h2>
    <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
      Discover upcoming events, browse our journal and publications, or connect with our leadership team on the <a href="{{ site.baseurl }}/officers/" style="color: var(--pie-heading-dark); text-decoration: underline;">Officers page</a> to see how you can get involved in upcoming conferences and workshops.
    </p>
  </div>

</div>