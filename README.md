# hello-sai
#include<stdio.h>
unsigned long amount=1000,deposit, withdraw;
int choice,pin,k;
main()
{
printf("Enter your secret pin number:");
scanf("%d",&pin);
if(pin!=1250)
printf("Please enter valid password");
do
{
printf("Welcome to ATM service");
printf("Menu\n 1.check balance 2. withdraw cash 3. Deposit cash 4.Quit\n");
printf("Enter choice");
scanf("%d",&choice);
switch(choice)
{
case 1:
printf("your balance is %/n", amount);
break;
case2:
printf("Enter amount to withdraw");
if(withdraw%100!=0)
{
printf("Enter amount in multiples of 100\n");
}
else
if(withdraw>(amount-500))
{
printf("Insufficient balance\n");
}
else
{
amount=amount-withdraw;
pritf("\n Collect the cash");
printf("\n Your balance is %\n", amount);
}
break;
case3:
printf("\nEnter amount to deposit");
scanf("%/n",&deposit);
amount=amount+deposit;
printf("your current balance is %\n", amount); 
case4:
printf("\Thank you for using ATM");
break;
default:
printf("Invalid choice");
}
printf("\nDo u wish to have another transaction?");
scanf("%c",&transaction);
if(transaction=='n'|| transaction=='N')
k=1;
}
while(!k);
printf("\nThanks for using ATM service");
}
