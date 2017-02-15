---
layout: default
img: chatbot.png
caption: Chatbot
title: Homework 4 "Your Chatbot!"
active_tab: homework
release_date: 2017-02-15
due_date: 2017-02-28T14:00:00EST
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


Training your Chatbot in  TensorFlow  <span class="text-muted">: Assignment 4</span> 
=============================================================

The point of this fourth homework assignment is to start training a new model and chatbot with new data. From the previous homeworks, we've been mostly using canned code and datasets. This is the time to break free and try to make your own model and use a dataset that you are interested in or passionate about.

What kind of conversations would you like to have with your own bot?

Be creative and have fun.
 

1. Make sure to first test your model with TensorFlow on your computer, or somewhere where you have FREE personal access.
2. Train the pick a dataset to train on. In the README.md file of your github repo, write the details about the dataset. Why did you pick it? What were your considerations?
3. Train the seq2seq model on the dataset.
4. Use a more sophisticated model than seq2seq. For example try to capture context, or infer question or topic, ...
5. Evaluate your model as well as the seq2seq model. Which does better? Also, try out your model from HW3. How does this do compared with models trained on your dataset?  Again, as you evaluate your chatbot, you should show some qualitative examples as well as train and test loss.
6. Integrate your models with Alexa Skills.
7. Submit homework [https://goo.gl/forms/0NrRbmfJk3OPJBmJ2](https://goo.gl/forms/0NrRbmfJk3OPJBmJ2).

