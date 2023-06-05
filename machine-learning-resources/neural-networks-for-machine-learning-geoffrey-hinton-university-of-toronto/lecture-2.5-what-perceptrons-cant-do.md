# Lecture 2.5 - What perceptrons can't do

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=10&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=mI6jTc-8sUY" %}



* If you use the right features, you can do almost anything --> thus, we can emphasize, that in learning, a big part of succeeding is learning the right features

## The limitations of perceptrons

* if you can choose features by hand and if you choose enough features, you cand o almost anything&#x20;
  * for binary input vectors, we can have a separate features unit for each of the exponentially many binary vectors, so that we can make any possible discrimination on binary input vectors&#x20;
    * but we need a lot of features here
    * and this type of table look-up won't generalize
    * many cases require new features
  * but once the hand-coded features have been determined, there are very strong limitations on what a perceptron can learn&#x20;

## What binary threshold neurons cannot do

* cannot tell if two single bit features are the same&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.48.08 PM.png" alt=""><figcaption><p>An example of bit features and binary threshold neurons</p></figcaption></figure>

* we can prove this algebraically&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.49.18 PM.png" alt=""><figcaption><p>There's no way to get all four cases right</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.49.58 PM.png" alt=""><figcaption><p>Binary decision unit </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.50.54 PM.png" alt=""><figcaption><p>When there's no hyperplane that can separate these points, we call them a set of cases that are not linearly separable.</p></figcaption></figure>

* What if we want to recognize a pattern, even if it's translated?

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.53.03 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.55.28 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.56.50 PM.png" alt=""><figcaption></figcaption></figure>

* Neural networks can only be really powerful if we can learn the feature vectors (not just the weights)&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 2.58.29 PM.png" alt=""><figcaption></figcaption></figure>
