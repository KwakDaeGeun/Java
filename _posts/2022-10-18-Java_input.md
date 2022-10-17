---
layout: single
title:  "[Java] input"
categories:
  - java
---

## input


### Scanner
```java
/*
		 * 1. Scanner 클래스
		 * 
		 *  1) console창을 통한 입력
		 *  `
		 *  2) java.util.Scanner 클래스로 존재
		 *  	(1) java.util.Scanner 로 사용
		 *  	(2) import 후 사용
		 *  		import 대상 : java.lang 이외의 모든 클래스
		 *  
		 *  3) Scanner 클래스의 객체 생성 방법
		 *  	Scanner 객체명 = new Scanner(입력스트림);
		 *  
		 *  4) Scanner 클래스의 객체 소멸 방법
		 *  	객체명.close();
		 *  
		 *  5) Scanner 클래스의 메소드
		 *  	(1) 문자열 입력
		 *  		- next() : 공백 전까지 입력
		 *  		- nextLine() : 엔터 전까지 입력
		 *  	(2) 정수 입력
		 *  		- nextInt(), nextByte(), nextShort(), nextLong()
		 *  	(3) 실수 입력
		 *  		- nextDouble(), nextFloat()
		 *  	(4) 논리 이력
		 *  		- nextBoolean()
		 *  	(5) 문자 입력
		 *  		- 문자열 입력(next(),nextLine()) 받은 뒤 첫번째 값(charAt(0))만 사용
		 *  		ex) String s = "happy"; -> s.charAt(0) == 'h'
		 */
     
    // 1. Scanner 객체 생성
    Scanner sc = new Scanner(System.in);
    
    // 이름 : String 입력 받기위해 nextLine 사용 
    System.out.println("이름 입력 >> ");
		String name = sc.nextLine();
		// 나이 : 정수 값을 입력 받기 위해 nextInt 사용
		System.out.println("나이 입력 >> ");
		int age = sc.nextInt();
		// 키 : 실수를 입력받기 위해 nextDouble 사용
		System.out.println("키 입력 >> ");
		double height = sc.nextDouble();
    
    
```

### 연산자 

```java
    /*
		 * 1. 산술연산자
		 * 			정수		실수
		 *  	+   덧셈		덧셈
		 * 	 	-	뺄셈		뺄셈
		 *  	*	곱셈		곱셈
		 *  	/	  몫		나누기
		 *  	%	나머지	 X
		 */
		int a = 10;
    int b = a/2;
    System.out.println(b); // 5의 값이 나온다.
   
		/*
		 * 2. 대입연산자
		 * 
		 *  =  : 대입
		 *  += : 더해서 대입
		 *  -= : 빼서 대입
		 * 	*= : 곱해서 대입
		 *  /= : 몫으로 대입(정수), 나눠서 대입(실수)
		 *  %= : 나머지를 구해서 대입
		 */
    
    /*
		 * 3. 증감 연산자
		 * 	1) 증가
		 * 		(1) a++ : a를 사용하고 증가
		 * 		(2) ++a : a를 증가하고 사용
		 * 	2) 감소
		 * 		(1) a-- : a를 사용하고 감소
		 * 		(2) --a : a를 감소하고 사용
		 * /
    int num2 = 10;
		System.out.println(num2);	// 변수 원본 출력
		System.out.println(num2++); // 출력 후 1증가
		System.out.println(++num2); // 1증가 후 출력
    
		/*
     *4. 시프트 연산자
		 *  1) 왼쪽 시프트
		 *  	(1) <<
		 *  	(2) 왼쪽으로 한 자리씩 밀어낸다.
		 *  	(3) 비트 연산
		 *  	(4) 2를 곱하는 효과가 있다.
		 *  2) 오른쪽 시프트
		 *  	(1) >>
		 *  	(2) 오른쪽으로 한 자리씩 밀어낸다.
		 *  	(3) 비트연산
		 *  	(4) 2로 나누는 효과가 있다.
		 */
     
     int num = 8;
		System.out.println("왼쪽 시프트 : " + (num << 2) );
		System.out.println("오른쪽 시프트 : " + (num >> 1) );

    /*
		 * 5. 관계 연산자(비교 연산자)
		 *  1) >= : 이상, 크거나 같다.
		 *  2)  > : 초과, 크다.
		 *  3) <= : 이하, 작거나 같다.
		 *  4)  < : 미만, 작다.
		 *  5) == : 같다. (기본 자료형)
		 *    equals() : 같다. (문자열 비교)
		 *  6) != : 같지 않다.
		 *   ! .equals() : 같지 않다. (문자열 비교)	
		 */
     
		/*  
		 * 6. 논리 연산자
		 *  1) && : and 연산
		 *  2) || :  or 연산 
		 *  3) !  : not 연산
		 *  4) short evaluate 를 지원
		 *   	- && : false가 나오면 그 이후는 처리 하지 않음 (어차피 false라서)★
		 *   	- || : true가 나오면 그 이후는 처리 하지 않음 (어차피 true라서)★
		 */
     int a = 10;
		System.out.println(a==10 && a < 100);		//  true
		System.out.println(a != 10 || a == 10);		//	true
		System.out.println(!(a==10));				//	false
    
    /*
		 * 7. 조건 연산자
		 *	1) (조건식) ? 조건식이 true인 경우 : 조건식이 false인 경우
		 *	2) if else문의 대용으로 사용된다.  
		 */
      String id = "admin";
		// id가 admin 이면 "인증성공", 아니면 "인증실패" 출력
		String auth = id.equals("admin") ? "인증성공" : "인증실패";
		System.out.println(auth);
```
