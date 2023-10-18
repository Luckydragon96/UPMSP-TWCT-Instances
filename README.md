# UPMSP-TWCT-Instances

The benchmark is derived from the one originally proposed by Chen and Powell (1999) for the weighted completion time variant of unrelated parallel machine scheduling problems. 

*Chen Z-L, Powell WB (1999) Solving Parallel Machine Scheduling Problems by Column Generation. Informs J Comput 11:78–94. https://doi.org/10.1287/ijoc.11.1.78*

## Integer Processing Time Instances
The dataset comprises instances with $m = \{2,4,8,12,16,20\}$ and $n = \{20,30,40,60,80,100\}$. In these instances, processing times ($p_{jk}$) are integers drawn from a uniform distribution $U [1, 100]$, while weights ($w_j$) are generated using a uniform distribution $U [1, 30]$. 
To expand the benchmark, we have introduced larger-scale instances with $m = 20$ and $n = \{120,140,160,200\}$. We conduct extensive numerical experiments to obtain three types of instances, that is, **Instance 1** that can be solved without branching，**Instance 2** that can be solved with few branches, and **Instance 3** that can be solved with more branches.

## Fractional Processing Time Instances

We have also generated instances with fractional processing times, where $p_{jk}$ values are fractional and drawn from a uniform distribution $U [1, 100]$. Other settings are the same as for **Integer Processing Time Instances**。
