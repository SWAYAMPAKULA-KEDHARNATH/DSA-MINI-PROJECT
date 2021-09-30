//Efficient code for large fibonaci numbers using C language.
#include <stdio.h>
#define N 20000
int main()
{ char a[N],b[N],c[N],carry=0;
  int temp,pre_id=N-1,n,i,j;
  a[N-1]=0;
  b[N-1]=1;
  
  printf("Enter position of Fibonaci number u like to find:");
  scanf("%d",&n);
  
  if(n==0)
    {printf("0");}
  else if(n==1)
    { printf("1");}
  else
    {for(i=2;i<=n;i++)
       {for(j=N-1;j>=pre_id;j--)
           {temp=a[j]+b[j]+carry;
            carry=temp/10;
            c[j]=temp%10;
            if(carry>0&&j==pre_id)
            pre_id--;
            }
            
        for(j=N-1;j>=pre_id;j--)
           {a[j]=b[j];
            b[j]=c[j];
           }
        }
  }
  
  for(j=pre_id;j<N;j++)
  {printf("%d",c[j]);}
    return 0;
}
