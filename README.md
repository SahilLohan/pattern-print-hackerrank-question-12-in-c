# pattern-print-hackerrank-question-12-in-c

#include <stdio.h>

int main()
{
    int n,k,i,j;// change krna h kuch 
   // scanf("%d", &n);
      // Complete the code to print the pattern.
      int arr [(2*n)-1][(2*n)-1];
    n=4+1;
    k=4;
    for(i=1;i<8;i++)
    {
        for(j=1;j<8;j++){
            if(j>=i&&j<((2*n)-i-1)&&i<n)
            printf("%d ",n-i);
            else if(j>=1&&j<i&&i<n)
            printf("%d ",n-j);
            else if(j>=(2*n)-i-1&&i<n)
            printf("%d ",j-n+2);
            else 
            printf("%d ",n);
            
            if(j==7)
            printf("\n");
            
            
        }
    }
    

    return 0;
}



#include <stdio.h>

int main()
{
    int n,k,i,j;
   scanf("%d", &k);
   n=k+1;
      // Complete the code to print the pattern.
    int a[n][n];
    
    
    for(i=1;i<n;i++)
    {
        for(j=1;j<2*k;j++)
        {
            if(j>=i&&j<((2*n)-i-1)&&i<n)
            {printf("%d ",n-i);
            a[i][j]=n-i;
            }
            else if(j>=1&&j<i&&i<n)
            {printf("%d ",n-j);
            a[i][j]=n-j;
                
            }
            else if(j>=(2*n)-i-1&&i<n)
            {printf("%d ",j-n+2);
            a[i][j]=j-n+2;
                
            }
            else 
            {printf("%d ",n);
            a[i][j]=n;
                
            }
            
            if(j==(2*k)-1)
            printf("\n");
        }}
         //now print the niche waali cheej thread_local\n
        
        for(i=k-1;i>=1;i++)
        {
            for(j=1;j<2*k;j++)
            {   if(j<k+2)
                printf("%d ",a[i][j]);
                else if(j>=k+2)
                {
                    printf("%d ",a[i][(2*k)-j]);
                }
                if(j==(2*k)-1)
            printf("\n");
                
             }
             i--;
             i--;
        }
    
    

    return 0;
}

