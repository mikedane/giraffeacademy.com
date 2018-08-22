---
date: 2017-11-15T17:52:38-05:00
title: "For Loops"
seo_title: "For Loops | PHP | Mike Dane"
subheader:
     greeting: PHP - Programming Language
     description: This course covers the basics of programming in PHP. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers for loops in PHP.
author: Mike Dane
image: for-loops.png
video: eP5GADljZcE
url: /web-development/php/for-loops/
weight: 25
---

## Code

{{< code lang="php" >}}
for($i = 0; $i < 5; $i++){
     echo $i;
}

$luckyNums = [4, 8, 15, 16, 23, 42];
foreach($luckyNums as $luckyNum){
     echo $luckyNum."<br>";
}
{{< /code >}}