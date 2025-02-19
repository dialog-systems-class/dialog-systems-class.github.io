---
layout: default
img: Alexa.png
caption: Hello Alexa    
title: Homework 1 "Say Hello Alexa"
active_tab: homework
release_date: 2020-01-27
due_date: 2020-02-05T15:00:00EST
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


Create a simple hello response bot using the Alexa SDK <span class="text-muted">: Assignment 1</span> 
=============================================================

The point of the first assignment is to get to acquainted with the Amazon Alexa SDK. The first step is to be able to integrate  with Alexa SDK. This involves creating an AWS account and learning how to start up and integrate with AWS Lambda. This code will be the base for all of the interactions and it makes sense to start with a practical "hello world" or more precisely a response. 

You should be excited about this assignment! You will be able to chat with your own bot!

The idea is to be able to chat with an Alexa enabled device. For example:
 
To Device:
“Alexa, open Jowtest.”
"Hi."
Device responds:
"Hello."
 
Be creative and have fun.
 

1. Sign up for [Amazon AWS](https://aws.amazon.com/console/). Note that you should to sign up with your @jhu.edu account, and then sign up for [AWS Educate](https://aws.amazon.com/education/awseducate/apply/).  You will need your [account ID](https://console.aws.amazon.com/billing/home?#/account), which you can find under "my account" from the AWS Admin Panel.  This should give you a $100 credit that you will use for the third assignment when you train your first neural network. You will also get [Free Tier access](https://aws.amazon.com/free/)
2. Figure out how to start a AWS Lambda session
3. Follow the instructions from [https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/testing-an-alexa-skill](https://developer.amazon.com/public/solutions/alexa/alexa-skills-kit/docs/testing-an-alexa-skill). You may also find this [guide from DeepPavlov](http://docs.deeppavlov.ai/en/master/integrations/amazon_alexa.html) useful. The main impediment is that you want to get the raw text and not use intent.
4. Setup a minimalist python interface. One example to draw from is [https://github.com/anjishnu/ask-alexa-pykit](https://github.com/anjishnu/ask-alexa-pykit).
Use the python ASK to respond "Hello". 
5. Create a mimic bot, so that if you say "I'm hungry" the device will respond "You said, "I'm hungry""
6. [Extra Credit] Have fun and try something else that's fun.

You should test your skill using Echosim.io.

 

7. You should have at least three files in the repository: (lambda_function.py and/or alexa_server.py)  and interaction_model.json, as well as a README.md for repro steps. Submit homework via [GradeScope](https://www.gradescope.com/courses/85654). For further inspiration and how to structure your code see [Daphne Ippolito's repo](https://github.com/daphnei/nn_chatbot/tree/master/homeworks/alexa_chatbot).