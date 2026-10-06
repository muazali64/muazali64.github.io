---
layout: page
permalink: /publications/
title: publications
description: Research papers, listed from newest to oldest.
nav: true
nav_order: 2
---

<!-- _pages/publications.md -->

<section class="publication-summary" aria-label="Publication counts">
  <dl class="publication-counts">
    <div><dt>Total</dt><dd>{% bibliography_count %}</dd></div>
    <div><dt>Peer-reviewed</dt><dd>{% bibliography_count --query @*[peer_reviewed=true] %}</dd></div>
    <div><dt>First-author</dt><dd>{% bibliography_count --query @*[first_author=true] %}</dd></div>
  </dl>
  <p>Totals include preprints; peer-reviewed includes accepted papers. First-author includes joint first authorship.</p>
</section>

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
