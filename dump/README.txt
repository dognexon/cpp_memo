새 프로젝트 => windows  데스크ㅗㅌㅂ 마법사 c++ 
템플릿에서 항목 모든 플랫폼 모든 언어으로 변경 

저장 위치 변경

우측 리소스 파일 아래 소스파일 우클 새 항목 추가

# 변수는 맨 위에

%5d 식으로 하면 뒤부터 5자리로 정수 출력 ex)l  100l
%-5d 식으로 하면 앞부터 5자리 정수 출력 ex)l100  l

printf("100을 16진수로 표현 : %x / 200을 8진수로 표현 : %o ", 100, 200);

#include <stdio.h>

void main()
{
	int a, sum;
	float b, fsum;
	a = 123.45;
	b = 200;
	sum = a + b;
	fsum = a + b;

	printf("a값 : %d\n", a);
	printf("b값 : %d\n", b);
	printf("정수형 : %d\n", sum);
	printf("실수형 : %f\n", fsum);

}

#include <stdio.h>

void main()
{
	int a, b, c, d;

	a = 100 + 100;
	b = a + 100;
	c = a + b -100;
	d = a+b+c;

	printf("a, b, c, d 의 값 ==> %d, %d, %d, %d\n", a,b,c,d);

	a = 100, b = 100, c = 100, d = 100;
	printf("a, b, c, d 의 값 ==> %d, %d, %d, %d\n", a, b, c, d);

	a = 100;
	a = a + 200;
	printf("a의 값==> %d\n", a);
	
}

#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	int first,second, result;
	char op;

	printf("첫 번째 수 입력 : ");
	scanf("%d", &first);
	printf("두 번째 수 입력 : ");
	scanf("%d", &second);
	printf("+, -, * / % 중 선택: ");
	scanf(" %c", &op); //**%c 한글자 입력 받을 때는 앞에 공백 주기**

	

	
}

#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	int first,second, result;
	char op;

	printf("첫 번째 수 입력 : ");
	scanf("%d", &first);
	printf("두 번째 수 입력 : ");
	scanf("%d", &second);
	printf("+, -, * / %% 중 선택: ");
	scanf(" %c", &op); //**%c 한글자 입력 받을 때는 앞에 공백 주기**
	if (op == '+') {
		result = first + second;
		printf("%d + %d = %d\n", first, second, result);
	}
	if (op == '-') {
		result = first - second;
		printf("%d - %d = %d\n", first, second, result);
	}
	if (op == '*') {
		result = first * second;
		printf("%d * %d = %d\n", first, second, result);
	}
	if (op == '/' ) {
		if (second != 0) {
			result = first / second;
			printf("%d / %d = %d\n", first, second, result);
		}
		else {
			printf("두 번째수가 0이어서 계산 불가\n");
		}
	}

	if (op == '%') {
		if (second != 0) {
			result = first % second;
			printf("%d %% %d = %d\n", first, second, result);
		}
		else {
			printf("두 번째수가 0이어서 계산 불가\n");
		}
	}
	if (first == second) {
		printf(" 두 수의 값이 같습니다.\n");
	}
	if (first > second) {
		printf(" 첫 번째 값이 큽니다.\n");
	}
	if(first < second) {
		printf(" 두 번째 값이 큽니다.\n");
	}
}

#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	int a,b,c, choice;
	float area;

	

	printf("<1> 사각형 <2> 삼각형 <3> 원 <4> 사다리꼴 : ");
	scanf("%d", &choice);
	if (choice == 1) {
		printf("가로 길이 입력 : ");
		scanf("%d", &a);
		printf("세로 길이 입력 : ");
		scanf("%d", &b);
		area = a * b;
		printf("가로 길이 %d 세로 길이 %d 인 사각형의 면적은 %.3f\n", a, b, area);
	}

	if (choice == 2) {
		printf("밑변의 길이 입력 : ");
		scanf("%d", &a);
		printf("높이 길이 입력 : ");
		scanf("%d", &b);
		area = a * b * 0.5;
		printf("밑변의 길이 %d 높이 길이 %d 인 삼각형의 면적은 %.3f\n", a, b, area);
	}
	if (choice == 3) {
		printf("원의 반지름 입력 : ");
		scanf("%d", &a);
		area = a * a * 3.14;
		printf("반지름이 %d 인 원의 면적은 %.3f\n", a, area);
	}
	if (choice == 4) {
		printf("밑변의 길이 입력 : ");
		scanf("%d", &a);
		printf("윗변의 길이 입력 : ");
		scanf("%d", &b);
		printf("높이 길이 입력 : ");
		scanf("%d", &c);
		area = (a + b) * c * 0.5;
		printf("밑변의 길이 %d 윗변의 길이 %d높이 길이 %d 인 사다리꼴의 면적은 %.3f\n", a, b, c, area);
	}
}


#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	printf("%d\n", 123);
	printf("%5d\n", 123);
	printf("%05d\n", 123);

	printf("%f\n", 123.45);
	printf("%7.1f\n", 123.45);
	printf("%7.3f\n", 123.45);

	printf("%s\n", "Basic-C");
	printf("%10s\n", "Basic-C");
}

%s는 %10s로 자리 확보하지 않으면 왼쪽 정렬 000000text    text

#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	int a, b;
	float c, d;

	a = 100;
	b = a;

	c = 111.1f;
	d = c;

	printf("a, b의 값 ==> %d , %d\n", a, b);
	printf("c, d의 값 ==> %5.1f , %5.1f\n", c, d);
}

#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	int a,b,c, choice;
	float area;

	

	printf("<1> 사각형 <2> 삼각형 <3> 원 <4> 사다리꼴 : ");
	scanf("%d", &choice);
	if (choice == 1) {
		printf("가로 길이 입력 : ");
		scanf("%d", &a);
		printf("세로 길이 입력 : ");
		scanf("%d", &b);
		area = a * b;
		printf("가로 길이 %d 세로 길이 %d 인 사각형의 면적은 %.3f\n", a, b, area);
	}

	if (choice == 2) {
		printf("밑변의 길이 입력 : ");
		scanf("%d", &a);
		printf("높이 길이 입력 : ");
		scanf("%d", &b);
		area = a * b * 0.5;
		printf("밑변의 길이 %d 높이 길이 %d 인 삼각형의 면적은 %.3f\n", a, b, area);
	}
	if (choice == 3) {
		printf("원의 반지름 입력 : ");
		scanf("%d", &a);
		area = a * a * 3.14;
		printf("반지름이 %d 인 원의 면적은 %.3f\n", a, area);
	}
	if (choice == 4) {
		printf("밑변의 길이 입력 : ");
		scanf("%d", &a);
		printf("윗변의 길이 입력 : ");
		scanf("%d", &b);
		printf("높이 길이 입력 : ");
		scanf("%d", &c);
		area = (a + b) * c * 0.5;
		printf("밑변의 길이 %d 윗변의 길이 %d높이 길이 %d 인 사다리꼴의 면적은 %.3f\n", a, b, c, area);
	}
}

short 작은 정수형
unsigned short 부호 - 없는 작은 정수형
int 정수형
unsigned int 부호 없는 정수형
long int(long) 큰 정수형
unsigned long 부호 없는 큰 정수형



#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	char ch;
	ch = 'a';
	printf(" %c\n", ch);
	printf(" %d\n", ch);
	ch = 88;
	printf(" %c\n", ch);
	printf(" %d\n", ch);
}

c를 d로 하면 숫자로 나옴


int a, b;
char c, d;

a = 0x41;
b = 0x50;

printf("16진수 0x41 코드 %c\n", a);
c = a;//c = 0x41
printf("16진수 0x41 코드 %c\n", b);
d = '#';
printf(" %c 의 ASCII 값은 %d 입니다", d, d);


#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>

void main()
{
	char aa[7] = "Hanbit"; //aa라는 변수애 [7] 자리 지정 (0 1 2 3 4 5 6

	printf(" %s\n", aa);
	aa[0] = 'D';
	printf(" %s\n", aa);
}
//# 문자열 출력하려면 무조건 #s
str1 = str3 처럼 문자열에 문자열 대입할 수 없음!XXXXX
strcpy(변수, 넣고싶은문자열)
또는 str1[0] = str2[0] 이런식으로(비효율적)


또한 7글자의 문자를 선언한다고 가정했을때 aa[8] 1더 크게 선언해야함

배열 array              =/=        구조체 
성격이 같은것을 모아둠         성격이 다른것을 모아둠




#define  _CRT_SECURE_NO_WARNINGS
#include <stdio.h>
#include <cstring>
void main()
{
	int type,data;
	printf("입력진수 결정 <1> 10진수 <2> 16진수 <3> 8진수 : ");
	scanf("%d", &type);
	printf("선택한 진수 %d: \n", type);

	if (type == 1){
		printf("값 입력 : ");
		scanf("%d", &data);
	}
	if (type == 2){
		printf("값 입력 : ");
		scanf("%x", &data);
	}
	if (type == 3){
		printf("값 입력 : ");
		scanf("%o", &data);
	}
	printf(" 10 진수 %d: \n", data);
	printf(" 16 진수 %x: \n", data);
	printf(" 8 진수 %o: \n", data);
}
