Welcome to Sprint 2.2 – Social Metadata & Sharing.

This is one of my favourite topics because it’s invisible until someone shares your article—and then it makes a huge difference.

⸻

Learning Goal

By the end of this sprint, you’ll understand:

* Why WhatsApp shows a preview
* How Facebook knows which image to display
* Why LinkedIn sometimes shows the wrong title
* Why Open Graph exists
* Why Twitter Cards are still worth adding
* How to test everything before publishing

This knowledge applies to every website you’ll ever build.

⸻

Imagine This Scenario

You publish your first article:

Saya Baru Bekerja. Apa Yang Perlu Saya Buat Dengan Gaji Pertama?

A reader shares it in a WhatsApp group.

Without Open Graph:

https://hairulanuarsulaiman.github.io/artikel/saya-baru-bekerja-gaji-pertama.html

That’s all people see.

Not very attractive.

⸻

With Open Graph:

+------------------------------------------------+
🖼 Hero Image
Saya Baru Bekerja.
Apa Yang Perlu Saya Buat Dengan Gaji Pertama?
Panduan lengkap mengurus gaji pertama
secara patuh Syariah.
hairulanuarsulaiman.github.io
+------------------------------------------------+

Much more inviting.

⸻

What is Open Graph?

Open Graph is simply a standard.

It was introduced by Facebook.

The idea was:

“Tell us what your page is about before we visit it.”

Today, many platforms understand it.

Including:

✅ Facebook

✅ LinkedIn

✅ WhatsApp

✅ Telegram

✅ Discord

…and several others.

⸻

The Five Essential Open Graph Tags

These are the ones we’ll include in every article.

⸻

1. og:title

<meta property="og:title"
      content="Saya Baru Bekerja. Apa Yang Perlu Saya Buat Dengan Gaji Pertama?">

Purpose

The title shown in the preview.

Usually the same as your <title>.

⸻

2. og:description

<meta property="og:description"
      content="Panduan langkah demi langkah mengurus gaji pertama untuk graduan dan profesional muda Muslim.">

This is the summary displayed below the title.

Think of it as your “elevator pitch.”

⸻

3. og:image

<meta property="og:image"
      content="https://hairulanuarsulaiman.github.io/assets/images/articles/gaji-pertama.webp">

Probably the most important one.

Without it:

No image.

With it:

Your article immediately looks more professional.

⸻

4. og:url

<meta property="og:url"
      content="https://hairulanuarsulaiman.github.io/artikel/saya-baru-bekerja-gaji-pertama.html">

This tells social platforms the canonical URL to associate with the preview.

⸻

5. og:type

For articles:

<meta property="og:type"
      content="article">

For your homepage:

<meta property="og:type"
      content="website">

Why?

Because the homepage is a website.

An article is an article.

Simple—but it helps platforms interpret the page correctly.

⸻

What about og:site_name?

I recommend adding it.

<meta property="og:site_name"
      content="Hairul Knowledge Base">

This consistently identifies your site across shared links.

⸻

Twitter Cards

Even if your audience isn’t active on X, many platforms understand these tags.

We’ll keep them.

Minimum setup

<meta name="twitter:card"
      content="summary_large_image">
<meta name="twitter:title"
      content="...">
<meta name="twitter:description"
      content="...">
<meta name="twitter:image"
      content="...">

Think of them as a backup format for rich previews.

⸻

Why do we repeat information?

You might notice the same title appears in several places:

* <title>
* og:title
* twitter:title

That’s normal.

Each tag serves a different consumer (search engines, social platforms, etc.), so some duplication is expected.

⸻

Image Guidelines

For article images, let’s set some standards from the beginning.

Item	Recommendation
Format	WebP
Size	1200 × 630 px
Aspect Ratio	1.91:1
File Size	Under 250 KB if possible
Alt Text	Descriptive and relevant

This size works well for most social previews.

⸻

How do we test it?

Before sharing an article widely, we can use validation tools.

For example:

* Facebook Sharing Debugger
* LinkedIn Post Inspector

They show you exactly what the preview looks like and can refresh cached metadata after you update a page.

For WhatsApp, the simplest test is often to paste the link into a chat (or a chat with yourself) and wait a few seconds for the preview to generate.

⸻

Sprint 2.2 Summary

Every article will include:

Tag	Purpose
og:title	Preview title
og:description	Preview summary
og:image	Preview image
og:url	Canonical page URL
og:type	Identify as an article
og:site_name	Site branding
twitter:card	Large image preview
twitter:title	Twitter/X title
twitter:description	Twitter/X summary
twitter:image	Twitter/X image

⸻

Homework

Create a new note in your docs/ folder:

social-metadata-notes.md

Inside, explain in your own words:

1. What Open Graph is.
2. Why og:image is important.
3. Why article pages use og:type="article" while the homepage uses website.
4. Why we still include Twitter Card metadata.

Don’t worry about writing a lot—one or two clear sentences for each point is enough.

⸻

One suggestion before Sprint 2.3

I’d also like us to create a small file called:

docs/naming-conventions.md

This will define rules such as:

* Article filenames: lowercase with hyphens (saya-baru-bekerja-gaji-pertama.html)
* Image filenames: match the article slug (gaji-pertama.webp)
* No spaces or uppercase letters in filenames.
* Consistent URL structure under /artikel/.

These seem like small details, but after 50–100 articles they make the project much easier to manage and reduce mistakes. It’s another example of investing a little effort now to save a lot of effort later.
