---
layout: single
title: "LV1.직사각형 별찍기"
categories: Programmers
tags: [Coding_Test]
toc: true
toc_sticky: true
---
# 문제설명
이 문제에는 표준 입력으로 두 개의 정수 n과 m이 주어집니다.
별(*) 문자를 이용해 가로의 길이가 n, 세로의 길이가 m인 직사각형 형태를 출력해보세요.
# 제한조건
n과 m은 각각 1000 이하인 자연수입니다.
# 입출력 예시
입력  

5 3  

출력  

\*\*\*\*\*  
\*\*\*\*\*   
\*\*\*\*\*  

# 코드
~~~python
a, b = map(int, input().strip().split(' '))
answer = b*(a*'*' + '\n')
print(answer)
~~~

# 코드 설명
map(a, b)는 b를 모두 a처리 해주는 함수이다.
위 코드에선 입력값을 공백으로 나눠서 int형 변수로 형변환해주는 역할을 한다.
예시와 같은 출력을 얻기 위해서 string형 변수는 스칼라 연산이 가능하다는 것이 핵심이다.
위 코드만이 정답이 아니며 print()함수의 특성을 이용해서 반복문으로 처리도 가능하다.