# Python

## for문 review1

```
# 01_for1
# for 문 : 정해진 횟수만큼 반복할 때 주로 사용
# 문법
# for 반복요소를 저장할 변수 in 반복을 위한 리스트 또는 범위 :
#   반복문장1
#   반복문장2...

# 리스트 ['홍길동','이몽룡','성춘향','변학도']의 요소를 모두 출력하시오
s_name = ['홍길동', '이몽룡', '성춘향', '변학도']

for a in s_name :
    print(a)

num = [1,2,3,4,5,6,7,8,9]
# 위 리스트의 요소들을 각각 출력하시오
for n in num :
    print(n)

# for num in num :
#   print(num)
# 결과는 잘 나옴 because 동일해보여도 파이썬 내부적으로는 다르게 생각하는 용어이므로!

# 위 리스트의 요소들을 한 라인에 출력하시오
print('===========================')
for n in num :
    print(n, end = '')

for num in num :
    print(num)

# ========================================
# 반복 범위 설정 : range()함수
# 특정 범위의 정수 생성
# range(start, stop, step)

# range(10) # start,step 생략 10개의 정수 0~9까지의 정수 (시작은 0)
# range(1,10) # step 생략 1에서 9까지의 정수 - start에서 stop-1까지의 정수
# range(1,10,2) # start 에서 stop-1까지 step 간격으로 정수 생성 - 1에서 9까지 2씩 건너뛰면서


print("================================")


# range(10) # start,step 생략 10개의 정수 0~9까지의 정수 (시작은 0)
for i in range(10) :
    print(i)

print("================================")
# range(1,10)
for i in range(1,10) :
    print(i)

print("================================")
for i in range(1,10,2) :
    print(i)

print("================================")
for i in range(11,21) :
    print(i)

print("================================")
for i in range(10,1,-1) :
    print(i)

# ========================================
# 02_list
# 리스트 생성 문법
# 리스트 식별자 = [요소값1, 요소값2, ... 요소값n]
# 리스트 크기는 가변적
# 다양한 종류의 데이터를 하나의 리스트에 저장 가능

scores = 100
print(scores)

scores = [100]
print(scores)

scores = [100, 200, 300, '인형']
print(scores)

print(scores[1])

test = ['연습', '시험']
print(test[0])

# ========================================
# 03_for_누적합

suma = 0
for a in range(1,11) :
    print(a)
    suma = suma + a
print('1부터 10까지 누적합 : ', suma)

# a가 1일때 suma는 0인 상태에서 suma = suma + a
# a가 2일때 suma는 1인 상태에서 suma = suma + a
# a가 3일때 suma는 3인 상태에서 suma = suma + a
# a가 4일때 suma는 6인 상태에서 suma = suma + a

suma = 0
## 1부터 100까지 더하는 프로그램을 작성하세요
for a in range(1,101) :
    print(a)
    suma = suma + a
    print('1부터 100까지 누적합 : ', suma)

# ========================================
# 04_for_구구단
# 구구단의 단수를 입력 받아서 해당 구구단을 출력하는 프로그램 작성
#
# 입력 양식
# 단 수 입력 : 7

# 출력 양식
dan = int(input('단 수 입력 : '))

for i in range(1, 10) :
    print('%d * %d = %d' %(dan, i, dan*i))

# ========================================
# 05_for_if
# 아래 리스트에 저장되어 있는 점수에 대하여 합격/불합격을 판별하는 프로그램을 작성
# 합격은 60점 이상으로 설정

# 출력양식
# 1번 90점 합격
# 2번 57점 불합격

scores = [90, 57, 88, 45, 78]

# for i in scores :
#     if i > 60 :
#         print('%점 합격' %i)
#     else :
#         print('%점 불합격' %i)

# 번호를 부착 해서 출력
number = 0
for i in scores :
    number = number + 1
    if i >= 60 :
        result = "합격"
    else :
        result = "불합격"
    print('%d번 %d점 %s' %(number, i, result))

# ========================================

# 07_for_명단확인
# 사용자가 입력한 이름이 명단리스트에 있는지 검색 후 결과를 출력

# 입력양식 :
# 이름 입력 : 홍길동

# 출력양식 :
# 명단에 있습니다 또는 명단에 없습니다

namelist = ['홍길동', '이몽룡', '성춘향', '변학도']

# 이름 입력
search_name = input('이름 입력 : ')

for name in namelist :
    if search_name == name :
        find = True
        break
    else :
        find = False

if find == True :
    print('명단에 있습니다')
else :
    print('명단에 없습니다')

# ========================================
# 08_중첩for
# 다중 for문 : for문 안에 for문을 포함하고 있는 문장

for y in range(3) :
    for x in range(5) :
        print(x, end ='')
    print()

# ========================================
# for_ex


for i in range(3, 21, 3) :
    print(i, end = '')


# ========================================
# for_ex1
n1 = eval(input('숫자1 입력 : '))
n2 = eval(input('숫자2 입력 : '))

if n1 > n2 :
    min = n2
    max = n1
else :
    min = n1
    max = n2

max = max + 1
sum = 0

for i in range(min, max) :
    sum += i

print("%d부터 %d까지의 합 : %d" %(min, max, sum))

# ========================================
# for_ex4
num = eval(input('시작 숫자를 입력하시오: '))

for i in range(num,0,-1) :
    print(i, end = '')
print('발사', end = '')

# ========================================
# for_ex5
# 변수를 다 따로 만들어서 1~12 값이 증가되게끔 누적변수를 만들어줘야 함
# for문 안에 for문을 넣기

a = 0
for i in range(1,13,1) :
    print(i)
    a += i
```