1]INPUT:
a=int(input("enter first number:"))
b=int(input("enter second number:"))
c=int(input("enter third number:"))

if a>b and a>c:
    largest=a
elif b>a and b>c:
    largest=b
else:
    largest=c

print("The largest numer is:", largest)

OUTPUT:
enter first number: 58
enter second number: 102
enter third number: 121212
The largest numer is: 121212

2]INPUT:
marks=float(input("Enter math marks:"))
if marks>=90:
    print("Grade: O")
elif marks>=80:
    print("Grade: A+")
elif marks>=70:
    print("Grade: A")
elif marks>=60:
    print("Grade: B")
elif marks>=50:
    print("Grade: C")
elif marks>=40:
    print("Grade: P")
else:
    print("Grade: F")

OUTPUT:
Enter math marks: 86
Grade: A+
