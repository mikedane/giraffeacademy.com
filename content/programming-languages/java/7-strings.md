---
date: 2017-10-22T11:34:28-04:00
title: "Strings"
seo_title: "Strings | Java | Giraffe Academy"
subheader:
     greeting: Java - Programming Language
     description: This course covers the basics of programming in Java. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers strings in Java.
author: Mike Dane
image: strings.png
video: yebwyol5M7k
url: /programming-languages/java/strings/
weight: 7
---

## Code

{{< code lang="java" >}}

String greeting = "Hello";
//      indexes:   01234

System.out.println( greeting.length() );
System.out.println( greeting.charAt(0) );
System.out.println( greeting.indexOf("llo") );
System.out.println( greeting.indexOf("z") );
System.out.println( greeting.substring(2) );
System.out.println( greeting.substring(1, 3) );
{{< /code >}}

