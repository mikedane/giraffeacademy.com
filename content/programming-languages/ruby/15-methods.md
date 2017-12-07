---
date: 2017-11-01T00:12:42-04:00
title: "Methods"
seo_title: "Methods | Ruby | Giraffe Academy"
subheader:
     greeting: Ruby - Programming Language
     description: This course covers the basics of programming in Ruby. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers methods in Ruby.
author: Mike Dane
image: methods.png
video: e1EpXUgSfN8
url: /programming-languages/ruby/methods/
weight: 15
---

## Code

{{< code lang="rb" >}}
def add_numbers(num1, num2=99)
     return num1 + num2
end

sum = add_numbers(4, 3)
puts sum
{{< /code >}}