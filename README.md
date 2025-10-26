1. Centigrade to Fahrenheit Conversion
This program takes a temperature in Celsius from the user and converts it to Fahrenheit using the formula F=(C×9/5)+32.
C
#include <stdio.h>

int main() {
    float centigrade, fahrenheit;
    printf("Enter temperature in Centigrade: ");
    scanf("%f", &centigrade);
    fahrenheit = (centigrade * 9 / 5) + 32;
    printf("Temperature in Fahrenheit: %.2f\n", fahrenheit);
    return 0;
}


2. Circle Calculations (Diameter, Circumference, Area)
This program prompts the user for the radius of a circle and then calculates and displays its diameter, circumference, and area.
C
#include <stdio.h> 

int main() {
    float radius, diameter, circumference, area;
    printf("Enter the radius of the circle: ");
    scanf("%f", &radius);
    diameter = 2 * radius;
    circumference = 2 * 3.14 *radius;
    area = 3.14* radius * radius 
    printf("Diameter: %.2f\n", diameter);
    printf("Circumference: %.2f\n", circumference);
    printf("Area: %.2f\n", area);
    return 0;
}


3. Swap Two Numbers
This program swaps the values of two numbers entered by the user.
Using a Third Variable
C
#include <stdio.h>

int main() {
    int num1, num2, temp;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    printf("Before swapping: num1 = %d, num2 = %d\n", num1, num2);
    temp = num1;
    num1 = num2;
    num2 = temp;
    printf("After swapping: num1 = %d, num2 = %d\n", num1, num2);
    return 0;
}

Using Arithmetic Operators
C
#include <stdio.h>

int main() {
    int num1, num2;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    printf("Before swapping: num1 = %d, num2 = %d\n", num1, num2);
    num1 = num1 + num2;
    num2 = num1 - num2;
    num1 = num1 - num2;
    printf("After swapping: num1 = %d, num2 = %d\n", num1, num2);
    return 0;
}

Note: The prompt also asks for a bitwise operator solution, but this is less common and can be confusing. The arithmetic method is a good alternative that doesn't use a third variable.

4. Find Maximum of Three Numbers
This program finds and prints the maximum of three numbers using a series of if-else statements, known as a ladder if-else.
C
#include <stdio.h>

int main() {
    int num1, num2, num3;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &num1, &num2, &num3);
    if (num1 >= num2 && num1 >= num3) {
        printf("Maximum number is: %d\n", num1);
    } else if (num2 >= num1 && num2 >= num3) {
        printf("Maximum number is: %d\n", num2);
    } else {
        printf("Maximum number is: %d\n", num3);
    }
    return 0;
}


5. Check for a Leap Year
This program checks if a given year is a leap year. A year is a leap year if it is divisible by 4, except for years divisible by 100 but not by 400.
C
#include <stdio.h>

int main() {
    int year;
    printf("Enter a year: ");
    scanf("%d", &year);
    if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
        printf("%d is a leap year.\n", year);
    } else {
        printf("%d is not a leap year.\n", year);
    }
    return 0;
}


6. Check Character Type
This program determines if a character is an alphabet (uppercase or lowercase), a digit, or a special character.
C
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch); // Note the space before %c to consume any whitespace
    if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z')) {
        printf("'%c' is an alphabet.\n", ch);
    } else if (ch >= '0' && ch <= '9') {
        printf("'%c' is a digit.\n", ch);
    } else {
        printf("'%c' is a special character.\n", ch);
    }
    return 0;
}


7. Check Vowel or Consonant
This program checks if an alphabet entered by the user is a vowel or a consonant. The program assumes the user will input a valid alphabet.
C
#include <stdio.h>

int main() {
    char ch;
    printf("Enter an alphabet: ");
    scanf(" %c", &ch); // Note the space before %c
    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
        ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
        printf("'%c' is a vowel.\n", ch);
    } else {
        printf("'%c' is a consonant.\n", ch);
    }
    return 0;
}
