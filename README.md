# python
5 Great Ways to Use Less-Conventional For Loops in Python
Simple techniques for avoiding basic looping, and creating faster algorithms

More on the for loop…


Before we dive into some awesome ways to not use for loop, let us take a look at solving some problems with for loops in Python. This will allow us to take note of how the loop is used in typical programming scenarios. Additionally, we can take a look at the performance problems that for loops can possibly cause. Let us take a look at the most traditional Pythonic for loop that many of us possibly learn when picking up the language:

data = [5, 10, 15, 20, 25, 30, 35, 40, 45, 50]
for i in data:
    print(i)
    
    
#for loop is expensive
  

# common for loop

from datetime import datetime
start_time = datetime.now()
# do your work here
p=[1,2,3,4,5,6,7,8,9,0]
for i in p:
    print(i)
end_time = datetime.now()
print('Duration: {}'.format(end_time - start_time))

executuion

1
2
3
4
5
6
7
8
9
0
Duration: 0:00:00.000174




#faster way  (onr line for loop)

    
#program



from datetime import datetime
start_time = datetime.now()
# do your work here
p=[1,2,3,4,5,6,7,8,9,0]
[print(i) for i in p]
end_time = datetime.now()
print('Duration: {}'.format(end_time - start_time))

execution

1
2
3
4
5
6
7
8
9
0
Duration: 0:00:00.000061





#by using while loop

from datetime import datetime
start_time = datetime.now()
# do your work here
p=[1,2,3,4,5,6,7,8,9,0]
i=0
while i<len(p):
    print(p[i])
    i=i+1
end_time = datetime.now()
print('Duration: {}'.format(end_time - start_time))


#execution

1
2
3
4
5
6
7
8
9
0
Duration: 0:00:00.000080



