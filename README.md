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
    int max;
    max = (a>b)?a:b;
    while(1)
    {
    if (max%a==0 && max%b == 0)
    {
    printf("the lcm of %d and %d is % d",a,b,max);
    break;
    }
    ++max;
    }   
    
}
int main()
{
    int a=56,b=78,max;
    printf("the lcm of %d and %d is % d\n",a,b,max);
    printf("hcf of %d and %d is %d",a,b,hcf(a,b));
    return 0;
}
