# Python

## if review1

```
# password = 1234
#
# # if password == 1234 :
# #     print("비밀번호가 일치합니다")
# #
# # print("끝")
#
# if password == 1234 :
#     print("비밀번호가 일치합니다")
# else :
#     print("비밀번호가 일치하지 않습니다 - else 문 내부")
#
# print("끝- if~else 문 밖입니다")
#
# if password == 12345 :
#     print("비밀번호가 일치합니다-if문 내부")
# else :
#     pass
#
# ########################################
# # 또 다른 조건이 있을 때 elif로 조건 추가 가능
# # if (조건식1) :
#     #조건식1이 참일경우 수행되는 문장
# # elif (조건식2) :
#     #조건식2가 참일경우 수행되는 문장
# # elif (조건식n) :
#     #조건식n이 참일경우 수행되는 문장
# # else :
#     #모든 조건식이 거짓일 경우 수행되는 문장
#
# num = int(input('정수 입력 : '))
#
# if num < 0 :
#     print("음수")
# elif num > 0 :
#     print("양수")
# else :
#     print("0")
#
# ########################################
# saveid = "flower"
# savepw = 1234
#
# id = input("아이디 입력 : ")
# pw = input("비밀번호 입력 : ")
#
# if (saveid == id) and (savepw == pw) :
#     print("로그인 성공")
# else :
#     print("로그인 실패")
#
# ########################################
#
# jumsu = eval(input("당신의 점수를 입력하세요 : "))
#
# if (jumsu >= 90) :
#     print("당신은 A 입니다")
# elif (jumsu >= 80) :
#     print("당신은 B 입니다")
# elif (jumsu >= 70) :
#     print("당신은 C 입니다")
# elif (jumsu >= 60) :
#     print("당신은 D 입니다")
# else :
#     print("당신은 F 입니다")

########################################
#
# w = eval(input('짐의 무게는 얼마입니까? '))
# if w > 20 :
#     print("무게 초과. 수수료 20,000원")
# else :
#     print("수수료 없음")
#
# print("종료합니다")

########################################

# a = eval(input('정수 입력 : '))
#
# if a % 2 == 0 :
#     print("짝수")
# else :
#     print("홀수")

########################################
#
# n1 = eval(input('정수1 입력 : '))
# n2 = eval(input('정수2 입력 : '))
# n3 = eval(input('정수3 입력 : '))
#
# if (n1 > n2) and (n2 > n3) :
#     print('제일  큰 수 : %d' %n1)
# elif (n1 < n2) and (n2 < n3) :
#     print('제일  큰 수 : %d' %n3)
# else :
#     print('제일  큰 수 : %d' %n2)

########################################

# figure = input('도형 입력(1: 사각형, 2: 삼각형, 3: 원) : ')
#
# if figure == '1' :
#     w = eval(input('가로 입력 : '))
#     l = eval(input('세로 입력 : '))
#     area = w*l
#     shape = '사각형'
# elif figure == '2' :
#     w = eval(input('밑변 입력 : '))
#     l = eval(input('높이 입력 : '))
#     area = w*l*0.5
#     shape = '삼각형'
# else :
#     r = eval(input('반지름 입력 : '))
#     area = 3.141592*r**2
#     shape = '원'
#
# print('%s의 면적 = %.2f' %(shape, area))

######################################## 7_중첩if부터~ (그전에 if_ex5다시해보기)

# figure = input("도형입력(1: 사각형, 2: 삼각형, 3: 원) : ")
#
# if figure == '1' :
#     w = eval(input('가로 입력 : '))
#     l = eval(input('세로 입력 : '))
#     area = w*l
#     shape = '사각형'
#
# elif figure == '2':
#     w = eval(input('밑변 입력 : '))
#     l = eval(input('높이 입력 : '))
#     area = w*l*0.5
#     shape = '삼각형'
# else :
#     r = eval(input('반지름 입력 : '))
#     area = 3.141592*r**2
#     shape = '원'
#
# print('%s의 면적 = %.2f' %(shape, area))

#########################################

# apple_quality = input('사과 상태 입력 : ')
#
# if apple_quality == '신선' :
#     apple_price = int(input('사과 가격 입력 : '))
#     if apple_price < 1000 :
#         print('10개를 산다')
#     else :
#         print('5개를 산다')
# else :
#     print('사과를 사지 않는다')

########################################
# num = int(input('번호 입력 (1. 현금, 2. 카드) : '))
#
# if num == 1 or num == 2 :
#     pay = int(input('지불액 입력 : '))
#     if num == 1 :
#         print('할인율 : 10%')
#         print('할인액 : %d' % (int(pay*0.1)) + '원')
#     else :
#         print('할인율 : 5%')
#         print('할인액 : %d' % (int(pay*0.05)) + '원')
#
# else :
#     print('잘못 입력했습니다. 종료 합니다')

########################################
# hong = input('홍길동 입력 : ')
# lee = input('이몽룡 입력 : ')
#
# if (hong == '가위' and lee == '보') or (hong == '바위' and lee == '가위') or (hong == '보' and lee == '바위') :
#     print('홍길동이 이겼습니다')
# elif hong == lee :
#     print('비겼습니다')
# else :
#     print('이몽룡이 이겼습니다')

########################################

# from random import randint
# n = randint(1,5)
# print(n)
#
# from random import randint
# n = randint(1,3)
#
# if n == 1 :
#     lee = '가위'
# elif n == 2 :
#     lee = '바위'
# else :
#     lee = '보'
#
# hong = input('홍길동 입력 : ')
#
# if (hong == '가위' and lee == '보') or (hong == '바위' and lee == '가위') or (hong == '보 and lee == '바위') :
#     print('홍길동님이 이겼습니다')
# elif hong == lee :
#     print('비겼습니다')
# else :
#     print('컴퓨터가 이겼습니다')

########################################

# if_ex6

lap = 1200000
cam = 400000

print('**********상품 정보**********')
print('1 노트북 : %d 원' %format(eval(lap), ','))
print('2 디지털카메라 : %d 원' %format(eval(cam), ','))
print('***************************')

no = eval(input('상품번호 입력 : '))

if no == 1 or no == 2 :
    num = eval(input('주문 수량 입력 : '))
    if no == 1 :
        product = '노트북'
        product_price = lap
        price = lap * num
        if price >= 1000000 :
            dc = 0.1 * price
        elif price >= 500000 :
            dc = 0.05 * price
        else :
            dc = 0
    else :
        product = '디지털카메라'
        product_price = cam
        price = cam * num
        if price >= 1000000 :
            dc = 0.1 * price
        elif price >= 500000 :
            dc = 0.05 * price
        else :
            dc = 0

    print('**********주문 내용**********')
    print('상품명 : %s' % product)
    print('가격 : %s 원' % format(product_price, ','))
    print('주문 수량 : %d' % num)
    print('주문액 : %s원' % format(price, ','))
    print('할인액 : %s원' % format(int(dc), ','))
    print('총지불액 : %s원' % format(int(price - dc), ','))


else :
    print('잘못 입력하였습니다. 종료합니다')
```