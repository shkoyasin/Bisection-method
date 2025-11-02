
# Bisection Method in Python

# Import necessary library
import math

# Define the function
def f(x):
    return x**3 - 7*x + 2   # Replace with your unique equation

# Bisection method function
def bisection(a, b, iterations):
    print(f"{'Iteration':^10} | {'a':^10} | {'b':^10} | {'c':^10} | {'f(c)':^12} | {'New Interval':^15}")
    print("-"*70)

    for i in range(1, iterations+1):
        c = (a + b)/2
        fc = f(c)

        # Determine new interval
        if f(a) * fc < 0:
            new_interval = f"[{a:.6f}, {c:.6f}]"
            b = c
        else:
            new_interval = f"[{c:.6f}, {b:.6f}]"
            a = c

        print(f"{i:^10} | {a:^10.6f} | {b:^10.6f} | {c:^10.6f} | {fc:^12.6f} | {new_interval:^15}")

    print("\nApproximate root after", iterations, "iterations:", c)

# Parameters
a = 1      # Start of interval
b = 3      # End of interval
iterations = 5  # Number of iterations

# Run Bisection Method
bisection(a, b, iterations)
