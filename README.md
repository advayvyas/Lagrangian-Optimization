# [A Lagrangian Approach to Loss Function Optimization on Traffic Network Regularity](https://ieeexplore.ieee.org/document/10534993)

This is the codebase for the aforementioned research project, complete with Jupyter notebooks and graph pickles.

## Abstract

The optimization of traffic, internet, and supply networks is a valuable tool for every major industry. The ability to optimize these networks is inherently difficult due to sheer scale, yet developing techniques at smaller scales with more feasible models can make the process more manageable. To develop our method to optimize irregularity on graphs, we constructed a method to randomly generate networks of various types by controlling the probability and distribution of node connections, including constant flow from the borders of the graph to introduce real-world complexity to the optimization problem. We developed a loss function that measured regularity and analyzed its convex gradient to create a minimization algorithm. Our novel solution to this problem was the use of Lagrange multipliers to solve for the absolute minima of the gradient, along a constraint. Through our methods, we managed to reduce irregularity by 31.3% in traffic networks. Our research will help industry and academia understand how to evaluate traffic networks through a computer-generated example and set up a framework for future research.
