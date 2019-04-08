#include <stdio.h>
#include <stdlib.h>

int main(void)
{
  int i, j, max, sum = 0;
  printf("請輸入最大值 => ");
  scanf("%d", &max);
  
  for(i = max; i >= 1; i--){
        printf("|%d|", i);
        sum += i;
}
  printf(" ==>從%d加到1的總和=%d\n", max, sum);
  
  for(i = max, j = 1, sum = 0; i >= 1;i--, j++, printf("\n"))
{
       printf("|%d-%d|", i, j);
       sum += i;
       sum += j;
       }
       printf(" ==>總和=%d\n", sum);
       system("PAUSE");
       return 0;
} 
