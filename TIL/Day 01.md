# 자바#1: <자바 기초>
# 1. 자바
## 자바?
- 제임스 고슬링의 주도하에 개발된 **객체 지향 프로그래밍 언어**

- 가전제품과 같은 전자기기 내부로의 탑재 목적으로 개발되었다가 웹 분야에서 널리 사용되는 언어가 되었음



## 사용 분야

### 1. 안드로이드 개발
- 자바는 코틀린과 함께 안드로이드 앱 개발에 사용되는 언어


### 2. DB 처리
- 웹 페이지의 데이터를 관리하는 데이터베이스에 데이터 읽기, 저장, 수정, 삭제 요청할 수 있음


### 3. 동적 웹 서버 개발

- **동적 페이지** : 사용자의 행동, 선호도, 관심사에 따라 변경되는 웹 콘텐츠

- **처리 과정!!**
    - 사용자의 요청은 웹 서버에 의해 처리되지만 웹 서버가 Java를 이해하지 못하므로 아래 과정을 거침

      (1) 사용자(클라이언트) 요청
      
      (2) 요청 페이지를 Tomcat 애플리케이션 서버로 전달
      
      (3) 요청 페이지의 Java 코드를 기반으로 필요한 동작 수행
      
      (4) HTML 페이지로 포맷된 완성된 응답을 웹 서버로 반환
      
      (5) 완성된 페이지가 웹 서버에서 클라이언트로 반환



## 자바 특징
### 1. 객체 지향 언어
- **객체 지향**: 프로그램을 작성할 때 객체들을 만들어 서로 소통하도록 하는 방법

- **객체**: 현실에 존재하는 사물을 추상적으로 표현한 것


### 2. 가비지 컬랙션
- **메모리 누수**: 프로그램이 필요하지 않은 메모리 공간을 계속해서 점유하는 현상

- 가비지 컬랙션은 이러한 메모리 누수 현상 방지

- 자바에서는 **JVM**이 사용하지 않는 메모리 삭제

- 자바스크립트, 파이썬과 같은 고수준 언어에 존재


### 3. JVM (Java Virtual Machine)
- 자바 바이트 코드(.class 파일) → OS 특화 코드 ⇒ 실행

- 가상머신의 개념을 도입한 것

- 운영체제에 독립적인 특징을 갖고 있어 다양한 운영체제에서 실행 가능

<aside>
    
    가상 머신
    
    - 하나의 물리적 컴퓨터에서 여러 운영체제를 실행하기 위한 소프트웨어
    - 서버 운영 등에 유용하게 사용
    
</aside>



# 2. 기본 문법
## 구문과 표현식

### 1. 구문
- 실행 가능한 최소의 독립적인 코드 조각

- 프로그램의 실행 순서 제어

- 세미콜론으로 끝남

```java
int a = 10;
System.out.println("Hello World");
```


### 2. 표현식
- 값을 생성하거나 변수 값 변경

- 하나 또는 그 이상의 값이나 변수 또는 연산자의 조합이며, 계산을 통해 단일 값 생성

```java
int a = 10; // 여기서는 10이 표현식인가?
int b = 4;
int result = a + b; // a + b가 표현식
```



## `System.out.println()` 메소드
- 메세지를 출력하는 가장 기본적인 방법

- `sout + Enter` 를 통해 바로 입력 가능

```java
System.out.println("Hello World");
System.out.println("sout 엔터!");
System.out.println(1);
```

- 콘솔 실행 화면
  
![image](https://github.com/shdbwls66/backendJava/assets/168792230/3bd4a6ed-0fc4-434d-9ca5-7b93ab6cfc4b)


<aside>

    💡 참고

    - `public class 파일명` 범위 내에서 코드 작성하기

    - 파일명 바뀌면 class 옆에 것도 바꾸기..

    - 파일 생성 시 src 디렉토리 내에 생성할 것!!!

    - 자바 클래스 파일 기본 구조?!
    
    ```java
    public class Test {

        public static void main(String[] args) {
            System.out.println("Hello World");
        }
    }
    ```
    
</aside>



## 주석
### 1. 한줄 주석
- `//` 사용

- `//` 부터 라인 끝까지 주석 처리

```java
// 이것은 한 줄 주석!!!
```


### 2. 범위 주석
- `/* */` 사이의 모든 범위를 주석 처리

- 단축키는 `ctrl + shift + /`

```java
/*
 * 이것은
 * 범위 주석
 */
```


### 3. JavaDoc
- `/** **/` 사이에 @로 제공되는 키워드 작성

```java
/**
 * @author 노유진
 * @implNote day7.test
 */
```

### 실행 화면

![image](https://github.com/shdbwls66/backendJava/assets/168792230/a5250064-8669-4bd1-9722-d0cdb6021523)

<hr>

# 참고
<aside>

    ❓ 단축키!!

    - `alt` + `shift` +  `↑` or `↓` : 코드 위치 바꾸기
    
        ![image](https://github.com/shdbwls66/backendJava/assets/168792230/f0d49ab2-9eca-4161-ba87-f5d8d8a8f1e7)

    - `psvm` + `Enter` : main 메소드 생성
    
        ![image](https://github.com/shdbwls66/backendJava/assets/168792230/5ddacb06-d895-46bc-9ab8-61ccf773b0c0)

    - `shift` + `F6` : 파일 이름 바꾸기

</aside>
