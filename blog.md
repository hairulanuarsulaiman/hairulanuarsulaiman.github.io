---
layout: default
title: Hub Pengetahuan Kewangan | Hairul Anuar Sulaiman
permalink: /artikel/
description: Artikel dan panduan untuk membantu individu dan keluarga memahami persoalan kewangan, menilai pilihan dan membuat keputusan kewangan dengan lebih yakin dan teratur.
category: Hub Pengetahuan
image: "/assets/images/homepage/homepage-architectural-path.jpg"
---

<!-- JSON-LD — Knowledge Hub -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Blog",
  "name": "Hub Pengetahuan Kewangan – Hairul Anuar Sulaiman",
  "description": "Artikel dan panduan untuk membantu individu dan keluarga memahami persoalan kewangan, menilai pilihan dan membuat keputusan kewangan dengan lebih yakin dan teratur.",
  "url": "{{ site.url }}{{ page.url }}",
  "author": {
    "@type": "Person",
    "name": "Hairul Anuar Bin Sulaiman",
    "jobTitle": "Associate Shariah Registered Financial Planner"
  }
}
</script>

<main class="luxury-canvas">

  <!-- =======================================================
       HUB PENGETAHUAN
       ======================================================= -->

  <section class="luxury-section">
    <span class="luxury-eyebrow">HUB PENGETAHUAN</span>

    <h1 class="luxury-heading">
      Memahami Sebelum Membuat Keputusan
    </h1>

    <p class="luxury-prose luxury-prose-lead">
      Artikel dan panduan untuk membantu anda memahami persoalan kewangan, menilai pilihan dan menentukan perkara yang patut diberi keutamaan — sebelum membuat keputusan.
    </p>
  </section>

  <hr class="luxury-divider">

  <!-- =======================================================
       MULA DI SINI — FEATURED ARTICLE
       ======================================================= -->

  {% assign featured_post = site.posts | where: "featured", true | first %}
  {% if featured_post %}
  <section class="luxury-section">
    <span class="luxury-eyebrow">MULA DI SINI</span>

    <h2 class="luxury-subheading">
      Bacaan Asas Untuk Kefahaman Anda
    </h2>

    <figure class="luxury-figure">
      <img
        src="{{ featured_post.image | relative_url }}"
        alt="{{ featured_post.image_alt | default: featured_post.title }}"
        width="1200"
        height="800"
        loading="eager"
      >
      {% if featured_post.image_caption %}
        <figcaption class="luxury-figcaption">
          {{ featured_post.image_caption }}
        </figcaption>
      {% endif %}
    </figure>

    <h3 class="luxury-item-title" style="font-size: 1.5rem; margin-top: 32px;">
      <a href="{{ featured_post.url | relative_url }}" class="luxury-article-link">
        {{ featured_post.title }}
      </a>
    </h3>

    <p class="luxury-prose">
      {{ featured_post.description | default: featured_post.excerpt | strip_html | truncate: 200 }}
    </p>

    <div>
      <a href="{{ featured_post.url | relative_url }}" class="luxury-btn-secondary">
        Baca Panduan →
      </a>
    </div>
  </section>

  <hr class="luxury-divider">
  {% endif %}

  <!-- =======================================================
       PERLINDUNGAN KEWANGAN
       ======================================================= -->

  {% assign perlindungan_posts = site.posts | where: "category", "Perlindungan Kewangan" %}
  {% if perlindungan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PERLINDUNGAN KEWANGAN</span>
    <h2 class="luxury-subheading" style="font-size: 1.5rem;">Melindungi Apa Yang Anda Bina</h2>

    <div class="luxury-article-grid">
      {% for post in perlindungan_posts %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.15rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>

    <div style="margin-top: 24px;">
      <a href="{{ '/artikel/perlindungan-kewangan/' | relative_url }}" class="luxury-btn-secondary">Lihat Semua Artikel Perlindungan →</a>
    </div>
  </section>
  {% endif %}

  <!-- =======================================================
       PELABURAN PATUH SYARIAH
       ======================================================= -->

  {% assign pelaburan_posts = site.posts | where: "category", "Pelaburan Patuh Syariah" %}
  {% if pelaburan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PELABURAN PATUH SYARIAH</span>
    <h2 class="luxury-subheading" style="font-size: 1.5rem;">Membina Kekayaan Dengan Disiplin</h2>

    <div class="luxury-article-grid">
      {% for post in pelaburan_posts %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.15rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>

    <div style="margin-top: 24px;">
      <a href="{{ '/artikel/pelaburan-patuh-syariah/' | relative_url }}" class="luxury-btn-secondary">Lihat Semua Artikel Pelaburan →</a>
    </div>
  </section>
  {% endif %}

  <!-- =======================================================
       PERANCANGAN PERSARAAN
       ======================================================= -->

  {% assign persaraan_posts = site.posts | where: "category", "Perancangan Persaraan" %}
  {% if persaraan_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PERANCANGAN PERSARAAN</span>
    <h2 class="luxury-subheading" style="font-size: 1.5rem;">Menyediakan Hari Tua Yang Tenang</h2>

    <div class="luxury-article-grid">
      {% for post in persaraan_posts %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.15rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>

    <div style="margin-top: 24px;">
      <a href="{{ '/artikel/perancangan-persaraan/' | relative_url }}" class="luxury-btn-secondary">Lihat Semua Artikel Persaraan →</a>
    </div>
  </section>
  {% endif %}

  <!-- =======================================================
       PERANCANGAN HARTA
       ======================================================= -->

  {% assign harta_posts = site.posts | where: "category", "Perancangan Harta" %}
  {% if harta_posts.size > 0 %}
  <section class="luxury-section" style="margin-bottom: 64px;">
    <span class="luxury-eyebrow">PERANCANGAN HARTA</span>
    <h2 class="luxury-subheading" style="font-size: 1.5rem;">Merancang Legasi Anda</h2>

    <div class="luxury-article-grid">
      {% for post in harta_posts %}
        <article class="luxury-article-card">
          <h3 class="luxury-item-title" style="font-size: 1.15rem;">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">{{ post.title }}</a>
          </h3>
          <p class="luxury-item-desc">{{ post.description | default: post.excerpt | strip_html | truncate: 120 }}</p>
        </article>
      {% endfor %}
    </div>

    <div style="margin-top: 24px;">
      <a href="{{ '/artikel/perancangan-harta/' | relative_url }}" class="luxury-btn-secondary">Lihat Semua Artikel Perancangan Harta →</a>
    </div>
  </section>
  {% endif %}

  <hr class="luxury-divider">

  <!-- =======================================================
       PENDEKATAN SAYA
       ======================================================= -->

  <section class="luxury-section">
    <span class="luxury-eyebrow">PENDEKATAN SAYA</span>

    <h2 class="luxury-subheading">
      Memahami keadaan sebelum menentukan apa yang patut dilakukan.
    </h2>

    <p class="luxury-prose">
      Artikel membantu anda memahami persoalan. Dalam perbualan sebenar, pendekatan saya bermula dengan memahami keadaan anda, menilai keperluan, menentukan keutamaan dan kemudian melihat pilihan yang sesuai.
    </p>

    <p class="luxury-prose">
      Anda tetap membuat keputusan. Peranan saya adalah membantu anda melihat keadaan dengan lebih jelas sebelum keputusan itu dibuat.
    </p>
  </section>

  <hr class="luxury-divider">

  <!-- =======================================================
       PERBUALAN
       ======================================================= -->

  {% include conversation.html %}

</main>
