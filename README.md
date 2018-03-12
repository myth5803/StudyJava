# StudyJava
자바기초정리

### 기본자료형(primitive data type)

키워드   	|	데이터	| 메모리 크기	|	표현범위 
--------|-----------|-----------|---------
boolean |	참/거짓	| 1바이트 		|	true/false
char    |	문자		| 2바이트 		| 	0~65535
byte    |	정수		| 1바이트 		|	-128 ~ 127
short   |	정수		| 2바이트  	|	-32768 ~ 32767
int     |	정수     | 4바이트  	|	-2147483648 ~ 2147483657 
long    |	정수     | 8바이트 		|	-9223372036854775808 ~ 9223372036854775807
float   |	실수     | 4바이트 		|	-3.4E38 ~ 3.4E38
double  |	실수     	| 8바이트 		|	-1.7E308 ~ +1.7E308


### 상수(literal)
- 이름이 없다
- 메모리에 저장된 상수의 값을 변경시킬 수 없다.
- 정수형(byte, short, int, long) 자료형은 int형으로 저장 - 4byte 메모리
- 실수형(float, double) 자료형은 double형으로 저장 - 8byte 메모리 

### 형변환(implicit conversion)
- byte -> short
- short -> int
- char -> int
- int -> long
- long -> float
- float -> double

### 비트 쉬프트 연산자
- 왼쪽비트열 이동은 2의 배수의 곱 ex) 2<<1=4 , 2<<2=8 , 2<<3=16
- 오른쪽비트열 이동은 2의 배수의 나눗셈 ex) 16>>1=8 , 16>>2=4 , 16>>3=2
> CPU에게 있어서 곱셈과 나눗셈은 매우 부담되는 작업이지만 비트를 이동시키는 연산은 전혀 부담되지 않는 작업이다.

### foreach 문
```java
// Iterable을 상속하여 구현 가능
for (type var: iterate) {
    body-of-loop
}
```