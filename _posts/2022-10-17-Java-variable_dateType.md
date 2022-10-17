---
layout: single
title:  "[Java] 변수 입력"
categories:
  - java
---

# variable dateType


### 변수 선언 (선언과 초기화 동시에 진행)
```java
    /*
		 * 출력할 내용
		 * 
		 * 1. A					-> char, String
		 * 2. 한					-> char, String
		 * 3. Hello World		-> String
		 * 4. 100				-> int		정수
		 * 5. 3.141592			-> double	실수
		 * 6. true				-> boolean	
		 * 7. false
		 * 
		 * sysout 으로 값만 출력하지 말고,
		 * 변수에 담아서 해당 변수를 출력하도록
		 */
      int num1 = 0;       //정수 입력
			float num2 = 0f;    // 
			double num3 = 0.0;  //실수입력
			char ch = 0;        // 빈 공간으로 출력
			char ch2 = 'a';     //문자 'A'
			int ch3 = 'a';      // 아스키코드표에 의하여 출력됨.
      String str1 = null; 	// null : 0번지(주소의 초기화를 0으로 하겠다.)
			String str2 = ""; 	// "" : 빈 문자열
 
```
### 다른 값 대입
```java
  
      num1 = 100;
			num2 = 1.5f;
			num3 = 1.5;
			ch = '한';
			str1 = "hello";
			str2 = "java";   //변수에서 값을 저장하고 끝.
 
```
