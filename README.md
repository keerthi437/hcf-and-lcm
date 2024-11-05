#include<stdio.h>
int hcf(int a,int b)
{
    int res = ((a<b)?a:b);
    while(res>0){
        if (a % res == 0 && b % res == 0){
            break;
        }
        res--;
    }
    return res;
}
int main()
{
    int a=56,b=78;
    printf("hcf of %d and %d is %d",a,b,hcf(a,b));
    return 0;
}
