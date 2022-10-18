---
layout: single
title:  "[Java] Operator"
categories:
  - java
---


### 연산자 


#### 1. 산술연산자

|연산자|정수|실수|
|:---:|:---:|:---:|
| + |덧셈|덧셈|
| - |뺄셈|뺄셈|
| * |곱셈|곱셈|
| / |몫|나누기|
| % |나머지|X|

##### 예시

> 5의 값이 나온다.

```java
int a = 10;
int b = a/2;
System.out.println(b);
```
 

#### 2. 대입연산자

- =  : 대입

- += : 더해서 대입

- -= : 빼서 대입

-	\*= : 곱해서 대입

- /= : 몫으로 대입(정수), 나눠서 대입(실수)

- %= : 나머지를 구해서 대입


#### 3. 증감 연산자

(1) 증가

  - a++ : a를 사용하고 증가

  - ++a : a를 증가하고 사용

(2) 감소

  - a-- : a를 사용하고 감소

  - --a : a를 감소하고 사용


##### 예시

```java
int num2 = 10;
System.out.println(num2);	    // 변수 원본 출력
System.out.println(num2++);       // 출력 후 1증가
System.out.println(++num2);       // 1증가 후 출력
```

#### 4. 시프트 연산자

- 왼쪽 시프트 (<<)

  - 왼쪽으로 한 자리씩 밀어냄.
  
  - 비트 연산
  
  - 2를 곱하는 효과가 있음.

- 오른쪽 시프트 (>>)

  - 오른쪽으로 한 자리씩 밀어냄.
  
  - 비트 연산
  
  - 2로 나누는 효과가 있음.

##### 예시

```java
int num = 8;
System.out.println("왼쪽 시프트 : " + (num << 2) );
System.out.println("오른쪽 시프트 : " + (num >> 1) );
```

#### 5. 관계 연산자(비교 연산자)

|연산자|설명|
|:---:|:---:|
| >= |이상, 크거나 같다.|
| > |초과, 크다.|
| <= |이하, 작거나 같다.|
| < |미만, 작다.|
| == |같다.(기본 자료형)|
| equals() |같다.(문자열 비교)|
| != |같지 않다.|
| ! .equals() |같지 않다.(문자열 비교)|


#### 6. 논리 연산자

- && : and 연산  

- \|\| : or 연산

- ! : not 연산

- short evaluate 를 지원

  - && : false가 나오면 그 이후는 처리 x (어차피 false라서)★

  - \|\| : true가 나오면 그 이후는 처리 x (어차피 true라서)★

##### 예시

```java
int a = 10;
System.out.println(a==10 && a < 100);		// true
System.out.println(a != 10 || a == 10);		// true
System.out.println(!(a==10));	            	// false
```

#### 7. 조건 연산자
 
- 형식 : "(조건식) ? 조건식이 true인 경우 : 조건식이 false인 경우"

- if else문의 대용

##### 예시

> id가 admin 이면 "인증성공", 아니면 "인증실패" 출력

```java
String id = "admin";
String auth = id.equals("admin") ? "인증성공" : "인증실패";
System.out.println(auth);
```
