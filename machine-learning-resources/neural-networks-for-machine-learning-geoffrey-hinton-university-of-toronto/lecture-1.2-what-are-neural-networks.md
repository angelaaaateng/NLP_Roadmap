# Lecture 1.2 - What are neural networks?

## Reasons to study neural computation:&#x20;

* to understand how the brain actually works
* to understand a style of parallel computations inspired by neurons and their adaptive connections
* to solve practical problems by using novel learning algorithms inspired by the brain (even if this isn't actually how the brain works)&#x20;

## A typical cortical neuron

* gross physical structure:&#x20;
  * axon that branches
  * dendritic tree that collects input from other neurons
* &#x20;axons typically contact dendritic trees at synapses
* spike generation
  * axon hillock
*   Synapses

    * when a spike of actvity arrives at an axon, these vesicles migrate to the surface and release chemicals
    * transmitter molecules diffuse across the synaptic cleft and bind to receptor molecules&#x20;

    <div align="center">

    <figure><img src="../../.gitbook/assets/Screen Shot 2023-05-09 at 4.56.26 PM.png" alt=""><figcaption><p>Cortical Neuron</p></figcaption></figure>

    </div>
* Synapses _adapt_, and that's most of what learning is&#x20;
  * the effectiveness of a synapse can be changed
  * synapses are slow, but they have advantages over RAM on a computer
    * small and low power
    * they can adapt using locally available signals

## How the brain works:

* each neuron receives inputs from other neurons
* the effect of each input line on the neuron is controlled by a synaptic weight
* the synaptic weights adapt so that the whole network learns to perform useful computations

## Modularity and the brain:&#x20;

* different parts of the cortex do different things
* the cortex is made of general purpose stuff that has the ability to turn into special purpose hardware in response to experience

