# Quadratic-Equation-Solver
Project: Quadratic Equation Solver

This Python program calculates the solutions of a quadratic equation using the quadratic formula.

Tools used:
- Python
- Thonny IDE

The user enters the values of a, b, and c, and the program calculates the possible values of x
import math


a = float(input("Enter a: "))
b = float(input("Enter b: "))
c = float(input("Enter c: "))

d = b**2 - 4*a*c

if d > 0:
    x1 = (-b + math.sqrt(d)) / (2*a)
    x2 = (-b - math.sqrt(d)) / (2*a)
    print("Two solutions:", x1, x2)

elif d == 0:
    x = -b / (2*a)
    print("One solution:", x)

else:
    print("No real solutions")
