# week-01
2021/03/25~2021/03/26

1. 산술연산자\
1.1 나누기 / : 7/3 = 2.33333333 > 실수형\
1.2 나누기// : 7/3 = 2 > 정수형\
1.3 제곱 : 2**2**2 = 16

*연습문제1
'아메리카노를많이많이많이좋아한다' 와 같은 출력값을 만들어보자

a = '아메리카노를'\
b = '좋아한다'\
c = '많이'\
sample = a + (c*3) + b\
print(sample) 

*연습문제2
좋아하는 음식 5개를 food라는 리스트에 담아보자
리스트 food의 가장 앞에 '파이썬'을, 가장 뒤에는 '집'이라는 단어가 오도록 수정하라
pop을 이용하여 파이썬을 삭제하라

food = ['딸기','바나나','사과','오렌지','배']\
#insert - 추가\
food.insert(0,'파이썬')\
food.insert(6,'집')

#remove - 제거\
food.remove('집')

#append - 추가\
food.append('집') #마지막 위치에 데이터 추가

#pop - 제거\
food.pop(0)
print(food)

*연습문제3
국어, 영어, 수학 점수가 키로 하는 딕셔너리를 만들어보자. 각각의 점수는 다음과 같다.\
국어:87, 영어:88, 수학:92\
점수의 평균을 구해보자

test = {'국어':87,'영어':88,'수학':92}\
print(test)

#key로 접근
avg_score = (test['국어']+test['영어']+test['수학'])/3\
print('평균점수:',avg_score)\
#get으로 접근
avg_score = (test.get('국어')+test.get('영어')+test.get('수학'))/3\
print('평균점수:',avg_score)


*연습문제4
a="20190505chicken19000"는 잘못 쓰여진 변수이다.
2019는 year변수에, 0505는 day변수에, chicken은 menu변수에, 19000을 money라는 변수에 인덱싱을 사용하여 각각 저장하고 출력하라

a="20190505chicken19000"\
year = a[:4]\
day = a[4:8]\
menu = a[8:15]\
money = a[15:]\
print('year:',year,'day:',day,'meny:',menu,'money:',money)
