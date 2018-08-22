---
date: 2017-11-01T00:12:45-04:00
title: "Classes & Objects"
seo_title: "Classes & Objects | Ruby | Mike Dane"
subheader:
     greeting: Ruby - Programming Language
     description: This course covers the basics of programming in Ruby. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers classes & objects in Ruby.
author: Mike Dane
image: classes-&-objects.png
video: sc5RhTIBf4c
url: /programming-languages/ruby/classes-objects/
weight: 29
---

## Code

{{< code lang="rb" >}}
class Book
     attr_accessor :title, :author
end

book1 = Book.new()
book1.title = "Harry Potter"
book1.author = "JK Rowling"

puts book1.title
{{< /code >}}