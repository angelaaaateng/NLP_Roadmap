---
description: My personal notes as I was reading the book by Andrew Glassner
---

# A Visual Approach to Deep Learning Notes

The book can be bought [here](https://www.amazon.com/Deep-Learning-Approach-Andrew-Glassner/dp/1718500726)

## Part I: Foundational Ideas&#x20;

## An Overview of Machine Learning

#### Expert Systems&#x20;

* Popular approach to learning from data before deep learning
* Intended to encapsulate how human experts thing&#x20;
* Study a human at work, watch what they do, how they do it, and ask them to describe their process out loud → capture thinking via a set of rules&#x20;
* Difficult to create and maintain (feature engineering)
* Ex. Recognizing Digits&#x20;

<figure><img src="https://lh6.googleusercontent.com/eLkop1q7l8e31Z9E9s3LDT2qnPJgFWxMjbE1mLEDlYREhpjsAYI_5xS0Mpj45ZPu1uihLlfRoCQC7oYBmpxBO3fN4eEo5Sf380bYDg6gH0x1VNGz44nD9SPwTqKsP8_w895SIYX9jH__rAjDKhRD3lo" alt=""><figcaption></figcaption></figure>

* Rule-based expert systems can work sometimes, but it’s hard to come up with rules and generalize the rules, keep them up to date, etc also makes it impractical to maintain&#x20;
* Discovers decision-making rules by examining the input data and extracting patterns
* Measures patterns in training data then uses those patterns to evaluate new data → produces decision or result based on examples it’s trained on&#x20;

### Supervised Learning

* Labeled&#x20;
* Ex. Image classifier → image and label
* Training and prediction&#x20;
* In response to the image the classifier tells us the likelihood for each of the labels that it was trained to recognize&#x20;

<figure><img src="https://lh6.googleusercontent.com/Pt8MVffr3aVcXNiEhc-EeRmVDGS7GV90-qJcz_qvguOKH1eVTbIcGhMUG_sciZuIynQUs0udK5mb07F5MKym4frAhuoheRhXhF6AIZ8xmJMu40tbTdQUMSZLwmo8nC2BqLH952nIHk4WHfqGOxyoUF4" alt=""><figcaption></figcaption></figure>

* &#x20;If the confidence isn’t reassuring, we could try a different algorithm or ask a human for help&#x20;

#### Unsupervised Learning&#x20;

* No labels&#x20;
* Algorithms learn about relationships between elements of the input rather than between each input and a label&#x20;
* Frequently used for clustering related data&#x20;

<figure><img src="https://lh3.googleusercontent.com/O1nOQoH0jeoTabkEGwUyuJ64lxtK1iyGBm1a_XntiJeUN_-8krv5ZaKftI2-F_Jqh9cxAcSipvW5ol7PZ4F9HMvkqL7V1Z5VcbcY7k5zS9GQX8s4SjiLvmEVK_MItZIXUnYgCQQ9G9jpiB5h2E5ugqY" alt=""><figcaption></figcaption></figure>

* Clustering algorithm&#x20;
* Can also be used to improve the quality of measured data or compress datasets

#### Reinforcement Learning&#x20;

* Sometimes we want to train a model to perform a task but we don’t know the best way to do it ourselves
* Ex. Scheduling elevators &#x20;

<figure><img src="https://lh4.googleusercontent.com/3HXg3TcxFzJkcMuryftpFEv1tiVdi9RoQXS0Ywxh6pnfCYLl0qfuXPdmnrO1hqhR4uNF8Sd8y6pwcu7ylK-KO-w7asRhd4b6kJMqZ2pl4NmSygec-GOBQQaqPEXcDJ2JhR6ZbFP872N7rxzyYRPH8kg" alt=""><figcaption></figcaption></figure>

* Try out different approaches over time and chose one that seems to be giving the best results
  * \*i.e. This could be affected by seasonality&#x20;
* Computer can invent a policy, then give it a score based on performance&#x20;
* Try out different variations and pick the policy with the best score&#x20;
* As patterns change, try new approaches and keep the schedule with the best score&#x20;

#### Deep Learning&#x20;

* Layers / steps of computation&#x20;
* Deep because of layers when drawn vertically and stacked&#x20;

<figure><img src="https://lh4.googleusercontent.com/zjABD8vtwRt6lX-N55SAXvR0YiOnVwzcZFyy56P2a0EFmsqor_HT07y2oJ_BEuoSP6xZdBjTwUmWqnRx8wdd1pm2gMuWWumgWBKLO0YOdLIJiniEH5fHQO3_0W6M919QhZmRvdp4ldK76Jg6ev7Nd9A" alt=""><figcaption></figcaption></figure>

* Layer = artificial neurons&#x20;
* Input = value of 4 pixels&#x20;
* Neuron - units that perform a tiny calculation&#x20;
* Each neuron in layer 1 gets one of the 4 starting numbers as input&#x20;
  * Dot on the line represents weight&#x20;
* Output of each neuron is a new number which is fed into neurons in layer 2, and then multiplied by a weight along the way&#x20;
* The values produced by the 2 neurons in layer 2 are the final output of the network&#x20;
  * Could interpret the output as the probability that the input is in each of the 2 classes&#x20;
* Each artificial neuron turns its input values into a number

1. These computations are fixed&#x20;
2. The only things that can change are the inputs and the weights&#x20;
3. Weights are initialized randomly and adjusted over time&#x20;

* Training a network: finding values for the weights so that every input produces desired output&#x20;
