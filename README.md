# C_Calculator
#include <stdio.h>  
int main()  
{  
    // declare local variables  
    char optn;  
    int n1, n2;   
    float res;  
    printf (" Choose an operator(+, -, *, /) to perform the operation in C Calculator \n ");  
    scanf ("%c", &optn); // to take an operator  
    if (optn == '+' )  
    {  
        printf (" You have selected: Addition");  
    }  
    else if (optn == '-')  
    {  
        printf (" You have selected: Subtraction");  
     }  
       
    else if (optn == '*')  
    {  
        printf (" You have selected: Multiplication");  
     }  
        else if (optns == '/')  
    {  
        printf (" You have selected: Division");  
     }     
    printf (" \n Enter the first number: ");  
    scanf(" %d", &n1); // to take fist number  
    printf (" Enter the second number: ");  
    scanf (" %d", &n2); // to take second number  
      
    switch(optn)  
    {  
        case '+':  
            res = n1 + n2; // to add two numbers  
            printf (" Addition of %d and %d is: %.2f", n1, n2, res);  
            break;  
          
        case '-':  
            res = n1 - n2; // to subtract two numbers  
            printf (" Subtraction of %d and %d is: %.2f", n1, n2, res);  
            break;  
              
        case '*':  
            res = n1 * n2; //to multiply two numbers  
            printf (" Multiplication of %d and %d is: %.2f", n1, n2, res);  
            break;            
          
        case '/':  
            if (n2 == 0)   // if n2 == 0, take another number  
            {  
                printf (" \n Divisor cannot be zero,it will tends to infinity.So, Please enter another value ");  
                scanf ("%d", &n2); //div defined as a float & cast any one variable n1 or n2       
                }  
            res = n1 /(float)n2; //to divide two numbers  
            printf (" Division of %d and %d is: %f", n1, n2, res);  
            break;  
        default:  /* use default to print default message if any condition is not satisfied */  
            printf (" Incorrect option! Please click the correct options ");               
    }  
    return 0;  
}  
