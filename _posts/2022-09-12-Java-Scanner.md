---
layout: single
title:  "[Java] Scanner 입력"
categories:
  - java
---

### Scanner 클래스

#### 1. console창을 통한 입력


#### 2. java.util.Scanner 클래스로 존재

  - java.util.Scanner 로 사용

  - import 후 사용
  
  > import 대상은 java.lang 이외의 모든 클래스

#### 3. Scanner 클래스의 객체 생성 방법

  - Scanner 객체명 = new Scanner(입력스트림);

#### 4. Scanner 클래스의 객체 소멸 방법

  - 객체명.close();

#### 5. Scanner 클래스의 메소드

  (1) 문자열 입력

    - next() : 공백 전까지 입력

    - nextLine() : 엔터 전까지 입력

  (2) 정수 입력

    - nextInt(), nextByte(), nextShort(), nextLong()

  (3) 실수 입력

     - nextDouble(), nextFloat()

  (4) 논리 이력

    - nextBoolean()

  (5) 문자 입력

    - 문자열 입력(next(),nextLine()) 받은 뒤 첫번째 값(charAt(0))만 사용

    - ex) String s = "happy"; -> s.charAt(0) == 'h'

#### 소스 예시

> Scanner 객체 생성

```java
Scanner sc = new Scanner(System.in);
```
##### nextLine, nextInt, nextDouble

>  이름 : String 입력 받기위해 nextLine 사용

```java
System.out.println("이름 입력 >> ");
String name = sc.nextLine();
```

> 나이 : 정수 값을 입력 받기 위해 nextInt 사용

```java
System.out.println("나이 입력 >> ");
int age = sc.nextInt();
```

> 키 : 실수를 입력받기 위해 nextDouble 사용

```java
System.out.println("키 입력 >> ");
double height = sc.nextDouble();
```
