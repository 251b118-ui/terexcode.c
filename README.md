#include <stdio.h>
#include <string.h> //For using functions like strlen,strcpy,strcat, etc.
 void lowercase_to_uppercase_uppercase_to_lowercase(char str[100])
 { int n = strlen(str);
   int i;
   for(i = 0; i < n ;i++)
   { if (str[i] >= 'A' && str[i]<= 'Z') // Using ASCII values for conversion.
      str[i] += 32;
      else if(str[i] >= 'a' && str[i]<= 'z')
      str[i] -=32;
    }}
 int main()
 { char str[100];
   printf("Enter string: ");
   fgets(str,sizeof(str),stdin);
   lowercase_to_uppercase_uppercase_to_lowercase(str);
   printf("\nSorted string: ");
   printf("%s",str);
   return 0;
 }
   
