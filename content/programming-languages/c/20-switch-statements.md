---
date: 2017-11-01T00:17:46-04:00
title: "Switch Statements"
seo_title: "Switch Statements | C | Mike Dane"
subheader:
     greeting: C - Programming Language
     description: This course covers the basics of programming in C. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers switch statements in C.
author: Mike Dane
image: switch-statements.png
video: LI_WqX7yVc8
url: /programming-languages/c/switch-statements/
weight: 20
---

## Code

{{< code lang="c" >}}
char myGrade = 'A';
switch(myGrade){
     case 'A':
          printf("You Pass\n");
          break;
     case 'F':
          printf("You fail\n");
          break;
     default:
          printf("Invalid grade\n");
}
{{< /code >}}