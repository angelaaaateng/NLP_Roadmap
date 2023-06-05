# Lecture 3.1 - Learning the weights of a linear neuron



{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=11&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=Q0mTl9dQ4_I" %}

* similar to perceptron, except the outputs are always getting closer to the target outputs&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.42.29 PM.png" alt=""><figcaption></figcaption></figure>

* how can we show that the learning procedure makes progress? &#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.43.17 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.44.19 PM.png" alt=""><figcaption></figcaption></figure>

## Why don't we solve it analytically?&#x20;

1. We want a method that real neurons could use --> we want to make sure we understand this
2. We want a method that we can generalize for non-linear neural networks

## A toy example that illustrates the iterative method

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.56.43 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.57.17 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.57.38 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.58.01 PM.png" alt=""><figcaption><p>The residual error is the difference between our target and the estimate </p></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.59.19 PM.png" alt=""><figcaption></figcaption></figure>

## Deriving the Delta Rule

1. Define the error&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 3.59.51 PM.png" alt=""><figcaption></figcaption></figure>

2. Differentiate the error using the chain rule&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 4.00.13 PM.png" alt=""><figcaption></figcaption></figure>

3. The batch delta rule changes the weights in proportion to their error derivates summed over training classes

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 4.01.15 PM.png" alt=""><figcaption></figcaption></figure>

## Behavior of the iterative learning procedure

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 4.02.09 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-05 at 4.02.44 PM.png" alt=""><figcaption></figcaption></figure>

{% file src="../../.gitbook/assets/lec3.pdf" %}
