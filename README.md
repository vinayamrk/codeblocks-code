# codeblocks-code
code for fibonacs series
#include <stdio.h>
main()
{
    int t1=0,t2=1,t3,i,n;
    printf("number of terms in series:");
    scanf("%d",&n);
    if(n==1)
        printf("the fibonacci series;%d",t1);
    else if(n>=2)
    {
        printf("the fibonacci series:%d %d",t1,t2);
        for(i=3; i<=n; i++)
        {
            t3=t1+t2;
            printf(" %d",t3);
            t1=t2;
            t2=t3;

        }
    }
    else
        printf("invalid no of terms");
}
