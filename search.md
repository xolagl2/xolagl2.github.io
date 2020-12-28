---
layout: page
title: Buscar
permalink: /search
---
<!-- Html Elements for Search -->
<div id="search-container">
  <input type="text" id="search-input" placeholder="define ...">
  <ul id="results-container"></ul>
</div>

<!-- Script pointing to search-script.js -->
<script src="/js/search-script.js" type="text/javascript"></script>

<!-- Configuration -->
<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById 'results-container'),
  json: '/search.json',
  searchResultTemplate: '<li><a href="{url}?query={query}" title="{desc}">{title}</a></li>',
  noResultsText: 'No results found',
  limit: 10,
  fuzzy: false,
  exclude: ['Welcome']
})
</script>