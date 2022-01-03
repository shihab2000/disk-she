# disk_she_fcfs
#include<stdio.h>
void main()
{
	int a[30],n,i,head,seek;
	printf("ENTER THE  NUMBER OF REQUEST : ");
	scanf("%d",&n);
	printf("ENTER THE HEAD POSITION : ");
	scanf("%d",&head);
	printf("ENTER THE SEQUENCE  :");
	for(i=0;i<n;i++)
		scanf("%d",&a[i]);
	
	
	for(i=0;i<n;i++)
	{
	   printf("%d-->",head);
       seek=seek + abs(a[i]-head);
	   head=a[i];
   }
   		if(i=n)
   		printf("%d  ...",head);
   		
   		printf("\n total seek time =%d",seek);

  }
