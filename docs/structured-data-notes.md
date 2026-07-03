Hairul…

I think this is the perfect moment to say congratulations.

Not because you created another Markdown file.

Because you’ve quietly crossed a line.

Most people have:

A website.

You now have:

A software project.

There’s a huge difference.

⸻

Before Sprint 2.3

Let’s officially freeze what we’ve built.

Hairul Knowledge Base (HKB)

Version : 0.5.0
Status  : Stable

Completed

✅ Repository Architecture
✅ Branding
✅ Content Strategy
✅ Editorial Workflow
✅ Documentation System
✅ Naming Convention
✅ HTML Head Notes
✅ Social Metadata Notes
✅ Version History
✅ Project Constitution

That’s an excellent foundation.

⸻

Now…

Welcome to what I think is the most fascinating part of modern SEO.

Sprint 2.3

Structured Data (JSON-LD)

⸻

First…

Forget HTML for a moment.

Imagine your article is a physical book.

A human picks it up.

Immediately they know:

* It’s a book
* The title
* The author
* The publisher
* The cover
* The publication date

Humans understand context.

Computers don’t.

Google only sees text like:

<h1>
<p>
<img>
<div>

Nothing tells Google

“This is an article.”

Unless…

…you explicitly tell it.

⸻

JSON-LD is basically an ID Card.

Think of it like this.

Your article has two identities.

Identity 1

Visible.

Humans read this.

Title
Paragraph
Image
Buttons

⸻

Identity 2

Invisible.

Machines read this.

Type
Author
Publisher
Date
Image
Headline

This second identity is JSON-LD.

⸻

The Evolution

Most beginners stop here.

HTML
↓
Browser

Professional websites go further.

HTML
↓
Browser
↓
JSON-LD
↓
Google
↓
AI Search
↓
Knowledge Graph

This is why structured data matters even more today than it did a few years ago. AI-powered search systems benefit from clear, machine-readable context.

⸻

The vocabulary

The first thing every JSON-LD contains is

{
 "@context":"https://schema.org"
}

Think of this as

“We’re speaking Schema.org.”

Exactly like saying

“This document is written in English.”

⸻

Next

@type

This tells Google

What is this thing?

For us

BlogPosting

NOT

Blog

A blog is a collection.

A BlogPosting is one article.

Very different.

⸻

Example

Imagine this.

Website
↓
Artikel
↓
Saya Baru Bekerja

The website

↓

Website

The article

↓

BlogPosting

⸻

Why this matters

Suppose in five years your site has

120 articles.

Google understands

Website
↓
contains
↓
120 BlogPosting

instead of

Website
↓
contains
↓
120 random HTML pages

That’s a much richer understanding.

⸻

Our JSON-LD

We’ll eventually include fields like these:

Property	Purpose
headline	Article title
description	Summary
author	You
publisher	Your website
image	Hero image
datePublished	Publish date
dateModified	Last updated
mainEntityOfPage	Canonical URL

Every property answers a question a search engine might ask.

⸻

One concept I want you to remember forever

HTML tells browsers how to display a page.

JSON-LD tells machines what the page means.

That’s the essence of structured data.

⸻

Why we’re learning this now

Because later, when we build article-template.html, the JSON-LD section won’t feel like mysterious code. You’ll know it’s simply your article introducing itself to search engines.

⸻

Homework

Create one more note:

docs/structured-data-notes.md

Answer these questions in your own words:

1. What problem does JSON-LD solve? help machine identify this is a blogpost, not just lines of code
2. Why is BlogPosting better than Blog for an individual article? machine can determine how many articles we published
3. What is the difference between HTML and JSON-LD? html is the code for machine to display information properly, json-ld is for the machine to understand what type of information they are displaying
4. List five pieces of information you think a search engine should know about one of your articles. type, author, publisher, date, headline

Keep it concise—these are your personal learning notes.

⸻

Then comes the part I’ve been waiting for

After Sprint 2.3, we finally begin building the visible article page:

* Breadcrumbs
* Article header
* Hero image
* Metadata
* Reading time
* Table of contents
* Article body
* “Nasihat Hairul”
* Author card
* Related articles
* CTA

At that point, we’ll start transforming templates/article-template.html into a reusable publishing template that will serve as the backbone for every article you publish.

One last suggestion

I’d like to add a simple rule to your project-constitution.md:

“Understand before implementing.”

I think that one sentence captures the way you’ve approached this entire project. It’s a principle that will serve you well not just for this website, but for any technical project you take on in the future.
