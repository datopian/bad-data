---
layout: example
title: Transport for London (TfL) Passenger Numbers
dataformat: CSV
author: Rufus Pollock
authorurl: https://okfn.org/members/rgrp
source: http://data.london.gov.uk/datafiles/transport/tfl_passengers.csv
categories: examples
cached: https://raw.github.com/rgrp/bad-data/master/data/tfl_passengers.csv
---

What's bad?

* No heading in first column (should be "date"?)
* Dates are of form: "2006/2007 - 1" rather than a month or similar (though not clear if it is monthly since 13 items in a year!)
* Percentage sign written into percentage column
* Huge number of blank rows

<iframe src="http://datapipes.okfnlabs.org/csv/html?url=http%3A%2F%2Fdata.london.gov.uk%2Fdatafiles%2Ftransport%2Ftfl_passengers.csv" width="100%" height="500px"></iframe>
