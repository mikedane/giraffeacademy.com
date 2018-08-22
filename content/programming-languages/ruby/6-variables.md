---
date: 2017-11-01T00:12:41-04:00
title: "Variables"
seo_title: "Variables | Ruby | Mike Dane"
subheader:
     greeting: Ruby - Programming Language
     description: This course covers the basics of programming in Ruby. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers variables in Ruby.
author: Mike Dane
image: variables.png
video: 4mWc6Q9shcQ
url: /programming-languages/ruby/variables/
weight: 6
---

## Code

{{< code lang="rb" >}}
=begin
 Names are case-sensitive and may begin with:
     letters, _
 After, may include
     letters, numbers, _
 Convention says
     Start with a lowercase word, then additional words are lowercase separated
     by an underscore
     ex. my_first_variable
=end

character_name = "George"
character_age = 70

puts "There once was a man named " + character_name
puts "He was " + character_age + " years old"
puts "He really liked the name " + character_name
puts "But didn't like being " + character_age

# You can also print variables using '#{}'
puts "My variable is #{character_name}"
{{< /code >}}