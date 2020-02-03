---
layout: default
img: ParlAi.png
caption: ParlAi
title: Homework 2 "PyTorch and ParlAi"
active_tab: homework
release_date: 2020-01-27
due_date: 2020-02-10T14:00:00EST
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


Learning ParlAi  <span class="text-muted">: Assignment 2</span> 
=============================================================

The point of the first assignment is to get to acquainted with PyTorch. The second step is to be able to train a seq2seq model. This involves installing PyTorch and ParlAi and then training the first models. This homework will get you acquanted with ParlAi.

You should be excited about this assignment! You will be able to chat with your own bot!

Be creative and have fun.
 

1. Make a fork of ParlAi and install it on your computer, or somewhere where you have FREE personal access.
2. Start a AWS or Google Cloud GPU instance with PyTorch installed.
3. Train the seq2seq model in ParlAi on the Twitter dataset which is automatically downloaded using ParlAi. (You may want to use [Google Colab](https://colab.research.google.com/), which allows for several hours of free GPU training). 
5. Record 5 chat logs with your chatbot and also 5 conversations from one of the ParlAi models in their [model zoo](https://www.parl.ai/docs/zoo.html). Please save the conversations in the [Forever chat json format](https://github.com/jkeen/forever-chat-format).
6. Submit homework via [gradescope](https://www.gradescope.com/courses/85654).

* Please check in the code that you used (i.e. your fork of ParlAI. Even if you used the code from the tutorial, please add this. Also, please check in your last checkpoint as well as the final perplexity number. The conversations should be in [Forever chat json format](https://github.com/jkeen/forever-chat-format).
