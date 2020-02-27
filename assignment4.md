---
layout: default
img: chatbot.png
caption: Chatbot
title: Homework 4 "Diverse Responses and Evaluation!"
active_tab: homework
release_date: 2020-02-27
due_date: 2020-03-11T15:00:00EST
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


Diverse Responses and Evaluation  <span class="text-muted">: Assignment 4</span> 
=============================================================

The point of the fourth assignment is to solve some issues from homework 3 and also evaluate! In particular, there are two issues (1) the responses seemed bland and (2) evaluation is difficult for social bots. The first step is to be able to train either a language model or a backwards model, so P(S|T). Then you should implement Maximum Mutual Information from [A Diversity-Promoting Objective Function for Neural Conversation Models](https://arxiv.org/abs/1510.03055). 


Be creative and have fun.
 

1. Re-implement the data filtering described in DialoGPT paper _OR_ [Improving Neural Conversational Models with Entropy-Based Data Filtering](https://www.aclweb.org/anthology/P19-1567/).
2. Using the filtered data train a model on OpenSubtitles using P(T\|S) and P(S\|T) with filters and also when the last character is a quesionmark("?").
3. Train P(T\|S) transformer models on the PersonaChat or DialyDialog dataset using either the model from (part 2) or  Reddit pre-trained model for P(T\|S).
4. Decoder with MMI-bidi objective.
5. Evaluate your chatbot on the mechanical turk SANDBOX using ParlAI's [model evaluator](https://parl.ai/docs/tutorial_mturk.html) and [code]((https://github.com/facebookresearch/ParlAI/tree/master/parlai/mturk/tasks/model_evaluator). 
6. Identify issues with your chatbot and suggest possible solutions and future work.
7. Submit homework on [Gradescpoe](https://www.gradescope.com/courses/85654).

Please remember to include a README. If there are too many files that simply point to your github ... sorry about Gradescope.

