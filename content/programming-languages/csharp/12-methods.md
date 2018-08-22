---
date: 2017-11-08T18:34:45-05:00
title: "Methods"
seo_title: "Methods | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers methods in C#.
author: Mike Dane
image: methods.png
video: MkDroqxS8LY
url: /programming-languages/csharp/methods/
weight: 12
---
## Code

{{< code lang="csharp" >}}
public static void Main(string [] args){
     int sum = AddNumbers(4, 60);
     Console.WriteLine(sum);
}

public static int AddNumbers(int num1, int num2){
     return num1 + num2;
}
{{< /code >}}