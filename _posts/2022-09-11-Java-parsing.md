---
layout: single
title:  "[Java] parsing"
categories:
  - java
---

### parsing

#### 문자열 -> 정수 (String -> int)

- Intrger.parseInt("10") -> 10 -> Integer는 int의 참조 자료형이다.
- 대문자로 시작하는 단어는 클래스라고 보면된다.
 
##### 예시 소스

> 문자열을 정수로 출력
```java
String strage = "20";
int age = Integer.parseInt(strage);
System.out.println(age);
```

#### 문자열 -> 실수 (string -> double)
- Double.parseDouble("3.14") -> 3.14

##### 예시 소스

> 문자를 실수로 출력
```java
String strHeight = "190.5";
double height = Double.parseDouble(strHeight);
System.out.println(height) ;
```


#### 정수 / 실수 -> 문자열 (int / double -> string)

- string.valueof(10) -> "10"
- string.valueof(3.14) -> "3.14"


#### 비교(equals, "=, >, <, >=, <=")

- 문자열 비교 : equals  
- 숫자 비교 :  =, >, <, >=, <= 등 사용  
