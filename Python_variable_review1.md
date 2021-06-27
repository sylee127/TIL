# Python 

## variable review1



```
result = 10
print(result)

result = "a"
print(result)

a, b, c, d = 1, 2, 3, 4
print(a)
print(b)
print(c)
print(d)

a, b, c, d = 1, 2, 3, 4
print(a, b, c, d)

a = b

a, b = 10, 20
a, b = b, a
print(a, b)

# -------------------------------------

# c_var = 100
# print(c_var)
# del c_var
# print(c_var)

name = '홍길동'
std_name = '김철수'
pro_name = "이몽룡'교수'"

print(name)
print(std_name)
print(pro_name)

print(name, std_name, pro_name)

address = '서울시 강남구'

print(name+"은 " + address + "에 삽니다.")

a = name + "은 " + address + "에 삽니다."
print(a)

age = 25

print(name + '은 ' + str(age) + '살 입니다.')
print(5+age)

w = 100
h = 200
a = w*h
print('면적 : ' + str(a))

print('면적 : ', a)

# -------------------------------------

name = '홍길동'
no = '2016001'
year = 4
grade = 'A'
average = 93.5
level = 10

print('성명 : ' + name)
print('학번 : ' + no)
print('학년 : ' + str(year))
print('학점 : ' + grade)
print('평균 : ' + str(average))
print('등급 : ' + str(level))

print('성명 : %s' % name)
print('학번 : %s' % no)
print('학년 : %d' %year)
print('학점 : %s' %grade)
print('평균 : %.1f' %average)
print('등급 : %d %%' %level)

# -------------------------------------

fTemp = 90
cTemp = (fTemp-32) * 5/9

print(cTemp)
print('%f' %cTemp)
print('%.3f' %cTemp)
print('%10.3f' %cTemp)
print('화씨온도 %d 를 섭씨온도로 변환하면 %.3f 입니다.' %(fTemp, cTemp))

# -------------------------------------

age = 25

print('내 나이는', age)

print('내 나이는', age, '살 입니다.')

print("내 나이는 %d 살 입니다." %age)

kor = 90
eng = 80
math = 80

total = kor + eng + math
average = total / 3
print('총점 : %d, 평균 : %.2f' %(total, average))

# -------------------------------------

# variable >> 06_constant 부터
PI = 3.141592
r = 10
area = r*r*PI

print(area)

# -------------------------------------
INT_RATE = 0.03
deposit = 10000
interest = deposit*INT_RATE
balance = deposit + interest

print(balance)
print(int(balance))
print(format(int(balance), ','))

INT_RATE = 0.04
deposit = 10000
interest = deposit*INT_RATE
balance = deposit + interest

print(balance)
print(int(balance))
print(format(int(balance), ','))

# -------------------------------------
# 정수
a = 0b1010
b = 300
c = 0o123
d = 0x12fc

print(a,b,c,d)

# 실수
f = 3.14
f1 = 1234.45
f2 = 1.234567e5

print(f,f1,f2)

# 문자열
char1 = 'A'
char2 = 'B'

print(char1, char2)

str1 = '홍길동'
str2 = 'Python'
str3 = """Python Programming"""
str4 = '''파이썬 프로그래밍'''

str5 = """ 여러줄로
나누어서
출력해도 됨"""

print(str5)

# 논리값/특수 리터럴
t = True
f = False

print(t,f)

val = None
val1 = ''
print(type(val), type(val1))

#########################################
# 한 줄의 코드를 여러줄에 나눠서 표현
'''
역슬래시(\) 또는
괄호() 사용
'''

a = 1+2+3+\
4+5+6

b = (1+2+3+\
     4+5+6)

print(a, b)

#################################
#print 함수를 이용해서 문자열을 출력하고자 할 때 여러행 입력

print("긴 문장을 입력할 때 중간에서 ~~~"
      "다음행으로 가고 자동 따옴표 처리되면서"
      " 1줄로 인식합니다")
print("긴 문장을 입력할 때 중간에서 ~~~ \n"
      "다음행으로 가고 자동 따옴표 처리되면서 \n"
      "1줄로 인식합니다")

print('한줄에') ; print('두개의 명령어')

#################################
print('first')
print("secon ")

print('first', end="")
print("second")

print('first', end="-")
print("secon ")
```