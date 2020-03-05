# 108-2-56-inclass-practice
 108-2-56節 資料科學程式設計（一） 課堂練習
 
#include <stdio.h>
#include <cs50.h>
#include <string.h>

   typedef struct
     {
      string name;
      string number;
     }
   person;

   int main (void)
     {
      person people[4];
 


   for (int i =0 ; i<4 ; i++)
     {
        if ( strcmp(people[i].name,"EMMA") == 0 )
        {
            printf("%s\n",people[i].number);
            return 0;
        }
     }
        printf("not found\n")
        return 1;
     }