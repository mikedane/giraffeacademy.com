---
date: 2017-10-22T11:34:29-04:00
title: "Methods"
seo_title: "Methods | Java | Giraffe Academy"
subheader:
     greeting: Java - Programming Language
     description: This course covers the basics of programming in Java. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers methods in Java.
author: Mike Dane
image: functions.png
video: Cx_ut1msINQ
url: /programming-languages/java/functions/
weight: 13
---

## Code

{{< code lang="java" >}}
public static void main(String [] args){
     int sum = addNumbers(4, 60);
     System.out.println(sum);
}

public static int addNumbers(int num1, int num2){
     return num1 + num2;
}

{{< /code >}}