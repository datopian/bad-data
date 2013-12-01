---
layout: home
title: Bad Data
subtitle: Real-world examples of how <strong>not</strong> to do data
---

Bad Data is site providing **real-world examples** of how **not** to prepare or provide data. It showcases the **poorly structured**, the **mis-formatted**, or the just plain ugly.

Its primary purpose is to **educate** &ndash; though there may also be some aspect of entertainment.

As a side-product it also provides a source of good practice material for budding data wranglers (the repo in fact began as a place to keep practice data for [Data Explorer][explorer]).

[New examples wanted and welcome &ndash; submit them here &raquo;][add]

[explorer]: http://explorer.okfnlabs.org/
[csv]: http://data.okfn.org/standards/csv
[add]: {{site.baseurl}}/add

## Examples

<ul class="thumbnails examples-list">
  {% for page in site.pages %}
  {% if page.categories == 'examples' and page.url != '/ex/template/index.html' %}
  {% capture url %}{{site.baseurl}}{{page.url | replace:'index.html',''}}{% endcapture %}
  <li class="span6">
    <div class="thumbnail">
      <h3><a href="{{url}}">{{page.title}}</a></h3>
      <a href="{{url}}"><img src="{{page.image}}" /></a>
    </div>
  </div>
  {% endif %}
  {% endfor %}
</ul>

