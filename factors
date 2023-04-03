#!/usr/bin/python3
"""Module that factorizes natural numbers into products of two smaller numbers"""
import sys

def factorize(n):
    """Prints the factorization of n, if possible"""
    factors = []
    for i in range(2, n):
        if n % i == 0:
            factors.append(i)
            factors.append(n // i)
            break
    if factors:
        factors.sort()
        print(f"{n}={factors[0]}*{factors[1]}")

if len(sys.argv) != 2:
    print("Usage: factors <file>")
    print("where <file> is a file containing natural numbers to factor")
    sys.exit(1)

with open(sys.argv[1]) as file:
    for line in file:
        n = int(line.strip())
        factorize(n)
