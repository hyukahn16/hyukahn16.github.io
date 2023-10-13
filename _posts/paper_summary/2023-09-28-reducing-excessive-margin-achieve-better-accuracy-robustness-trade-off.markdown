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
  <b>Claim (1):</b>  Adversarial training causes the decision boundaries of the network to shift unncessarily far in the adversarial direction.<br><br>
  Using CIFAR-10 and ResNet-18 (94.6% accuracy, 0% robustness to PGD L-inf attacks) fine-tuned with adversarial training (83.3% accuracy, 51.6% robustness), the authors first show that the network overfits or accounts excessively for the initial adversarial training directions as show in the graph below.<br><br>
  <a href="/assets/images/rade_margin_0.PNG" target="_blank">
    <img src="/assets/images/rade_margin_0.PNG"/>
  </a><br>
  The central argument from this graph is that the left-most image shows greatest difference between the initial margins and the final margins. This difference in the margins may mean that the effect of adversarial training is pushing the decision boundaries unncessarily farther in the direction of the initial adversarial training while only slightly pushing it for later adversarial training.<br><br>

  <b>Claim (2):</b>  <em>The drastic rise in the margin along the initial adversarial training direction is directly correlated to the observed reduction in accuracy."</em><br><br>
  Using an adversarially fine-tuned network (trained on CIFAR-10) using TRADES with various robustness-accuracy trade-off variable. As this variable was increased in the experiment, the margin also increased in the direction of the initial adversarial direction along with increased reduction in accuracy.<br><br>
  <a href="/assets/images/rade_1.PNG" target="_blank">
    <img src="/assets/images/rade_1.PNG" height="50" width="50"/>
  </a><br>
  
  <b>Claim (3):</b>  New algorithm called "Helper-based Adversarial Training" (HAT) provides better robustness without sacrificing the accuracy compared to existing adversarial defenses.<br><br>
  The effect of <em>Helper-based Adversarial Training (HAT)</em> is claimed through...<br>
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
