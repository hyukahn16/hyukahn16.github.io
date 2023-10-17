---
layout: single
title: Reducing Excessive Margin to Achieve a Better Accuracy vs. Robustness Trade-off
categories: paper_summary
classes: wide
---
{% assign question_font_size = "4.5" %}
{% assign answer_font_size = "4" %}
{% assign post_name = "rade" %}
\
[Paper Link](https://openreview.net/pdf?id=Azh9QBQ4tR7){:target="_blank"}{:rel="noopener noreferrer"}\
[GitHub Code Link](https://github.com/imrahulr/hat){:target="_blank"}{:rel="noopener noreferrer"}



<h2>Comprehension</h2>
<font size= "4.5">
<ins>What is the research problem the paper attempts to address?</ins><br>
  <font size="4">
  {% include_relative {{ post_name | append: "_0.html" }} %}<br><br>
  </font>
  
<ins>What are the claimed contributions of the paper?</ins><br>
  <font size="4">
  {% include_relative {{ post_name | append: "_0.html" }} %}<br><br>
  </font>
  
<ins>How do the authors substantiate their claims? bruh bruh</ins><br>
  <font size="4">
  {% include_relative {{ post_name | append: "_claim_0.html" }} %}<br><br>
  {% include_relative {{ post_name | append: "_claim_1.html" }} %}<br><br>
  
  <b>Claim (3):</b>  Pushing the decision boundary only slightly achieves enough robustness (while maintaining accuracy). New algorithm called "Helper-based Adversarial Training" (HAT) provides better robustness without sacrificing the accuracy compared to existing adversarial defenses.<br><br>
  The effect of <em>Helper-based Adversarial Training (HAT)</em> is claimed through experimental results that compare the accuracy and robustness of the networks adversarially trained with HAT and 3 other adversarial training methods.<br><br>
  <a href="/assets/images/rade_2.PNG" target="_blank">
    <img src="/assets/images/rade_2.PNG"/>
  </a><br><br>
  </font>
<ins>What are the conclusions?</ins>
</font>  

<h2>Evaluation</h2>
<font size="4.5">
<ins>Is the research problem significant?</ins><br>
  <font size="4">
  Yes, the research problem is significant. Adversarial training is an actively researched field as one of the adversarial defense methods. Despite the benefits provided by adversarial training, the comparative downside of lowered accuracy has been a challenge among researchers (postulated by <em>Theoretically Principled Trade-off between Robustness and Accuracy</em>). Either solving or reducing the effect of this trade-off would be a significant milestone in cementing adversarial training as the leading methods of adversarial defense.
  </font>
<ins>Are the contributions significant?</ins><br>
<ins>Are the claims valid?</ins><br>
</font>


<h2>Synthesis</h2>
<font size="4.5">
<ins>What is the crux of the research problem?</ins><br>
</font>
