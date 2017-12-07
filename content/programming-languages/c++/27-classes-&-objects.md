---
date: 2017-11-07T01:21:27-05:00
title: "Classes & Objects"
seo_title: "Classes & Objects | C++ | Giraffe Academy"
subheader:
     greeting: C++ - Programming Language
     description: This course covers the basics of programming in C++. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers classes & objects in C++.
author: Mike Dane
image: classes-&-objects.png
video: wGyCsWXVD9E
url: /programming-languages/c++/classes-objects/
weight: 27
---

## Code

{{< code lang="cpp" >}}
class Book{
     public:
          string title;
          string author;
};

int main(){

     Book book1;
     book1.title = "Harry Potter";
     book1.author = "JK Rowling";

     cout << book1.title << endl;

     Book book2;
     book2.title = "Lord of the Rings";
     book2.author = "JRR Tolkien";

     cout << book2.title << endl;

     return 0;
}
{{< /code >}}