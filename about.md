---
layout: default
title: About Us
permalink: /about/
---

<!-- Custom CSS matching index.md -->
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

  /* Navigation Pills matching index dark style */
  .about-nav-btn {
    background-color: var(--primary-navy, #1C2B36);
    color: #ffffff;
    padding: 10px 18px;
    border-radius: 4px;
    text-decoration: none;
    font-weight: bold;
    font-size: 0.85rem;
    transition: background-color 0.2s ease, color 0.2s ease;
  }

  .about-nav-btn:hover {
    background-color: var(--burgundy-accent, #7A0C2E);
    color: #ffffff;
  }
</style>

<!-- Top Hero Sloped Dark Box -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Paragraphs -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">About Us</h1>
      <p style="color: #ffffff; font-size: 0.98rem; line-height: 1.6; margin-bottom: 12px;">
        The mission of the Performance in Education SIG (formerly the Speech, Drama, and Debate SIG) is to provide a forum for teachers and academics to discuss research, and implement oral interpretation, speech, debate, drama and other forms of performance in language education. The main activities are the publication of a newsletter and the <em>Mask & Gavel</em> journal, as well as sponsoring conferences and workshops, including annual conferences in Okinawa and Sapporo. Other activities have included supporting chapter events and running local, regional, and national speech contests.
      </p>
      <p style="color: var(--pie-light-lilac); font-size: 0.92rem; line-height: 1.6; margin-bottom: 12px;">
        In the beginning, we created events by ourselves, which established our SIG as a vibrant entity. We started collaborative ventures by providing speakers to chapters upon request (Tokyo, Fukui, Fukuoka, Gifu, Nagoya, Okayama, Hiroshima, etc.). Many of these collaborations grew into co-sponsoring whole conferences, which we have done several times with Yokohama Chapter since 2015, Okinawa Chapter since 2015, and Hokkaido Chapter since 2019. Ever-evolving, these conferences have become annual.
      </p>
      <p style="color: var(--pie-light-lilac); font-size: 0.92rem; line-height: 1.6; margin: 0;">
        We have also collaborated with other SIGs, such as the LLL SIG, the BRAIN SIG, and the Critical Thinking SIG. We do these projects to tap into the regional bases which attract many participants, but we also enjoy the synergy that comes from working with new colleagues with different skill sets.
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

<!-- Section Sub-Navigation Menu Bar -->
<div style="display: flex; gap: 12px; margin-bottom: 30px; flex-wrap: wrap;">
  <a href="#what-we-are" class="about-nav-btn">WHAT WE ARE</a>
  <a href="#what-we-do" class="about-nav-btn">WHAT WE DO</a>
  <a href="/officers/" class="about-nav-btn">PIE SIG OFFICERS</a>
  <a href="#" class="about-nav-btn">CONSTITUTION</a>
</div>

<!-- WHAT WE ARE Section (Seamless lilac background matching podcast block) -->
<div id="what-we-are" style="margin-bottom: 35px; padding: 10px 5px;">
  <h2 class="heading-serif" style="margin-bottom: 12px;">WHAT WE ARE</h2>
  <p style="font-style: italic; margin-bottom: 20px; color: #555; font-size: 0.95rem;">
    "INTRODUCING, for Your Enlightenment and Entertainment... The Performance in Education SIG!" (Drumroll and trumpet fanfare)<br>
    A little too dramatic? Yes, well, that's who we are. Who are we, you ask?
  </p>

  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; line-height: 1.6; font-size: 0.92rem; color: var(--text-dark, #222222);">
    <div>
      <p><strong>We are Dramatic.</strong><br>
      One focus of the SIG is drama, and many members have theatre backgrounds or an interest in theatre. Yes, we do put on plays, radio dramas, and readers theatre productions in our schools, but we also incorporate into our classes roleplays, simulations, theatre games, improv activities, and process drama techniques. Never heard of process drama? It can enhance EFL classes in many ways. Ask one of our members to explain it to you personally or at a chapter meeting.</p>
    </div>
    <div>
      <p><strong>We are Creative.</strong><br>
      It is amazing how many creative, artistic people we meet whenever we gather together. If there were a group equivalent to Mensa for creative people, we would be a chapter of that group.</p>
    </div>
    <div>
      <p><strong>We are Flamboyant.</strong><br>
      Not all of us, but a great many of us dress in flamboyant colors (guilty as charged) and talk and gesture dramatically. We can't help it—it is like we are living in the "Bohemian Rhapsody" world. That is also how we teach. Students are not bored in our classes!</p>
    </div>
    <div>
      <p><strong>We are Argumentative.</strong><br>
      Debate is another focus of the SIG and it is interesting how many of the flamboyant, dramatic people are also the debate people. Formal debate teaches important critical thinking and public speaking skills, but it is also exciting and fun, and the way we teach it is fun, yet challenging. Students are not bored in these classes, either.</p>
    </div>
    <div>
      <p><strong>We are Orators.</strong><br>
      We teach speech and presentation, and we are unusually good orators. At SIG forums at PanSIG or the JALT international conference, I am amazed at the consistently excellent quality of speakers in the SIG.</p>
    </div>
    <div>
      <p><strong>We are Serious Professionals.</strong><br>
      In addition to being good teachers, we also write articles, textbooks, and performance pieces, we conduct research, we go to great lengths to mentor the younger members, we volunteer in the JALT organization, and we make it a point to go to conferences to spread the word about the value of performance in the learning process.</p>
    </div>
  </div>
</div>

<!-- WHAT WE DO Section -->
<div id="what-we-do" style="margin-bottom: 35px; padding: 10px 5px;">
  <h2 class="heading-serif" style="margin-bottom: 12px;">WHAT WE DO</h2>
  <p style="margin-bottom: 20px; font-size: 0.95rem; color: var(--text-dark, #222222);">
    Organizationally speaking, we are a relatively young SIG, officially founded in 2012. We are also a small SIG with membership hovering in the low to mid-70s. However, we are also a very active SIG. Our main activities are:
  </p>

  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; line-height: 1.6; font-size: 0.92rem; color: var(--text-dark, #222222);">
    <div>
      <p><strong>Publication Producer</strong><br>
      <em>Mask & Gavel</em> is our official peer-reviewed journal that comes out once a year. And the <em>PIE SIG Classroom Resources Journal</em>, which is a collection of My Share-type articles, comes out whenever we accumulate a sufficient number of articles.</p>
    </div>
    <div>
      <p><strong>News Station</strong><br>
      Current news about events relevant to our SIG or involving SIG members is announced to members and interested people on our social media.</p>
    </div>
    <div>
      <p><strong>Event Producer</strong><br>
      In our first year, we produced our biggest event when we co-sponsored with Oxford University Press to bring Carolyn Graham (of Jazz Chants fame) and Ken Wilson (improv and Smart Choice) to Nagoya. We have co-sponsored with OUP to have Ken Wilson present at our events four times in the last seven years.</p>
    </div>
    <div>
      <p><strong>Presentation Agent</strong><br>
      We have been asked to provide presenters at several JALT chapters and have even produced one-day mini-conferences for chapters. Please contact us if you are interested in presenting at or sponsoring a PIE SIG/chapter mini-conference.</p>
    </div>
    <div>
      <p><strong>Conference Sponsor</strong><br>
      Every year we sponsor our own conference(s). They have been member-friendly—our 2018 Travelling Conference set up the big tent in the Kansai, Tokai, and Kanto areas to bring the conference to members who do not have institutional financial support to travel to conferences. Conferences have been held in Okinawa, Sapporo, and Nagoya.</p>
    </div>
    <div>
      <p><strong>Club & Networking</strong><br>
      Although a small SIG, our networking dinners sometimes feature close to half of our total membership! These events are serious, loud, raucous, humorous, and most of all, a family gathering. Both Apollo and Dionysus are members of our SIG.</p>
    </div>
    <div>
      <p><strong>Podcast</strong><br>
      The PIE SIG Podcast is a monthly show featuring conversations with educators working in performance-based teaching, both within PIE, across other SIGs, and beyond the PIE sphere. Since its launch in July 2025, it has reached a growing audience and provides practical classroom approaches.</p>
    </div>
  </div>
</div>