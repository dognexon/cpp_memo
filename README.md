# cpp_memo
If you find some errors or have any questions, please contact me at any time ;)



# 자료형의 종류
|**정수형**|<u>**int**<u>|**부호 있는 10진 정수(4byte)**|-2^31^ ~(2^31^ -1)|
|--|--|--|--|
|〃|unsigned int|부호 없는 10진 정수(4byte)|0~(2^32^ -1)
|〃|long long|부호 있는 10진 정수(8byte)|-2^63^ ~(2^63^ -1)
|〃|unsigned long long|부호 없는 10진 정수(8byte)|0~(2^64^ -1)|
|**실수형**|<u>**float**<u>|**단정도 부동 소수점(4byte)**|$$\pm3.4E-38~\pm3.4E+38$$
|**〃**|<u>**double**<u>|**배정도 부동 소수점(8byte)**|$$\pm1.7E-308~\pm1.7E+308$$|
|**문자형**|<u>**char**<u>|**아스키코드(1byte)**|**-128~127**|
|**논리형**|<u>**bool**<u>|**논리값(1byte)**|**true,false**|
> ### 변수 이름의 작성 규칙
> - **변수의 이름은 알파벳, 숫자, ' _ '의 조합으로 만들 수 있다**
> - 변수 이름은 **대소문자를 구분하며, 첫 글자에는 숫자를 사용할 수 없다.**
> - 시스템 예약어(연산자 및 라이브러리 함수 등`if ,char ,for등등`)는 변수 이름으로 사용할 수 없다
> 
> `이는 거의 모든 프로그램언어에서 대동소이하게 적용됨`

# 제어 문자의 종류


|제어 문자|의미|제어문자|의미|
|--|--|--|--|
|\a|경고음|\t|수평탭|
|\b|백스페이스|\v|수직탭|
|\f|폼 피드| \\\ |<u>**백슬래시**<u>|
|\n|<u>**개행**<u>`줄바꿈`| \\'|<u>**작은따옴표**<u>|
|\r|캐리지 리턴|\\"|<u>**큰따옴표**<u>|




 # 서식 지정자의 종류

|서식 지정자|출력 형태|서식 지정자|출력 형태|
|--|--|--|--|
|**%c**|<u>**단일 문자**<u>|**%x**|<u>**부호 없는 16진 정수, 소문자 사용**<u>|
|**%d**|<u>**부호 있는 10진 정수**<u>|%X|부호 없는 16진 정수, 대문자 사용|
|%i|부호 있는 10진 정수`%d와 같음`|%e|e 표기법에 의한 실수|
|**%f**|<u>**부호 있는 10진 실수**<u>|%E|E 표기법에 의한 실수|
|**%s**|<u>**문자열**<u>|%g|값에 따라서 %f, %e 둘 중 하나를 선택|
|**%o**|<u>**부호 없는 8진 정수**<u>|%G|값에 따라서 %f, %E 둘 중 하나를 선택|
|%u|부호 없는 10진 정수|**%%**|<u>**% 기호 출력**<u>|
# 비교 연산자와 논리 연산자
|종류|기호|문법|의미|
|--|--|--|--|
|**비교 연산자**|**==**|**a == 3**| <u>**a와 3이 같은가?**|
|〃|**!=**|**a != 3**|<u>**a와 3이 다른가?**|
|〃|**>,<**|**a > 3,<br> a < 3**|<u>**a가 3보다 큰(작은)가?**|
|〃|**>=,<=**|**a >= 3, <br>a <= 3**|<u>**a가 3보다 크거(작거)나 같은가?**|
|**논리 연산자**|**&&**| **a && b**|<u>**a와 b가 모두 참일 경우에만 참**|
|〃|**\|\|**| **a \|\| b**|<u>**a와 b가 모두 거짓일 경우에만 거짓**|
|〃|**!**| **!a**|<u>**a가 참이면 거짓, 거짓이면 참**|

# 복합 대입 연산자와 증감 연산자
> 복합 대입 연산자 
> 
> **변수에 특정 값의 연산 결과를 대입해야 하는 연산식을 간단하게 기술**하도록 도와준다. `복합 대입 연산자는 다양한 종류가 있으나, 기본적으로 대입 연산자와 산술, 비교,논리, 비트 연산자가 합쳐진 구조`
> + 복합 대입 연산자 a += 1과  a = a + 1의 결과가 동일함

>증감 연산자
>변수의 값을 1씩 증가 또는 감소시키는 연산자이며`주로 for문에서 사용`, **위치에 따라 연산의 시점이 달라진다**, 
>
>**전위`앞쪽, prefix`에 사용된 경우는 계산이 수행되기 전에 먼저 실행**되지만, 
>**후위`뒤쪽, postfix`에 사용된 경우에는 계산을 수행한 후 실행**된다 
>```cpp
>#include <stdio.h>
>void main()
>{	
>	int a = 3, b = 2;
>	printf("%d, %d\n",++a, b--); 
>	a += 1; b -=1;
>	printf("%d %d\n", a, b);
>}
>```
>실행 결과
>```cpp
>4 2
>5 0
>```

|종류|기호|문법|의미|
|--|--|--|--|
|복합 대입 연산자|+=|a += 1| a = a + 1|
|〃|-=|a -= 1| a = a - 1|
|〃|*=|a *= 1| a = a * 1|
|〃|/=|a /= 1| a = a / 1|
|〃|%=|a %= 1| a = a % 1|
------------
|증가 연산자|++|++a 또는 a++|a = a + 1|
|--|--|--|--|
|감소 연산자|--|--a 또는 a--|a = a - 1|

# 연산자 우선순위
수학 계산식에서 먼저 계산을 수행하는 우선순위가 있듯이, C언어에서도 여러가지 연산자가 복합적으로 사용될 때 연산자 우선순위가 있다.

**우선순위가 높을수록 먼저 계산**되고, 같은 순위의 연산자가 여러 개가 사용된 경우 **결합 순서에 의해 계산 순서가 결정**된다.

|기능별 분류|연산자|결합 순서|우선순위|
|--|--|--|--|
|  |  |
