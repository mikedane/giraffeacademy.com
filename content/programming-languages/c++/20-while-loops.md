---
date: 2017-11-07T01:21:26-05:00
title: "While Loops"
seo_title: "While Loops | C++ | Giraffe Academy"
subheader:
     greeting: C++ - Programming Language
     description: This course covers the basics of programming in C++. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers while loops in C++.
author: Mike Dane
image: while-loops.png
video: 25JxBoPwmkQ
url: /programming-languages/c++/while-loops/
weight: 20
---

## Code

{{< code lang="cpp" >}}
int index = 1;
while(index <= 5){
     cout << index << endl;
     index++;
}

index = 1;
do{
     cout << index << endl;
     index++;
}while(index <= 5);
{{< /code >}}