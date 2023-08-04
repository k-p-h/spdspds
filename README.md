# spdspds
spdspds 

This is the main paper containing the algorithm 'spdspds' (Symmetric Primal-Dual Symplex Pivot Decision Strategy). 
The classical Simplex Pivoting Operation of Dantzig is redefined here as 'symplex' 
which is a simple exchange between a basic (dependent) variable and a non-basic (independent) variable, 
in the Tucker’s Compact Symmetric Tableau (CST) which is a unique symmetric representation 
common to both the primal as well as the dual of a 
linear programming problem in its standard canonical form.
From this viewpoint, the classical simplex pivoting operation of Dantzig may be considered as a restricted special case. 

The infeasibility index associated with a symplex tableau is defined as the sum of the number of primal variables and the number of dual variables that are infeasible. 
A measure of goodness as a global effectiveness measure of a pivot selection is defined/determined as/by the decrease in the infeasibility index associated with such a pivot selection. 
At each iteration the selection of the symplex pivot element is governed by the anticipated decrease in the infeasibility index - 
seeking the best possible decrease in the infeasibility index - 
from among a wide range of candidate choices with non-zero values - 
limited only by considerations of potential numerical instability. 
The algorithm terminates when further reduction in the infeasibility index is not possible; 
then the tableau is checked for the terminal tableau type to facilitate the problem classification - 
a termination with an infeasibility index of zero indicates optimum solution. 
Even in the absence of an optimum solution, the versatility of the spdspds algorithm allows one to explore/determine the most suitable alternative solutions in a given context, 
including a comprehensive parametric analysis, etc. 
The worst case computational complexity of spdspds is shown to be O(L^1.5).
