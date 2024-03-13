# maximum-word-frequency
#problem 3
#maximum word frequency
n=int(input())
d={}
for i in range(n):
  x=input()
  if x not in d:
    d[x]=1
  else:
    d[x]=d[x]+1
x=d.values()
m=max(x)
a=[]
for i in d:
  if d[i]==m:
    a.append(i)
print(max(a),m)
