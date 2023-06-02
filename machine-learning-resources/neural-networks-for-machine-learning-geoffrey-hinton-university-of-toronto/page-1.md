# Lecture 1.3 - Some simple models of neurons

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=3&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&t=6s&v=iKKfoP-naN8" %}

## Idealized Neurons&#x20;

* To model things we have to idealize them (i.e. atoms)&#x20;
  * we need to make simplifications to show how these might work&#x20;
  * idealization removes the complicated details that are not essential for understanding the main principles&#x20;
  * when we understand the basic principles, it's easier to add complexity
* It is often worth understanding models that are known to be wrong (but we must not forget that they're wrong)&#x20;

## Linear Neurons&#x20;

*   these are simple but computationally limited&#x20;

    * if we can make them learn, we may get insight into more complicated neurons
    * output as a function of bias, and the sum of all the activities on the neuron, times the weight



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.31.13 PM.png" alt=""><figcaption><p>Linear Neurons</p></figcaption></figure>

    &#x20;

    *   we can also plot this as a curve --> we get a straight line that goes through 0&#x20;

        <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.32.14 PM.png" alt=""><figcaption></figcaption></figure>

## Binary Threshold Neurons

*   McCulloch-Pitts (1943):

    * influenced Von Neumann&#x20;
    * 1\) Compute the weighted sum of the inputs&#x20;
    * 2\) Send out fixed size spike of activity if the weighted sum exceeds a threshold&#x20;
    * 3\) McCulloch and Pitts thought that each spike is like the truth value of a proposition and each neuron combines the truth values to compute the truth value of another propostion&#x20;
    * Logic was the main paradigm as to how the brain might work at that time&#x20;



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.35.55 PM.png" alt=""><figcaption><p>Binary Threshold Neuron</p></figcaption></figure>


* Ways to write the equation for a binary threshold neuron:&#x20;
  *

      <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.37.02 PM.png" alt=""><figcaption></figcaption></figure>

## Rectified Linear Neuron (Linear Threshold Neurons)&#x20;

* compute a linear weighted sum of their input
* output is a non-linear function of the total input&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.37.48 PM.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.38.37 PM.png" alt=""><figcaption></figcaption></figure>

* How do we make decisions at 0?&#x20;

## Sigmoid Neurons&#x20;

* probably the most common type of neuron to use&#x20;
*   these give a real-valued output that is a smooth and bounded fucntion of their total input

    * typically use the logistic function&#x20;



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.39.57 PM.png" alt=""><figcaption></figcaption></figure>

    * If the total input `z` is big and positive, then the output will be 1. If the total input is negative, then the output will be 0.



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.40.25 PM.png" alt=""><figcaption></figcaption></figure>

    * the sigmoid has smooth derivatives that are nicely behaved, which makes it easy to do learning

## Stochastic Binary Neurons&#x20;

* use the same equations as logistic units (compute total input the same way, and use the logistic function to compute a real value)
* But they treat the output of the logistic as the **probability** of producing a spike in a short time window (i.e. they don't output the probability directly)&#x20;
* They treat the _p_ as the probability of producing a 1, and not a real number&#x20;



<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.46.28 PM.png" alt=""><figcaption></figcaption></figure>

* we can do a similar trick for RELu:&#x20;
  * the output is treated as the Poisson rate for spikes&#x20;
  * \*random process (there is intrinsic randomness in the units which determines when the spikes are actually produced)

