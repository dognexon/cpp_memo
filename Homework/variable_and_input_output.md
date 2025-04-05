# 변수와 입출력
> 1.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("Good luck hope full!");
>}
>```
>output? :
>
<br>

>2.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 1;
>	printf("%d".a);
>	return 0;
>}
>```
>output? :

<br>

>3.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char c = 't'
>	printf("%c", c);
>	return 0;
>}
>```
>output? :

<br>

>4.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a;
>	scanf("%d", &a); //3 입력
>	printf("%d", a);
>	return 0;
>}
>```
>output? :

<br>

>5.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("1+2");
>	return 0;
>}
>```
>output? :

<br>

>6.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("%d", 4*7);
>	return 0;
>}
>```
>output? :

<br>

>7.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("a-b");
>	return 0;
>}
>```
>output? :

<br>

>8.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("good job");
>	return 0;
>}
>```
>output? :

<br>

>9.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int x=1;
>	int y=2;
>	printf("x:%d y:%d",x,y);
>}
>```
>output? :

<br>

>10.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char x;
>	scanf("%c",&x); // F입력
>	printf("%c input",x);
>	return 0;
>}
>```
>output? :

<br>

>11.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("%f", 5.5f);
>	return 0;
>}
>```
>output? :

<br>

>12.
>```cpp
>#include <stdio.h>
>int main()
>{
>	float a = 20.1234f;
>	printf("%f", a);
>	return 0;
>}
>```
>output? :

<br>

>13.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 10;
>	printf("a");
>	return 0;
>}
>```
>output? :

<br>

>14.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("%s", "string");
>	return 0;
>}
>```
>output? :

<br>

>15.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char txt = 'p';
>	printf("%c", txt);
>	return 0;
>}
>```
>output? :

<br>

>16.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 1, b = 4;
>	printf("%d %d",b, a);
>	return 0;
>}
>```
>output? :

<br>

>17.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char t1 = 't', t2 = '5';
>	printf("%c %c%c",t1, t2, t1);
>	return 0;
>}
>```
>output? :

<br>

>18.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int s1;
>	scanf("%d", &s1); //8 입력
>	printf("%d%d", s1, s1);
>	return 0;
>}
>```
>output? :

<br>

>19.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char c2;
>	scanf("%c", &c2); // s 입력
>	printf("%c %c", c2, c2);
>	return 0;
>}
>```
>output? :

<br>

>20.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a,b;
>	scanf("%d", &a); //5 입력
>	scanf("%d", &b); //10 입력
>	printf("%d %d", b, a);
>	return 0;
>}
>```
>output? :

<br>

>21.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("Now I am\nC Master");
>	return 0;
>}
>```
>output? :

<br>

>22.
>```cpp
>#include <stdio.h>
>int main()
>{
	>	int a;
	>	a=30;
	>	printf("%d\n",a);
	>	printf("%d\n",a*2);
>	return 0;
>}
>```
>output? :

<br>

>23.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 7, b, c;
	>	scanf("%d", &b); // 20 입력
	>	scanf("%d", &c); // 21 입력
	>	pritnf("%d %d %d", a, b, c);
>	return 0;
>}
>```
>output? :

<br>

>24.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 10;
>	a  = a * 10;
>	printf("answer is\n%d", a);
>	return 0;
>}
>```
>output? :

<br>

>25.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 3;
>	float b = 3.14f;
>	printf("%d %f", a, b);
>	return 0;
>}
>```
>output? :

<br>

>26.
>```cpp
>#include <stdio.h>
>int main()
>{
>	float a = 3.14f;
>	printf("%.4f, a);
>	return 0;
>}
>```
>output? :

<br>

>27.
>```cpp
>#include <stdio.h>
>int main()
>{
>	float a = 5.1234f;    //실수값에 f붙인건 자료형이 float라는것을 알리기 위해 사용함`굳이 안써도 정상 출력은됨`
>	float b = 6.678910f;
>	printf("%.2f %.3f, a, b);
>	return 0;
>}
>```
>output? :

<br>

>28.
>```cpp
>#include <stdio.h>
>int main()
>{
>	float c  = 0.9624f
>	pritnf("%.1f", c);
>	return 0;
>}
>```
>output? :

<br>

>29.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a =4;
>	float b = 0.12f;
>	char c = 'y';
>	printf("%c ", c);
>	printf("%d ", a);
>	printf("%f ", b);
>	return 0;
>}
>```
>output? :

<br>

>30.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a  =65, b;
>	scanf("%d," &b); // 100 입력
>	printf("Score is %c, %dpoint", a, b);
>	return 0;
>}
>```
>output? :

<br>

>31.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 30, b =10, temp;
>	printf("%d %d\n", a, b);
>	temp = a;
>	a = b;
>	b = temp;
>	printf("%d %d", a, b);
>	return 0;
>}
>```
>`hint: 어디서 본거 같지 않나요?(두 수 교환)`
>output? :

<br>

>32.
>```cpp
>#include <stdio.h>
>int main()
>{
>	printf("\\\"\'");
>	return 0;
>}
>```
>output? :

<br>

>33.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char a;
>	scanf("%c", &a); // A 입력
>	printf("%d", a);
>	return 0;
>}
>```
>output? :

<br>

>34.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int n;
>	scanf("%d", &n); // 66 입력
>	printf("%c", n);
>	return 0;
>}
>```
>output? :

<br>

>35.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char a;
>	scanf("%c", &a); // E 입력
>	printf("%c", a+32);
>	return 0;
>}
>```
>output? :

<br>

>36.
>```cpp
>#include <stdio.h>
>int main()
>{
>	char a;
>	scanf(" %c", &a); // F 입력
>	printf("%d %c\n", a, a);
>	a +=10;
>	printf("%d %c", a, a);
>	return 0;
>}
>```
>output? :

<br>

>37.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 11,b = 0x41;
>	printf("%x %d %x", a ,b ,b);
>	return 0;
>}
>```
>output? :

<br>

>38.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 10;
>	printf("%o", a);
>	return 0;
>}
>```
>output? :

<br>

>39.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a = 13;
>	printf("%X", a);
>	return 0;
>}
>```
>output? :

<br>

>40.
>```cpp
>#include <stdio.h>
>int main()
>{
>	int a =13;
>	printf("%X", a-3);
>	return 0;
>}
>```
>output? :

<br>

***끝 !
 고생하셨습니다!***
