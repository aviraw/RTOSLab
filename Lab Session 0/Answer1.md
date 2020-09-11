# (Initial Source Code)
```
#include<stdio.h>
void disp()
{
        printf("Hello");
}
int d=123;
static int s;
int main(){
	printf("Aviral");
        disp();
        return 0;
}
```
![one](./Screenshots/1-1.png)

# (Upon changing the print string we see a change in text but bss and data remains same)
```
#include<stdio.h>
void disp()
{
        printf("");
}
int d=123;
static int s;
int main(){
	printf("Aviral");
        disp();
        return 0;
}
```
![two](./Screenshots/1-2.png)

# (Now upon changing the initialised state we change in both data and bss)
```
#include<stdio.h>
void disp()
{
        printf("");
}
int d;
static int s=0;
int main(){
	printf("Aviral");
        disp();
        return 0;
}
```
![three](./Screenshots/1-3.png)
# (Now adding more global varibles we see a change in bss)
```
#include<stdio.h>
void disp()
{
        printf("");
}
int d;
static int s=0;
int e;
int main(){
	printf("Aviral");
        disp();
        return 0;
}
```
![four](./Screenshots/1-4.png)
# (Now adding pointer for DMA)
```
#include<stdlib.h>
#include<stdio.h>
void disp()
{
        printf("");
}
int dd;
static int s=0;
int e;
int main(){
	printf("Aviral");
	scanf("%d",&dd);
  	int *ptr = (int*) malloc(dd * sizeof(int));
        disp();
        return 0;
}
```
![five](./Screenshots/1-5.png)
#
Name : Aviral Kumar Srivastava
Roll No :. 20
SAP ID : 500068442
Class : CSE IOT B1
RTOS LAB 0
