# RTOPDP

This repository contains the instances and results used in our paper "Robust Team Orienteering Problem with Decreasing Profits".

This paper studies a robust variant of the team orienteering problem with decreasing profits (TOP-DP), where a fleet of vehicles are dispatched to serve customers with decreasing profits in a limited time horizon. The service times at customers are assumed to be uncertain, which are characterized by a budgeted uncertainty set. Our goal is to determine the set of customers to be served and the vehicle routes such that the collected profit is maximized; meanwhile, all the planned routes remain feasible for any realization of
service times within the uncertainty set.

## Instances
- [Instances](./Instances) includes all instances used in our paper. One can see the geographic distribution of customers, the number of custoemrs and the time horizon from the filename of each instance, for example, "C25_1" means that there are 25 customers that located in clusters, and the time horizon for each vehicle is the first quartile of all customers's deadline.

- Instance file format:
  - All the networks are modified based on the [Solomon benchmark for the VRPTW](http://web.cba.neu.edu/~msolomon/problems.htm). 
  - C, R and RC refer to the cluster-located network, random-located network and a mixture of cluster-random located network.
  - The first node is considered as the starting depot as well as the ending depot.
  - 'DELAYRATIO' is rate that 'PROFIT' decreases linearly with the arrival time.
  
  ```
    <The number of nodes>
    XCOORD. YCOORD. PROFIT  DELAYRATIO  SERVICETIME SERVICETIME
    40	50	0	0.000	0	0
    45	68	10	0.027	70	70
    45	70	30	0.030	110	110
    ...    
  ```

## Results
- [Results](./Results) includes all results from three solution methods, i.e., CPLEX for solving the model directly, a branch-and-price (B&P) exact method and a tabu search (TS) heuristic method. All the three methods are set a computing time limit as one hour.

## Contact Info
Feel free to contact us for more information about our paper via email: 
 - Qinxiao Yu (yuqinxiao@tju.edu.cn), 
 - Chun Cheng (chun.cheng@polymtl.ca).
