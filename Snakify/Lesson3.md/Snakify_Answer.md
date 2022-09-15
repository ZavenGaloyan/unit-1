```.py
Is positive
a = int(input())
if a > 0 :
    print("YES")
else:
    print("NO")
    
Is odd
a =  int(input())
if a/2 > a//2:
    print("YES")
else:
    print("NO")
Is even
a = int(input())
if a % 2 == 0:
    print('YES')
else:
    print('NO')
    
Ends on seven
a = int(input())
if a%10 == 7:
    print("YES")
else:
    print("NO")

Minimum of two numbers
a = int(input())
b = int(input())
if a > b:
    print(b)
else:
    print(a)
    
Are both odd
a = int(input())
b = int(input())
if a/2 > a//2 and b/2 > b//2:
    print("YES")
else:
    print("NO")

At least one odd
a = int(input())
b = int(input())
if a/2 > a//2 or b/2 > b//2:
    print("YES")
else:
    print("NO")
   
Exactly one odd
a = int(input())
b = int(input())
if a % 2 == 1 and b % 2 == 0 or a % 2 == 0 and b % 2 == 1:
    print('YES')
else:
    print('NO')
    
Sign function
x = int(input())
if x > 0:
    print("1") 
elif x < 0:
    print("-1")   
elif x == 0:
    print("0")
    
Numbers in ascending order
a = int(input())
b = int(input())
c = int(input())
if c > b > a:
    print("YES")
else:
    print("NO")

Is three digit
a = int(input())
if a >= 100 and a < 1000:
    print("YES")
else:
    print("NO")
    
Minimum of three numbers
a = int(input())
b = int(input())
c = int(input()) 

if a >= b <= c:
    print(b)
elif b >= a <= c:
    print(a)
else:
    print(c)    
    
 Equal numbers
 a = int(input())
b = int(input())
c = int(input()) 
if a == b == c:
    print(3)
elif a == b or a == c or b==c:
    print(2)
elif a != b or a != c or b!=c:
    print(0)
    
Rook move
x1 = int(input())
y1= int(input())
x2= int(input())
y2 = int(input())

if x1 == x2 or y1 == y2:
    print("YES")
else:
    print("NO")   

Chess board - black square
x1 = int(input())
y1 = int(input())
if (x1 + y1) % 2 == 0:
    print("BLACK")
else:
    print("WHITE")
    
Chess board - same color
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if (x1 + y1 + x2 + y2)%2 == 0:
    print("YES")
else:
    print("NO")
    
 Distance to closest point
dis_1 = int(input())
dis_2 = int(input())
dis_3 = int(input())
if abs(dis_1-dis_2) <= abs(dis_1-dis_3):
    print(abs(dis_1-dis_2))
else:
    print(abs(dis_1-dis_3))
 
Digits in ascending order
a = int(input())
b = a//100
c = a//10%10
d = a%10
if d > c > b:
    print("YES")
else:
    print("NO")
    
  Four-digit palindrome 
a = int(input())
thou = a//1000
hund = a//100%10
tens = a//10%10
ones = a%10
if thou == ones and hund == tens:
    print("YES")
else:
    print("NO")   
    
 King move  
a = int(input())
b = int(input())
c = int(input())
d = int(input())
if (abs(a-c) <= 1) and (abs(b-d) <= 1):
    print("YES")
else:
    print("NO")  
    
 Bishop moves  
 x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 - x2 == y1 - y2 or x1 - x2 == y2 - y1:
    print('YES')
else:
    print('NO')  
    
   Queen move
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
if x1 - x2 == y1 - y2 or x1 - x2 == y2 - y1 or x1 == x2 or y1 == y2:
    print('YES')
else:
    print('NO')
    
  Index of outlier
a = int(input())
b = int(input())
c = int(input())
if a == c:
    print(2)
if b == c:
    print(1)
if a == b:
    print(3)
    
Knight move
x1 = int(input())
y1= int(input())
x2= int(input())
y2 = int(input())
z1 = abs(x1 - x2)
z2 = abs(y1 - y2)
if z1 == 1 and z2 == 2 or z1 == 2 and z2 == 1:
    print("YES")
else:
    print("NO")
    
 Chocolate bar
 n = int(input())
m = int(input())
k = int(input())
if k < n * m and ((k % n == 0) or (k % m == 0)):
    print('YES')
else:
    print('NO')
    
Leap Year    
 a =  float(input())

if a //4 == a/4 and a%100 != 0 or a%400 == 0:
    print("LEAP")
else:
    print("COMMON")   

Days in month
a = int(input())
if a == 1 or a == 3 or a == 5 or a == 7 or a == 8 or a == 12 or a == 10:
    print("31")
if a == 2 :
    print("28")    
if a == 4 or a == 6 or a == 9 or a == 11:
    print("30")    

Next day
m=int(input())
d=int(input())
if (m==12) and (d==31):
  m=1
  d=1
elif (m == 1 or m==3 or m==5 or m==7 or m==8 or m==10 or m==12) and (d==31):
  m=m+1
  d=1
elif m==2 and d==28:
  m=m+1
  d=1
elif (m==4 or m==6 or m==9 or m==11) and (d==30):
  m=m+1
  d=1
else :
  d=d+1
print(m)
print(d)

Linear equation
a = int(input())
b=  int(input())

if a == 0 and b != 0:
    print("no solution")
if a == 0 and b == 0:
    print ("many solutions")
elif b % a == 0:
    print(b//a)
else:
    print("no solution")
    
Vertices of rectangle
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
x3 = int(input())
y3 = int(input())
x4 = 0
y4 = 0 
if x1 == x2:
    x4 = x3
elif x2 == x3:
    x4 = x1
elif x1 == x3:
    x4 = x2
if y1 == y2:
    y4 = y3
elif y2 == y3:
    y4 = y1 
elif y1 == y3:
    y4 = y2
print(x4)
print(y4)

Sort three numbers
a = int(input())
b = int(input())
c = int(input())
if a >= b >= c:
    print(c)
    print(b)
    print(a)
elif b >= a >= c:
    print(c)
    print(a)
    print(b)
elif c > a > b:
    print(b)
    print(a)
    print(c)
elif c>= b >= a:
    print(a)
    print(b)
    print(c)
elif a>= c >= b:
    print(b)
    print(c)
    print(a)
elif b>= c >= a:
    print(a)
    print(c)
    print(b)
    
  White pawn move
x1 = int(input())
y1 = int(input())
x2 = int(input())
y2 = int(input())
xd = (x2-x1)
yd = y2 - y1

if y1 > 1 and (
    (xd == 0 and ((yd == 1) or (yd == 2 and y1 == 2))) or
    (abs(xd) == 1 and yd == 1)):
    print("YES")
else:
    print("NO")
    
    
    
