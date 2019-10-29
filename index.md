---
title: Deep Learning for Automated Discourse- EN.601.767  - Johns Hopkins University
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
:  - Deep Learning Methods for Automated Discourse

Instructor
: [João Sedoc](https://sites.google.com/site/jsedoc/)

Discussion Forum
: [Piazza](https://piazza.com/)

Time and place
: Spring 2020, Tuesdays and Thursdays 3-4:15,  Hodson 303

Prerequisites
: 

Course Readings
: The course will have [weekly required readings](readings.html).  A student will lead the discussion for each week's papers.

Grading
: This course is project based:

* Paper Presentation 10% 
* Project Demonstration 20% (checkpoints 5%)
* Written report 35%
* Report Review 5%
* Homeworks (4) 20% 
* Reading assignments 10%

Course materials
: We're going to be working with Amazon Echo and PyTorch.

Assignments
: Quick outline for the next assignments.

* Project checkpoint 1 - due ~ March 16th
  * write a two page overview of the project and a 10 minute presentation

* Project checkpoint 2 - due ~ April 13th
   * modify first document to 4 pages with initial results, another 10 minute presentation, and first demo

* Final project paper submission - due ~ April 27th 
   * submit 6 page paper - for open review

* Final paper reviews due - due May 1st

* During the final exam period (TBD)  20-30 minute presentation and demo

* Final paper submission - due ~ May 9th
