# LFR Networks for Fake News Thesis

In this repository you'll find 100 Lancichinetti-Fortunato-Radicchi (LFR) networks used for a Thesis.

The networks, found in the folder `networks`, are in the format `gpickle` and where generated via the Python library [NetworkX](https://networkx.org/) using the generator algorithm [LFR_benchmark_graph](https://networkx.org/documentation/stable/reference/generated/networkx.generators.community.LFR_benchmark_graph.html).

The parameters for generating the networks were: 
| Parameter | Value  |
| --- | --- |
| n | 1000 |
| tau1 | 3 |
| tau2 | 2 |
| mu | 0.07 |
| average_degree | 5 |
| min_community | 50 |

The parameter `max_iters` was used but its value is unknown since this repository was done much later than the generation. The parameter `seed` was also used and its value is the name of each network file.

These parameters were chosen to generate networks where each community represents at least 5% of the network, communities are sparsely connected, and networks are scale-free. 

**Warning:** Some of these networks might not be connected (have nodes that don't have a path to every other node) due to nature of the LFR generation algorithm and the parameters chosen.