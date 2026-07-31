---
layout: default
title: Home
---

The Performance in Education (PIE) Special Interest Group (SIG) of the Japan Association for Language Teaching (JALT), founded in 2011 as the Speech, Drama, & Debate SIG, is involved with a myriad of teaching activities (still including drama and debate, but now much more!) that require students to cooperate and collaborate together, so it is natural that our SIG also participates in many collaborative activities with JALT chapters and SIGs[cite: 1].

---

## Podcast

The PIE SIG Podcast features conversations with educators who use performance to make language teaching more engaging, creative, and effective. New episodes are released monthly.

Listen on the PIE SIG website or Spotify, and follow along so you never miss one!

---

## News

<ul class="news-list">
  {% for post in site.posts limit:5 %}
    <li>
      <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
      <span class="post-date">{{ post.date | date: "%Y-%m-%d" }}</span>
      <p>{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
    </li>
  {% endfor %}
</ul>