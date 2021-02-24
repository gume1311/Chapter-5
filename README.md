# Chapter-5
Solve the the exercises from chapter 5 of "Practical C programming" and add an original exercise.  Upload all exercises to a new folder in github called "chapter5" and attach just only that link.

### Exercise 5-1: Write a program that converts Centigrade to Fahrenheit.

```c
#include <stdio.h>
float temp_f;     
float temp_c;    
char line_text[50];       

int main() {
	printf("Escribe tu temperatura (in Centigrade): ");
	fgets(line_text, sizeof(line_text), stdin);
	sscanf(line_text, "%f", &temp_c);

	temp_f = ((9.0 / 5.0) * temp_c) + 32.0;
	printf("%f degrees Fahrenheit.\n", temp_f);

	return(0);
}

```
### Exercise 5-2: Write a program to calculate the volume of a sphere.

```c
#include <stdio.h>
float myradius;   
float myvolume;              
const float PI = 3.14159265358979323846264338327950288419716939937510;

int main() {
	printf("Input the radius of the sphere : ");
	
	myvolume = (4.0 / 3.0) * PI * (myradius * myradius * myradius);  /* volumn=(4/3) * pi * r^3*/
	printf("The volume of sphere is %f.\n", myvolume);

	return(0);
}

```

### Exercise 5 -4: Write a program that converts kilometers per hour to miles per h our.
miles = (kilometer ·0.6213712

```c
#include <stdio.h>
float kmph;              
float miph;              

int main()
{
	printf("Input kilometers per hour: ");

	miph = (kmph * 0.6213712);
	printf("%f miles per hour\n", miph);

	return(0);
}

```

### Exercise 5-5: Write a program that takes hours and minutes as input, and then
outputs the total number of minutes. (1 hour 30 minutes = 90 minutes).

```c
#include <stdio.h>
int hrs;          / horas/
int mins;         
int tot_mins;     / total de horas/

const int MINaHOUR = 60;     

int main() {
	printf("Input hours: ");
	printf("Input minutes: ");
	tot_mins = mins + (hrs * MINaHOUR);
	printf("Total: %d minutes.\n", tot_mins);

	return(0);
}
```
###Exercise 5 -6: Write a program that takes an integer as the number of minutes, and
outputs the total hours and minutes (90 minutes = 1 hour 30 minutes).

```c
#include <stdio.h>
int tot_mins;  /* given number of minutes */
int hrs;          /* number of hours (to be computed) */
int mins;        /* number of minutes (to be computed) */

const int MINaHOUR = 60;      /* number of minutes in an hour */

int main() {
	printf("Input minutes: ");
	fgets(line_text, sizeof(line_text), stdin);
	sscanf(line_text, "%d", &tot_mins);

	hrs = (tot_mins / MINaHOUR);
	mins = (tot_mins % MINaHOUR);
printf("%d Hours, %d Minutes.\n", hrs, mins);

	return(0);
}
```
