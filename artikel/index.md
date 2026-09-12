---
layout: default
title: Hub Pengetahuan Kewangan & Legasi | Hairul Anuar Sulaiman
permalink: /artikel/
description: Perpustakaan pendidikan kewangan Islam percuma. Terokai panduan berkaitan perlindungan kewangan, pelaburan patuh syariah, persaraan, dan perancangan harta.
image: "/assets/images/homepage/homepage-architectural-path.jpg"
---

<main class="luxury-canvas">

  <section class="luxury-section">
    <span class="luxury-eyebrow">HUB PENGETAHUAN</span>
    <h1 class="luxury-heading">Koleksi Panduan Kewangan & Legasi</h1>
    <p class="luxury-prose luxury-prose-lead">
      Keputusan kewangan yang bijak bermula dengan kefahaman yang betul. Terokai panduan strategik kami mengikut empat tonggak utama kewangan Islam.
    </p>
  </section>

  <hr class="luxury-divider">

  <!-- PILAR 1: PERLINDUNGAN KEWANGAN -->
  {% assign perlindungan_posts = site.posts | where: "category", "Perlindungan Kewangan" %}
  {% if perlindungan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PILAR 1</span>
    <h2 class="luxury-heading" style="font-size: 1.75rem; margin-bottom: 24px;">Perlindungan Kewangan</h2>
    <div class="luxury-article-grid">
      {% for post in perlindungan_posts | limit: 3 %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.25rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>
    {% if perlindungan_posts.size > 3 %}
    <div style="margin-top: 24px;">
      <a href="/artikel/perlindungan-kewangan/" class="luxury-btn-secondary">Lihat Semua Artikel Perlindungan →</a>
    </div>
    {% endif %}
  </section>
  {% endif %}

  <!-- PILAR 2: PELABURAN PATUH SYARIAH -->
  {% assign pelaburan_posts = site.posts | where: "category", "Pelaburan Patuh Syariah" %}
  {% if pelaburan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PILAR 2</span>
    <h2 class="luxury-heading" style="font-size: 1.75rem; margin-bottom: 24px;">Pelaburan Patuh Syariah</h2>
    <div class="luxury-article-grid">
      {% for post in pelaburan_posts | limit: 3 %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.25rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>
    {% if pelaburan_posts.size > 3 %}
    <div style="margin-top: 24px;">
      <a href="/artikel/pelaburan-patuh-syariah/" class="luxury-btn-secondary">Lihat Semua Artikel Pelaburan →</a>
    </div>
    {% endif %}
  </section>
  {% endif %}

  <!-- PILAR 3: PERANCANGAN PERSARAAN -->
  {% assign persaraan_posts = site.posts | where: "category", "Perancangan Persaraan" %}
  {% if persaraan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PILAR 3</span>
    <h2 class="luxury-heading" style="font-size: 1.75rem; margin-bottom: 24px;">Perancangan Persaraan</h2>
    <div class="luxury-article-grid">
      {% for post in persaraan_posts | limit: 3 %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.25rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>
    {% if persaraan_posts.size > 3 %}
    <div style="margin-top: 24px;">
      <a href="/artikel/perancangan-persaraan/" class="luxury-btn-secondary">Lihat Semua Artikel Persaraan →</a>
    </div>
    {% endif %}
  </section>
  {% endif %}

  <!-- PILAR 4: PERANCANGAN HARTA -->
  {% assign harta_posts = site.posts | where: "category", "Perancangan Harta" %}
  {% if harta_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PILAR 4</span>
    <h2 class="luxury-heading" style="font-size: 1.75rem; margin-bottom: 24px;">Perancangan Harta</h2>
    <div class="luxury-article-grid">
      {% for post in harta_posts | limit: 3 %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.25rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>
    {% if harta_posts.size > 3 %}
    <div style="margin-top: 24px;">
      <a href="/artikel/perancangan-harta/" class="luxury-btn-secondary">Lihat Semua Artikel Perancangan Harta →</a>
    </div>
    {% endif %}
  </section>
  {% endif %}

  <hr class="luxury-divider">

  {% include conversation.html %}

</main>
