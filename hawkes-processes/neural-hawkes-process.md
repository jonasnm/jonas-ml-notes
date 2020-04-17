# Neural Hawkes process for SSI?
I have a random comment I forgot to mention in the meeting: I have been
thinking that a point process could be a good fit for the SSI problem.
In short this is a continuous time process that is exited by a discrete
process. This can be suited to fit missing data problems as well. The
paper 
Mei and Eisner Nips 2017, https://arxiv.org/pdf/1612.09328.pdf creates a
modified Hawkes process with a continuous time LSTM. The idea is that a
surgery excites the patient state and we will try to predict the next
discrete event based on this. 


The focus is on discrete events in continuous time?

A Hawkes process (Hawkes, 1971; Liniger, 2009) supposes that past events
can temporarily raise the probability of future events, assuming that
such excitation is ① positive, ② additive over the past events, and ③
exponentially decaying with time.

Real world patterns does not always follow these asumptions.


Adds stuff to handle missing data.



