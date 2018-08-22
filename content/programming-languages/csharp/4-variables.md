---
date: 2017-11-08T18:34:44-05:00
title: "Variables"
seo_title: "Variables | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers variables in C#.
author: Mike Dane
image: variables.png
video: vYQZCum3rDk
url: /programming-languages/csharp/variables/
weight: 4
---
## Code

{{< code lang="csharp" >}}
/*
Names are case-sensitive and may begin with:
     letters, _, @
After, may include
     letters, numbers, _
Convention says
     Start with a lowercase word, then additional words are capitalized
     ex. myFirstVariable
*/

string characterName = "George";
int characterAge = 70;

Console.WriteLine("There once was a man named " + characterName);
Console.WriteLine("He was " + characterAge + " years old");
Console.WriteLine("He really liked the name " + characterName);
Console.WriteLine("But didn't like being " + characterAge);
{{< /code >}}