# Задача 12: Петя и Катя – брат и сестра. Петя – студент, а Катя – школьница. 
# Петя помогает Кате по математике. Он задумывает два натуральных числа X и Y (X,Y≤1000), а Катя должна их отгадать. 
# Для этого Петя делает две подсказки. Он называет сумму этих чисел S и их произведение P. 
# Помогите Кате отгадать задуманные Петей числа.

s1 = int(input("Введите первое число <= 1000 : "))
s2 = int(input("Введите второе число <= 1000 : "))
x = s1 + s2
print('x =',x)
if (x > 1000):
    print("число > 1000 введите новое:")
p1 = int(input("Введите первое число <= 1000 : "))
p2 = int(input("Введите второе число <= 1000 : "))
y = p1 * p2
print('y =',y)
if(y > 1000):
    print("число > 1000 введите новое:")




# Задача 10: На столе лежат n монеток. Некоторые из них лежат вверх решкой, а некоторые – гербом.
# Определите минимальное число монеток, которые нужно перевернуть, чтобы все монетки были повернуты
# вверх одной и той же стороной. Выведите минимальное количество монет, которые нужно перевернуть.

    
Coins = int(input("Введите количество монет N: "))
o = 0
r = 0
i = 0
for i in range(Coins):
    x = int(input("Орел(1) или решка(0)? "))
    if x == 1:
        o += 1
    else:
        r += 1
if o < r:
    print(f"Переверните {o} монет с орла на решку, их меньше всего")
elif o == r:
    print(f"Количество орлов и решек одинаково, по {o} штук")
else:
    print((f"Переверните {r} монет с решки на орла, их меньше всего"))




# Задача 14: Требуется вывести все целые степени двойки (т.е. числа вида 2k), не превосходящие числа N.

N = int(input("Введи число N:"))
i = 0
while 2 ** i <= N:
    print(f"числа вида 2к {i} равна {2 ** i}")
    i += 1
    



