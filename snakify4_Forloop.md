#solution to snakify 4

#4-1
![](snakify4-1.jpeg)

'''.py

a = int(input())
b = int(input())

for i in range(a,b+1):
    print(i)
#print('end of the loop')

'''

#4-2
![](snakify4-2.jpeg)

'''.py
a = int(input())
b = int(input())

if a < b:
    for i in range(a,b+1,1):
        print(i)
else:
    for i in range(a,b-1,-1):
        print(i)
'''


#4-3
![](snakify4-3.jpeg)
'''.py
res = 0
for i in range(10):
    res += int(input())
print(res)

'''

#4-4
![](snakify4-4.jpeg)
'''.py
n = int(input("Type the number of lines you want to calculate"))
result = 0
for i in range (n):
    result += int(input())
print(result)
'''


#4-5
![](snakify4-5.jpeg)
'''.py
sum = 0
num = int(input())
for i in range(num):
    sum += (i+1)**3
print(sum)

'''

#4-6
![](snakify4-6.jpeg)
'''.py
sum = 1
n = int(input())
for i in range(1,n):
    sum *= (i+1)
print(sum)
'''

#4-7
![](snakify4-7.jpeg)
'''.py
sumofzero = 0
n = int(input())
for i in range(n):
    number = int(input())
    if number == 0 :
        sumofzero += 1

print(sumofzero)

'''

#4-8
![](snakify4-8.jpeg)
'''.py
factorial = 1
sum = 0
for i in range(1,int(input())+1):
    factorial *= (i)
    sum += factorial
print(sum)

'''
