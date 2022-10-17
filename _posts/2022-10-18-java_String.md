---
layout: single
title:  "[Java] String"
categories:
  - java
---


### String
```java
    System.out.println(str1.toLowerCase());		// 기존 문자열을 소문자로 변환
		System.out.println(str1.toUpperCase());		// 기존 문자열을 대문자로 변환
		System.out.println(str1.indexOf('v'));		// 지정문자의 index 번호 반환 
		System.out.println(str1.charAt(2));			// 지정된 index의 문자 반환
		System.out.println(str1.startsWith("J"));	// 지정된 문자열로 시작되는지(boolean)
		System.out.println(str1.endsWith("a"));		// 지정된 문자열로 끝나는지(boolean)
		System.out.println(str1.contains("a"));		// 지정한 문자열을 포함하는지(boolean)
		System.out.println(str1.substring(1));		// 지정한 index 부터 모든 문자열을 반환
		System.out.println(str1.substring(1,3));	// 지정한 첫 번째 index 부터 두 번째 index 직전 까지의 문자열을 반환
		if(str1.equals(str2)) {				// 두 개의 문자열 비교(boolean)
			System.out.println(true);
		}else {
			System.out.println(false);
		}

```


