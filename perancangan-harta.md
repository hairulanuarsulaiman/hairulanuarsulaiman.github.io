---
layout: default
title: Perancangan Harta & Legasi Syariah | Hairul Anuar Sulaiman
description: Membantu individu dan keluarga merancang pembahagian harta, wasiat, dan hibah supaya legasi anda terpelihara dan keluarga anda dilindungi.
category: Perancangan Harta
image: "/assets/images/estate/estate-architectural-archive.webp"
permalink: /perancangan-harta/
---

<main class="luxury-canvas">

  <!-- HERO -->
  <section class="luxury-section">
    <span class="luxury-eyebrow">PERANCANGAN HARTA & LEGASI</span>

    <h1 class="luxury-heading">
      Harta Yang Anda Bina Hari Ini Adalah Legasi Untuk Generasi Akan Datang.
    </h1>

    <p class="luxury-prose luxury-prose-lead">
      Perancangan harta bukan tentang ketakutan akan kematian. Ia tentang tanggungjawab dan kasih sayang terhadap keluarga yang anda tinggalkan. Saya membantu anda merancang pembahagian harta dengan jelas, adil, dan selaras dengan prinsip Syariah.
    </p>

    <div>
      <a href="{{ '/hubungi/' | relative_url }}" class="luxury-btn-primary">
        Mulakan Perbualan →
      </a>
    </div>
  </section>

  <!-- IMAGE -->
  <figure class="luxury-figure">
    <picture>
      <source srcset="{{ '/assets/images/estate/estate-architectural-archive.webp' | relative_url }}" type="image/webp">
      <img 
        src="{{ '/assets/images/estate/estate-architectural-archive.jpg' | relative_url }}" 
        alt="Langit malam yang penuh bintang dengan jalur Bima Sakti melengkung di atas sawah padi yang tenang di Malaysia, mencerminkan cahaya bintang di permukaan air." 
        width="1200"
        height="800"
        loading="eager"
        fetchpriority="high"
      >
    </picture>
    <figcaption class="luxury-figcaption">
      Sesuatu yang kekal melangkaui satu generasi — legasi yang terpelihara bermula dengan perancangan yang teliti.
    </figcaption>
  </figure>

  <hr class="luxury-divider">

  <!-- CONTEXT -->
  <section class="luxury-section">
    <span class="luxury-eyebrow">REALITI PUSAKA</span>

    <h2 class="luxury-subheading">
      Mengapa Perancangan Harta Penting?
    </h2>

    <p class="luxury-prose">
      Ramai orang bekerja keras sepanjang hayat untuk membina rumah, perniagaan, dan simpanan. Namun, persoalan tentang apa yang akan berlaku kepada harta tersebut selepas kita tiada sering dilupakan atau dianggap terlalu awal untuk difikirkan.
    </p>

    <p class="luxury-prose">
      Tanpa perancangan yang jelas, harta pusaka boleh terbeku, mencetuskan konflik keluarga, dan menyebabkan proses pentadbiran yang panjang. Perancangan harta yang teliti memastikan legasi anda terpelihara dan keluarga anda dilindungi.
    </p>
  </section>

  <hr class="luxury-divider">

  <!-- PHILOSOPHY -->
  <section class="luxury-section">
    <span class="luxury-eyebrow">FALSAFAH PERANCANGAN</span>

    <h2 class="luxury-subheading">
      Memahami Instrumen Perancangan Harta Islam
    </h2>

    <p class="luxury-prose">
      Perancangan harta Islam merangkumi beberapa instrumen yang saling melengkapi: <em>Wasiat</em>, <em>Hibah</em>, dan <em>Amanah</em>. Setiap satu mempunyai peranan yang berbeza dalam memastikan harta anda diagihkan dengan jelas dan teratur.
    </p>

    <p class="luxury-prose">
      Sebagai perancang, saya membantu anda memahami perbezaan antara instrumen ini dan bagaimana ia boleh digunakan bersama untuk mencapai matlamat perancangan harta anda.
    </p>

    <div class="luxury-author-block">
      Saya juga dilantik sebagai <strong>Perancang Harta Pusaka Islam (IEP)</strong> di bawah <strong>as-Salihin Trustee Berhad</strong>, yang menyediakan perkhidmatan perancangan harta dan wasiat patuh Syariah. Perkhidmatan ini adalah di bawah as-Salihin dan tidak berkaitan dengan peranan saya sebagai IFAR atau Unit Trust Scheme Consultant.
    </div>
  </section>

  <hr class="luxury-divider">

  <!-- SOLUTION -->
  <section class="luxury-section">
    <span class="luxury-eyebrow">PILAR PERANCANGAN HARTA</span>

    <h2 class="luxury-subheading">
      Tiga Asas Perancangan Harta
    </h2>

    <p class="luxury-prose">
      Tiga komponen utama ini saling melengkapi bagi memastikan legasi anda terpelihara dan keluarga anda dilindungi:
    </p>

    <div class="luxury-border-list">
      <div class="luxury-border-item">
        <span class="luxury-item-badge">01. WASIAT</span>
        <h3 class="luxury-item-title">Arahan Bertulis</h3>
        <p class="luxury-item-desc">
          Menentukan bagaimana harta anda diagihkan mengikut kehendak anda, dalam had yang dibenarkan oleh Syariah.
        </p>
      </div>

      <div class="luxury-border-item">
        <span class="luxury-item-badge">02. HIBAH</span>
        <h3 class="luxury-item-title">Pemindahan Semasa Hidup</h3>
        <p class="luxury-item-desc">
          Memindahkan harta tertentu kepada penerima yang dipilih semasa anda masih hidup, mengurangkan harta pusaka dan mempercepatkan proses.
        </p>
      </div>

      <div class="luxury-border-item">
        <span class="luxury-item-badge">03. AMANAH</span>
        <h3 class="luxury-item-title">Pengurusan Berterusan</h3>
        <p class="luxury-item-desc">
          Menyediakan struktur yang membolehkan harta diuruskan secara berterusan untuk manfaat generasi akan datang.
        </p>
      </div>
    </div>
  </section>

  <hr class="luxury-divider">

  <!-- RELATED ARTICLES -->
  {% assign harta_posts = site.posts | where: "category", "Perancangan Harta" %}
  {% if harta_posts.size > 0 %}
  <section class="luxury-section">
    <span class="luxury-eyebrow">BACAAN PENGETAHUAN PERANCANGAN HARTA</span>

    <h2 class="luxury-subheading">
      Artikel Pilihan Perancangan Harta
    </h2>

    <div class="luxury-article-grid">
      {% for post in harta_posts limit: 3 %}
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

  <!-- CTA -->
  {% include conversation.html %}

</main>
