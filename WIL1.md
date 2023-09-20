# 2023-2-BackEnd-Study
## Java와 객체 지향 프로그래밍
### Java
java는 썬 마이크로 시스템즈에서 개발하여 1996년 1월에 공식적으로 발표한 객체지향 프로그래밍 언어이다.
자바의 대표적 특징을 정리해보자면 다음과 같다.
#### 운영체제에 독립적이다.
운영체제와 하드웨어에 관계없이 실행이 가능하다.
#### JVM을 이용한다.
(Java Virtual Machine:java가 운영체제에 종속받지 않고 인식 및 실행할 수 있게 하는 가상 컴퓨터)
#### 객체지향 언어이다.
상속, 캡슐화, 다형성
#### 자동 메모리 관리
#### 네트워크와 분산처리를 지원한다.
#### 멀티쓰레드를 지원한다.
#### 동적 로딩을 지원한다.
-----
### 객체지향 프로그래밍
프로그래밍에서 필요한 데이터를 추상화시켜 객체로 만들어, 객체들간의 상호작용을 통해 로직을 구성하는 프로그래밍 방법이다.
#### 장단점
##### 장점
1. 코드의 재사용성이 높다.(다른 클래스를 가져와 사용하거나 상속을 통해 확장이 가능하다.)

2. 유지보수가 쉽다.(수정할 부분이 클래스 내부에 멤버 변수 혹은 메소드로 존재하기 때문에 해당 부분만 수정하면 된다.)

3. 대형 프로젝트에 적합하다. (클래스 단위로 모듈화가 가능하므로 업무 분담의 용이성을 가진다.)
##### 단점
1. 처리 속도가 느리다.
2. 객체가 많으면 용량이 커질 수 있다.
3. 설계 시 많은 노력과 시간이 필요하다.
#### 특징
##### 추상화
객체에서 공통된 속성과 행위를 추출하는 것. 중요한 정보만을 표현함으로써 프로그램을 간단하게 만든다.
##### 캡슐화
데이터 구조와 데이터를 다루는 방법들을 결합시켜 묶는 것. 낮은 결합도를 유지할 수 있도록 한다.
속성과 기능을 정의하는 변수와 메소드를 클래스라는 캡슐에 넣어서 분류하는 것으로 재사용이 원할하다는 장점이 있다.
접근 제어자의 활용을 통해 정보은닉을 활용할 수 있다.
##### 상속
클래스의 속성과 행위를 하위 클래스에 물려주거나 / 하위 클래스가 상위 클래스의 속성과 행위를 물려받는 것을 말한다.
새로운 클래스가 기존의 클래스를 활용할 수 있도록 해준다.
범용성이 증가하여 자유롭게 메소드와 자료를 사용 및 추가할 수 있으나, 상위 클래스의 변경이 어려워지거나 불필요한 클래스가 증가할 수 있다.
##### 다형성
하나의 변수명, 함수명이 상황에 따라 다른 의미로 해석될 수 있는 것을 의미한다.
하나의 클래스 내부에 같은 이름의 행위를 여러 개 정의하거나 상위 클래스의 행위를 하위 클래스에서 재정의하여 사용 가능한 것이 객체지향 프로그래밍의 특징이다.
###### 오버라이딩
상위 클래스가 가지고 있는 메소드를 하위 클래스에서 재정의하여 사용하는 것.
###### 오버로딩
같은 이름의 메소드가 인자의 개수나 자료형에 따라 다른 기능을 하는 것.





