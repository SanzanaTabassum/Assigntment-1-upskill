
# Assignment 1: Big O notation plots

import numpy as np</br>
import matplotlib.pyplot as plt</br>
x = np.arange(0.01, 7, 0.05)</br>
y = (x\*\*2)</br>
z= (x\*\*3)</br>
a= (x\*\*4)</br>
b= np.log(x)</br>
fig, ax = plt.subplots()</br>
plt.plot(x,b, label= 'O(log n)')</br>
plt.plot(x,x, label= 'O(n)')</br>
plt.plot(x,y, label = 'O($n^2$)')</br>
plt.plot(x,z, label= 'O($n^3$)')</br>
plt.plot(x,a, label= 'O($n^k$)')</br>

plt.title('Big O Notation')</br>
plt.xlabel('n')</br>
plt.ylabel('y(n)')</br>

plt.ylim(0, 100)</br>
leg = ax.legend()</br>
plt.savefig('Big O notation.png', dpi=300)
plt.show()

![IBig O notation](https://dl.dropboxusercontent.com/s/x7ulhsk0aix0h1p/Big%20O%20notation.png?fbclid=IwAR1wHLeNH_m20aGpWLvGXlVRWQ61654l2BW_n6FW3aJ0Lw2CYW_sXBsXCtY)



# Caterogize from best to worst for n= 7 and k = 4

O(logn) > O(n) > O(n <sup> 2 </sup> ) > O( n <sup> 3 </sup>) > O(n<sup> k </sup>)
