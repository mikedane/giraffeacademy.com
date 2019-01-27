---
date: 2017-10-22T11:58:05-04:00
title: "Class Methods"
seo_title: "Class Methods | Python | Mike Dane"
subheader:
     greeting: Python - Programming Language
     description: This course covers the basics of programming in Python. Work your way through the videos/articles and I'll teach you everything you need to know to start your programming journey!
description: This tutorial covers class methods in Python.
author: Mike Dane
image: class-methods.png
video: yVR8241iIac
url: /programming-languages/python/class-methods/
weight: 33
---

## Code

{{< code lang="py" >}}
class Student:
    def __init__(self, name, major, gpa):
        self.name = name
        self.major = major
        self.gpa = gpa

    def has_honors(self):
         if self.gpa >= 3.5:
               return True
          return False
{{< /code >}}