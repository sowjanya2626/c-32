# c-32
Reverse a string by using an user defined function and pass the string to the sub function to get the reverse string
#include<stdio.h>
#include<string.h>
void rstring(char str[])
{
    int len=strlen(str);
    for(int i=0;i<len/2;i++){
        char temp=str[i];
        str[i]=str[len-i-1];
        str[len-i-1]=temp;
    }
}
int main()
 {
     char str[]="Gunasree";
     printf("original string:%s\n",str);
     rstring(str);
     printf("reversed string:%s",str);
     return 0;
     
 }
