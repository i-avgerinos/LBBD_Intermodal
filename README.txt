Instance_#.txt:		Lists of parameters for Instance #
J[j]:				ID of DC hub j
K[k]:				ID of Intermediate k
L[l]:				ID of Satellite hub l
I[i]:				ID of node i
N[n]:				ID of order n
demand[n]:			Quantity of order n
hub[n]:			Dedicated DC hub of order n
release[n]:			Release time of order n
Nj[j]:			Partition of set N into |J| subsets; if hub[n] = j, then n is subset Nj[j]
Gj[j]:			Partition of set G into |J| subsets
G[g]:				ID of compartment g
deadline[n]:		Deadline of order n (in hours)
weight[n]:			Weight of order n, multiplied by the number of days of delayed delivery to compute the respective penalty
q:				Capacity of compartments; identical for all g in G
M[m]:				ID of mode m; 0 for roadway, 1 for railway, 2 for seaway
M_description[m]:		Description of mode m
accessibility[i][m]:	Binary matrix, indicating whether node i is accessible by mode m
S[s]:				ID of intermodal service s
origin[s]:			Origin node of service s
destination[s]:		Destination node of service s
departure[s]:		Departure time of service s (in hours)
arrival[s]:			Arrival time of service s (in hours)
Q[s]:				Capacity of service s (in number of compartments)
cfixed[s]:			Fixed cost of service s
ctravel[s]:			Variable cost (cost per compartment) of service s
mode[s]:			Mode of service s
delivery_process[l]:	Indicating whether Satellite hub l complies with a Direct-Shipment or a Cross-Docking policy
distance_ln[l][n]:	Travel cost from Satellite hub l to delivery point n
distance_nn[n][m]:	Travel cost from delivery point n to delivery point m
vans[l]:			Number of available reusable vans in Satellite hub l
