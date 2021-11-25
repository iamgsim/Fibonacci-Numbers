# Fibonacci-Numbers

#Task : Create a list consisting of Fibonacci numbers from 1 to 55 using control flow statements.

def fibonacci_nums(n):
  if n <= 0:
    return [0]
  sequence = [1, 1]
  while len(sequence) <= n:
    next_value = sequence[len(sequence) - 1] + sequence[len(sequence) - 2]
    sequence.append(next_value)
  return sequence
print("fibonacci ==>", (fibonacci_nums(9)))
