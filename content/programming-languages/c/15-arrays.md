---
date: 2017-11-01T00:17:43-04:00
title: "Arrays"
seo_title: "Arrays | C | Mike Dane"
subheader:
     greeting: C - Programming Language
     description: This course covers the basics of programming in C. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers arrays in C.
author: Mike Dane
image: arrays.png
video: uR3_mxP3VeA
url: /programming-languages/c/arrays/
weight: 15
---

## Code

{{< code lang="c" >}}
// int luckyNumbers[6];
int luckyNumbers[] = {4, 8, 15, 16, 23, 42};
//        indexes:    0  1  2   3   4   5

luckyNumbers[0] = 90;
printf("%d \n", luckyNumbers[0]);
printf("%d \n", luckyNumbers[1]);
{{< /code >}}