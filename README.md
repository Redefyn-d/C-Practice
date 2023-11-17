# C-Practice
C Question to practice to help you improve your skills 
//Program to print the area of square and rectangle
#include <stdio.h>
int main(){
    int a,l,b;
    printf("Enter the length of side of a square");
    scanf("%d",&a);
    printf("Area of the given square with sides as %d is:%d",a,a*a);
    printf("\nEnter the value of length and breadth");
    scanf("%d%d",&l,&b);
    printf("Area of the given rectangle with length %d and breadth %d is:%d",l,b,l*b);
}
//Program to findd the largest of the three numbers
#include <stdio.h>
int main(){
    int a,b,c;
    printf("Enter the three numbers");
    scanf("%d%d%d",&a,&b,&c);
    if (a>b&&a>c){
        printf("A is largest of the three");
    }
    else if (b>a&&b>c){
        printf("B is largest of the three");
    }
    else{
        printf("C is largest of the three");
    }
}
//Program to print the tables of the number input
#include <stdio.h>
int main(){
    int x;
    printf("Enter the number for which you want to print tables");
    scanf("%d",&x);
    for (int i=1;i<=10;i++){
        printf("%dx%d=%d\n",x,i,x*i);
    }
}
//Proogram to print Even number upto a range
#include <stdio.h>
int main(){
    int x;
    printf("Enter the range of numbers");
    scanf("%d",&x);
    for (int i=0;i<=x;i++){
        if (i%2==0){
            printf("%d\n",i);
        }
    }
}
//Program to print average of odd numbers below range 
#include <stdio.h>
int main(){
    int x;
    printf("Enter the range ");
    scanf("%d",&x);
    for (int i=0;i<x;i++){
        if(i%2!=0){
            printf("%d\n",i);
        }
    }
}
//program to print net salary of an employee
#include <stdio.h>
int main(){
    int sal,ctc,tax;
    printf("Enter the salary of the employee");
    scanf("%d",&sal);
    printf("Enter the cost to company and tax to be paid");
    scanf("%d%d",&ctc,&tax);
    printf("Net salary of the employee is:%d",sal-ctc-tax);
}
//Program to print result of student
#include <stdio.h>
int main(){
    int s1,s2,s3;
    printf("Enter the marks for three subjects");
    scanf("%d%d%d",&s1,&s2,&s3);
    if (s1+s2+s3>=150){
        printf("The student has passed his exams");
    }
    else{
        printf("The student has successfully failes the exams");
    }
}
//Program to print prime numbers
#include <stdio.h>
int main(){
    int x;
    printf("Enter the value till which you want to print the prime numbers");
    scanf("%d",&x);
    for (int i=0;i<=x;i++){
        if (i%10==1||i%10==3||i%10==5||i%10==7){
            printf("%d\n",i);
        }
    }
}
//Program to print perfect numbers
#include <stdio.h>
int main(){
    int x,sum=0;
    printf("Enter the number");
    scanf("%d",&x);
    for (int i=1;i<=x;i++){
        if(x%i==0){
        sum+=i;
        }
    }
    if(sum==x*2){
        printf("The number is perfect number");
    }
    else{
        printf("The number is not a perfect number");
    }
}
//Program to print armstrong number
#include <stdio.h>
#include <math.h>
int main(){
    int x,cp,sum;
    printf("Enter a number");
    scanf("%d",&x);
    cp=x;
    while (cp!=0){
        sum+=pow(cp%10,3);
        cp/=10;
    }
    if (sum==x){
        printf("The number is armstrong number");
    }
    else {
        printf("The number is not armstrong number");
    }
}
//program to print palindrome number
#include <stdio.h>
int main(){
    int x,c,sum;
    printf("Enter A Number");
    scanf("%d",&d);
    c=x;
    while(c!=0){
        sum=sum*10+c;
        c/=10;
    }
    if(c==x){
        printf("The number is a palindrome");
    }
    else{
        printf("The number is not a plaindrome");
    }
}
//Program to print wether a character is vowel or not 
#include <stdio.h>
int main(){
    char x;
    printf("Enter the character");
    scanf("%c",&x);
    if(x=='a'||x=='e'||x=='i'||x=='o'||x=='u'){
        printf("The character is a vowel:");
    }
    else{
        printf("The character is not vowel:");
    }
}
//Program to print sum of digits of a number
#include <stdio.h>
int main(){
    int x,sum;
    printf("Enter the number");
    scanf("%d",&x);
    while(x!=0){
        sum+=x%10;
        x/=10;
    }
    printf("Sum of the digits is :%d",sum);
}
//Program to create a four function calculator
#include <stdio.h>
int main(){
    char x;
    int a,b;
    printf("Enter the character");
    scanf("%c",&x);
    printf("Enter two numbers");
    scanf("%d%d",&a,&b);
    switch(x){
        case '+':
        printf("%d",a+b);
        break;
        case '-':
        printf("%d",a-b);
        break;
        case '*':
        printf("%d",a*b);
        break;
        case '/':
        printf("%d",a/b);
        break;
    }
    return 0;
}
