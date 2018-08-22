---
date: 2017-11-07T01:21:25-05:00
title: "Variables"
seo_title: "Variables | C++ | Mike Dane"
subheader:
     greeting: C++ - Programming Language
     description: This course covers the basics of programming in C++. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers variables in C++.
author: Mike Dane
image: variables.png
video: K8Rqul0V8_U
url: /programming-languages/c++/variables/
weight: 6
---

## Code

{{< code lang="cpp" >}}
/*
Names are case-sensitive and may begin with:
     letters, _
After, may include
     letters, numbers, _
Convention says
     Start with a lowercase word, then additional words are capitalized
     ex. myFirstVariable
*/

// #include <string>
string characterName = "George";
int characterAge = 70;

cout << "There once was a man named " << characterName << endl;
cout << "He was " << characterAge << " years old" << endl;
cout << "He really liked the name " << characterName << endl;
cout << "But didn't like being " << characterAge << endl;
{{< /code >}}