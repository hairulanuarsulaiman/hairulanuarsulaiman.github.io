---
layout: default
title: Artikel Kewangan Halal & Panduan Pelaburan | Hairul Anuar Sulaiman
permalink: /artikel/
pagination:
  enabled: true
  collection: posts
description: Pendidikan dan panduan kewangan Islam percuma. Terokai artikel berkaitan takaful, pelaburan unit trust, dan perancangan persaraan bebas riba di Malaysia.
category: Artikel
image: "/assets/images/homepage/homepage-architectural-path.jpg"
---

<!-- Page-specific Blog Schema -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Blog",
  "name": "Artikel Kewangan Halal – Hairul Anuar Sulaiman",
  "description": "Pendidikan kewangan Islam percuma untuk individu dan keluarga di Malaysia yang mahu membina asas kewangan dan pelaburan halal.",
  "url": "{{ site.url }}{{ page.url }}",
  "author": {
    "@type": "Person",
    "name": "Hairul Anuar Bin Sulaiman",
    "jobTitle": "Islamic Financial Adviser Representative & Unit Trust Scheme Consultant"
  }
}
</script>

<!-- MASTER EDITORIAL CANVAS (640PX LANE) -->
<main class="luxury-canvas">

  <!-- ========================================== -->
  <!-- STAGE I: HUB PENGETAHUAN HEADER            -->
  <!-- ========================================== -->
  <section class="luxury-section">
    <span class="luxury-eyebrow">
      III. HUB PENGETAHUAN & MONOGRAF
    </span>

    <h1 class="luxury-heading">
      Artikel Kewangan Halal & Panduan Pelaburan
    </h1>

    <p class="luxury-prose luxury-prose-lead">
      Keputusan kewangan yang bijak bermula dengan kefahaman yang betul. Terokai panduan ringkas berkaitan perlindungan Takaful, pelaburan Unit Trust patuh Syariah, dan perancangan persaraan untuk membantu anda membuat pilihan dengan lebih yakin.
    </p>
  </section>

  <hr class="luxury-divider">

  <!-- ========================================== -->
  <!-- STAGE II: LISTING ARTIKEL (PAGINATED LOOP) -->
  <!-- ========================================== -->
  <section class="luxury-section">
    <div class="luxury-border-list">
      {% for post in paginator.posts %}
        <article class="luxury-border-item">
          <span class="luxury-item-badge">
            {{ post.category | default: "KEWANGAN" | upcase }}
          </span>

          <h2 class="luxury-item-title">
            <a href="{{ post.url | relative_url }}" class="luxury-article-link">
              {{ post.title }}
            </a>
          </h2>

          <div class="luxury-article-meta">
            <span>{{ post.date | date: "%d %B %Y" }}</span>
            {% if post.read_time %}
              <span class="luxury-article-meta-divider">•</span>
              <span>{{ post.read_time }} minit bacaan</span>
            {% endif %}
          </div>

          <p class="luxury-item-desc">
            {{ post.description | default: post.excerpt | strip_html | truncate: 160 }}
          </p>

          <div style="margin-top: 16px;">
            <a href="{{ post.url | relative_url }}" class="luxury-btn-secondary">
              Baca Panduan →
            </a>
          </div>
        </article>
      {% endfor %}
    </div>

    <!-- ========================================== -->
    <!-- PAGINATION NAVIGATION CONTROLS             -->
    <!-- ========================================== -->
    {% if paginator.total_pages > 1 %}
      <nav class="luxury-pagination" style="margin-top: 48px; display: flex; justify-content: space-between; align-items: center; border-top: 1px solid rgba(0,0,0,0.08); padding-top: 24px;">
        <div>
          {% if paginator.previous_page %}
            <a href="{{ paginator.previous_page_path | relative_url }}" class="luxury-btn-secondary">
              ← Halaman Sebelumnya
            </a>
          {% endif %}
        </div>

        <span style="font-size: 0.85rem; letter-spacing: 0.05em; text-transform: uppercase; opacity: 0.7;">
          Halaman {{ paginator.page }} daripada {{ paginator.total_pages }}
        </span>

        <div>
          {% if paginator.next_page %}
            <a href="{{ paginator.next_page_path | relative_url }}" class="luxury-btn-secondary">
              Halaman Seterusnya →
            </a>
          {% endif %}
        </div>
      </nav>
    {% endif %}

    <!-- Peringatan Kemaskini -->
    <div class="luxury-author-block" style="margin-top: 64px; text-align: center;">
      Penulisan baharu dikemas kini secara berkala berasaskan data dan prinsip kewangan Syariah terkini.
    </div>
  </section>

  <hr class="luxury-divider">

  <!-- ========================================== -->
  <!-- STAGE III: NEXT STEP (UNIFORM INVITATION)  -->
  <!-- ========================================== -->
  {% include conversation.html %}

</main>
