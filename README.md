#include <stdio.h>
int main()
{
   long int binaryval, hexadecimalval = 0, i = 1, remainder;
   scanf("%ld", &binaryval);
   while (binaryval != 0)
     {
        remainder = binaryval % 10;
        hexadecimalval = hexadecimalval + remainder * i;
        i = i * 2;
        binaryval = binaryval / 10;
     }

    printf("%lX", hexadecimalval);

    return 0;

}
