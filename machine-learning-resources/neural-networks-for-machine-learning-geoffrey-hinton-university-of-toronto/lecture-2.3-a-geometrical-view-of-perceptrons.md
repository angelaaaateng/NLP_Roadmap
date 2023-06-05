---
description: What happens when a perceptron learns?
---

# Lecture 2.3 - A geometrical view of perceptrons

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=10&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=0T57_yjjB58" %}

* Dealing with hyperplanes in 14-dimensional spaces

## Weight-Space

* this space has one dimension per weight
* a point in space represents a particular setting of weights&#x20;
* assuming that we've eliminated the threshold, each training case can be represented as a hyperplane through the origin
  * weights must lie on one side of the hyperplane in order to get the answer correct

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.32.03 PM.png" alt=""><figcaption><p>On one side of the perceptron, we have all correct answers. On the other side, we have all wrong answers. </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.33.01 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.34.43 PM.png" alt=""><figcaption><p>In general, in ML if you get a convex learning problem, those are easier to solve.</p></figcaption></figure>
