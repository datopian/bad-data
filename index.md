---
layout: default
title: Bad Data
subtitle: Examples of poorly structured, formatted,<br />mangled or just plain ugly data
---

Bad Data is site listing real-world examples of poorly structured, formatted, mangled or just plain ugly data. It exists to instruct, entertain and provide material for practice (the repo in fact began as a place to keep practice data for [Data Explorer][explorer]).

* [Here's the current bad data list &raquo;][list]
* Contributions wanted and welcome &ndash; see below

Want to see "bad data" fixed? Check out the related ["Data Issues"
project][dataissues] focused on reporting and fixing issues with (open) data.


[list]: https://github.com/okfn/bad-data/issues
[explorer]: http://explorer.okfnlabs.org/
[csv]: http://data.okfn.org/standards/csv
[new]: https://github.com/okfn/bad-data/issues/new
[dataissues]: https://github.com/datasets/issues

## Bad Data Examples

<div class="results">
  <ul>
  {% for page in site.pages %}
  {% if page.categories == 'examples' %}
    <li><h4><a href="{{site.url}}{{page.url | replace:'index.html',''}}">{{page.title}}</a></h4></li>
  {% endif %}
  {% endfor %}
  </ul>
</div>

## How to contribute

Preference for examples of tabular data and especially for [CSV][csv] but all
forms of bad data accepted!

[Just open an issue &raquo;][new]

Please include:

* Data source (link and info)
* File format
* A description of what's wrong

Optional (but preferred):

* Screenshot of the data
* Copy of the data (if the file is more than ~100kb please provide a chopped down version illustrating the main "badness"). Please upload a the sample data file to the data directory (fork and pull this repo!)

