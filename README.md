# RTOPDP

This repository contains the instances and results used in our paper "Robust Team Orienteering Problem with Decreasing Profits".

This paper studies a robust variant of the team orienteering problem with decreasing profits (TOP-DP),　where a fleet of vehicles are dispatched to serve customers with decreasing profits in a limited time horizon.　The service times at customers are assumed to be uncertain, which are characterized by a budgeted　uncertainty set. Our goal is to determine　the set of customers to be served and the vehicle routes such that　the collected profit is maximized; meanwhile, all the planned routes remain feasible for any realization of
service times within the uncertainty set.

## Instances
- [Instances](./Instances) includes all instances used in our paper. One can see the geographic distribution of customers, the number of custoemrs and the time horizon from the filename of each instance, for example, "C25_1" means that there are 25 customers that located in clusters, and the time horizon for each vehicle is the first quartile of all customers's deadline.
　
