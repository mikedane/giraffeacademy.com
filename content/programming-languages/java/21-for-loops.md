---
date: 2017-10-22T11:34:29-04:00
title: "For Loops"
seo_title: "For Loops | Java | Giraffe Academy"
subheader:
     greeting: Java - Programming Language
     description: This course covers the basics of programming in Java. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers for loops in Java.
author: Mike Dane
image: for-loops.png
video: 2Z90SJZ4N88
url: /programming-languages/java/for-loops/
weight: 21
---

## Code

{{< code lang="java" >}}
for(int i = 0; i < 5; i++){
     System.out.println(i);
}

int luckyNums[] = {4, 8, 15, 16, 23, 42};
for(int luckyNum : luckyNums){
     System.out.println(luckyNum);
}

{{< /code >}}