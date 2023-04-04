#include <stdio.h>

int main() {
    int amount, notes, rem;
    int denominations[] = {500, 100, 50, 20, 10, 5, 2, 1};
    int i;

    printf("Enter the amount: ");
    scanf("%d", &amount);

    printf("Denominations:\n");

    for (i = 0; i < 8; i++) {
        notes = amount / denominations[i];
        if (notes != 0) {
            printf("%d notes of Rs %d\n", notes, denominations[i]);
        }
        rem = amount % denominations[i];
        amount = rem;
    }

    return 0;
}
