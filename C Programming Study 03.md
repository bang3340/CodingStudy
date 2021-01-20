# C programming -3

RMK_
	Printf(“ %d “, &y);  만약 ‘%d’를  출력하고 싶으면 \” 쓰면된다.
1) 	\”. -> %d
2) 	\\ -> \
3) 	%% -> % 	가 출력이 된다.

Scanf(“%d%f”, &x, &y);  -> %d%f 붙혀서 입력함 도중에 %d,%f 콤마가 들어가면 에러!

### ● 	Expression(수식)
Operands : 변수, 상수		ex)a+b  a+3  a,b는 변수, 3은 상수
Operators

##  	Operators(연산자)
		Arithmetic operator(산술연산자)
		Relational operator(관계연산자)
		Logical operator(	논리연산자)
	
1) 	Arithmetic operator(산술연산자)
binary = operand가 2개		ex)a+b    -> +,-,*,/,% 	같은것들
unary = operand가 1개 		ex) -3, -a  -> 부호임

unary > binary(* / + - %). 		
	Ex) -a+b

##  	Assignment
X=y;   -> y(위치값)을 X에 넣어라 .  라는 뜻		
ex) x=y=z=0.;
		z=0 (0을 z에) -> y=z (z를 y에) -> x=y(y를 x에)

##  	Compound Operator
*) += 
	Ex)x+=3; 		현재의 x 값을 3증가시켜라!   x=x+3과 동일!
*) -=
     Ex)x-=1; 		현재의 x 값을 1감소시켜라!   X=x-1과 동일!

+= , -= , *= , /=, %=  의미를 알아야함! \
(현재 자신의 값을 증가,감소,나누기,mod를 함) 
 	Increment operator 		++ : 해당 변수의 값을 1 증가시켜라 
 	Decrement operator 		 -- : 해당 변수의 값을 1 감소시켜라 

많이 쓰는 operator이며 unary operator임을 반드시 기억해두자!

Ex) x++   -> x=x+1;
Ex) x--    -> x=x-1;

##  	PREFIX , POSTFIX
Prefix -> ++x;
Postfix -> x++;
	
	둘다 x = x+1 라는 것은 변함이 없으나!
 	++X 는 해당 문장이 수행되기 전에 1 증가 시킴
	X++는 해당 문장이 수행된 후에 1 증가 시킴
	
	Ex1 )	 x=3;
		Y=++x;
		X=4;
		Y=4;

	Ex2)	x=3;
		Y=x++;
		X=4 임
		Y=3 임

	Ex3)	x=3;
		Y=2;
		Z=x++ +y;
		X=4 임
		Y=2 임
		Z=5 임

`	Ex4)	x=3;
		y=2;
		z=--x -y;
		x=2 임
		y=2 임
		z=0 임
##  	강력권장사항
한 문장에서 동일변수에 2회이상 사용하지 말것x=3;
Y=++x * ++x;		<- 헷갈림! 

### ● 	Relational operators (관계 연산자)
수치 데이터의 대소관계 판별
결과는 true/ false임 
Ex) (a>b)가?  => true/false로 나옴

	> <     |    ==		==은 같다는 뜻임 x=y는 y를 x에 넣어라이고, ==은 같다.
	>= <=  |    != 		거의 쓰지는 않지만  왼쪽이 우선순위가 더 높음 
					> , < , >=, <=   >>>>>>>> == , !=
					>= 일때 >(부등호) 먼저 =(등호) 나중 
	
### ● 	Logical Operator (논리 연산자) 
Logical AND => 둘다 참 일 때 TRUE	symbol : && 
Logical OR  => true가 있으면  TRUE 	symbol: || 
Logical NOT 				symbol: !

	Ex) !(x>3)  == x가 3보다 크지 않다면!


&&  ||.   <   !
(binary). 	      (unary)

계산 우선순위 :  ! > && > ||    반드시 외워야함! 

### ● 	C 언어에서 true / false 값의 표현

1) 	판정 할 때
모든 non zero -> true
Zero -> false 임
2) 	값을 생성 할 때
True -> 1
False -> 0

	*산술(Arithmetic) > 관계(Relational) > 논리(Logical) à 상식적으로 됨
*( ) 괄호 사용은 프로그램의 의도대로 강제함
### ● 	Control statement
컨트롤 제어 구조가 뭐가 있는지

프로그램 실행 흐름

순차(sequence) – 프로그램 쓴 순서대로
선택(selection)
반복(iteration = loop) 

### ● 	Selection (선택)

If – statement

If(조건식) 
(      );			<- 조건식이 true 일 때 수행 할 문장
Else
(      );			<- 조건식이 false 일 때 수행 할 문장

EX) 예제
	If(a>3)
	a=5;
	else 
	b=3;  			1) else part는 나타나고 안타나날 수 있다.
				2)해당 명령이 두 문장 이상이면 { } 로 묶는다

Ex1)	If(x>3).    
	{
	 a=3;
	 b=5;
	}
	

연습 ) 주어진 한 개 정수가 짝수이면 “even” 홀수이면 “odd” 출력하는 program을 작성하시오



연습 2) 숙제 1번 
	한개의 숫자(정수)를 입력 받아 해당 학점을 출력하시오
	
	-0~100까지 입력 받을 수 있음
	- 90~100 (A)
	- 80~ 89 (B)
	- 70 ~ 79 ©
	- 60 ~ 69 (D)
	-60점 밑으로 (F)
### ● 	Indentation (들여쓰기)
Ex)
	If(x>a) 
{
a=3; 
b=5;				<-들어가 있으면 이해하기 쉬움 , 줄을 맞춰줌
c=6;
	}
		


		
