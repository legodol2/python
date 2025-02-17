# python
backjoon

''' 리스트 입출력
import sys
A,B = map(int,sys.stdin.readline().split())


list1=[]
list2= map(int, sys.stdin.readline().split())

for i in list2:

    if i < B:
        list1.append(i)


print(" ".join(map(str,list1)))


4153 직각삼각형 맞는지 아닌지
while True:
    a,b,c=map(int,input().split())
    if (a==0&b==0&c==0):
        break
    elif(a*a+c*c==b*b):
        print("right")
    elif(b*b+c*c==a*a):
        print("right")
    elif(a*a+b*b==c*c):
        print("right")
    else:
        print("wrong")
'''
'''
import math
num=int(input())

size=list(map(int,input().split()))
T,P = map(int,input().split())
sum2=0
sum=list()
for i in size:
    result= math.ceil(i//T)
    sum.append(result)
for s in sum:
    sum2=s+sum2

print(sum2)
