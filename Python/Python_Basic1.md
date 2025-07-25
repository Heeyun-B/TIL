  # Python Basic Syntax 1

Onboarding → Objectives → Build → Run → Test → Review

학습 시작 → 학습 목표 → 이론 → 실습 → 확인 문제 → 학습 정

## 프로그래밍

문제를 해결하기 위한 명령어들의 집합

**프로그래밍의 핵심**

새 연산을 정의하고 조합해 유용한 작업을 수행하는 것

**프로그래밍 언어**

컴퓨터에게 작업을 지시하고 문제를 해결하는 도구

## Python

## Python을 배우는 이유

- 쉽고 간결한 문법
    - 읽기 쉽고 쓰기 쉬운 문법을 가지고 있어 쉽게 배우고 활용할 수 있음
- Python 커뮤니티의 지원
    - 세계적인 규모의 풍부한 온라인 포럼 및 커뮤니티 생태계를 형성함
- 광범위한 응용 분야
    - 웹 개발, 데이터 분석, 인공지능, 자동화 스크립트 등 다양한 분야에서 사용함

### 왜 인공지능(AI)과 머신러닝(ML) 개발에 Python을 사용할까?

- 압도적인 전문 라이브러리
    - TensorFlow, Pytorch 등 AI 개발의 핵심 도구들이 파이썬으로 제공돼 복잡한 기능을 쉽게 구현할 수 있음
    - TensorFlow : 구글이 만든 딥러닝 도구
    - Pytorch : 페이스북이 만든 딥러닝 도구
- 쉬운 문법과 높은 생산성
    - 문법이 간결해 배우기 쉽고, 아이디어를 빠르게 프로토타입으로 만들 수 있어 연구와 개발에 가장 효율적
- 강력한 커뮤니티와 생태계
    - 수많은 개발자들이 파이썬을 사용하므로 관련 자료를 찾기 쉽고 문제 해결에 대한 도움을 얻기 용이

## Python  실행

Python  프로그램이 실행되는 과정

- 컴퓨터는 기계어로 소통하기 때문에 사람이 기계어를 직접 작성하기 어려움
- 인터프리터가 사용자의 명령어를 운영체제가 이해하는 언어로 바꿈

Python  인터프리터를 사용하는 방법

- shell 이라는 프로그램으로 한 번 한 명령어씩 입력해서 실행
- 터미널을 켜고 `python -i`를 입력하면 파이썬 인터프리터 환경이 실행
- 확장자가 .py인 파일에 작성된 python 프로그램을 실행
    - 터미널을 종료할 때, `exit()` 를 하거나, kill 터미
    - 터미널에서  X를 누르는 건 그냥 숨기는 것. 터미널이 멈추거나 문제가 생겼을 땐 kill 터미널을 해야함(휴지통표시)
    - Run 버튼을 눌러도 실행하긴 함. 하지만 우리는 계속 코드로 실행하자.
        
        코드 시행 명령어 : `python  파일명.py`
        

### 표현식과 값

**표현식(Expression)** : 하나의 ‘값’으로 평가될 수 있는 모든 코드

- 평가 : 표현식을 계산하여 그 결과인 ‘값’을 만들어내는 과정
- 표현식을 평가하면 하나의 값이 됨

**값 (value)** : 표현식이 평가된 결과

더 이상 계산되거나 평가될 수 없는 프로그램의 가장 기본적인 데이터 조각

- 불리언 (Boolean) : 컴퓨터에서 참과 거짓을 나타내는 숫자 1과 0만을 이용하는 방식

### 변수와 메모리

**변수 (Variable)** :  값을 나중에 다시 사용하기 위해 그 값에 붙여주는 고유한 이름 → “**객체를 가리키는 이름**”

**변수 할당 (Variable assignment)** : 표현식이 만들어 낸 값에 이름을 붙이는 과정(연결)

**변수명 규칙**

- 영문 알파벳, 언더스코어(_), 숫자로 구성
- 숫자로 시작할 수 없음
- 대소문자를 구분
- 아래 키워드는 파이썬의 내부 예약어(Reserved)이므로 사용 불가
```    
['False', 'None', 'True', '__peg_parser__', 'and', 'as', 'assert',
'async', 'await', 'break', 'class', 'continue', 'def', 'del',
'elif', 'else', 'except', 'finally', 'for', 'from', 'global',
'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not',
'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']
``` 

**메모리 주소** 

- 각 사물함을 구별하기 위해 붙어 있는 절대 겹치지 않는 고유한 ‘사물함 번호’
- 컴퓨터가 특정 데이터 값을 정확히 찾아가기 위해 사용하는 기계적인 숫자 주소
- 객체가 저장된 고유한 위

**타입 (Type)**

- 제품의 종류 (예 : 정수, 실수, 문자열 등)

**값 (Value)**

- 제품의 실제 내용물

> 값+타입+주소 정보를 묶은 것을 **객체(Object)**라고 부름
> 

**객체(Object)** : 값, 타입, 그리고 관련된 행동까지 하나로 묶인 개념. 객체는 파이썬에서 다루는 모든 **데이터의 실체**

변수는 특정 객체를 ‘가리키는(refer to/point to)’ 이름표

변수는 메모리 주소를 ‘가지지(contain)’  않음

**재할당 (Reassignment)**

- 이미 값이 할당된 변수에 새로운 값을 다시 할당하는 것
- 변수는 특정 값을 ‘기억’하거나 ‘가리키는’ 이름
- 재할당은 이 변수가 가리키는 대상을 새로운 값으로 변경하는 행위
- 재할당이 이루어지면, 변수는 이전 값을 완전히 잊고 새로운 값만 기억하게 된다

## Data Types

### 타입

변수나 값이 가질 수 있는 데이터의 종류를 의미

### **Data Types**

값의 종류와 그 값으로 할 수 있는 ‘동작(연산)’을 결정하는 속성

데이터 타입이 필요한 이유

- 각 타입에 따라 가능한 기능과 연산이 다르기 때문

**데이터 타입 분류 5가지**

- Numeric Types : int(정수),  float(실수), complex(복수수)
- Text Sequence Type : str(문자열)
- Sequence Types : list, tuple, range
- Non-sequence Types : set, dict
- 기타 : Boolean, None, Functions

**숫자형**

- 값을 계산하고, 수량을 세고, 데이터를 분석하는 등 가장 기본이 되는 데이터 타입
- int : 소수점이 없는 숫자를 표현 (양수, 0, 음수 포함)
- float : 소수점이 있는 더 정밀한 숫자를 표현
- 숫자현 데이터의 핵심 ‘행동’은 바로 계산
- 데이터 타입은 ‘값의 종류’와 ‘적용 가능한 행동’의 묶음

**Sequence Types**

여러 개의 값들을 순서대로 나열하여 저장하는 자료형

순서 (Oder)

- 값들이 순서대로 저장 (정렬X)

인덱싱(Indexing)

- 각 값에 고유 번호 (인덱스)를 가지고 있으며, 인덱스를 사용해 특정 위치의 값을 선택하거나 수정할 수 있음

슬라이싱(Slicing)

- 인덱스 범위를 조절해 전체 데이터 중 원하는 부분만 값을 잘라내서 사용할 수 있음

길이((Length)

`len()` 함수를 사용하여 저장된 값의 개수(길이)를 구할 수 있음

반복(Iteration)

- 반복문을 사용해 각 값을 하나씩 순서대로 꺼내 사용할 수 있음

**문자열**

문자들의 순서가 있는 *변경 불가능*한 시퀀스 자료형

작은 따옴표(’) 또는 큰따옴표(”)로 감싸서 표현

이스케이프 시퀀스 (Escape Sequence)

- 역슬래시(\)와 문자를 조합해 특별한 기능을 수행(줄바꿈,탭 등)
    - `\n` : 줄바꿈
    - `\t` : 탭
    - `\\` : 백슬래시
    - `\’` : 작은 따옴표
    - `\”` : 큰 따옴표

**f-string**

문자열 내에 변수나 표현식의 결과를 손쉽게 삽입하는 강력한 방법

문자열 시작 전 ‘f’ 접두어를 붙이고,  삽입할 부분(표현식)을 중괄호{ }로 감싸줌

시퀀스로서의 문자열

문자열은 시퀀스이므로 인덱싱, 슬라이싱, 길이 확인, 반봅 등 공통 기능을 모두 사용할 수 있음

**인덱스 (Index)**

- 시퀀스 자료형에서 각 값의 위치를 식별하기 위해 부여된 고유한 번호
- 인덱스가 0부터 시작하는 이유
    - ‘거리’의 개념으로 이해하면 쉬움
    - 인덱스는 ‘시작점으로부터 얼마나 떨어져 있는가’를 의미
    - 첫 번째 값은 시작점 바로 그 차제이므로, 떨어진 거리가 0
    - 두 번째 값은 시작점에서 1만큼 떨어져 있다
    
    ⇒ index  0은 ‘첫 번째 항목’을 의미하며, 이는 대부분의 프로그래밍 언어에서 통용되는 매우 중요한 규칙
    
- 파이썬은 음수 인덱스를 지원한다. → -1은 맨 마지막 값을 의미

**슬라이싱(Slicing)**

- 시퀀스의 일부분을 잘라내어 새로운 시퀀스를 만드는 작업
- 시작 인덱스와 끝 인덱스를 지정해 해당 범위의 값을 포함하는 새로운 시퀀스 생성
- 대괄호[ ] 안에 시작 위치, 끝 위치, 간격(Step)을 콜론(:)으로 구분하여 지정
    - start : 슬라이싱을 시작할 인덱스 (포함됨)
    - stop : 슬라이싱을 끝낼 인덱스 (***포함되지 않음***)
    - step : 몇 개씩 건너뛰며 값을 가져올지에 대한 간격 → ***방향***을 가리킨다(디폴트는 1)

**문자열을 바꾸려면?**

기존 문자열의 일부와 새로운 값을 조합하여 *새로운 문자열을 만들어야 함*

### 정수형의 진법 표현

접두사를 붙인다.

2진수 : 0b

8진수 : 0o

16진수 : 0x

### **부동소수점 (반올림) 오차 (Floating-point Rounding Error)**

**발생 원인**

- 컴퓨터는 2진법 사용
    - 컴퓨터는 모든 숫자를 0과 1로 이루어진 2진수로 변환해 저장
- 무한 소수의 발생과 근사값 저장
    - 우리가 쓰는 10진수 소수 중 일부(0,1)는 2진수로 바꾸면 무한히 반복되는 무한 소수가 ㅇ됨
    - 메모리는 유한하기 때문에, 컴퓨터는 이 무한 소수를 어쩔 수 없이 가장 가까운 근사값으로 잘라서 저장함

**해결책**

- 대표적으로 decimal 모듈을 사용해 부동소수점 연산의 정확성을 보장하는 방법
- decimal은 실수를 2진수로 변환하지 않고, 10진수 자체로 정확히 연산할 수 있게 해줌

### 표현식과 문장

**문장(Statement)**

- 특정 ‘동작(action)’을 지시하는 실행 가능한 코드의 최소 단위
- 문장은 동작을 ‘기술’하는 것을 넘어, 그 자체로 완결된 하나의 명령

**표현식** : 하나의 ‘값’으로 평가될 수 있는 모든 코드

### Style Guide

코드의 일관성과 가독성을 향상시키기 위한 규칙과 권장 사항들의 모음

여러 사람이 함께 작업하거나 미래의 내가 코드를 쉽게 알아볼 수 있도록 가독성과 일관성을 높여주는 역할

**파이썬에서의 대표적인  Style Guide**

변수명은 무엇을 위한 변수인지 직관적인 이름을 가져야 함

공백(Space) 4칸을 사용해 코드 블록을 들여쓰기

한 줄의 길이는 79자로 제한, 길어질 경우 줄 바꿈을 사용

문자와 밑줄(_)을 사용해 함수, 변수, 속성의 이름을 작성

함수 정의나 클래스 정의 등의 블록 사이에는 빈 줄을 추가

### 주석

프로그램 코드 내에 작성되는 설명이나 메모

#으로 쓴다

블럭을 잡고 `ctr + /`를 하면 주석처리됨