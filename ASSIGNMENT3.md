1]INPUT:
a=float(input("enter first side:"))
b=float(input("enter second side:"))
c=float(input("enter third side:"))
if a>b and a>c:
    hypotenuse=a
    side1,side2=b,c
elif b>a and b>c:
    hypotenuse=b
    side1,side2=a,c
else:
    hypotenuse=c
    side1,side2=a,b

def check_right_triangle(hypotenuse,side1,side2):
    if hypotenuse**2==side1**2+side2**2:
        return True
    else:
        return False

if check_right_triangle(hypotenuse,side1,side2):
    print("The triangle is a right angled triangle")
else:
    print("the triangle is NOT a right angled triangle")

OUTPUT:
enter first side: 3
enter second side: 4
enter third side: 5
The triangle is a right angled triangle

2]INPUT:
def unique_prime_factors(n):
    factors=set()
    divisor=2
    while divisor<=n:
        while n%divisor==0:
            factors.add(divisor)
            n=n//divisor
        divisor+=1
    return sorted(factors)
num=int(input("Enter a number:"))
print(f"unique prime factors of {num}: {unique_prime_factors(num)}")

OUTPUT:
Enter a number: 56
unique prime factors of 56: [2, 7]

3]INPUT:
for num in range(1,101):
    if num%2==0:
        print(num)

OUTPUT:
2
4
6
8
10
12
14
16
18
20
22
24
26
28
30
32
34
36
38
40
42
44
46
48
50
52
54
56
58
60
62
64
66
68
70
72
74
76
78
80
82
84
86
88
90
92
94
96
98
100

4]INPUT:
import math
a = float(input("Enter coefficient a: "))
b = float(input("Enter coefficient b: "))
c = float(input("Enter coefficient c: "))
discriminant = b**2 - 4*a*c
if discriminant < 0:
    raise ValueError("math domain error")
root1 = (-b + math.sqrt(discriminant)) / (2 * a)
root2 = (-b - math.sqrt(discriminant)) / (2 * a)
print("the roots are", root1,root2)
OUTPUT:
enter coefficent a: 1
enter coefficent b: -5
Enter coefficient c: 6
the roots are: 3.0 2.0
