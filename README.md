
n = int(input())

son = 1
count = 0

while count < n:
    temp = son
    yigindi = 0

    while temp > 0:
        yigindi += temp % 10
        temp //= 10

    kvadrat = yigindi ** 2

    if son % kvadrat == 0:
        count += 1

    if count == n:
        print(son)

    son += 1
