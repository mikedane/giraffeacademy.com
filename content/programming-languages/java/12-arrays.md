---
date: 2017-10-22T11:34:28-04:00
title: "Arrays"
seo_title: "Arrays | Java | Giraffe Academy"
subheader:
     greeting: Java - Programming Language
     description: This course covers the basics of programming in Java. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers arrays in Java.
author: Mike Dane
image: arrays.png
video: GmtkYHfAFOo
url: /programming-languages/java/arrays/
weight: 12
---

## Code

{{< code lang="java" >}}
// int [] luckyNumbers = new int[10];
int [] luckyNumbers = {4, 8, 15, 16, 23, 42};
//         indexes:    0  1  2   3   4   5

luckyNumbers[0] = 90;
System.out.println(luckyNumbers[0]);
System.out.println(luckyNumbers[1]);
System.out.println(luckyNumbers.length);
{{< /code >}}