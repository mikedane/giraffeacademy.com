---
date: 2017-11-08T18:34:44-05:00
title: "Strings"
seo_title: "Strings | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers strings in C#.
author: Mike Dane
image: strings.png
video: h6_x9Rxh5rU
url: /programming-languages/csharp/strings/
weight: 6
---
## Code

{{< code lang="csharp" >}}
string greeting = "Hello";
//      indexes:   01234

Console.WriteLine( greeting.Length );
Console.WriteLine( greeting[0] );
Console.WriteLine( greeting.IndexOf("llo") );
Console.WriteLine( greeting.IndexOf("z") );
Console.WriteLine( greeting.Substring(2) );
Console.WriteLine( greeting.Substring(1, 3) );
{{< /code >}}