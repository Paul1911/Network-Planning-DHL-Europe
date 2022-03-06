# Project Modelling Ideas

Overall, we're minimizing cost.
Basically, for facilitation of the problem, I suggest a four step approach:
#### 1. Reduce freight volumes for air transport by using the Road Feeder Service (RFS) network. 
Trucking is nearly always cheaper than sending a plane. We truck directly whatever the time constrains allow to truck. The network is not optimized in this step yet.

#### 2. Aggregate remaining freight volumes to 'Business Centers' (Airports with greatest time constraints) wherever possible

#### 3. Optimize the air transport schedule. 
Also multileg flights are an option

#### 4. Optimize the RFS network
Look, which flying OnDs still have enough capacity to take further freight and make a direct road feeder unnecessary. 

#### Notes
For the flight cost calculation, we need to rely on an approximation as we used a separate program for the calculation of the cost. We have the exact cost for all flights to LEJ, but sometimes multileg flights make sense. In this case we have to rely on cost estimates for the second leg. I am currently solving this by a linear regression per A/C-type with distance as the dependent variable. 
The same applies to flight times.

The first point is solved, we have the distances and we truck whatever is possible. 
The next step would now be to check whether 2. and 3. can be combined and be formulated as a minimization problem.

I have not worked on this problem for a longer time, and it is also not high priority as this is more of an operations research problem. However I plan on coming back to it once I have a better foundation in Data Science & AI methods. 
