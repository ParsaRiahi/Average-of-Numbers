# Average-of-Numbers
Originally called moadel.c

#include <stdio.h>

int main (void)
{
    float input;
    float output = 0;
    int counter = -1;

    printf("\nPlease Enter all the numbers you want the moadel from.\nPress 0 to end it: ");

    while(1)
    {
        if(input != 0)
        {     
            scanf("%f", &input);
            printf("\nMore: ");
            output = output + input;
            counter = counter + 1;
        }
        else if(input == 0)
        {
            break;
        }  
    }
    output = output / counter;
    printf("%.2f", output);

    return 0;
}
