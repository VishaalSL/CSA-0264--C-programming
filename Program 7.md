#include <stdio.h>
#include <math.h>

int main() {
    int num, count;
    
    printf("Enter an integer: ");
    scanf("%d", &num);
    
    // Count the number of digits using logarithmic functions
    count = (int)log10(num) + 1;
    
    printf("The number of digits in the given integer is: %d", count);
    
    return 0;
}
