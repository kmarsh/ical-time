# ical-time

Utility for pulling data out of iCal, useful for time tracking


## Usage

<div style="float: right"><img src="http://farm4.static.flickr.com/3409/3449709123_f19087dee4_o.png"></div>

Create events in iCal when you work on a project. Titles are mostly
irrelevant, but if you want to track projects, make sure they begin with the
project name in brackets.

<pre>~$ ical-time --summary CalendarName
------------------------------  
04/13/2009 - Today
------------------------------
Project N                12.25
Project C                 4.25
Project O                 4.00
Project S                 2.75
Project H                 2.00
Unassigned                2.00
Project M                 1.75
Project B                 1.50
Project R                 1.25
Project F                 1.00
==============================
Total                    32.75</pre>

You can also pass `--from DATE` and `--to DATE` to narrow the scope of events returned.
Dates are parsed using Chronic, so many types of natural date strings like:

- `yesterday`
- `monday`
- `april 1st`

Pass `-c FILENAME.csv` to output event information in CSV. You'll get one line
per event, with columns for Date, Project, Event Title, and Duration. This is
perfect for importing to a database or doing further analysis.


## Copyright

Copyright (c) 2009 Kevin Marsh. See LICENSE for details.
