# Project-file
#include <stdio.h>

int main() {
    float input;
    int option;

    printf("Unit Converter\n");
    printf("1. Kilometers to Miles\n");
    printf("2. Miles to Kilometers\n");
    printf("3. Celsius to Fahrenheit\n");
    printf("4. Fahrenheit to Celsius\n");
    printf("Enter your choice: ");
    scanf("%d", &option);

    switch(option) {
        case 1:
            printf("Enter distance in kilometers: ");
            scanf("%f", &input);
            printf("%.2f km = %.2f miles\n", input, input * 0.621371);
            break;
        case 2:
            printf("Enter distance in miles: ");
            scanf("%f", &input);
            printf("%.2f miles = %.2f km\n", input, input * 1.60934);
            break;
        case 3:
            printf("Enter temperature in Celsius: ");
            scanf("%f", &input);
            printf("%.2f C = %.2f F\n", input, (input * 9 / 5) + 32);
            break;
        case 4:
            printf("Enter temperature in Fahrenheit: ");
            scanf("%f", &input);
            printf("%.2f F = %.2f C\n", input, (input - 32) * 5 / 9);
            break;
        default:
            printf("Invalid option selected\n");
            break;
    }

    return 0;
}
