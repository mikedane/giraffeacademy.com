---
date: 2017-11-15T17:52:37-05:00
title: "Functions"
seo_title: "Functions | PHP | Giraffe Academy"
subheader:
     greeting: PHP - Programming Language
     description: This course covers the basics of programming in PHP. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers functions in PHP.
author: Mike Dane
image: functions.png
video: lBPa92h2AqE
url: /web-development/php/functions/
weight: 18
---

## Code

{{< code lang="php" >}}
function addNumbers($num1, $num2=99){
     return $num1 + $num2;
}

$sum = addNumbers(4, 3);
echo $sum;
{{< /code >}}