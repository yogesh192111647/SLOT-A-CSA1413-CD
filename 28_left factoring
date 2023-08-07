#include<stdio.h> 
#include<string.h> 
#define SIZE 10 
 int main() { 
 char nterm,beta,alpha,prod[10][SIZE]; 
 int num,index=3; 
 printf("Enter Number of Production : "); 
 scanf("%d",&num); 
 printf("Enter the grammar as E->E-A :\n"); 
 for(int i=0;i<num;i++){ 
 scanf("%s",prod[i]); 
 } 
 for(int i=0;i<num;i++){ 
 printf("\nGRAMMAR : : : %s",prod[i]); 
 nterm=prod[i][0]; 
 if(nterm==prod[i][index]) { 
 alpha=prod[i][index+1]; 
 printf(" is left recursive.\n"); 
 while(prod[i][index]!=0 && prod[i][index]!='|') 
 index++; 
 if(prod[i][index]!=0) { 
 beta=prod[i][index+1]; 
 printf("Grammar without left recursion:\n"); 
 printf("%c->%c%c\'",nterm,beta,nterm); 
 printf("\n%c\'->%c%c\'|E\n",nterm,alpha,nterm); 
 } 
 else 
 printf(" can't be reduced\n"); 
 } 
 else 
 printf(" is not left recursive.\n"); 
 index=3; 
 }
}
