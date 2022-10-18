---
layout: single
title:  "[Java] casting"
categories:
  - java
---

### casting(형 변환)
#### 자동 형 변환(묵시적)
- java 스스로 형 변환
- 타입이 섞인 경우 작은 크기의 타입을 큰 크기의 타입으로 통일시키는 방향으로 형 변환
- ex) short와 int의 연산 -> 둘다 int로 변환된 뒤에 연산
- 정수와 실수가 섞인 경우 정수를 실수로 변환
##### 예시 소스
> java 스스로 1.0 + 1.5로 변환 후 연산
```java
System.out.println(1 + 1.5);
```
> java 스스로 double a = 10.0 으로 변환 후 처리
```java
double a = 10;
System.out.println(a);		
```

#### 강제 형 변환(명시적)
- 개발자가 직접 형 변환
- 타입 상관없이 원하는 타입으로 변환
- (자료형)변수, (자료형)값
- ex) "int num = 10;" 로 선언 및 초기화 되어있을 떄,  "(double)num" 형태로 num을 실수로 처리.


##### 예시 소스
> 개발자가 입력데이터를 강제로 int로 변경하여 저장
```java
int b = (int)20.9;
System.out.println(b);
```
> 1/2 계산된 값을 출력.
```java
int c = 1;
int d = 2;
double e = c/(double)d;
System.out.println(e); 
```
