# Python

## data_type review1 

```
num = 100
print("num:", type(num))

PI = 3.14
print("PI:", type(PI))

name = "홍길동"
print("name:", type(name))

done = True
print("done:", type(done))

a = 100 #class int
b = 'hello' #class str
print('age:', type(a))
print('word:', type(b))

###################################
print("나는 현재 " + "23" +"살 입니다")
print("나는 현재 " + str(23) +"살 입니다")

print("나는 현재 " + str(169.5) + "cm 입니다")

###################################
# --------- 사용자로부터 숫자를 입력받아 100과 더한 결과를 출력하는 프로그램
# 사용자로부터 키보드를 이용해서 값을 입력받기 : input() - 컴퓨터는 사용자 입력을 대기하는 상태가 됨)
# 키보드로 입력되는 모든 데이터는 문자열로 입력이 됨
# 키보드로 입력되는 숫자 데이터로 처리하고자 할때는 형변환을 진행해야 함

# num = input("숫자를 입력하세요 : ")
# print(int(num)+ 100)
#
# num = int(input('100과 더할 값을 입력하세요 : '))
# print(num+100)

## 실수 입력
# x = input("실수 입력 : ")
# x = 'a'
# y = x*3
# print(y)

# x = float(input('실수 입력 : '))
# y = x*3
# print(y)
#
# print(int(3.57483))
#
# ################################### >> 03_input()부터 ~~
# x = int(input("숫자 1 입력(정수만 입력하세요) : "))
# y = float(input("숫자 2 입력 : "))
# z = eval(input("숫자 3 입력 : "))
#
# print(z)
#
# a = eval(input('수식입력 : '))
# print(a)
# print(type(a))
#

# 연습1
# a = eval(input('국어 점수 입력 : '))
# b = eval(input('영어 점수 입력 : '))
# c = eval(input('수학 점수 입력 : '))
#
# total = a + b + c
# avg = total/3
#
# print("총점 : ", total)
# print("평균 : %.2f" %avg)

# 연습2
# weight = eval(input(("몸무게(킬로그램): ")))
# height = eval(input("키(미터): "))
#
# bmi = weight/(height**2)
#
# print("당신의 BMI : %.2f" %bmi)

# 연습3

x = eval(input('예금액 입력 : '))
y = eval(input('이자율 입력(%) : '))
interest = int(x * y / 100)
deposit = x + interest
print('---------------------------')
print('예금액 : %d 원' %x)
print('이자율 : %.1f %%' %y)
print('예금이자 : %d 원' %interest)
print('잔액 : %d 원' %deposit)
print('---------------------------')
print('예금액 : %s 원' %format(x,','))
print('이자율 : %.1f %%' %y)
print('예금이자 : %s 원' %format(int(interest), ','))
print('잔액 : %s 원' %format(int(deposit), ','))
```