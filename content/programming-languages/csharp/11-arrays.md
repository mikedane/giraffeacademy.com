---
date: 2017-11-08T18:34:45-05:00
title: "Arrays"
seo_title: "Arrays | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers arrays in C#.
author: Mike Dane
image: arrays.png
video: XxKABkLsJcg
url: /programming-languages/csharp/arrays/
weight: 11
---
## Code

{{< code lang="csharp" >}}
//int [] luckyNumbers = new int[10];
int[] luckyNumbers = { 4, 8, 15, 16, 23, 42 };
//         indexes:    0  1  2   3   4   5

luckyNumbers[0] = 90;
Console.WriteLine(luckyNumbers[0]);
Console.WriteLine(luckyNumbers[1]);
Console.WriteLine(luckyNumbers.Length);
{{< /code >}}