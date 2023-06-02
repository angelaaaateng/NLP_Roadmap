# Lecture 2.1 - Types of neural network architectures

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=6&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=l0foB9mUrc4" %}
An overview of the main types of neural network architecture&#x20;
{% endembed %}



* architecture: the way in which the neurons are connected together&#x20;
* Symmetrically connected network --> weights are the same&#x20;

## Feed-Forward Neural Networks&#x20;

* most common type of neural network in practice&#x20;
* compute transformations between input and output --> each layer, you get a new representation of the output

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 1.55.56 PM.png" alt=""><figcaption></figcaption></figure>

## Recurrent Networks

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 1.56.42 PM.png" alt=""><figcaption><p>Recurrent Neural Networks</p></figcaption></figure>

*   these NNs are a natural way to model sequential data

    * at each time step, the states of each time step determine the states of the following time step&#x20;
    * Note that we use the same weights at every time step&#x20;
    * they can remember information in their hidden state for a long time



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 1.58.12 PM.png" alt=""><figcaption></figcaption></figure>
* Examples of what RNNs can do:&#x20;
  * Ilya Sutskever (2011)&#x20;
    * trained a special type of RNN to predict the next character in a sequence
    * after training, one way of seeing how well it can do is to see if it assigns a high probabilty to the next character that actually occurs
    *   you can also use this to generate text&#x20;

        * generates by predicting the probability distribution for the next character and then sampling a character from this distribution (trained on Wikipedia)



        <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 2.00.44 PM.png" alt=""><figcaption><p>An example of the output by Ilya</p></figcaption></figure>



## Symmetrically Connected Networks&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 2.03.35 PM.png" alt=""><figcaption></figcaption></figure>
