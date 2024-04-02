Exp 1: 
Mean and variance of a discrete distribution

Date:25.08.23

Aim :
To find mean and variance of arrival of objects from the feeder using probability distribution

Software required :
Python and Visual components tool

Theory:
The expectation or the mean of a discrete random variable is a weighted average of all possible values of the random variable. The weights are the probabilities associated with the corresponding values. It is calculated as,
![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/3386d678-2beb-4132-ae1b-1a72a34da5fe)


The variance of a random variable shows the variability or the scatterings of the random variables. It shows the distance of a random variable from its mean. It is calcualted as

![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/ce37dda9-c9b8-4a5b-895a-8a7020a56b7d)


Procedure :
Construct frequency distribution for the data

Find the probability distribution from frequency distribution.

Calculate mean using

![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/4eec41b8-d29e-4664-b01f-19208c53e818)


Find

![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/9f19fdb0-9056-4700-b323-ad1277cb1a58)


Calculate variance using

![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/108508f7-99c7-4386-9795-17a909df3b9a)


Experiment :
![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/94e08e17-78ed-47d7-a9fa-520d0eb59e59)


Program :
Developed by : M. GAYATHIRI ROSHINI
Register number : 212223110012
````
import numpy as np
L=[int(i) for i in input().split()]
N=len(L); M=max(L) 
x=list();f=list()
for i in range (M+1):
    c = 0
    for j in range(N):
        if L[j]==i:
            c=c+1
    f.append(c)
    x.append(i)
sf=np.sum(f)
p=list()
for i in range(M+1):
    p.append(f[i]/sf) 
mean=np.inner(x,p)
EX2=np.inner(np.square(x),p)
var=EX2-mean**2 
SD=np.sqrt(var)
print("The Mean arrival rate is %.3f "%mean)
print("The Variance of arrival from feeder is %.3f "%var) 
print("The Standard deviation of arrival from feeder is %.3F "%SD)
````
Output :
![image](https://github.com/23006823/Mean-and-Variance/assets/138971409/6d3f40c7-ab1b-4b8e-9634-fbd656d9bdd3)
Results :
The mean and variance of arrivals of objects from feeder using probability distribution are calculated.


