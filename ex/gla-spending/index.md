---
title: Greater London Authority Spending
author: Rufus Pollock
---

This isn't about a single data file but an entire dataset. The dataset is the UK's Greater London Authority spend data:

http://www.london.gov.uk/mayor-assembly/gla/spending-money-wisely/budget-expenditure-charges/expenditure-over-250

The good news is that, as per UK government policy, the GLA provides regular data on spending over £250, and, furthermore, the data is in simple [CSV files][csv].

[csv]: http://datahub.io/docs/data-formats/csv

That's where the good news ends. Here are primary issues:

* Data is in **many separate files** (**65** as per summer 2013) with no consistent naming scheme so downloading them requires [scraping][] (or tedious click and save)
* Amongst the 65+ CSV files one find approximately **25+ different structures** (structure means things like: number of blank or non-data lines at top of files, blank columns, varying headers). This therefore requires [elaborate coding][process] to consolidate the data into a single form. You can see a full summary of all the different file structures in this [data wrangle][headings]

[scraping]: https://github.com/rgrp/dataset-gla/blob/master/scripts/scrape.js
[process]: https://github.com/rgrp/dataset-gla/blob/master/scripts/process.js#L22
[headings]: http://explorer.okfnlabs.org/#rgrp/63e14589091a917d175a/view/grid

Additional specific errors:

* Almost every file does not start with actual data headers but with random metadata (see file to left as an example)
* (July 2013) [Period 8 2012/13](http://static.london.gov.uk/gla/expenditure/docs/2012-13-P8-250.csv) is not a CSV file but is in fact an HTML file showing a 403 Access Denied from someone's login session. (It suggests that each CSV file is produced by manual download of a file from an internal system (probably SAP-based to judge by some file headings). See cached [HTML version](bad-month-401.html)
  * <del>(March 2013) Bad file for [Period 8 2012/13 (13 October - 10 November)](http://www.london.gov.uk/sites/default/files/Mayor's%20250%20Report%20-%202012-13%20-%20P8%20%20-%20Final.csv).  The file is not named in the usual way "Mayor's%20250%20Report%20-%202012-13%20-%20P8%20%20-%20Final.csv" and appears to be an Excel file that was not converted to CSV!</del>
* Amounts are formatted with "," making them appear as strings to computers.
* Dates vary substantially in format from "16 Mar 2011" in [this file](http://static.london.gov.uk/gla/expenditure/docs/2010-11-P13-500.csv) to "21.01.2010" in [January 2010 data](http://legacy.london.gov.uk/gla/expenditure/docs/january_2010.csv)
* Use of (978) to indicate negative amounts rather than -978
* Repeated data in [2012-13-P4 file (HTML view on datapipes)](http://datapipes.okfnlabs.org/csv/html/?url=http://static.london.gov.uk/gla/expenditure/docs/2012-13-P4-250.csv#L870)

## Update

2016-04-06

The original web page now 404s:

<http://www.london.gov.uk/mayor-assembly/gla/spending-money-wisely/budget-expenditure-charges/expenditure-over-250>

And all the raw spending files have moved without redirects so they break ... e.g. this no longer works:

<http://static.london.gov.uk/gla/expenditure/docs/2010-11-P13-500.csv>

The new web page only list files back to 2013 and it is not clear where the earlier files are located.

