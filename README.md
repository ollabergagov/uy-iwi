# uy-iwi
1.13

a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))

D = b*b - 4*a*c
if D > 0:
    x1 = (-b + math.sqrt(D)) / (2*a)
    x2 = (-b - math.sqrt(D)) / (2*a)
    print(x1, x2)
elif D == 0:
    x = -b / (2*a)
    print(x)
else:
    print("Haqiqiy ildiz yo‘q")

1.14
kg = float(input("Kg: "))
print("Funt:", kg * 2.20462)

funt = float(input("Funt: "))
print("Kg:", funt / 2.20462)

1.15 
pul = float(input("Boshlang‘ich pul: "))
foiz = float(input("Yillik foiz (%): "))

for i in range(5):
    pul += pul * foiz / 100

print("5 yildan keyin:", pul)

1.16 
n = int(input("3 xonali son: "))
print("Yuzlik:", n//100)
print("O‘nlik:", (n//10)%10)
print("Birlik:", n%10)

1.17 
soat = int(input("Soat: "))
daq = int(input("Daqiqa: "))

print("Jami minut:", soat*60 + daq)

1.18 3 ta sondan o‘rtacha
a = float(input())
b = float(input())
c = float(input())
print((a+b+c)/3)

1.19 
N = int(input("N: "))
print(N*(N+1)//2)

1.20 
for i in range(4):
    x = int(input())
    if x % 2 == 0:
        print(x)

1.21
n = int(input())
print("Kvadrat:", n**2)
print("Kub:", n**3)

1.22 
b1 = int(input())
b2 = int(input())
b3 = int(input())
print("O‘rtacha:", (b1+b2+b3)/3)

1.23 
import math
r = float(input("Radius: "))
print(2 * math.pi * r)

1.24 
v0 = float(input())
a = float(input())
t = float(input())

s = v0*t + (a*t*t)/2
print(s)

1.25 
a = float(input())
b = float(input())

print("Perimetr:", 2*(a+b))
print("Yuza:", a*b)

1.26
N = int(input("Sekund: "))

soat = (N // 3600) % 24
minut = (N % 3600) // 60

print(soat, ":", minut)

1.27 
n = int(input())
teskari = (n%10)*10 + n//10

if n == teskari:
    print("Teng")
else:
    print("Teng emas")

1.28 
n = int(input())
print(n % 4 == 0)

1.29 
n = int(input())
a = n//100
b = (n//10)%10
c = n%10

print(a < b < c)

1.30 
h1, m1 = map(int, input("1-vaqt (soat daqiqa): ").split())
h2, m2 = map(int, input("2-vaqt (soat daqiqa): ").split())

t1 = h1*60 + m1
t2 = h2*60 + m2

print("Farq (minut):", abs(t2 - t1))
