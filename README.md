# demo1
#include <stdio.h>

#include <stdlib.h>

int main(void)

{

FILE *fp=fopen("data.txt","r");

if (!fp)

{

fp=fopen("data.txt","w");

printf("请输入姓名:");

char *name;

scanf("%s",name);

printf("请输入学号:");

char *num;

scanf("%s",num);

fprintf("%s %s",name,num);

fclose(fp);

return 0;

}

char *name,*num;

fscanf("%s %s",name,num);

fclose(fp);

printf("姓名为:%s\n学号为:%s",name,num);

return 0;

}
