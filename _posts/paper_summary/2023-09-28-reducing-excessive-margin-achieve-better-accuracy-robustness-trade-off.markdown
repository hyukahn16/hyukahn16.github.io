---
layout: single
title: Reducing Excessive Margin to Achieve a Better Accuracy vs. Robustness Trade-off
categories: paper_summary
classes: wide
---

[Paper Link]([https://link-url-here.org](https://openreview.net/pdf?id=Azh9QBQ4tR7))

<h2>Comprehension</h2>
<font size="4">
<ins>What is the research problem the paper attempts to address?</ins><br>
  <font size="3.5">
  While adversarial training is known to be a method to protect models against adversarial attacks, it is known to reduce the accuracy. This paper attempts to address this robustness-accuracy tradeoff, which has been postulated by previous works, that they are at odds with one another.<br><br>
  </font>
  
<ins>What are the claimed contributions of the paper?</ins><br>
  <font size="3.5">
  The paper attempts to address the research problem by studying the effects of adversarial training ("<em>examin[ing] the changes induced in the decision boundary of a deep network during adversarial training</em>"). They claim that (1) adversarial training causes "<em>unwarranted increase in the margin along certain adversarial directions</em>" which leads to lower accuracy. The main claimed contribution of this paper is the (2) new algorithm <em>Helper-based Adversarial Training (HAT)</em> which provides better robustness without sacrificing the accuracy compared to existing adversarial defense<br><br>
  </font>
  
<ins>How do the authors substantiate their claims?</ins><br>
  <font size="3.5">
  (1) Using CIFAR-10 and ResNet-18 (94.6% accuracy, 0% robustness to PGD L-inf attacks) fine-tuned with adversarial training (83.3% accuracy, 51.6% robustness), <br>
  (2) The effect of <em>Helper-based Adversarial Training (HAT)</em> is claimed through...<br>
  <br>
  </font>
<ins>What are the conclusions?</ins>
</font>  

<h2>Evaluation</h2>
<font size="4">
<ins>Is the research problem significant?</ins><br>
  <font size="3.5">
  Yes, the research problem is significant. Adversarial training is an actively researched field as one of the adversarial defense methods. Despite the benefits provided by adversarial training, the comparative downside of lowered accuracy has been a challenge among researchers (postulated by <em>Theoretically Principled Trade-off between Robustness and Accuracy</em>). Either solving or reducing the effect of this trade-off would be a significant milestone in cementing adversarial training as the leading methods of adversarial defense.
  </font>
<ins>Are the contributions significant?</ins><br>
<ins>Are the claims valid?</ins><br>
</font>


<h2>Synthesis</h2>
<font size="4">
<ins>What is the crux of the research problem?</ins><br>
</font>
