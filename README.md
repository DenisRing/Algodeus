# ALGODEUS
##LINK TO ALGODEUS.MIDI 
https://onlinesequencer.net/706045

## DEPENDENCIES
There are some depencies needed to run these files, they are
* Tensorflow
* pandas
* numpy
* msgpack
* glob
* tqdm 

## INSTRUCTIONS
The ‘finished’ product is available in the uploaded files as Algodeus.midi, or can be listened to at the link above. Warning: Have the volume turned down low, it’s not pretty.
Otherwise: Run python2 rbm_chords.py to train the music contained in Mozart Samples. This will generate a collection of notes. Then run python2 merge_samples.py to create the midi called Algodeus.midi
TECHNICAL
This project uses Tensorflow to generate short samples of using using a Restricted Boltzmann Machine. RBMs are shallow, two-layer neural nets that constitute the building blocks of deep-belief networks. The first layer of the RBM is called the visible, or input, layer, and the second is the hidden layer.
 
Each circle in the graph above represents a neuron-like unit called a node, and nodes are simply where calculations take place. The nodes are connected to each other across layers, but no two nodes of the same layer are linked. That is, there is no intra-layer communication – this is the restriction in a restricted Boltzmann machine. Each node is a locus of computation that processes input, and begins by making stochastic decisions about whether to transmit that input or not. Gibbs sampling is using to create audio samples during training by randomly obtaining them from a generated probability distribution based on the inputs data.
The merging function is a simple script.

## FUTURE WORK
I don’t not have the time to fully dedicate to this project and so I’m unsatisfied with what I am submitting. This is something I hope to flesh out greatly soon, as in its current sense I see it as being in its Alpha State. Looking forward I hope to delve more into Long Short Term Memory networks and eventually Generative adversarial networks. As somewhat of a stepping stone to a more complete understanding of possibilities I am hoping to take apart the code behind DeepBach, a project which has successfully had a network generate baroque music nearly exactly the same as Johann Sebastian Bach.

## CREDIT
Credit for the original code goes to Dan Shiebler(dshieble) and to Siraj Raval (llSourcell) for the wrapper
