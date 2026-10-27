#include <stdio.h>
#include <string.h>
int main()
{
 char name[50]={0};
 char response[10]={0};
 char responses[]="Yes";
 int repon;
 int arr[50]={},i=0;
 int store;
 int ans;
 printf("Hey I am Swarup a Mind Reader\n");
 printf(" Tell Me Your Name: ");
 scanf("%s",name);
 printf("Hello %s So Do You Want To Play With me? I Will Read Your Mind: ",name);
 scanf("%s",response);
 while (strcmp(response,responses)==0)
 {
  printf("Ok, Lets play!!!\n");
  printf("Think a Large Number Then Enter 1\n");
  printf("(You Can Use Pen & Paper If You Want, %s)\n",name);
  scanf("%d",&repon);
  if (repon==1)
  {
   printf("GreatJob! Now Scramble Those Numbers, & Make an Another Number & Enter 1: ");
   scanf("%d",&repon);
   if (repon==1)
   {
    printf("Now You Have 2 Numbers, Substract the smaller one from bigger one, Then Enter 1: ");
    scanf("%d",&repon);
    if (repon==1)
    {
     printf("Now You Have Only One Number, From That SKIP One Number in Your Mnd\n");
     printf("                                         (DONT SKIP 0)\n                                                                ");
     printf("Now Tell Me The Remainig Numbers After Skipping One Number: ");
     scanf("%d",&arr[i]);
     {
      while (arr[i])
      {
       store=arr[i]+arr[i+1];
       i=i+1;
      }
      if (store<=9)
      {
       ans=9-store;
       printf("You Skipped %d",ans);
       break;
      }
      if (store<=18)
      break;
      {
       ans=18-store;
       printf("You Skipped %d",ans);
       break;
      }
      if (store<=27)
      {
       ans=27-store;
       printf("You Skipped %d",ans);
       break;
      }
     }
    }
   }
  }
 }
}
 


   
 






















     
