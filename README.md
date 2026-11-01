 simple_calculator
 I have built a simple calculator using c 
 

#include<stdio.h>

#include<math.h>

double sum(double a , double b);

double diff(double a , double b);

double prod(double a , double b);

double div(double a , double b);


double rem(double a ,double b);
 
 //function prototype/declaration

int main() {

double a,b;

printf("enter first number :\n ");

scanf("%lf",&a);

printf("enter secomd number : \n");

scanf("%lf",&b);

 double s= sum(a,b);

double d = diff(a,b);

double p= prod(a,b);

printf(" the sum is %lf \n",s);        

//function call a+b

printf("the difference is %lf  \n",d);   //function call a-b

printf("the product is %lf \n",p);        //function call a*b

//condition check if division by zero error doesnot arrise

if (b==0) {

printf("Invalid ! Division by zero is not possible"); }
 
else {

double q =div(a,b);    //function call

double r = rem(a,b);   //function call

printf("The quotient is %lf \n",q);

printf("the remainder is %lf \n",r); }

return 0;
 }

//function definations 

double sum(double a, double b) {
return a + b;
}


double diff( double a , double b){
return a-b;
}


double prod(double a, double b){
return a*b;
 }
 

double div(double a , double b)  {
return a/b;
 }
 

double rem(double a , double b)  {
 return fmod(a,b);
}
