---
date: 2017-11-01T00:17:34-04:00
title: "Variables"
seo_title: "Variables | C | Giraffe Academy"
subheader:
     greeting: C - Programming Language
     description: This course covers the basics of programming in C. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers variables in C.
author: Mike Dane
image: variables.png
video: 17DnxMHEtMU
url: /programming-languages/c/variables/
weight: 6
---

## Code

{{< code lang="c" >}}
/*
Names are case-sensitive and may begin with:
     letters, _
After, may include
     letters, numbers, _
Convention says
     Start with a lowercase word, then additional words are capitalized
     ex. myFirstVariable
*/

char characterName[] = "George";
int characterAge = 70;

printf("There once was a man named %s", characterName);
printf("He was %d years old", characterAge);
printf("He really liked the name %s", characterName);
printf("But didn't like being %d", characterAge);
{{< /code >}}