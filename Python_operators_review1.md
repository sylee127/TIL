# Python

## operators review1

```
print(2**7)

x = 3
y = 3*x**2 + 7*x + 9
print(y)

print(2**1/2)
print(2**(1/2))

# -----------------------------------
seconds = 1000
minutes = 1000//60
remainder = 1000%60
print("%d분 %d초" %(minutes,remainder))

# -----------------------------------
# 현금이 5,000원이 있고, 사탕 가격이 120원인 경우
# 최대한 살 수 있는 사탕의 개수와 나머지 돈은 얼마인가?

balance = 5000
candy = 120

candies = balance//candy
change = balance%candy

print("사탕 %d 개를 사고 남은 돈 : %d원" %(candies,change))

# -----------------------------------
b = 3
a = b
print(a)

a = a+1 ; a += 1
a = a-1 ; a -= 1

# 연습1
x =3
y = x**3 + 3*x**2 + 7*x + 10
print(y)

# -----------------------------------
result = 100 > 10
print(result)

x = 200
y = 200
result = x == y
print(result)

result = (x != y)
print(result)

# -----------------------------------
a = 15
print((a>=10) and (a<=20))
print((a%3==0) or (a%5==0))
print(not(a==100))
```