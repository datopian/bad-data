---
layout: home
title: Bad Data
subtitle: Real-world examples of how <strong>not</strong> to do data
---

Bad Data is site providing **real-world examples** of how not to prepare or provide data. It showcases the poorly structured, the mis-formatted, or the just plain ugly.

Its primary purpose is to **educate** &ndash; though there may also be some aspect of entertainment.

As a side-product it also provides a source of good practice material for budding data wranglers (the repo in fact began as a place to keep practice data for [Data Explorer][explorer]).

## Submit a Bad Data Example

[New examples wanted and welcome &ndash; submit them here &raquo;][add]

[explorer]: http://explorer.okfnlabs.org/
[csv]: http://data.okfn.org/standards/csv
[add]: {{site.baseurl}}/add
[new]: https://github.com/okfn/bad-data/issues/new
[dataissues]: https://github.com/datasets/issues

## Current Examples

<div class="results">
  {% for page in site.pages %}
  {% if page.categories == 'examples' and page.url != '/ex/template/index.html' %}
  <div class="result">
    <h4><a href="{{site.baseurl}}{{page.url | replace:'index.html',''}}">{{page.title}}</a></h4>
  </div>
  {% endif %}
  {% endfor %}
</div>

