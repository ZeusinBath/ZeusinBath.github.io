---
layout: post
title: "Search"
permalink: /search/
---

<input type="text" id="search-input" placeholder="Search posts..." style="width:100%; padding:10px; font-size:16px;">

<ul id="results-container"></ul>

<script src="https://unpkg.com/simple-jekyll-search/dest/simple-jekyll-search.min.js"></script>

<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{ "/search.json" | relative_url }}',
  searchResultTemplate: '<li><a href="{url}">{title}</a><p>{content}</p></li>',
  noResultsText: '<li>No results found</li>',
  limit: 10,
  fuzzy: false
})
</script>
