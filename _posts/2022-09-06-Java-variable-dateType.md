---
layout: single
title:  "[Java] 변수 자료형"
categories:
  - java
---

### 변수 데이터 타입

|데이터 타입|설명|예시|
|:---:|:---:|:---:|
|int|정수|100|
|float|실수|3.141592(double 보다 범위가 작다.), 0f, 0.0|
|double|실수|3.141592|
|char|문자|A, 한|
|String|문자열|Hello World|
|boolean|참과 거짓|true, false|

- 정수 표현 : int  
- 실수 표현 : float, double  
- 문자 표현 : char  
- 문자열 표현 : String  
- 참과 거짓의 표현 : boolean  

#### 변수 선언 (선언과 초기화 동시에 진행)
> 아래 예시는 변수에 담아서 해당변수 출력.(sysout에 직접 값 넣고 출력 X)

1) 정수
```java 
int num1 = 0;
```
2) 실수
```java
float num2 = 0f;
double num3 = 0.0;
```
3) 문자 및 문자열
```java
char ch = 0;              // 빈 공간으로 출력
char ch2 = 'a';           //문자 'A'
int ch3 = 'a';            // 아스키코드표에 의하여 출력됨.
String str1 = null; 	  // null : 0번지(주소의 초기화를 0으로 하겠다.)
String str2 = ""; 	  // "" : 빈 문자열
```

4) 다른 값 대입
> 변수에서 값을 저장하고 끝.
```java
num1 = 100;
num2 = 1.5f;
num3 = 1.5;
ch = '한';
str1 = "hello";
str2 = "java";
```
