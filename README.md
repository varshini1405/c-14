# c-14
to count vowels,num,spaces,consonants
#include<stdio.h>
int main()
{
    char str[20]="Jamesbond 007";
    int count=0,con=0,digit=0,space=0;
    for(int i=0;str[i]!='\0';i++)
    {
        if(str[i]== 'a'||str[i]=='e'||str[i]=='i'||str[i]=='o'||str[i]=='u'||str[i]=='A'||str[i]=='E'||str[i]=='I'||str[i]=='O'||str[i]=='U')
        {
            count=count++;   
        }
        else if(str[i]=='0'||str[i]=='1'||str[i]=='2'||str[i]=='3'||str[i]=='4'||str[i]=='5'||str[i]=='6'||str[i]=='7'||str[i]=='8'||str[i]=='9')
        {
            digit++;
        }
        else if(str[i]==' '){
            space++;
        }
        else
        {
            con++;   
        }        
    }
    printf("vowels=%d\n",count);
    printf("consonants=%d\n",con);
    printf("no. of digits=%d\n",digit);
    printf("spaces=%d\n",space);
   return 0;
}
