# Lecture 1.4 - A simple example of learning

{% embed url="https://www.youtube.com/watch?ab_channel=ColinReckons&index=4&list=PLoRl3Ht4JOcdU872GhiYWf6jwrk_SNhz9&v=RcgfwZ-FFBI" %}
Lecture 1d
{% endembed %}



## A very simple way to recognize handwritten shapes&#x20;

* consider a neural net with 2 layers of neurons&#x20;
  * neurons in the top layer represent known shapes
  * neurons in the bottom layer represent pixel intensities&#x20;
* if a pixel gets active: it votes for particular shapes&#x20;
  * a pixel gets to vote if it has ink on it
  * each inked pixel can vote for several different shapes&#x20;
* the shape that gets the most votes wins&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.50.58 PM.png" alt=""><figcaption></figcaption></figure>

## How to display the weights&#x20;

* we need to see the value and sizes of the weights&#x20;
* give each output unit its own "map" of the input image and display the weight coming from each pixel in the location of that pixel in the map
* black and white blob: area represents the magnitude, color represents the sign &#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.51.57 PM.png" alt=""><figcaption><p>Weight representation</p></figcaption></figure>

## How to learn the weights&#x20;

* Show the network an image and increment the weights from active pixels to the correct class&#x20;
* How do we keep the weights under control?&#x20;
  * decrement the weights from active pixels to whatever class the network guesses
  * train it to do the right thing rather than what it has the tendency to do&#x20;
*   show this a few hundred training examples and then look at the weights again

    * now they've started to form regular patterns&#x20;
    * now they have their future values --> the weights now look like little templates of the shapes



    <figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.55.12 PM.png" alt=""><figcaption><p>The learned weights</p></figcaption></figure>



## Why the simple learning algorithm is insufficient

* a two layer network with 1 winner in the top layer is equivalent to having a rigid tempalte for each shape&#x20;
  * the winner is the template that has the biggest overlap with the ink
* the ways in which handwritten digits vary are too complicated to be captured by simple template matches of whole shapes
  * to capture allowable variations of a digit, we need to learn all the **features** it is composed of&#x20;
  * look at the arrangements of the features&#x20;

<figure><img src="../../.gitbook/assets/Screen Shot 2023-06-02 at 12.57.14 PM.png" alt=""><figcaption></figcaption></figure>
