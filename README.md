num = int(input("Enter a number: "))
original = num
total = 0

while num > 0:
    digit = num % 10

    fact = 1
    for i in range(1, digit + 1):
        fact = fact * i

    total = total + fact
    num = num // 10

if total == original:
    print("The given number is a Strong number")
else:
    print("The given number is not a Strong number")
