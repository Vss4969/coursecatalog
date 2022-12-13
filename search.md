---
layout: page
title: Search
permalink: /search
---


<form class="searchbar" id="search-container">
    <h1>Search here</h1>
    <input class="form-control me-2" type="search" placeholder="search..." aria-label="Search" id="search-input">
    <!-- <button class="btn btn-outline-success" type="submit"><i class="fa-solid fa-magnifying-glass"></i></button> -->
    <div id="results-container" class="courselist"></div>
</form>

<!-- <h1>Search here</h1>
<div id="search-container">
<input type="text" id="search-input" placeholder="search...">
<ul id="results-container"></ul>
</div> -->

<script src="assets/js/search-script.js" type="text/javascript"></script>

<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: "assets/search.json"
})
</script>