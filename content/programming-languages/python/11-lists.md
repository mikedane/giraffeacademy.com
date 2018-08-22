---
date: 2017-10-22T11:58:02-04:00
title: "Lists"
seo_title: "Lists | Python | Mike Dane"
subheader:
     greeting: Python - Programming Language
     description: This course covers the basics of programming in Python. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers lists in Python.
author: Mike Dane
image: arrays.png
video: c2C7bvkVGbI
url: /programming-languages/python/lists/
weight: 11
---

## Code

{{< code lang="py" >}}
lucky_numbers = [4, 8, "fifteen", 16, 23, 42.0]
#       indexes  0  1       2      3   4   5

lucky_numbers[0] = 90
print(lucky_numbers[0])
print(lucky_numbers[1])
print(lucky_numbers[-1])
print(lucky_numbers[2:])
print(lucky_numbers[2:4])
print(len(lucky_numbers))
{{< /code >}}