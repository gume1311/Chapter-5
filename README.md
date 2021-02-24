# Chapter-5
Solve the the exercises from chapter 5 of "Practical C programming" and add an original exercise.  Upload all exercises to a new folder in github called "chapter5" and attach just only that link.

### Exercise 5-1: Write a program that converts Centigrade to Fahrenheit.

```c
#include <stdio.h>
float temp_f;     /* degrees fahrenheit */
float temp_c;     /* degrees centigrade */
char line_text[50];        /* a line of input */

int main() {
	printf("Input a temperature (in Centigrade): ");
	fgets(line_text, sizeof(line_text), stdin);
	sscanf(line_text, "%f", &temp_c);

	temp_f = ((9.0 / 5.0) * temp_c) + 32.0;
	printf("%f degrees Fahrenheit.\n", temp_f);

	return(0);
}

```
