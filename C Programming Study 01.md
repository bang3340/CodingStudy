# C programming Study 01

### *전산학의 특징 : 알고 모르는 것의 차이가 과장돼서 느낌
### *순서 (Algorithm -> C ->Source code Compile -> executable code -> run -> 결과)

## $ C 프로그램 , 기본구조      

#include <stdio.h>                        ß형식 써놓고 하자
int main()
{
/ ~~~~~문제해결 명령어 …/
return 0;
}


### ● 	기본 출력 명령
Printf(“_____”);  “   “ 안의 내용을 화면으로 출력하라. (모든 단위명령의 끝은 ; 이다)
Ex1) printf(“Hello world !”);
Ex2) printf(“Hello”);
Ex2) printf(“world”);   
 ->결과값 = Helloworld	 //줄을 바꾸고 싶으면 줄을 바꿔라 
\n = newline 줄바꿈.

Ex3) printf(“Hello \n handong”); -> \n\n도 가능 -> Hello (줄바뀜) handong

### ● 	Comments 주석-설명 
■ 	/* ~~~~~~~~~~~~
■ 	~~~~~~~~~~~~~*/         à 소스코드를 사람이 알기 위해!
(ex 과제를 낼때에 학번, 이름 ,과제이름 등 주석을 써줌)

### ● 	Data 표현
■ 	변수 (variables) : 임의의 값이 저장 될 수 있는 공간 ->변수 name을 가져야함
■ 	상수 (constants) : 표현자체가 특정 값 

### ● 	변수명 규칙(identifier)
1. 영문자, 숫자, ’_’ 		ex) abc_de
2. 숫자로 시작할 수 없음 	ex) 3ry (X)
3. 중간 여백이 올 수 없음 	ex) total sum (X) -> total_sum(O) 언더바로 대체
4. 대소문자 구분
5. 31자(256자)까지 유효
6. keywords(reserved word)는	ex) if , for 등
	  변수로 사용할 수 없다.
7. 변수명의 가급적 의미(쓰임)과 연관하여 naming을 한다. -> readability *가독성*
 Ex) int boxCount , float starCount 

### ● 	변수의 type(유형)
■ 	23+4.5 라면 정수, 실수를 나눠야하는데..
◆ 	1) 정수 int
◆ 	2) 실수 float
■ 	모든 변수 명(identifier)은 사용되기전에 반드시 ‘선언’ 되어야 함.
Ex) int x, y, z; 
◆ 	3)상수 표현		->정수 : 23  125 // 실수 : 2.5  3.4	
◆ 	                         2(정수)  2.0(실수)

### ● 	Assignment (대입) 
■ 	X=Y; 	<- Y의 값을 X에 넣어라
■ 	X=3; 	<-우변의 내용의 수식 값을 좌변의 변수 값에 넣어라.

### ● 	연산자 (operator)
■ 	산술 연산자 :   * , / , % (먼저)     + , - (후에)
Ex) x =8; 
   Y= x%3;   -> 결과 : y는?
Ex) int x, y, z
	X=3;
	Y=(x+2)%3;
	Z=x+y*2;    -> x, y, z는?
	
### ● 	서로 다른 type의 산술 연산
■ 	자동 변환 
■ 	정수(실수로 바뀜) + 실수 ex) 2+2.0  => 2.0+ 2.0 = 4.0

### ● 	Assignment 연산
■ 	= 의 좌우 변 type 다를때
■ 	좌변 변수 type으로 변환하여 저장!! 
 

### ● 	EXERCISE@
int x, y , z;
float a, b;
x=3;
y=2;
z=x/y;			z 값은?
a=x/y;			a 값은?

	a=x/2		a=x/2.0		 z=x/2.0    	a, z의 값은?






