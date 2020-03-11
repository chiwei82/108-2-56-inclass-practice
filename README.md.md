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

  for (long i=10 ; i<(10^17); i=i*10)
  {
    n= n+(P%i)*2;
    P=(P/(i*10));
  }
  
  
  
   
   printf ("%i\n",n) ;
}

