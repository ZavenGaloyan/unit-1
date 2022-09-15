
```.py
Last digit of integer
a = int(input())
print(a%10)

Two digits
a = int(input())
b = a%10
a = a//10
print(a,b)

Swap digits
a = int(input())
b = a%10
a = a//10
c = b*10+a
print(c)

Last two digits
a = int(input())
b = a%100
print(b)

Tens digit
a = int(input())
a = a%100
a= a//10
print(a)

Sum of digits
a = int(input())
b = a//100
c = a//10 % 10
d = a%10
z = c + b + d
print(z)

Reverse three digits
my_number = int(input())
print(str(my_number)[::-1])
 
Merge two numbers
num1 = int(input())
num2 = int(input())
print(str(num1)[0]+str(num2)[0]+str(num1)[1]+str(num2)[1])

Cyclic rotation
a = int(input())
tens_a = a // 100
units_a = a % 10
hundreds_a = a%100
print(hundreds_a*100+tens_a )

Fractional part
a = float(input())
print(float(a%1))

First digit after decimal point
num = float(input())
num_2 = float(num%1*10)
print(num_2//1)

Statement
import math 
num_1 = int(input())
num_2 = int(input())
b = num_2/num_1
print(math.ceil(b))

Day of week
k = int(input())
print((k + 3) % 7)

Digital clock
N = int(input())
hour = N // 60 
minute = N % 60
print(hour , minute)

Total cost
a = int(input())
b = int(input())
n = int(input())
total = n * (100 * a + b)
print(total // 100, total % 100)

Century
import math
num_1 = float(input())
num_1 = num_1/100
print(math.ceil(num_1))

Snail
from math import ceil
h = int(input())
a = int(input())
b = int(input())
print(ceil((h - a) / (a - b)) + 1)

Clock face - 1
h = int(input())
m = int(input())
s = int(input())

print(h * 30 + m * 30 / 60 + s * 30 / 3600)





