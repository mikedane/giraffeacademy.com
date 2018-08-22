---
date: 2017-11-15T17:52:37-05:00
title: "Strings"
seo_title: "Strings | PHP | Mike Dane"
subheader:
     greeting: PHP - Programming Language
     description: This course covers the basics of programming in PHP. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers strings in PHP.
author: Mike Dane
image: strings.png
video: lRUljf_chOE
url: /web-development/php/strings/
weight: 8
---

## Code

{{< code lang="php" >}}
$greeting = "Hello";
//indexes:   01234

echo  strlen($greeting)."<br>";
echo  $greeting[0]."<br>";
echo  $greeting[-1]."<br>";
echo  str_replace("l", "Z", $greeting)."<br>";
echo  strchr($greeting, "ll")."<br>";  
{{< /code >}}