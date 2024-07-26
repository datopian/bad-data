# Bad Data

## Real-world examples of how *not* to do data

Bad Data is a site providing **real-world examples** of how **not** to prepare or provide data. It showcases the **poorly structured**, the **mis-formatted**, or the just plain ugly.

Its primary purpose is to **educate** &ndash; though there may also be some aspect of entertainment.

As a side-product it also provides a source of good practice material for budding data wranglers (the repo in fact began as a place to keep practice data for [Data Explorer][explorer]).

[New examples are wanted and welcome &ndash; submit them here &raquo;][add]

[explorer]: http://explorer.okfnlabs.org/
[csv]: http://data.okfn.org/standards/csv
[add]: #add

## Examples

- [Plain Text (ASCII) Spreadsheet from US Government Bureau of Labor Statistics](/ex/bls-us-employment/)
- [Cairo Transport Authority Data](/ex/cairo-transport-authority/)
- [Greater London Authority Spending](/ex/gla-spending/)
- [List of Mexican Towns With Population Under 5000](/ex/mex-list-towns-pop-under-5000/)
- [Nature Magazine supplementary information](/ex/nature-magazine-supplementary/)
- [Russian foreign trade statistics](/ex/russian-foreign-trade-statistics/)
- [Passenger Numbers for Humans Only](/ex/tfl-passenger-numbers/)

## Add an Example

New examples are wanted! Here's how to submit one.

### What information to provide

What's we'd like to see in a good example is:

* Original data url (and name of organization providing the data)
* File format (e.g. CSV, Shapefile etc)
* A description of what's wrong
* A nice illustrative image or screenshot

Optional (but desirable): a backup of the data in case it goes away! (If the file is more than ~100kb please provide a chopped down version illustrating the main "badness").

Also don't forget to credit yourself in an appropriate way (if you want to be credited!).

Lastly, note that your contribution will be licensed under this site's general <a href="http://creativecommons.org/licenses/by/3.0/">CC Attribution License</a>.

## How to Contribute

### Option 1: Fork and Pull

This website is stored in a [github repo][repo] which you can fork and pull to add your example. Here are detailed instructions:

[repo]: https://github.com/datopian/bad-data
[fork]: https://github.com/datopian/bad-data/fork 

1. [Fork the bad-data github repository][fork]

2. Choose a "slug" for your example e.g. `my-bad-data-example`

3. Copy and paste the `ex/template/` to a directory `ex/{your-slug}`

4. Edit the `ex/{your-slug}/index.md` file

    * Change the frontmatter attributes (i.e. key/value items at very top of file) as appropriate
    * Add the description (markdown formatted) to the main section of that page

5. Commit the new file

6. Then submit the [pull request][pull]

[pull]: https://help.github.com/articles/using-pull-requests

## Option 2: Open an Issue

If the thought of forks and pulls give you the jitters there's an ultra-simple alternative: just [open an issue][issues] in the issue tracker and add the information requested!

[issues]: https://github.com/okfn/bad-data/issues/new
