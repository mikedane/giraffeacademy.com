---
date: 2017-11-08T18:34:46-05:00
title: "For Loops"
seo_title: "For Loops | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers for loops in C#.
author: Mike Dane
image: for-loops.png
video: ad38jqt7XDs
url: /programming-languages/csharp/for-loops/
weight: 20
---
## Code

{{< code lang="csharp" >}}
for(int i = 0; i < 5; i++){
     Console.WriteLine(i);
}

int[] luckyNums = {4, 8, 15, 16, 23, 42};
foreach(int luckyNum in luckyNums){
     Console.WriteLine(luckyNum);
}
{{< /code >}}