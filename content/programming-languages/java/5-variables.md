---
date: 2017-10-22T11:34:28-04:00
title: "Variables"
seo_title: "Variables | Java | Giraffe Academy"
subheader:
     greeting: Java - Programming Language
     description: This course covers the basics of programming in Java. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers variables in Java.
author: Mike Dane
image: variables.png
video: TVSj_N2Rmfo
url: /programming-languages/java/variables/
weight: 5
---


## Code

{{< code lang="java" >}}
/*
 Names are case-sensitive and may begin with:
     letters, $, _
 After, may include
     letters, numbers, $, _
 Convention says
     Start with a lowercase word, then additional words are capitalized
     ex. myFirstVariable
*/
String characterName = "George";
int characterAge = 70;

System.out.println("There once was a man named " + characterName);
System.out.println("He was " + characterAge + " years old");
System.out.println("He really liked the name " + characterName);
System.out.println("But didn't like being " + characterAge);
{{< /code >}}