---
date: 2017-11-01T00:17:39-04:00
title: "Getting Input From Users"
seo_title: "Getting Input From Users | C | Mike Dane"
subheader:
     greeting: C - Programming Language
     description: This course covers the basics of programming in C. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers getting input from users in C.
author: Mike Dane
image: getting-input-from-users.png
video: SHs2k3GfS0M
url: /programming-languages/c/getting-input-from-users/
weight: 12
---

## Code

{{< code lang="c" >}}
// strings
char name[10];
printf("Enter your name: ");
fgets(name, 10, stdin);
printf("Hello %s! \n", name);

// ints
int age;
printf("Enter your age: ");
scanf("%d", &age);
printf("You are %d \n", age);

// chars
char grade;
printf("Enter your grade: ");
scanf("%c", &grade);
printf("You got an %c on the test \n", grade);

// doubles
double gpa;
printf("Enter your gpa: ");
scanf("%lf", &gpa);
printf("Your gpa is %f \n", gpa);
{{< /code >}}