print("---Number Guessing Game---")
import random
result = random.randint(1,100)
count = 0
while True:
    number = int(input("Enter a number: "))
    count += 1
    if number >= 0 and number <= 100:
        if number > result:
            print("Your number is too high!")
        elif number < result:
            print("Your number is too low!")
        elif number == result:
            print("---Your number is correct!---")
            print("---Your did it %d times---" % count)
            break
