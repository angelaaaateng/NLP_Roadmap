---
description: Notes from the book by Andrew Glassner
---

# A Visual Approach to Deep Learning Notes

The book can be bought [here](https://www.amazon.com/Deep-Learning-Approach-Andrew-Glassner/dp/1718500726)





Part I: Foundational Ideas&#x20;

1. An Overview of Machine Learning
2.
   1. Expert Systems&#x20;
   2.
      1. Popular approach to learning from data before deep learning
      2. Intended to encapsulate how human experts thing&#x20;
      3. Study a human at work, watch what they do, how they do it, and ask them to describe their process out loud → capture thinking via a set of rules&#x20;
      4. Difficult to create and maintain (feature engineering)
      5. Ex. Recognizing Digits&#x20;
      6.
         1. ![](https://lh6.googleusercontent.com/eLkop1q7l8e31Z9E9s3LDT2qnPJgFWxMjbE1mLEDlYREhpjsAYI\_5xS0Mpj45ZPu1uihLlfRoCQC7oYBmpxBO3fN4eEo5Sf380bYDg6gH0x1VNGz44nD9SPwTqKsP8\_w895SIYX9jH\_\_rAjDKhRD3lo)
         2. Rule-based expert systems can work sometimes, but it’s hard to come up with rules and generalize the rules, keep them up to date, etc also makes it impractical to maintain&#x20;
      7. Discovers decision-making rules by examining the input data and extracting patterns
      8. Measures patterns in training data then uses those patterns to evaluate new data → produces decision or result based on examples it’s trained on&#x20;
   3. Supervised Learning
   4.
      1. Labeled&#x20;
      2. Ex. Image classifier → image and label
      3. Training and prediction&#x20;
      4. In response to the image the classifier tells us the likelihood for each of the labels that it was trained to recognize&#x20;
      5. ![](https://lh6.googleusercontent.com/Pt8MVffr3aVcXNiEhc-EeRmVDGS7GV90-qJcz\_qvguOKH1eVTbIcGhMUG\_sciZuIynQUs0udK5mb07F5MKym4frAhuoheRhXhF6AIZ8xmJMu40tbTdQUMSZLwmo8nC2BqLH952nIHk4WHfqGOxyoUF4)
      6. &#x20;If the confidence isn’t reassuring, we could try a different algorithm or ask a human for help&#x20;
   5. Unsupervised Learning&#x20;
   6.
      1. No labels&#x20;
      2. Algorithms learn about relationships between elements of the input rather than between each input and a label&#x20;
      3. Frequently used for clustering related data&#x20;
      4. ![](https://lh3.googleusercontent.com/O1nOQoH0jeoTabkEGwUyuJ64lxtK1iyGBm1a\_XntiJeUN\_-8krv5ZaKftI2-F\_Jqh9cxAcSipvW5ol7PZ4F9HMvkqL7V1Z5VcbcY7k5zS9GQX8s4SjiLvmEVK\_MItZIXUnYgCQQ9G9jpiB5h2E5ugqY)
      5. Clustering algorithm&#x20;
      6. Can also be used to improve the quality of measured data or compress datasets
   7. Reinforcement Learning&#x20;
   8.
      1. Sometimes we want to train a model to perform a task but we don’t know the best way to do it ourselves
      2. Ex. Scheduling elevators &#x20;
      3. ![](https://lh4.googleusercontent.com/3HXg3TcxFzJkcMuryftpFEv1tiVdi9RoQXS0Ywxh6pnfCYLl0qfuXPdmnrO1hqhR4uNF8Sd8y6pwcu7ylK-KO-w7asRhd4b6kJMqZ2pl4NmSygec-GOBQQaqPEXcDJ2JhR6ZbFP872N7rxzyYRPH8kg)
      4. Try out different approaches over time and chose one that seems to be giving the best results
      5.
         1. \*i.e. This could be affected by seasonality&#x20;
      6. Computer can invent a policy, then give it a score based on performance&#x20;
      7. Try out different variations and pick the policy with the best score&#x20;
      8. As patterns change, try new approaches and keep the schedule with the best score&#x20;
   9. Deep Learning&#x20;
   10.
       1. Layers / steps of computation&#x20;
       2. Deep because of layers when drawn vertically and stacked&#x20;
       3. ![](https://lh4.googleusercontent.com/zjABD8vtwRt6lX-N55SAXvR0YiOnVwzcZFyy56P2a0EFmsqor\_HT07y2oJ\_BEuoSP6xZdBjTwUmWqnRx8wdd1pm2gMuWWumgWBKLO0YOdLIJiniEH5fHQO3\_0W6M919QhZmRvdp4ldK76Jg6ev7Nd9A)
       4. Layer = artificial neurons&#x20;
       5. Input = value of 4 pixels&#x20;
       6. Neuron - units that perform a tiny calculation&#x20;
       7. Each neuron in layer 1 gets one of the 4 starting numbers as input&#x20;
       8.
          1. Dot on the line represents weight&#x20;
       9. Output of each neuron is a new number which is fed into neurons in layer 2, and then multiplied by a weight along the way&#x20;
       10. The values produced by the 2 neurons in layer 2 are the final output of the network&#x20;
       11.
           1. Could interpret the output as the probability that the input is in each of the 2 classes&#x20;
       12. Each artificial neuron turns its input values into a number
       13.
           1. These computations are fixed&#x20;
           2. The only things that can change are the inputs and the weights&#x20;
           3. Weights are initialized randomly and adjusted over time&#x20;
       14. Training a network: finding values for the weights so that every input produces desired output&#x20;

\


2. Essential Statistics&#x20;
3.
   1. Goal: develop enough intuition and understanding to help us make good decisions when we do ML&#x20;
   2.
      1. Stats generally split into 2 categories:&#x20;
      2.
         1. Random numbers and how to describe them in ways that are of most value in ML&#x20;
         2. Ways we can choose objects from a collection and how to measure how well such selections represent the collection as a whole&#x20;
   3. Describing Randomness&#x20;
   4.
      1. Select a random number between a given min and max
      2. Average / mean&#x20;
      3.
         1. Median
         2. Mode&#x20;
   5. Random Variables and Probability Distributions
   6.
      1. ![](https://lh4.googleusercontent.com/92cgftcAAtIzDsYDZB\_ppt7qSxUsw3CWyLx0eD2S8M824sVed6HRlCToJyzm1pIPtBQW3LWuRgAayKicDQ60dAILpIfj22DsXiBDnDPGSnpxiFpA6V4a6UaOHQquajcEDqIf5ga1DUC930UEimwTIcU)
      2. ![](https://lh6.googleusercontent.com/ANNf3xPR4x\_dvqeLlk\_hnXevquo9u8d6uLmQCMek1xpwQnCd-lG8nkwnw\_lo7iS4PbvuUOQmu1npC24PtByUxO0l2MbCHQ-MrZzBM0ti6Htjn93qngGACWMfT575-FAU-Wq5tsccJTzAAGd8aMhCYJI)
      3. ![](https://lh3.googleusercontent.com/\_gQgC7ulih5szE8qIT9yD1msD54g8iwhXQKuGXnSWj5sEGpxN07rZtbi7Lku-ZMzH5KHjocLVZPi0jlVh9rS-7TeJtvdSiBeXdCJ6zxu0YNeTVMejiEziEZqGw\_PBUlqZhn4qXn7Cu1VXiUqPPiWj1A)
      4. Probability distribution
      5. Normalized version of the probability distribution&#x20;
      6. ![](https://lh5.googleusercontent.com/dW5Y6hLjcaqDGlHb90yqKxtKrWJP4oINJDK40c6GGrqZni59y8iF26MAxLpvNCibLasBl12Z1bavjdyCuIvP-c2daRbdgYAPBqm\_y3p0KurduA2iV4y4oG6orVFiiiqYp6v4R-eQvZxRYPmXPVaZPlQ)
      7. Random variable - picking a value at random from a list of options&#x20;
      8.
         1. A random variable is a function which takes a probability distribution as an input and produces a single value as an output&#x20;
         2. Drawing a value from the random variable&#x20;
      9. Probability mass function - finite number of possible return values&#x20;
      10.
          1. Discrete probability distribution&#x20;
      11. ![](https://lh5.googleusercontent.com/zsnlNSC\_s9W5pU7THF5sL\_gYikzxyBTlyw6T5Pv4R0kF0uc6tb59a6-BDPlTX\_DlCogssRmBjuQwpdyApyuFeeN718GBQcf6nbHZFjUa\_GV8prqUjMUyLBj54KNRFK4l6w4MlDd-nqDmzI0upUw8wJU)
      12. Continuous probability distribution / probability density function&#x20;
      13. Discrete - all possible return values need to add up to 1&#x20;
      14. Continuous - all the area under the curve adds up to 1
