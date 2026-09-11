---
layout: default
title: Hub Pengetahuan Kewangan | Hairul Anuar Sulaiman
permalink: /artikel/
pagination:
  enabled: true
  collection: posts
description: Artikel dan panduan untuk membantu individu dan keluarga memahami persoalan kewangan, menilai pilihan dan membuat keputusan kewangan dengan lebih yakin dan teratur.
category: Hub Pengetahuan
image: "/assets/images/homepage/homepage-architectural-path.jpg"
---

<!-- =========================================================
     JSON-LD — Knowledge Hub
     ========================================================= -->

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
  },
  "publisher": {
    "@type": "Person",
    "name": "Hairul Anuar Bin Sulaiman"
  }
}
</script>


<!-- =========================================================
     KNOWLEDGE HUB
     ========================================================= -->

<div class="luxury-canvas">

  <!-- =======================================================
       I. HUB PENGETAHUAN
       ======================================================= -->

  <section class="hero">

    <div class="stage-label">
      I. HUB PENGETAHUAN
    </div>

    <h1>
      Memahami Sebelum Membuat Keputusan
    </h1>

    <p class="hero-lead">
      Artikel dan panduan untuk membantu anda memahami persoalan kewangan,
      menilai pilihan dan menentukan perkara yang patut diberi keutamaan —
      sebelum membuat keputusan.
    </p>

  </section>


  <!-- =======================================================
       II. PILIH MENGIKUT KEADAAN ANDA
       ======================================================= -->

  <section class="section">

    <div class="stage-label">
      II. PILIH MENGIKUT KEADAAN ANDA
    </div>

    <h2>
      Apa yang anda sedang cuba fahami?
    </h2>

    <p class="section-intro">
      Setiap orang datang dengan keadaan yang berbeza. Mulakan dengan
      persoalan yang paling hampir dengan keadaan anda sekarang.
    </p>


    <div class="decision-grid">


      <!-- =================================================
           SPOKE 1 — STARTING
           ================================================= -->

      <article class="decision-card">

        <div class="decision-number">
          01
        </div>

        <h3>
          Saya Baru Nak Mula
        </h3>

        <p>
          Anda baru bekerja, baru berkeluarga, atau baru mula memikirkan
          tentang perlindungan, simpanan dan pelaburan. Fahami asas dahulu
          sebelum menentukan apa yang perlu dibuat.
        </p>

        <div class="decision-question">
          “Apa yang patut saya buat dahulu?”
        </div>

      </article>


      <!-- =================================================
           SPOKE 2 — CHECKING
           ================================================= -->

      <article class="decision-card">

        <div class="decision-number">
          02
        </div>

        <h3>
          Saya Nak Semak
        </h3>

        <p>
          Anda sudah mempunyai Takaful, simpanan, pelaburan atau rancangan
          kewangan. Sekarang anda mahu tahu sama ada apa yang anda ada
          masih sesuai dengan keadaan dan keperluan semasa.
        </p>

        <div class="decision-question">
          “Apa yang saya ada sekarang, cukup ke?”
        </div>

      </article>


      <!-- =================================================
           SPOKE 3 — STRUCTURING
           ================================================= -->

      <article class="decision-card">

        <div class="decision-number">
          03
        </div>

        <h3>
          Saya Perlu Susun
        </h3>

        <p>
          Anda mempunyai beberapa keperluan kewangan pada masa yang sama.
          Anda mahu menentukan keutamaan dan memahami bagaimana semuanya
          boleh disusun dengan lebih teratur.
        </p>

        <div class="decision-question">
          “Macam mana nak susun semua ini?”
        </div>

      </article>

    </div>

  </section>


  <!-- =======================================================
       III. ARTIKEL TERKINI
       ======================================================= -->

  <section class="section" id="artikel-terkini">

    <div class="stage-label">
      III. ARTIKEL TERKINI
    </div>

    <h2>
      Panduan Untuk Membantu Anda Berfikir Dengan Lebih Jelas
    </h2>

    <p class="section-intro">
      Bahan bacaan yang ditulis untuk membantu anda memahami persoalan,
      menilai pilihan dan membuat keputusan kewangan dengan lebih teratur.
    </p>


    <!-- =====================================================
         ARTICLE GRID
         ===================================================== -->

    <div class="article-grid">

      {% for post in paginator.posts %}

        <article class="article-card">

          <!-- Category -->
          {% if post.category %}
            <div class="article-category">
              {{ post.category }}
            </div>
          {% endif %}


          <!-- Title -->
          <h3 class="article-title">

            <a href="{{ post.url | relative_url }}">
              {{ post.title }}
            </a>

          </h3>


          <!-- Meta -->
          <div class="article-meta">

            {% if post.date %}
              <span>
                {{ post.date | date: "%d %B %Y" }}
              </span>
            {% endif %}

            {% if post.read_time %}
              <span aria-hidden="true">·</span>
              <span>
                {{ post.read_time }} min membaca
              </span>
            {% endif %}

          </div>


          <!-- Description -->
          <p class="article-excerpt">

            {% if post.description %}
              {{ post.description }}
            {% else %}
              {{ post.excerpt
                | strip_html
                | strip_newlines
                | truncate: 160
              }}
            {% endif %}

          </p>


          <!-- CTA -->
          <a
            class="article-link"
            href="{{ post.url | relative_url }}"
            aria-label="Baca {{ post.title }}"
          >
            Baca →
          </a>

        </article>

      {% else %}

        <div class="article-empty">

          <p>
            Artikel baharu sedang disediakan.
          </p>

        </div>

      {% endfor %}

    </div>


    <!-- =====================================================
         PAGINATION
         ===================================================== -->

    {% if paginator.total_pages > 1 %}

      <nav
        class="pagination"
        aria-label="Navigasi artikel"
      >

        {% if paginator.previous_page %}

          <a
            href="{{ paginator.previous_page_path | relative_url }}"
            class="pagination-prev"
            aria-label="Artikel sebelumnya"
          >
            ← Sebelumnya
          </a>

        {% endif %}


        <span class="pagination-current">
          {{ paginator.page }} / {{ paginator.total_pages }}
        </span>


        {% if paginator.next_page %}

          <a
            href="{{ paginator.next_page_path | relative_url }}"
            class="pagination-next"
            aria-label="Artikel seterusnya"
          >
            Seterusnya →
          </a>

        {% endif %}

      </nav>

    {% endif %}

  </section>


  <!-- =======================================================
       IV. PENDEKATAN HAIRUL
       ======================================================= -->

  <section class="section approach-reminder">

    <div class="stage-label">
      IV. PENDEKATAN HAIRUL
    </div>

    <h2>
      Memahami keadaan sebelum menentukan apa yang patut dilakukan.
    </h2>

    <p class="section-intro">
      Artikel membantu anda memahami persoalan. Dalam perbualan sebenar,
      pendekatan saya bermula dengan memahami keadaan anda, menilai
      keperluan, menentukan keutamaan dan kemudian melihat pilihan yang
      sesuai.
    </p>

    <p>
      Anda tetap membuat keputusan. Peranan saya adalah membantu anda
      melihat keadaan dengan lebih jelas sebelum keputusan itu dibuat.
    </p>

    <p class="section-action">
      <a href="{{ '/cara-saya-bekerja/' | relative_url }}">
        Lihat Cara Saya Bekerja →
      </a>
    </p>

  </section>


  <!-- =======================================================
       V. PERBUALAN
       ======================================================= -->

  <section class="section conversation-section">

    {% include conversation.html %}

  </section>

</div>
