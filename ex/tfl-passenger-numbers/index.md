---
layout: example
title: Passenger Numbers for Humans Only
dataformat: CSV
datapublisher: Greater London Authority London Datastore
dataurl: http://data.london.gov.uk/datafiles/transport/tfl_passengers.csv
cached: https://raw.github.com/rgrp/bad-data/master/data/tfl_passengers.csv
author: Rufus Pollock
authorurl: https://okfn.org/members/rgrp
categories: examples
---

This is a CSV provided by data.london.gov.uk about Transport for London (TfL) passenger numbers. The problem is the CSV is so messy only a human could use it! What specifically is wrong?

* The first column is missing a heading (one guesses this should be "date"?)
* Dates are not of a recognizable format instead being of form: "2006/2007 - 1". One assumes this should be a month or similar (but its not entirely clear if these are months since 13 items in a year!)
* Percentage sign written into percentage column
* Large number of trailing blank rows and columns

