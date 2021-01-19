# C programming -2


## ● 	Data 출력
Printf(“ 출력내용의 형식“ ,출력값데이타);

Ex)
	Int x,y;
	X=3;
	Y=5;
	printf(“X=%d, Y=%d \n”,x, y);     %d ß conversion spec(데이터가 나올 위치를 의미)
		(x)1번째	(y)2번째 데이터값
						 % 개수와 x,y 개수가 일치해야함

printf(“The sum = %d \n”, x+y)l.   x+y ß 수식도 가능
    	출력값 : The sum = 8;
X=3; y=5;
Printf(“%d+%d = %d \n”, x ,y, x+y);     \n ß 보통 습관적으로 함, 
				값으로 된 어떤 표현도 가능
		출력 값 : 3 + 5 =8 


## ● 	%d = 정수 값
%f =  실수(float) 값  à 소수점 이하 6자리 까지

## ● 	Keyboard로부터 한개의 정수 값을 읽어 x에 넣는다.
1. 	Scanf(“ %d “, &x);       &xß 읽어드릴 값의이름과 위치를 & == 연산자

2. 	두개를 읽고 x,y에 넣는다.
Scanf(“%d %d” , &x, &y);    %d%d ß %d , %d 아님! ‘ , ’ 를 넣지않는다!
두개의 정수가 읽힐때까지 wating 한다. Space 와 enter로 나눠줌.

## ● 	Example
두개의 정수값에 평균을 구하는 프로그램

#include <stdio.h>

int main() {
  int x,y;
  	float average;
  	scanf("%d%d",&x,&y);
  	average=(x+y)/2.0;
  	printf("average = %f \n",average);

 	 return 0;
}

## ● 	Example 2
섭씨온도’C’를 화씨온도 ‘F’로 변환

1. 	섭씨온도를 입력
2. 	해당되는 화씨온도로 계산
3. 	출력

공식 F= (9.0/5.0)*C+32;  
-> F=(9/5)*C+32 로 하면 9/5가 항상 1이므로 9.0/5.0으로 계산
	
	#include <stdio.h>

int main() {
  	float sub,hwa;

  	scanf("%f",&sub);
  	hwa=(9.0/5.0)*sub+32;
  	printf("F=%f \n",hwa);

 	 return 0;
}	

## ● 	Printf 에서 출력 형식 지정
Ex) printf(“X=%d \n”,x); -> %d는 x를 출력 즉 x를 정수형태로 출력하라.
Conversion spec 이라고도 함. 




%d = 정수(decimal)
%f = 실수(float)
%e = 지수(e)
%g = %f or %e 자동 결정 ( ~보다 커지면 %f나 %e로 하라임.)
	
일단 이정도만 알고 넘어가자.

## ● 	자릿수 지정

%d -> 최소한의 자릿수로 (앞뒤 여백없이) 

Ex) x=123; y=25; printf(“X=%d,Y=%d \n”,x,y); 
 	x=123,y=25

%5d ->최소한 5자리

Ex) x=123; y=25; printf(“X=%5d,Y=%5d \n”,x,y);
 	x=  123,y=   25

숫자는 오른쪽 줄 맞춤, 문자는 왼쪽 줄 맞춤이 기본이다. 
만일 %3d 인데 1234면 compact하게 나온다. 

32
34
1234 <- 이렇게 튀어 나옴.

왼쪽 줄 맞춤을 하고싶다면
%-5d  -> left justify 

## ● 	알아두기 

1. 	%05d     “앞의 여백을 0으로 채우겠다” 라는 뜻
	
	Ex) x=123; printf(“x=%05d \n”,x);
		X=00123


%f ->소수점 6자리
%8.5f 총 8자리 소수점 이후 5자리

Ex)



	

 



