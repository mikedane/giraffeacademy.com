---
date: 2017-10-22T11:58:05-04:00
title: "Classes & Objects"
seo_title: "Classes & Objects | Python | Giraffe Academy"
subheader:
     greeting: Python - Programming Language
     description: This course covers the basics of programming in Python. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers classes & objects in Python.
author: Mike Dane
image: classes-&-objects.png
video: 6chvxajS3yc
url: /programming-languages/python/classes-objects/
weight: 31
---

## Code

{{< code lang="py" >}}
class Book:
    def __init__(self, title, author):
        self.title = title
        self.author = author

book1 = Book("Harry Potter", "JK Rowling");
# book1.title = "Half-Blood Prince"

print(book1.title)
{{< /code >}}