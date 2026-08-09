---
layout: default
title: Meet the Officers
permalink: /officers/
---

<!-- Custom Styling matching publications.md & index.md design system -->
<style>
  :root {
    --pie-heading-dark: #8a48b8;    /* Darkened lilac/purple for headings */
    --pie-purple-pink: #e28cb9;     /* Purple-pink accent */
    --pie-light-lilac: #e3daf5;     /* Light lilac text inside dark boxes */
  }

  body {
    background-color: var(--bg-lavender, #F4F3F7);
  }

  /* Sloped hero container matching publications.md / index.md */
  .sloped-box-top {
    position: relative;
    background-color: var(--primary-navy, #1C2B36) !important;
    clip-path: polygon(0 0, 100% 12px, 100% 100%, 0 calc(100% - 12px));
    padding: 35px 25px 40px 25px;
    margin-bottom: 30px;
    border-bottom: 4px solid;
    border-image: linear-gradient(to right, var(--pie-heading-dark), var(--pie-purple-pink)) 1;
  }

  .officer-avatar-main {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    object-fit: cover;
    border: 2px solid rgba(138, 72, 184, 0.25);
    flex-shrink: 0;
  }

  .officer-avatar-sub {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    object-fit: cover;
    border: 2px solid rgba(138, 72, 184, 0.25);
    margin: 0 auto 10px auto;
    display: block;
  }

  .officer-card-content {
    flex: 1;
  }

  .officer-card-wrapper {
    display: flex;
    gap: 20px;
    align-items: flex-start;
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.18);
    border-radius: 8px;
    padding: 22px;
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .officer-card-wrapper:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 16px rgba(138, 72, 184, 0.1);
    border-color: var(--pie-heading-dark);
  }

  .officer-subcard {
    background: #ffffff;
    border: 1px solid rgba(138, 72, 184, 0.18);
    border-radius: 8px;
    padding: 15px;
    text-align: center;
    box-shadow: 0 2px 6px rgba(0,0,0,0.02);
    transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
  }

  .officer-subcard:hover {
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

  @media (max-width: 600px) {
    .officer-card-wrapper {
      flex-direction: column;
      align-items: center;
      text-align: center;
    }
  }
</style>

<!-- Top Hero Sloped Dark Box (Matching publications.md) -->
<div class="sloped-box-top">
  <div style="display: flex; justify-content: space-between; align-items: flex-start; flex-wrap: wrap; gap: 20px;">
    <!-- Left Intro Text -->
    <div style="flex: 1 1 300px; max-width: 650px;">
      <h1 style="color: #ffffff; font-size: 2rem; margin-bottom: 12px; font-weight: bold; margin-top: 0;">MEET THE OFFICERS</h1>
      <p style="color: var(--pie-light-lilac); font-size: 1rem; line-height: 1.6; margin: 0;">
        Get to know the dedicated team behind the JALT Performance in Education Special Interest Group.
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

<!-- Detailed Bios Grid (Single Column with Left Circular Profile Picture) -->
<div class="officers-bio-grid" style="display: grid; grid-template-columns: 1fr; gap: 20px; margin-bottom: 35px;">

  <!-- Darren Kinsman -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/kinsman.jpeg" alt="Darren Kinsman" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">DARREN KINSMAN</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">PIE President</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Darren has been teaching in Japan since 1998. Originally from eastern Canada, he earned his bachelor’s degree in political science followed by a bachelor’s degree in education with training in educational drama from renown Canadian playwright and educator Ilkay Silk. After teaching in Japan for some years, he returned to Canada to get his CELTA certification and later a Master of Arts degree.
      </p>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
        Over his career, he has taught at language schools, and a private high school, where he instructed students in both drama and choral singing in addition to traditional subjects. He currently teaches at the university level and is a Member-at-Large for JALT Sendai Chapter. He has written articles on drama, choral English, and the use of portfolios in the writing classroom. He has given numerous talks on the topic of drama in the language classroom at local, national, and international conferences.
      </p>
    </div>
  </div>

  <!-- Kevin Bergman -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/bergman.jpeg" alt="Kevin Bergman" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">KEVIN BERGMAN</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">Vice President & Drama Chair</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Kevin has been involved with English education in Japan since 1986, primarily as a full-time teacher at Musashi High School and Junior High School in Tokyo, where he recently retired after 30 years of teaching English, Speech, and Drama. Before that he team-taught with Japanese English teachers on the JET Program in Shikoku and travelled around the country as an Educational Consultant for a major ELT publishing company.
      </p>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
        Prior to coming to Japan, he studied theater directing at West Virginia University and trained as an actor at The Juilliard School in New York. Kevin loves interacting with people who believe in, and practice drama as means of communication, and would like to help build alliances among such teachers and artists in Japan and other countries.
      </p>
    </div>
  </div>

  <!-- Kim Rockell -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/rockell.jpeg" alt="Kim Rockell" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">KIM ROCKELL</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">Music Chair</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Originally from New Zealand, Kim Rockell is an ethnomusicologist and classical guitarist active throughout the Asia-Pacific region. In Japan he had the opportunity to experience traditional Noh theatre, inspiring him to experiment with original English language Noh-style plays as a member of PIE. He draws on a range of musical strategies when teaching Performance in English and World Music and Culture courses at Komazawa University in Tokyo. Kim also supervises Music Liberal Arts Graduation theses at the Tokyo College of Music.
      </p>
    </div>
  </div>

  <!-- Anthony Brian Gallagher -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/gallagher.jpeg" alt="Anthony Brian Gallagher" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">ANTHONY BRIAN GALLAGHER</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">Assistant Program Chair</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Brian is heavily involved with JALT (PIE & CALL SIGs) as a very active member, contributor, conference organiser, editor, and reviewer. As a youngster, Brian attended elocution and drama lessons from where he also got his first experiences with prose, theatre, and performance arts.
      </p>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
        With a focus on THE USER EXPERIENCE (UX), the last ten years have seen research in improving student writing using virtual learning environments and computer-assisted language learning to benefit students at each of the institutions Brian has worked, and beyond. With a focus on quality assurance and an aim to help others improve their own teaching and course-quality, he continues to present at conferences in the Asia-Pacific region and provide workshops for faculty and independent groups.
      </p>
    </div>
  </div>

  <!-- David Kluge -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/kluge.jpeg" alt="David Kluge" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">DAVID KLUGE</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">PIE Founder, Membership Chair, Oral Interpretation Chair, Debate Chair, Conferences Chair</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        David Kluge (Chukyo University, Adjunct Professor) has been teaching English for 43 years (35 at Japanese universities) and has been involved in Performance in Education (PIE) for 54 years. He is the founder and former president of the JALT Performance in Education SIG. His interests also include Computer-Assisted Language Learning (He was a founding officer of the JALT CALL SIG), cooperative learning, composition, and oral communication, having written textbooks and edited collections on these topics and on PIE.
      </p>
    </div>
  </div>

  <!-- Zach Strickland -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/strickland.jpeg" alt="Zach Strickland" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">ZACH STRICKLAND</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">PIE Drama Chair</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Zach Strickland is a tenured lecturer and English Coordinator at Kyoto Koka Women’s University. He earned a bachelor’s degree in journalism and TV news in his home state of Colorado and later got his master’s in Learning Design and Technology.
      </p>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
        Zach has been in Japan since 2004 and has taught all ages and education levels from infants to seniors. He was a performer and Media Director of The Pirates of the Dotombori, a bilingual, improv comedy group for 10 of those years and performed across Japan and Asia while also teaching all-ages performance workshops. During the COVID pandemic he was lead director of a series of 36 YouTube, educational videos produced by the Osaka City Board of Education that also aired on TV Osaka. He currently lives with his wife and daughters in Osaka.
      </p>
    </div>
  </div>

  <!-- Fatima Mei Ataka -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/ataka.jpeg" alt="Fatima Mei Ataka" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">FATIMA MEI ATAKA</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">AET Liaison</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Fatima Mei Ataka brings twelve years of English teaching experience from her time in Pakistan and Japan to her current role in Saudi Arabia. She has been involved with English drama for high school students for the past seven years, using performance to support language learning. Fatima’s teaching focuses on engaging students through practical and diverse methods to help them develop their English skills effectively. Her interests include Drama and Second Language Acquisition and Drama in Education.
      </p>
    </div>
  </div>

  <!-- Brett Edman -->
  <div class="officer-card-wrapper">
    <img src="{{ site.baseurl }}/assets/images/officers/edman.jpeg" alt="Brett Edman" class="officer-avatar-main">
    <div class="officer-card-content">
      <h2 style="color: var(--pie-heading-dark); font-size: 1.25rem; font-weight: bold; margin-bottom: 2px; margin-top: 0;">BRETT EDMAN</h2>
      <h3 style="color: var(--primary-navy, #1C2B36); font-size: 0.95rem; font-weight: bold; margin-bottom: 12px; margin-top: 0;">AET Liaison</h3>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin: 0;">
        Brett Edman has been teaching since 2019. Originally completing a Bachelor of Engineering (Electrical) and Diploma in Languages (Chinese) at the University of Newcastle (UoN), Australia, he then studied Chinese at the Beijing Film Academy in 2012. This is where he had his first taste of teaching at evening and weekend English conversation classes.
      </p>
      <p style="font-size: 0.9rem; line-height: 1.6; color: #333; margin-top: 10px; margin-bottom: 0;">
        After a few years in the mining and construction industry in Australia he decided to switch to education, completing a Master of Teaching (Secondary) at the UoN in 2018, and a Diploma in Languages (Japanese) between UoN and Nagoya University of Foreign Studies (2019). Brett has taught languages, science, and social science at both private and public schools in Australia. Outside of work hours he can often be seen in musical theatre productions. He currently teaches English at elementary and junior high schools in Kumamoto City as an ALT.
      </p>
    </div>
  </div>

</div>

<!-- Compact Additional Officers Directory Grid -->
<h2 class="heading-serif" style="margin-top: 35px; margin-bottom: 20px;">ADDITIONAL OFFICERS & ROLES</h2>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 15px; margin-bottom: 35px;">

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/diaz.jpeg" alt="Max Diaz" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">MAX DIAZ</strong>
    <span style="font-size: 0.85rem; color: #555;">Web Administrator</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/ford-mihashi.jpeg" alt="Ashley Ford-Mihashi" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">ASHLEY FORD-MIHASHI</strong>
    <span style="font-size: 0.85rem; color: #555;">Assistant Publicity Chair</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/head.jpeg" alt="Philip Head" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">PHILIP HEAD</strong>
    <span style="font-size: 0.85rem; color: #555;">Publication Chair, Publication Editor, & Journal Editor</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/bussinguer-khavari.jpeg" alt="Vivian Bussinguer-Khavari" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">VIVIAN BUSSINGUER-KHAVARI</strong>
    <span style="font-size: 0.85rem; color: #555;">Program Chair</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/saiki.jpeg" alt="Yukari Saiki" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">YUKARI SAIKI</strong>
    <span style="font-size: 0.85rem; color: #555;">Translator / Japanese Language Coordinator</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/rees.jpeg" alt="Gordon Rees" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">GORDON REES</strong>
    <span style="font-size: 0.85rem; color: #555;">Social Events Chair</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/higa.jpeg" alt="James Higa" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">JAMES HIGA</strong>
    <span style="font-size: 0.85rem; color: #555;">Treasurer</span>
  </div>

  <div class="officer-subcard">
    <img src="{{ site.baseurl }}/assets/images/officers/kobayashi.jpeg" alt="Dawn Kobayashi" class="officer-avatar-sub">
    <strong style="color: var(--pie-heading-dark); display: block; font-size: 1rem;">DAWN KOBAYASHI</strong>
    <span style="font-size: 0.85rem; color: #555;">Membership Chair & Member-at-Large</span>
  </div>

</div>