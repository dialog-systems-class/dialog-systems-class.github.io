---
layout: default
img: TensorFlow.png
caption: Chatbot
title: Homework 3 "First Chatbot!"
active_tab: homework
release_date: 2017-01-31
due_date: 2017-02-16T14:00:00EST
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


Training your first Chatbot in  TensorFlow  <span class="text-muted">: Assignment 3</span> 
=============================================================

The point of the third assignment is to start training a chatbot with TensorFlow. In the Alexa Prize we want to design a deep learning social bot. The first step is to be able to train a seq2seq model. Now that you've understood how to train the basic seq2seq model, we'll focus on starting to reproduct the Neural Conversation Model code.

You should be excited about this assignment! You will be able to chat with your own bot!

Be creative and have fun.
 

1. Make sure to first test your model with TensorFlow on your computer, or somewhere where you have FREE personal access.
2. Train the Neural Conversation Model using Twitter, or Ubutu corpus. For the dataset, you may choose between the twitter datasets [https://github.com/suriyadeepan/datasets/tree/master/seq2seq/twitter](https://github.com/suriyadeepan/datasets/tree/master/seq2seq/twitter) and the Ubuntu dataset [https://github.com/rkadlec/ubuntu-ranking-dataset-creator](https://github.com/rkadlec/ubuntu-ranking-dataset-creator). For both datasets there are good reference code to look at, particularly for the Ubuntu dataset there is [http://www.wildml.com/2016/07/deep-learning-for-chatbots-2-retrieval-based-model-tensorflow/](http://www.wildml.com/2016/07/deep-learning-for-chatbots-2-retrieval-based-model-tensorflow/).
3. Integrate your chatbot with Alexa skill
4. Evaluate your chatbot. Here, you should show some qualitative examples as well as train and test loss. Furthermore, try to be creative and see if you can make a metric for how well your chatbot is doing. 
5. Identify issues with your chatbot and suggest possible solutions and future work.
6. Submit homework [https://goo.gl/forms/FcvNJVwol6eV9T7j2](https://goo.gl/forms/FcvNJVwol6eV9T7j2).

