---
title: "Java, 인터페이스"
# excerpt_separator: "<!--more-->"
date: 2020-01-18 10:33:00 +0800
categories: 
  - Java
tags: 
  - Java
  - 인터페이스
---

## 인터페이스?

***

- 구현된 것은 아무 것도 없고 밑그림만 그려져 있는 <span style="color:red">기본 설계도</span><br>

- 추상 클래스보다 추상성이 더욱 심화된 개념<br>
상수와 추상 메서드 외에 다른 멤버를 갖지 못하게 함으로써 추상 클래스보다 더욱 완벽한 추상화를 제공함.<br>

- 규칙 : 
1. 모든 멤버 변수는 public static final이어야 하고, 이를 생략 가능
2. 모든 메서드는 public abstract이어야 하고, 이를 생략 가능

- 구문 : 

    ```java
    public interface 인터페이스명 [extends 부모인터페이스명, ...]{
        // 상수 : final 예약어를 이용해서 멤버 변수를 선언해야 함
        // 추상 메서드 : 인터페이스는 객체를 생성할 수 없으므로, 상수는 static 예약어를 붙여서 선언해야 함
    }
    ```

- 예제 :

    ```java
    public interface Fruit{
        public static final int BANANA = 1
        public static final int APPLE = 2
        public static final int KIWI = 3
        public abstract void eat();
        public abstract move(int x, int y);
    }
    ```
<br>

## 인터페이스의 활용
***

1. 논리적으로 'is a ~ ' 관계가 성립하지 않는 경우<br>
<br>
2. 다중상속을 받고 싶은경우<br>

<br>

- 인터페이스를 포함하는 클래스 구문의 형태
```java
[modifiers] class 클래스명 [extends 부모 클래스]
    implements 인터페이스1, 인터페이스2, ... ] {

    }
```
- 인터페이스를 상속하는 클래스는 인터페이스에 정의된 추상 메서드들을 Overriding 해야 함
    - 블록을 추가하여 추상 메서드의 기능을 구현해야 함



<br>
## 출처
> 본 게시물은 삼성 SW Expert Academy의 강의 내용을 바탕으로 공부한 게시물입니다.
출처 : [https://swexpertacademy.com](https://swexpertacademy.com/)



