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
