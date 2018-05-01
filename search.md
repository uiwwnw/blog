---
layout: page
title: Search
permalink: /search/
---

<style>
    .searchInput {
        width: 100%;
        height: 2em;
        box-sizing: border-box;
        font-size: 1em;
        font-family: inherit;
    }
</style>
<input class="searchInput" type="text" id="search-input" placeholder="검색어를 입력해주세요.">
<ul class="resultsWrap" id="results-container"></ul>
<!-- <script src="{{ site.baseurl }}/asset/js/simple-jekyll-search.min.js"></script> -->
<script src="https://cdn.rawgit.com/christian-fei/Simple-Jekyll-Search/master/dest/simple-jekyll-search.min.js"></script>
<script>
    var sjs = SimpleJekyllSearch({
        searchInput: document.getElementById('search-input'),
        resultsContainer: document.getElementById('results-container'),
        json: '{{ site.baseurl }}/search.json',
        noResultsText: '검색결과가 없습니다.',
        limit: 10,
        fuzzy: false
    })
</script>