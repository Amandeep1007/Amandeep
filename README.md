#include <stdio.h>

int main() {
 int m,n;
 int choice;
    printf("enter A(1-100):");
    scanf("%d",&m);
    printf("enter B(1-100):");
    scanf("%d",&n);
    
     if(m>0&&m<=33)
    {choice=1;
        printf("STONE");}
    else if(33<m&&m<=66)
    {choice=2;
        printf("PAPER");}
    else if(66<m&&m<=100)
    {choice=3;
        printf("SCISSOR");}
    else
    printf("invalid");
    
    printf("\n");
    
     if(n>0&&n<=33)
    {
        printf("STONE");}
    else if(33<n&&n<=66)
    {
       
        printf("PAPER");}
    else if(66<n&&n<=100)
    {
       
        printf("SCISSOR");}
    else
    printf("invalid");
    
    printf("\n");
    
    switch (choice)
   {
       case 1:
    {
        if(m>0&&m<=33 && n>0&&n<=33)
        printf("ITS A TIE");
        else if(m>0&&m<=33 && n>33&&n<=66)
        printf("PAPER WINS");
        else if(m>0&&m<=33 && n>66&&n<=100)
        printf("STONE WINS");
    break;
        }
    case 2:
    {
        if(m>33&&m<=66 && n>0&&n<=33)
        printf("PAPER WINS");
        else if(m>33&&m<=66 && n>33&&n<=66)
        printf("ITS A TIE");
        else if(m>33&&m<=66 && n>66&&n<=100)
        printf("SCISSOR WINS");
    break;
        } 
    case 3:
    {
        if(m>66&&m<=100 && n>0&&n<=33)
        printf("STONE WINS");
        else if(m>66&&m<=100 && n>33&&n<=66)
        printf("SCISSOR WINS");
        else if(m>66&&m<=100 && n>66&&n<=100)
        printf("ITS A TIE");
    break;
        }
     default:
     printf("invalid choice");
     
   }
    return 0;
}