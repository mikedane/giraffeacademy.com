---
date: 2017-11-08T18:34:46-05:00
title: "While Loops"
seo_title: "While Loops | C# | Giraffe Academy"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers while loops in C#.
author: Mike Dane
image: while-loops.png
video: uqMbyuATj2Y
url: /programming-languages/csharp/while-loops/
weight: 18
---
## Code

{{< code lang="csharp" >}}
int index = 1;
while(index <= 5){
     Console.WriteLine(index);
     index++;
}

index = 1;
do{
   Console.WriteLine(index);
   index++;
}while(index <= 5);
{{< /code >}}