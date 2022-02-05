//# Sum-of-diagonal-elements-of-matrix-in-C
// Program to initialize a 3x3 array, insert elements into the array, read and print an array of elements using only pointers. Also find and print the sum of all diagonal elements.

#include<stdio.h>
int main()
{
  int i,j,rows,columns,a[10][10],sum=0;
  printf("\n Please enter number of rows and columns: ");
  scanf("%d %d",&i,&j);
  printf("\n Please enter the matrix elements: ");
  for(rows=0;rows<i;rows++)
  {
    for(columns=0;columns<j;columns++)
    {
      scanf("%d",&a [rows][columns]);
    }
  }
  for(rows=0;rows<i;rows++)
  {
    sum=sum+a[rows][rows];
  }
  printf("\n The sum of the diagonal elements of the matrix= %d",sum);
  return 0;
}
      
