# Rotate-Array-1
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
     int t,x;
     scanf("%d",&t);
    for(x=0;x<t;x++)
    {
        int r,n,i=0,s;
        scanf("%d %d",&r,&n);
        int a[n],c[n];
        for(int y=0;y<n;y++)
            {
                scanf("%d",&a[y]);
                c[y]=a[y];
            }
        s=r-1;
        int z=0;
        while(z<(n-r))
        {
            a[z]=a[z+r];
            z++;
        }
         while(s>=0)
           {
               a[n-s-1]=c[i];
               s--;
             i++;
           } 
        
         for(i=0;i<n;i++)
             printf("%d ",a[i]);
        printf("\n");
    }

    /* Enter your code here. Read input from STDIN. Print output to STDOUT */    
    return 0;
}
