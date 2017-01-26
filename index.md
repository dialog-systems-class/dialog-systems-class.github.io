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
: [Piazza](https://piazza.com/upenn/spring2017/cis7007)

Time and place
: Spring 2017, Tuesdays and Thursdays 2-3:30, Levine 512

Prerequisites
: [CIS 419/519](http://www.cis.upenn.edu/~cis519/fall2014/) or [CIS 520](https://alliance.seas.upenn.edu/~cis520/wiki)

Course Readings
: The course will have [weekly required readings](readings.html).  A student will lead the discussion for each week's papers.

Grading
: This course is project based:

* Paper Presentation 10% 
* Project Demonstration 20% (checkpoints 5%)
* Written report 40% 
* Homeworks (4) 20% 
* Reading assignments 10%

Course materials
: We're going to be working with Amazon Echo.

Assignments
: Quick outline for the next assignments.

* HW3 - due Feb 9th 
  * integrate your chatbot with Alexa skill 
  * evaluate your chatbot

* HW4 - due Feb 28th
  * find a dataset to train your model on.
  * train with seq2seq model
  * Use a model a bit more sophisticated than seq2seq model
  * evaluate model both models as well as model from HW3
  * integrate models with Alexa skill 

* Project checkpoint 1 - due March 14th
  * write a two page overview of the project and a 10 minute presentation

* Project checkpoint 2 - due April 11th
   * modify first document to 4 pages with initial results, another 10 minute presentation, and first demo

* Final project submission - due April 27th
   * present results, and 20-30 minute presentation and demo
   * submit 6 page paper - for open review

* Final paper reviews due - due May 1st

* Final paper submission - due May 9th