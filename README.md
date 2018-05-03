EE 511 Simulation Methods for Stochastic Systems Project #2: Random Number Generation
------------------------
[Networking Again]
---------------------
Note: you need a network/graph plotter e.g. networkx (python) and igraph (R)
Given n=50 people in a social network. Suppose any given unordered pair of two people are
connected at random and independently with probability p
 Generate and plot three network samples for each value of p in {0.02, 0.09, 0.12}.
Briefly discuss the structure of these sample graphs.
 Count the number of connections each vertex or node on a sample graph from the
previous question. This statistic is the degree of the vertex. Plot a histogram of the
vertex degrees for each of your sample graphs.
 Vertex degree is supposedly binomially distributed for small network sizes.
Generate a network with (n, p) = (100, 0.06) and plot a histogram of the vertex
degrees. Does you histogram support the binomial distribution assumption?
[Waiting]
-----------
 Use the inverse CDF method to generate 1000 independent samples, Xi, of the exponential
random variable with an average waiting time of 0.2 time units. Evaluate the quality of your
RNG with goodness of fit tests.
 Each exponential random sample represents the waiting time until an event occurs. Implement a
routine to count the number of exponentially-distributed time intervals that occur in 1 time unit.
Generate such counts for 1000 separate unit time intervals. How are these counts distributed?
Justify your answer
[Double Rejection]
---------------------
The random variable X has a bimodal distribution made up of an equally weighted, convex summation of
a beta and a triangle distribution:
f ( x )={0.5×Beta(8,5) ,0<x≤ 1
0.5×( x−4) , 4<x ≤5
−0.5×( x−6) ,5< x≤ 6
0,else
Implement rejection sampling routines for X. Generate 1000 samples of the random variable using each
envelope. Track the rejection rate of your rejection sampling RNGs. The rejection rate is the average
number of rejected candidates per sample. This is a measure of the efficiency of your RNG.
Turn in:
- A summary of your experiments including any relevant plots and relevant tables
- brief discussions of the results
- a print out of your code (or a link to your github repo).
