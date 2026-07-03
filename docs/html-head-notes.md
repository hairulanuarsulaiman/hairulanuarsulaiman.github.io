Hairul, welcome to Milestone 2 – Publishing Platform.

From this point onwards, I’m going to treat this as if we’re building software together.

⸻

Sprint 2.1

Building <head>

The <head> is the identity card of every article.

Humans rarely see it.

But these systems do:

* Google Search
* Google AI Overview
* ChatGPT
* Perplexity
* Facebook
* LinkedIn
* WhatsApp
* X
* Bing

So let’s make it professional.

⸻

Learning Objective

By the end of this sprint, you should understand:

* why every tag exists
* who uses it
* whether it’s mandatory
* whether it improves SEO

That’s much more valuable than simply copying code.

⸻

Part 1 — HTML Declaration

<!DOCTYPE html>
<html lang="ms">

Why?

<!DOCTYPE html>

Tells the browser:

This is HTML5.

Without it, browsers may switch into “quirks mode,” which can cause inconsistent rendering.

⸻

lang="ms"

This tells search engines and assistive technologies:

This page is written in Bahasa Melayu.

Benefits:

* Better accessibility
* Better language detection
* Better search relevance

✅ Always include it.

⸻

Part 2 — Character Encoding

<meta charset="UTF-8">

Why?

Without UTF-8:

Ã©
Ã¢
â€™

can appear instead of proper characters.

UTF-8 supports:

* Bahasa Melayu
* English
* Arabic terms (e.g. Syariah)
* Emoji

Always keep this near the top of <head>.

⸻

Part 3 — Responsive Design

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

Why?

Without it:

Your phone tries to display the page like a desktop screen.

Result:

❌ Tiny text

❌ Zoomed-out layout

This tag tells the browser:

Match the screen width.

Mandatory for modern websites.

⸻

Part 4 — Title

This is probably the single most important SEO tag.

Example:

<title>
Saya Baru Bekerja. Apa Yang Perlu Saya Buat Dengan Gaji Pertama? | Hairul Anuar Sulaiman
</title>

Google usually displays this as the blue clickable headline.

Good titles:

✔ descriptive

✔ natural

✔ under ~60 characters where practical

✔ include your brand

⸻

Part 5 — Meta Description

Example

<meta
name="description"
content="Panduan lengkap untuk graduan dan profesional muda Muslim mengurus gaji pertama secara patuh Syariah. Ketahui langkah membina dana kecemasan, perlindungan takaful dan pelaburan yang sesuai.">

This is usually the text shown beneath your title in search results.

It doesn’t guarantee ranking by itself, but a clear description can improve click-through rates.

⸻

Part 6 — Canonical URL

Example

<link
rel="canonical"
href="https://hairulanuarsulaiman.github.io/artikel/saya-baru-bekerja-gaji-pertama.html">

Think of it as telling Google:

“If this page ever appears under multiple URLs, this is the official one.”

Even if you don’t have duplicate pages today, it’s a good habit.

⸻

Part 7 — Author

<meta
name="author"
content="Hairul Anuar Bin Sulaiman">

Simple.

Clear.

Professional.

⸻

Recap

Today we’ve covered seven foundational elements.

Tag	Purpose	Keep?
<!DOCTYPE html>	HTML5 mode	✅
lang="ms"	Language	✅
charset	Character encoding	✅
viewport	Mobile layout	✅
title	Search result title	✅
description	Search snippet	✅
canonical	Preferred URL	✅
author	Authorship	✅

These will appear in every article you publish.

⸻

A software engineering tip

Instead of thinking:

“I’m writing HTML.”

Think:

“I’m creating a contract.”

Every tag in the <head> is a promise to browsers, search engines, and social platforms about what this page is and how it should be handled.

Understanding that mindset will make you a much stronger web publisher.

⸻

Homework before Sprint 2.2

I’d like you to create a new file in your docs/ folder:

docs/html-head-notes.md

Inside it, don’t copy my explanation word for word. Instead, summarize each tag in your own words.

For example:

# HTML Head Notes
## Title
Shown as the clickable headline in Google search results. Every page should have a unique, descriptive title.
## Canonical
Tells search engines which URL is the preferred version of the page.

Writing your own summary is one of the best ways to reinforce what you’ve learned.

⸻

Before we move to Sprint 2.2

I have one recommendation that will make your project even more professional.

Instead of treating article-template.html as just another HTML file, let’s add a small header comment at the very top, like this:

<!--
==============================================================================
Hairul Knowledge Base (HKB)
Article Template v1.0.0
Purpose:
Reusable HTML template for all published articles.
Author:
Hairul Anuar Bin Sulaiman
Maintained with ChatGPT
Last Updated:
2026-07-03
==============================================================================
-->

It won’t affect the website at all, but it immediately tells Future Hairul—or anyone else looking at the code—what the file is, its purpose, and its version. That’s a small habit borrowed from professional software projects, and I think it fits perfectly with the thoughtful way you’re building this site.
