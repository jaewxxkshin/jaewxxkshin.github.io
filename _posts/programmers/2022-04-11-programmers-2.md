---
layout: single
title: "LV1. x만큼 간격이 있는 n개의 숫자"
categories: Programmers
tags: [Coding_Test]
toc: true
toc_sticky: true
---
# 문제설명
함수 solution은 정수 x와 자연수 n을 입력 받아, x부터 시작해 x씩 증가하는 숫자를 n개 지니는 리스트를 리턴해야 합니다.  
다음 제한 조건을 보고, 조건을 만족하는 함수, solution을 완성해주세요.  
# 제한조건  
x는 -10000000 이상, 10000000 이하인 정수입니다.  
n은 1000 이하인 자연수입니다.
# 입출력 예시    




| x | n | answer |
| --- | ----- | ---- |
| 2 | 5 | [2,4,6,8,10] |
| 4 | 3 | [4,8,12]|
|-4 | 2 | [-4,-8] | 

# 코드
~~~python
def solution(x, n):
answer = []
for i in range(n):
answer.append(i*x +x)
return answer
~~~

# 코드 설명
본인은 append()함수를 반복해서 구현했다.  
간단하게 한줄로 `answer = [i*x + x for i in range(n)]`으로도 구현할 수 있을 것이다.  
`answer = [i\*x for i in range(1, n + 1)]` 이런것도 당연히 가능할 것이다.