# Everything you need to know about LSTM

## What is an LSTM model?
Long-short-term-memory (LSTM) models are a form of a **recurrent neural network (RNN)**
## What you need to know before I explain RNN and LSTM
neurons:
* neurons act as storers of data - they store the data and pass/recieve data between themselves
* the neuron is also responsible for deriving the inputs and producing an output
input:
* the input is simply the data that we run through the neurons - in our case, the data would be stock prices
output:
* the output is the one answer for the input
input/output relationship:
* there is only one output for every one input - often referred as the input-output pair
batch:
* a batch is how many input-output pairs are run through the network in one single pass through
epoch:
* how many times a batch is run forwards and backwards through the neural network
**back propagation**
* this is what makes RNN's so unique. To put this into terms we understand already, take a Monte Carlo for example: a monte carlo is another way of "forecasting" data points, but in order to do so, the simulation runs every possible scenario in order to find what is most likely to happen. An RNN takes a batch, runs it though its neural network, finds the results from each neuron, then passes it back through the network. By doing this, the network can discover which neurons are the most error prone and weight the next run-through accordingly. The output is then simplified, in a way, from a Monte Carlo in the sense that it has already accounted for any error or things outside the normal standard deviation and returns the one most likely point instead of all possible points.

## RNN main points
RNN purpose:
* RNN's are good at modeling data that are in a sequence. They are most commonly used for handwriting or speech recognition software or to analyze data that is in a time-series
Why are RNN's good at that?
* due to their use of back propagation, RNN's can take sequential data and analyze them in a way that makes the output error minimal. The reason the data must be sequential is due to its use of input-output pairs as well as back propagation. Using these allows it to test for correlation between older data and new data and use that to predict future data.

