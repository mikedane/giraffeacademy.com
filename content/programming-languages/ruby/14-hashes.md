---
date: 2017-11-01T00:12:42-04:00
title: "Hashes"
seo_title: "Hashes | Ruby | Mike Dane"
subheader:
     greeting: Ruby - Programming Language
     description: This course covers the basics of programming in Ruby. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers hashes in Ruby.
author: Mike Dane
image: hashes.png
video: BtHKhsDUPwQ
url: /programming-languages/ruby/hashes/
weight: 14
---

## Code

{{< code lang="rb" >}}
test_grades = {
    "Andy" => "B+",
    :Stanley => "C",
    "Ryan" => "A",
    3 => 95.2
}

test_grades["Andy"] = "B-"
puts test_grades["Andy"]
puts test_grades[:Stanley]
puts test_grades[3]
{{< /code >}}