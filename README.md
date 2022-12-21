# Get_airport_cost

# Question 

You are given a list of estimated connection costs between ‘n’ airports. Your job is to find the
minimum cost to connect these airports such that there is at least one path(direct or indirect)
between any two airports. If it is not possible to connect all airports in a way described above,
return -1. You can assume that airport names are always 1,2,3,4,. . . .,n in the input.

Input: n : integer = total number of airports

costs: list of lists. costs[i] = [airport_a, airport_b, cost_ab] = cost_ab is the connection cost
between given two airports( airport_a&airport_b). All numbers are integers.

Expected time complexity = Llog(n) where L = length of costs.

# Example 1:

n = 3, costs = [[1,2,4],[1,3,9],[2,3,7]]

output: 11

Airport 1 can be connected to 2 and 2 can be connected to 3. This way all airports
are connected (1 and 3 are indirectly connected through 2)
with minimum cost of connections 4+7 = 11

# Example 2:

n = 4, costs = [[1,2,3],[3,4,4]]

output = -1

It is not possible to connect
all airports in this case.
