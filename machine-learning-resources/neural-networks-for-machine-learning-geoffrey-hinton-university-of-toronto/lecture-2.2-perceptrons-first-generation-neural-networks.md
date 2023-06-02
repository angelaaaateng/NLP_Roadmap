# Lecture 2.2 - Perceptrons: First-generation neural networks

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=8&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=YRMvQuutgS8" %}

* investigated in the early 1960s, but fell into disfavor for a time because of their limitations

## The standard paradigm for statistical pattern recognition&#x20;

1. Convert the raw input vector into a vector of feature activations&#x20;
   * Use handwritten programs based on common sense to define the features
2. Learn how to weight each of the feature activations to get a single scalar quantity
   * The weights on the feature gives you how much evidence the feature gives you on the hypothesis that the current feature gives you the type of feature you want to recognize&#x20;
3. If this quantity is above some threshold, decide that the input vector is a positive example of the target class

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 3.32.44 PM.png" alt=""><figcaption></figcaption></figure>

* Perceptrons were popularized in the early 1960s by Rosenblatt --> very powerful learning algorithm&#x20;
  * people claimed that they could tell the difference between pictures of tanks and pictures of trucks, even if they were obscured in a forest --> some of these claims were proved false (sunny day vs cloudy day --> total intensity of the pixels)&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 3.36.21 PM.png" alt=""><figcaption></figcaption></figure>

## Binary threshold neurons (Decision units of the neural network)&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 3.37.15 PM.png" alt=""><figcaption></figcaption></figure>

## How to learn biases using the same rule as we use for learning weights&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 3.39.53 PM.png" alt=""><figcaption></figcaption></figure>

## The perceptron convergence procedure: training binary output neurons as classifiers&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 3.41.22 PM.png" alt=""><figcaption></figcaption></figure>
