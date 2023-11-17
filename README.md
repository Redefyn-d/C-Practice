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
