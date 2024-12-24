PRINTING PATTERN:
1

2*3

4*5*6

7*8*9*10

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows/columns as input from the user and store it in any variable.(‘r‘ in this case).
Run a loop ‘r’ number of times to iterate through each of the rows. From i=0 to i<r The loop should be structured as for( i=0 ; i<r: i++).
Run a nested loop to iterate through the columns. From j=0 to j<r. The loop should be structured as for(j=0 ; j<r; j++).
increment count and run an if condition if(j!=0).
if true then print star and count else print only count.
outside the nested loop print a newline
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,r,count;                                      //declaring integer variables i,j for loops , r for number of rows and count for increment in value
count=0;                                              //initialising count
printf("Enter the number of rows :\n");               //Asking user for input
scanf("%d",&r);                                       //taking number of rows and saving it in variable r
for(i=0;i<r;i++)                                      // loop for number of rows
  {
    for(j=0;j<=i;j++)                                 // loop for digits per each row
      {
        count++;                                      //incrementing count
        if(j!=0)                                      //if statement to print star and digit
        printf("*%d",count);                          //printing star and digit
        else                                          //else statement to print only digit 
        printf("%d",count);                           //printing digits
      }
    printf("\n");                                     // printing newline after each row
  }
}
TAKING INPUT:DISPLAYING OUTPUT:

