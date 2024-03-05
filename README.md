# Ant-Hill-Problem

Coutesy: Optiver, leading proprietary trading firm

An ant leaves its anthill in order to forage for food. It moves with the speed of 10cm per second, but it doesn’t know where to go, therefore every second it moves randomly 10cm directly north, south, east or west with equal probability.

1. If the food is located on east-west lines 20cm to the north and 20cm to the south, as well as on north-south lines 20cm to the east and 20cm to the west from the anthill, how long will it take the ant to reach it on average?

    We do know that for 1-D random walk, mean position after starting from origin is 0, variance however goes as *(number of steps)^{-1/2}*. For 2-d random walks, the displacements are random variables with identical means of zero, and their difference is also a random variable. Averaging over this distribution, which has equally likely positive and negative values yields an expectation value of 0, so

 <|z|^2>=N. 	

The root-mean-square distance after N unit steps is therefore

 |z|_(rms)=sqrt(N), 	
 
so with a step size of l, this becomes

 d_(rms)=lsqrt(N). 	

In order to travel a distance d,

 N is approximately (d/l)^2. This is 4 in our test case and as we saw, mode in our simulation was 5, as we increase d, this should give us an estimate of where mode lies. 

3. What is the average time the ant will reach food if it is located only on a diagonal line passing through (10cm, 0cm) and (0cm, 10cm) points?
4. Can you write a program that comes up with an estimate of average time to find food for any closed boundary around the anthill? What would be the answer if food is located outside an area defined by ( (x – 2.5cm) / 30cm )2 + ( (y – 2.5cm) / 40cm )2 < 1 in coordinate system where the anthill is located at (x = 0cm, y = 0cm)?
