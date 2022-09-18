#include<stdio.h>
int main()
{
    int a, b, c;
    printf(" first: ");
    scanf_s("%d", &a);
    printf(" second: ");
    scanf_s("%d", &b);
    printf(" third: ");
    scanf_s("%d", &c);
    if ((a == 0 && b == 0)||(a == 0 && c == 0)||(b == 0 && c == 0))
    {
        printf("Nuli ne protivopolzhnie");
        return 0;
    }
    if (a == -b || a == -c || b == -c)
    {
        if (a == -b)
        {
            printf("%d", c);
        }
        else
        {
            if (a == -c)
            {
                printf("%d", b);

            }
            else
            {
                if (b == -c)
                {
                    printf("%d", a);
                }
            }
        }
    }
    else
        printf("No");
    return 0;
}
