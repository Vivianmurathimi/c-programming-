# c-programming-;loops

#contains line of code of various loops with their examples.
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
// for looops
// Write a C program that prints the first n terms of the Fibonacci series.
// The Fibonacci series starts with 0 and 1, and each subsequent term is the sum of the two preceding ones.
/*int main()
{
  //first we prompt the user input
  int n;
  printf("enter the nth term of the series\n");
  scanf("%d",&n);
//validate the user input
if (n<=0){
    printf("the input is invalid");
return 1;// in this case it shows an error because return 0 shows the output is successful.
}
int firstnum = 0;
int secondnum = 1;

for(int i=1;i<=n;i++)
    {
    printf("%d",firstnum);
int next= firstnum + secondnum;
//update now
firstnum= secondnum;
secondnum= next;
}
printf("\n");// just giving a new line.
return 0;
}*/
//Write a C program that uses a for loop to print a pattern of asterisks.
//The program should prompt the user to enter the number of rows for the pattern and
//then display a pattern where each row has the same number of asterisks as its row number.
//*
//**

/*int main(){
//enter no of rows
int rows;
printf("enter no of rows\n");
scanf("%d",&rows);
//check if rows are more than 1..validate rows
if(rows<1){
    printf("invalid input");
    return 1;
}
for(int i=1 ;i<=rows ;i++){
    printf("\n",rows);
        for(int j=1;j<=i;j++){
        printf("*",rows);
        }
}
  return 0;
}*/
//Write a C program that uses a for loop to print a reversed pattern of numbers.
 //The program should prompt the user to enter the number of rows for the pattern
//then display a pattern where each row has numbers in descending order from the total number of rows to 1.

/*int main()
{
    int num;
    printf("enter no of numbers :");
    scanf("%d",&num);
for(int i=num ;i>=1 ;i--)
{
    printf("%d\n",i);
}
return 0;*/
//WHILE LOOPS EG
// write a code that continues only when the user writes their name
/*int main()
{//use input name
    char name[30];

    printf("what is your name?");
    fgets(name,30,stdin);// this includxes the new line character when you enter therfore
    name[strlen(name)-1]='\0'; //this is for removing that firs character.

    while(strlen(name)==0)// in this case note that the strlen here is used to count the characters.
    //(characters counted =0 )?then the person didnt write anthing
        {
    printf("you did not write your name\n");
    printf("what is your name?\n");
    fgets(name,30,stdin);
    name[strlen(name)-1]='\0';
}

printf("hello %s",name);
return 0;

}*/
//Write a C program that prompts the user to enter a positive integer.
//The program should use a while loop to repeatedly ask the user for input until a positive integer is entered.
//Once a positive integer is provided, the program should display the square of that number.
/*int main()
{
    int num;
printf("enter an integer\n");
scanf("%d",&num);
while (num<=0)
    {
        printf("enter a positive integer\n");
printf("enter an integer\n");
scanf("%d",&num);
}
printf("the square of%d is %d",num,num*num);
return 0;
}*/
//Write a C program that prompts the user to guess a secret number between 1 and 10.
//The program should generate a random secret number and use a while loop to repeatedly ask the user for their guess until they correctly guess the number.
//Provide hints such as "Too high" or "Too low" after each incorrect guess.
/*int main()
{
    int num=4;
   int sectretnum;
while( sectretnum>=0);
{
    printf("guess a secret number between 1 and 10\n");
    scanf("%d",&sectretnum);
    if(sectretnum<num){
        printf("too low\n");
    }
        else if(sectretnum==num)
        {
            printf("you got it!\n");
            break;
        }
        else{
            printf("too high\n");
        }
}while( sectretnum>=0);
return 0;
}*/
//continue and break
int main()
{
    for(int i=0 ;i<=10;i++)
    {
        if (i==7){
            break;// exists the loop or switch.
        }// continue  skips the rest of the code and forces the next iteration of the loop.
        printf("%d",i);
    }
}

