编写代码实现，模拟用户登录情景，并且只能登录三次（只允许输入三次密码，如果密码正确则提示登录成功，否则三次均输入错误，则退出程序


#define _CRT_SECURE_NO_WARNINGS

#include<stdio.h>

#include<string.h>

#include<stdlib.h>

int main()
{
    char wl[10] = "  ";
    
    int i;
    
    for (i = 0; i < 3; ++i)
    {
        printf("please  input:");
        
        scanf("%s",&wl);
        
        if (strcmp(wl, "love") == 0)
        
            break;
            

        if (i == 3)
        
            return 0;
        else
        
            printf("继续\n");
    }
}
