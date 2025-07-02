# C Programming Practice Programs

## 1. Control Statements

### Program 1: 1.WRITE A C PROGRAM TO ACCEPT TWO INTEGERS AND CHECK WHETHER THEY ARE EQUAL OR NOT ?

'''C
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

### Program 2: WRITE A C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS EVEN OR ODD?

'''C
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

### Program 3: .WRITE A C PROGRAM TO CHECK WHETHER A GIVEN NUMBER IS POSITIVE OR NEGATIVE?

'''C
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

### Program 4: WRITE A C PROGRAM TO FIND WHETHER A GIVEN YEAR IS A LEAP YEAR OR NOT?

'''C
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

### Program 5: WRITE A C PROGRAM TO READ THE AGE OF A CANDIDATE AND DETERMINE WHETHER HE IS ELIGIBLE TO CAST HIS/HER OWN VOTE?

'''C
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

### Program 6: WRITE A C PROGRAM TO READ THE VALUE OF AN INTEGER M AND DISPLAY THE VALUE OF N IS 1 WHEN M IS LARGER THAN 0, 0 WHEN M IS 0 AND -1 WHEN M IS LESS THAN 0.

'''C
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

### Program 7:WRITE A C PROGRAM TO FIND THE LARGEST OF THREE NUMBERS?

'''C
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

### Program 8:.WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS A VOWEL OR CONSONANT?

'''C
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

### Program 9:.WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS AN ALPHABET OR NOT?

'''C
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

### Program 10: WRITE A C PROGRAM TO FIND MINIMUM OR MAXIMUM BETWEEN TWO NUMBERS?

'''C
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

### Program 11: WRITE A C PROGRAM TO ENTER WEEK NUMBER AND PRINT DAY OF WEEK?

'''C

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

### Program 12: WRITE A C PROGRAM TO CHECK WHETHER A CHARACTER IS UPPERCASE OR LOWERCASE?

'''C

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

### Program 13: WRITE A C PROGRAM TO FIND NUMBER OF DAYS IN MONTH?

'''C
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

### Program 14: WRITE A C PROGRAM TO FIND MAXIMUM BETWEEN TWO NUMBERS USING SWITCH CASE?
