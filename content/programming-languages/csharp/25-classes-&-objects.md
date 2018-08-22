---
date: 2017-11-08T18:34:47-05:00
title: "Classes & Objects"
seo_title: "Classes & Objects | C# | Mike Dane"
subheader:
     greeting: C# - Programming Language
     description: This course covers the basics of programming in C#. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers classes & objects in C#.
author: Mike Dane
image: classes-&-objects.png
video: -ETZ0nOCU14
url: /programming-languages/csharp/classes-objects/
weight: 25
---
## Code

{{< code lang="csharp" >}}
public class Book{
     public string title;
     public string author;
}

public class App
{
     public static void Main(string[] args)
     {
          Book book1 = new Book();
          book1.title = "Harry Potter";
          book1.author = "JK Rowling";

          Console.WriteLine(book1.title);

          Book book2 = new Book();
          book2.title = "Lord of the Rings";
          book2.author = "JRR Tolkien";

          Console.WriteLine(book2.title);
     }
}

{{< /code >}}