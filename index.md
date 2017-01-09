---
title: Deep Learning Methods for Automated Discourse - CIS 700  Special Topics - University of Pennsylvania
layout: default
img: HAL.png
img_link: https://en.wikipedia.org/wiki/HAL_9000
caption: I am putting myself to the fullest possible use, which is all I think that any conscious entity can ever hope to do. 
active_tab: main_page 
---


<!-- Display an alert about upcoming homework assignments -->
{% capture now %}{{'now' | date: '%s'}}{% endcapture %}
{% for page in site.pages %}
{% if page.release_date and page.due_date %}
{% capture release_date %}{{page.release_date | date: '%s'}}{% endcapture %}
{% capture due_date %}{{page.due_date | date: '%s'}}{% endcapture %}
{% if release_date < now and due_date >= now %}
<div class="alert alert-info">
<a href="{{page.url}}">{{ page.title }}</a> has been released.  
{% if page.deliverables %}
The assignment has multiple deliverables.
{% for deliverable in page.deliverables %}
The {{deliverable.description}} is due before {{ deliverable.due_date | date: "%I:%M%p" }} on {{ deliverable.due_date | date: "%A, %B %-d, %Y" }}.  
{% endfor %}
{% else %}
It is due before {{ page.due_date | date: "%I:%M%p" }} on {{ page.due_date | date: "%A, %B %-d, %Y" }}.
{% endif %}
</div>
{% endif %}
{% endif %}
{% endfor %}
<!-- End alert for upcoming homework assignments -->


Course number
: CIS 700-7 - Special Topics - Deep Learning Methods for Automated Discourse

Instructors
: [João Sedoc](https://sites.google.com/site/jsedoc/)
: [Chris Callison-Burch](http://www.cis.upenn.edu/~ccb/)
: [Lyle Ungar](http://www.cis.upenn.edu/~ungar/)

Discussion Forum
: [Piazza]()

Time and place
: Spring 2017, Tuesdays and Thursdays 2-3:30, Levine 512

Prerequisites
: [CIS 419/519](http://www.cis.upenn.edu/~cis519/fall2014/) or [CIS 520](https://alliance.seas.upenn.edu/~cis520/wiki)

Course Readings
: Each lecture has an accompanying set of [academic papers](lectures.html)

Grading
: TBD

Course materials
: We're going to be working with Amazon Echo.

