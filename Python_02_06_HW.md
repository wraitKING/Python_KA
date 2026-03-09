# Во всех работат используеться цикл FOR.
## Задание 1
...

sum1 = 0
for i in range(1012, 9639):
    if i % 7 == 0 and i % 10 == 1:
        sum1 += i
print("Задача 1:", sum1)  
...

## Задание 2
...

count2 = 0
for i in range(1125, 7857):
    if i % 3 == 0 and i % 7 != 0 and i % 5 != 0:
        count2 += 1
print("Задача 2:", count2)
...

## Задание 3
...

sum3 = 0
for i in range(100, 1000):
    s = str(i)
    if s == s [::-1]:
        sum3 += i
print("Задача 3:", sum3)
...

## Задание 4
...

N = int(input("Введите N: "))
K = int(input("Введите K: "))

current = 1
print("Задача 4:", end=" ")

for i in range(N):
    print(current, end=" ")
    current += K
...

## Задание 5
...

N = int(input("Введите N: "))

for x in range(0, N + 1):
    y = x * x + 5 * x - 7
    print(y, end=" ")
...

## Задание 6
...

N = int(input("Введите количество чисел: "))

total = 0

for i in range(N):
    num = int(input())
    if 100 <= num <= 999 and num % 7 == 0:
        total += num
print(total)
...

## Задание 7
...

N = int(input("Введите количество чисел: "))

max_num = 0

for i in range(N):
    num = int(input())
    if num % 7 == 0 and num % 9 != 0:
        if num > max_num:
            max_num = num
...

## Задание 8
...

N = int(input("Введите количество чисел: "))

min_num = 1000

for i in range(N):
    num = int(input())
    if 10 <= num <= 99:
        oct_num = oct(num)[2:]
        if oct_num.endswith("3"):
            min_num = num
...

## Задание 8
...

N = int(input("Введите N: "))

for i in range(1, N + 1):
    print(i, N - i + 1)
...

## Задание 9
...

N = int(input("Введите число: "))

is_prime = True

if N < 2:
    is_prime = False
else:
    for i in range(2, N):
        if N % i == 0:
            is_prime = False
            break
if is_prime:
    print("Простое")
else:
    print("Не простое")
...

## Задание 10
...

N = int(input("Введите N: "))

value = 1

for i in range(N):
    print(value, end=" ")
    value = value / 2
