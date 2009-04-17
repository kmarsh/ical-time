= ical-time

git remote add origin git@github.com:willcodeforfoo/ical-time.git

== Usage

Create events in iCal when you work on a project. Titles are mostly irrelevant, but if you want to track projects, make sure they begin with the project name in brackets.

If my green calendar in this example is named Calendar, running ical-time with the following options would produce output like:

~$ ical-time --summary Calendar
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
Total                    32.75

You can also pass --from DATE. DATE is parsed using Chronic, so many types of natural date strings like:
* yesterday
* monday
* april 1st 

== Copyright

Copyright (c) 2009 Kevin Marsh. See LICENSE for details.
