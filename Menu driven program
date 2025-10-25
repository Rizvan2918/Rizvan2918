#include <stdio.h>

int main() {
    int num, choice, i, fact, flag;

    while (1) {
        printf("\n===== MENU =====\n");
        printf("1. Find Factorial\n");
        printf("2. Check Prime or Not\n");
        printf("3. Check Odd or Even\n");
        printf("4. Exit\n");
        printf("Enter your choice (1-4): ");
        scanf("%d", &choice);

        if (choice == 4) {
            printf("Exiting program... Goodbye!\n");
            break;
        }

        printf("Enter a number:");
        scanf("%d", &num);

        switch (choice) {
            case 1:
                fact = 1;
                for (i = 1; i <= num; i++) {
                    fact *= i;
                }
                printf("Factorial of %d = %d\n", num, fact);
                break;

            case 2:
                flag = 0;
                if (num < 2) {
                    flag = 1;
                } else {
                    for (i = 2; i <= num / 2; i++) {
                        if (num % i == 0) {
                            flag = 1;
                            break;
                        }
                    }
                }
                if (flag == 0)
                    printf("%d is a Prime Number.\n", num);
                else
                    printf("%d is NOT a Prime Number.\n", num);
                break;

            case 3:
                if (num % 2 == 0)
                    printf("%d is Even.\n", num);
                else
                    printf("%d is Odd.\n", num);
                break;

            default:
                printf("Invalid choice! Please select between 1 to 4.\n");
        }
    }

    return 0;
}
