---
title: "Java, 추상클래스"
date: 2020-01-18 11:33:00 +0800
categories: [Java, 추상 클래스]
tags: [Java, 추상 클래스]
---

## 추상클래스?

***

메서드의 <span style = "color:red"> 시그니쳐(리턴타입, 메서드명, 매개변수)</span>만 정의한 클래스
구체적인 행위, 즉 블록({}) 부분은 정의되지 않은 특수한 메서드

사용법 : 자식 클래스에서 Overriding을 해서 추상 메서드를 구현해야한다.
(구현 하지 않을 시 에러 발생)

추상클래스는 상속과 밀접한 관련이 있다.<br>


구문 :

```java
abstract class AbstrackClass {
    public void methodA(){...}
    public void methodB(){...}
}
```

<br>

## 추상클래스 특징 
***

1. 객체 생성 불가 : 아무런 기능도 제공하지 않는 추상 메서드가 호출된다는 것은 논리적으로 맞지 않음.
<br><br>
2. 유지보수 편의성 증가 : 추상클래스로 메서드를 공유하지 않으면 객체에서 각각 구현한 메서드가 다르기 때문에 <span style = "color:red">더 많은 소스코드들을 수정해야함</span>, 사용하려는 객체 변경 시 많은 수정이 발생한다면, 유지보수는 더욱 어려워지게 됨.<br>

<br>

## 추상클래스의 활용
***

모든 클래스의 메서드 시그니쳐를 통일 할 수 없음.
다른 TV 클래스에 어떤 메서드가 정의되어 있는지 일일이 확일할 수 없음.
<br><br>
이 경우, "추상 클래스를 적용하면, 모든 TV 클래스들의 메서드를 통일할 수 있음"<br>







<br>
## 출처
> 본 게시물은 삼성 SW Expert Academy의 강의 내용을 바탕으로 공부한 게시물입니다.<br>
출처 : [https://swexpertacademy.com](https://swexpertacademy.com/)