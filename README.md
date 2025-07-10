c
# C Programming Practice Programs

## 1. Control Statements

### Program 1: WRITE A C PROGRAM TO ACCEPT TWO INTEGERS AND CHECK WHETHER THEY ARE EQUAL OR NOT ?

```c
#include<stdio.h>
int main(){
    int a,b;
    printf("Enter 2 numbers: ");
    scanf("%d %d",&a,&b);
    if(a==b){
        printf("%d %d are equal",a,b);
    }
    else{
        printf("%d %d are not equal",a,b);
    } 
}
```

### Program 2: WRITE A C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS EVEN OR ODD?

```c
#include<stdio.h>
int main(){
    int n;
    printf("Enter a number: ");
    scanf("%d",&n);
    if(n%2==0){
        printf("%d is a even number",n);
    }
    else{
        printf("%d is not a odd number",n);
    }  
}
```
### Program 3: .WRITE A C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS POSITIVE OR NEGATIVE?

```c
#include<stdio.h>
int main(){
    int n;
    printf("Enter a number: ");
    scanf("%d",&n);
    if(n<0){
        printf("%d is a negative number",n);
    }
    else if(n>0){
        printf("%d is a Positive number",n);
    }
    else{
        printf("%d is a Nuetral number",n);
    }
}
```
### Program 4: WRITE A C PROGRAM TO FIND WHETHER A GIVEN YEAR IS A LEAP YEAR OR NOT?

```c
#include <stdio.h>

int main()
{
    int n;
    printf("Enter a year: ");
    scanf("%d",&n);
    if(n%100!=0 && n%4==0){
        printf("Given %d is a leap year",n);
    }
    else if(n%400==0)
    printf("Given %d is a leap year",n);
    else
    printf("Given %d is not an leap year",n);
}
```
### Program 5: WRITE A C PROGRAM TO READ THE AGE OF A CANDIDATE AND DETERMINE WHETHER HE IS ELIGIBLE TO CAST HIS/HER OWN VOTE?

```c
#include <stdio.h>
int main()
{
    int age;
    printf("Enter the age: ");
    scanf("%d",&age);
    if(age>=18){
        printf("%d years of age is eligible to her/his vote",age);
    }
    else
    printf("%d years of age is not eligible to her/his vote",age);
}
```
### Program 6: WRITE A C PROGRAM TO READ THE VALUE OF AN INTEGER M AND DISPLAY THE VALUE OF N IS 1 WHEN M IS LARGER THAN 0, 0 WHEN M IS 0 AND -1 WHEN M IS LESS THAN 0.

```c
#include <stdio.h>
int main()
{
    int m,n;
    printf("Enter M value: ");
    scanf("%d",&m);
    if(m>0){
        n=1;
        printf("The value of n is: %d",n);
    }
    else if(m==0){
        n=0;
        printf("The value of n is: %d",n);
    }
    else{
        n=-1;
        printf("The value of n is: %d",n);
    }
}
```
### Program 7:WRITE A C PROGRAM TO FIND THE LARGEST OF THREE NUMBERS?

```c
#include <stdio.h>
int main()
{
    int a,b,c;
    printf("Enter a b c values: ");
    scanf("%d %d %d",&a,&b,&c);
    if(a>b){
        if(a>c){
            printf("%d is the largest number",a);
        }
        else
        printf("%d is the largest number",c);
    }
    else if(b>c){
        printf("%d is the largest number",b);
    }
    else{
        printf("%d is the largest number",c);
    }
}
```
### Program 8:.WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS A VOWEL OR CONSONANT?

```c
#include <stdio.h>
int main()
{
    char ch;
    printf("Enter a character: ");
    scanf("%c",&ch);
    if(ch=='a' || ch=='e' || ch=='i' || ch=='o' || ch=='u' || ch=='A' || ch=='E' || ch=='O' || ch=='I' || ch=='U'){
        printf("Given character %c is an vowel",ch);
    }
    else{
        printf("Given chracter %c is an Consonant",ch);
    }
}
```
### Program 9:.WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS AN ALPHABET OR NOT?

```c
#include <stdio.h>
int main()
{
    char ch;
    printf("Enter a character: ");
    scanf("%c",&ch);
    if((ch>='a' && ch<='z') ||( ch>='A' && ch<='Z')){
        printf("Given character %c is an Alphabet",ch);
    }
    else{
        printf("Given chracter %c is not an Alphabet",ch);
    }
}
```
### Program 10: WRITE A C PROGRAM TO FIND MINIMUM OR MAXIMUM BETWEEN TWO NUMBERS?

```c
#include <stdio.h>

int main()
{
    int num1,num2;
    printf("Enter 2 numbers: ");
    scanf("%d %d",&num1,&num2);
    if(num1>num2){
        printf("%d is the maximum number \n",num1);
        printf("%d is the minimum number",num2);
    }
    else{
        printf("%d is the maximum number \n",num2);
        printf("%d is the minimum number",num1);
    }
}
```
### Program 11: WRITE A C PROGRAM TO ENTER WEEK NUMBER AND PRINT DAY OF WEEK?

```c

#include <stdio.h>
int main()
{
    int num;
    printf("Enter a week number: ");
    scanf("%d",&num);
    switch(num){
        case 1:
        printf("Monday");
        break;
        case 2:
        printf("Tuesday");
        break;
        case 3:
        printf("Wednesday");
        break;
        case 4:
        printf("Thursday");
        break;
        case 5:
        printf("Friday");
        break;
        case 6:
        printf("Saturday");
        break;
        case 7:
        printf("Sunday");
        break;
        default :
        printf("Invalid Week number!!!");
    }
}
```
### Program 12: WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS UPPERCASE OR LOWERCASE?

```c

#include <stdio.h>
int main()
{
    char ch;
    printf("Enter a character: ");
    scanf("%c",&ch);
    if(ch>='a' && ch<='z'){
        printf("Given character is in Lower Case");
    }
    else if(ch>='A' && ch<='Z'){
        printf("Given character is in Upper case");
    }
    else
    printf("Not an Character");
}
```
### Program 13: WRITE A C PROGRAM TO FIND NUMBER OF DAYS IN MONTH?

```c
#include <stdio.h>
int main()
{
    int num,year;
    printf("Enter a month number from(1-12): ");
    scanf("%d",&num);
    if(num == 2){
        printf("Enter year: ");
        scanf("%d",&year);
        if((year%400==0) || ((year%100!=0) && (year%4==0))){
            printf("29 days\n");
        }
        else{
            printf("28 days\n");
        }
    }
    else {
        switch(num){
            case 1:
            case 3:
            case 5:
            case 7:
            case 8:
            case 10:
            case 12:
            printf("31 days");
            break;
            case 4:
            case 6:
            case 9:
            case 11:
            printf("30 days");
            break;
            default:
            printf("Invalid month number");
        }
    }  
}
```
### Program 14: WRITE A C PROGRAM TO FIND MAXIMUM BETWEEN TWO NUMBERS USING SWITCH CASE?

```c

#include <stdio.h>
int main()
{
    int num1,num2;
    printf("Enter 2 numbers: ");
    scanf("%d %d",&num1,&num2);
    switch(num1>num2){
        case 1:
        printf("%d is maximum",num1);
        break;
        case 0:
        if(num2>num1){
            printf("%d is maximum number",num2);
        }
        else
        printf("Both are equal");
        break;
        default:
        printf("Enter appropriate number");
    }
}
```
### Program 15: WRITE A C PROGRAM TO PRINT EVEN NUMBERS BETWEEN 1 TO 20 USING A FOR LOOP?

```c
#include <stdio.h>
int main()
{
    printf("Even numbers between 1 to 20 are: ");
    for(int i=1;i<=20;i++){
        if(i%2==0){
            printf("%d ",i);
        }
    }
}
```
### Program 16: WRITE A C PROGRAM TO CALCULATE THE SUM OF NUMBERS FROM 1 TO 100 USING A WHILE LOOP?

```c
#include <stdio.h>
int main()
{
    int i=1;
    int sum=0;
    while(i<=100){
        sum+=i;
        i++;
    }
    printf("Sum of numbers from 1 to 100 are: %d",sum);
}
```
### Program 17: WRITE A C PROGRAM TO FIND THE FACTORIAL OF A GIVEN NUMBER USING A FOR LOOP?

```c

#include <stdio.h>
int main()
{
    int n,i,fact=1;
    printf("enter a number: ");
    scanf("%d",&n);
    for(i=1;i<=n;i++){
        fact*=i;
    }
    printf("Factorial is: %d",fact);
}
```
### Program 18: WRITE A C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS PRIME OR NOT USING A WHILE LOOP?

```c
#include <stdio.h>
int main()
{
   int i=2,n,is_prime=1;
   printf("Enter a number: ");
   scanf("%d",&n);
   if(n<=1){
       is_prime=0;
   }
   else{
       while(i<=n/2){
           if(n%i==0){
               is_prime=0;
               break;
           }
           i++;
       }
   }
   if(is_prime==1){
       printf("%d is a prime",n);
   }
   else{
       printf("%d is not a prime",n);
   }
}
```
### Program 19: WRITE A C PROGRAM TO FIND THE SUM OF DIGITS OF A NUMBER USING A WHILE LOOP?

```c
#include <stdio.h>
int main()
{
    int n,sum=0,digit;
    printf("Enter a number: ");
    scanf("%d",&n);
    while(n!=0){
        digit=n%10;
        sum+=digit;
        n/=10;
    }
    printf("Sum of the didgits are: %d",sum);
}
```
### Program 20: WRITE A C PROGRAM TO PRINT FIBONACCI SERIES UP TO N TERMS USING A FOR LOOP?

```c
#include <stdio.h>
int main()
{
    int i,n,a=0,b=1,next;
    printf("Enter no.of terms to print fibonacci series: ");
    scanf("%d",&n);
    if(n==0){
        printf("not valid for zero");
    }
    if(n>=1){
        printf("%d ",a);
    }
    if(n>=2){
        printf("%d ",b);
    }
    for(i=2;i<n;i++){
            next=a+b;
            printf("%d ",next);
            a=b;
            b=next;
    }
}
```
### Program 21: WRITE A C PROGRAM TO REVERSE A GIVEN NUMBER USING A WHILE LOOP?

```c
#include <stdio.h>
int main()
{
    int n,rem,reverse=0;
    printf("Enter a number: ");
    scanf("%d",&n);
    while(n!=0){
        rem=n%10;
        reverse=reverse*10+rem;
        n/=10;
    }
    printf("Reversed numeber is: %d",reverse);
}
```
### Program 22: WRITE A C PROGRAM TO FIND THE LARGEST ELEMENT IN AN ARRAY USING A FOR LOOP?

```c
#include <stdio.h>
int main()
{
    int i,n,arr[50],largest;
    printf("Enter the size of array: ");
    scanf("%d",&n);
    for(i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    largest=arr[0];
    for(i=1;i<n;i++){
        if(arr[i]>largest){
            printf("%d",largest);
        }
    }
}
```
### Program 23:WRITE A C PROGRAM TO FIND THE SMALLEST ELEMENT IN AN ARRAY USING A WHILE LOOP?

```c
#include <stdio.h>
int main(){
    int i,n,arr[50],smallest;
    printf("Enter the size of the array: ");
    scanf("%d",&n);
    printf("Enter the %d elements: ",n);
    for(i=0;i<n;i++)
    scanf("%d",&arr[i]);
    smallest=arr[0];
    for(i=1;i<n;i++){
        if(arr[i]<smallest){
            smallest=arr[i];
        }
    }
    printf("smallest array element in the given array is: %d",smallest);
}
```
### Program 24: WRITE A C PROGRAM TO PRINT ALL THE ELEMENTS OF AN ARRAY USING A FOR LOOP?

```c
#include <stdio.h>
int main(){
    int i,n,arr[50];
    printf("Enter the size of the array: ");
    scanf("%d",&n);
    printf("Enter the %d elements: ",n);
    for(i=0;i<n;i++)
    scanf("%d",&arr[i]);
    printf("Array elements are: ");
    for(i=0;i<n;i++)
    printf("%d ",arr[i]);
}
```
### Program 25: WRITE A C PROGRAM TO FIND THE SUM OF ELEMENTS IN AN ARRAY USING A WHILE LOOP?

```c
#include <stdio.h>
int main()
{
    int i,n,arr[50],sum=0;
    printf("Enter the size of the array: ");
    scanf("%d",&n);
    printf("Enter %d array elements: ",n);
    for(i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++){
        sum+=arr[i];
    }
    printf("The sum of the given array elements are: %d",sum);
}
```
### Program 26: WRITE A C PROGRAM TO COUNT THE NUMBER OF WORDS IN A GIVEN STRING USING A WHILE LOOP?
