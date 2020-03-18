# 108-2-56-inclass-practice
 108-2-56節 資料科學程式設計（一） 課堂練習
#include <cs50.h>
#include <stdio.h>
#include <math.h>

int main (void)
{
  long credit;
  int n=0; // sum the second-to-last digit
  credit=get_long("Number: ");
  long P=credit;
  long Q=credit;

  for ( int i=0 ; i<9 ; i++ )
  {
    long r = (P%10) ;
    n=n+r;
    P=(P/100);
    printf("i:%i",i+1);
    printf(" r:%li",r);
    printf(" n:%i",n);
    printf(" P:%li",P);
    printf("\n");
  }    

  printf("\n");
  Q=Q/10;
  printf("Q:%li\n",Q);

  for ( int i=0 ; i<9 ; i++ )
  {
    long s = (Q%10)*2 ;
    if (s>10)
    {
      n=n+(s/10)+(s%10);
      Q=(Q/100);
    }
    else
    {
      n=n+s;
      Q=(Q/100);
    }
    printf("i:%i",i+1);
    printf(" s:%li",s);
    printf(" n:%i",n);
    printf(" Q:%li",Q);
    printf("\n");
  }
  if(n%10 ==0)
  {
      
  }
  printf("n:%i\n",n);
}
