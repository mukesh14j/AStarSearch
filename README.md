Sanjana is a lecturer working in a university at Bangalore. Due to Covid pandemic, she is
handling online classes from her native place, Mumbai. Since the situation is under control, the
government has removed the lockdown restrictions. The University management issued a
circular stating that all the lecturers has to handle the classes from the University. Now, she
needs to come back to the University.

However, due to a mass movement of public, all flights from Mumbai have been booked and
she is left with the only option of road transport. Matters have been further complicated by
some technical issue with Google maps making them unavailable for the time being.
Help her using your knowledge of informed search strategies. Create a search agent to find the
most optimal path to reach Bangalore. Below is a map of road connectivity between various
cities.

![image](https://user-images.githubusercontent.com/13768727/132235455-2358c0df-7b74-4c4b-aec5-c07fd507a663.png)


Solution:- 
A* is part of informed search technique and use heuristic values to solve the problem. The solution is guaranteed. A* always gives an optimal solution (shortest path with low cost) But it is not guaranteed to that AO* always provide an optimal solution. A* search finds the shortest path through a search space to goal state using heuristic function. This technique finds minimal cost solutions and is directed to a goal state called A* search.

![image](https://user-images.githubusercontent.com/13768727/132237091-cbd54233-3f1b-4978-8539-6ac1c7519258.png)

![image](https://user-images.githubusercontent.com/13768727/132237190-d912e000-50b4-47df-9883-ffc7735e8ade.png)

**Haversine Formula:
Haversine formula is used to find the shortest distance between two points on a sphere using their latitudes and longitudes.
In our case we use the Haversine formula to calculate the distance between two cities. Using the given latitude and longitude data for the cities, create a function which calculates the heuristic distance from each city to the destination city.

Haversine formula: a = sin²(Δφ/2) + cos φ1 ⋅ cos φ2 ⋅ sin²(Δλ/2) c = 2 ⋅ atan2( √a, √(1−a) )
d = R ⋅ c
where φ is latitude, λ is longitude, R is earth’s radius (mean radius = 6,371km); note that angles need to be in radians to pass to trig functions
