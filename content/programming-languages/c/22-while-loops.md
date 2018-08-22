---
date: 2017-11-01T00:17:47-04:00
title: "While Loops"
seo_title: "While Loops | C | Mike Dane"
subheader:
     greeting: C - Programming Language
     description: This course covers the basics of programming in C. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers while loops in C.
author: Mike Dane
image: while-loops.png
video: DMoDZPNJ-ZQ
url: /programming-languages/c/while-loops/
weight: 22
---

## Code

{{< code lang="c" >}}
int index = 1;
while(index <= 5){
     printf("%d \n", index);
     index++;
}

index = 1;
do{
     printf("%d \n", index);
     index++;
}while(index <= 5);
{{< /code >}}