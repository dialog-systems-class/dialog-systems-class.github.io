---
layout: default
img: chatbot.png
caption: Chatbot
title: Homework 3 "HRED"
active_tab: homework
release_date: 2020-02-11
due_date: 2020-02-21T15:00:00EST
---

<!-- Check whether the assignment is up to date -->
{% capture this_year %}{{'now' | date: '%Y'}}{% endcapture %}
{% capture due_year %}{{page.due_date | date: '%Y'}}{% endcapture %}
{% if this_year != due_year %} 
<div class="alert alert-danger">
Warning: this assignment is out of date.  It may still need to be updated for this year's class.  Check with your instructor before you start working on this assignment.
</div>
{% endif %}
<!-- End of check whether the assignment is up to date -->

<div class="alert alert-info">
This assignment is due before {{ page.due_date | date: "%I:%M%p" }} on {{ page.due_date | date: "%A, %B %-d, %Y" }}.
</div>


Implementing HRED in ParlAi  <span class="text-muted">: Assignment 3</span> 
=============================================================

The point of the third assignment is to reimplement HRED in ParlAi. The focus of this project is to start to be able to build a model in the ParlAi framework and start to try different datasets. 

You should be excited about this assignment! You will be able to chat with your own bot!

Be creative and have fun.
 

1. Implement the HRED model within ParlAi. This involved creating the context vector and manipulating the data loading process. This does not have to be an exact reproduction of HRED. You may want to look at Harshal's [implementation](https://github.com/hsgodhia/hred) or Julian Serban's [old fork of ParlAi](https://github.com/julianser/ParlAI).
2. Train the HRED model use any dataset that you'd like.
3. Integrate your chatbot with Alexa skill
4. Evaluate your chatbot. Here, you should show some qualitative examples as well as train and test loss. Furthermore, try to be creative and see if you can make a metric for how well your chatbot is doing. 
5. Identify issues with your chatbot and suggest possible solutions and future work.
6. Submit homework on [Gradescpoe](https://www.gradescope.com/courses/85654).

Please remember to include a README. If there are too many files that simply point to your github ... sorry about Gradescope.

