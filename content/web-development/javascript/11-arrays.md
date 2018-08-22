---
date: 2017-10-22T11:23:34-04:00
title: "Arrays"
seo_title: "Arrays | Javascript | Mike Dane"
subheader:
     greeting: Javascript - Program the Web
     description: This course covers the basics of programming in Javascript. Work your way through the videos and we'll teach you everything you need to know to make your website more responsive!
description: This tutorial covers arrays in Javascript.
author: Mike Dane
image: arrays.png
video: JQ-wmaarWTQ
url: /web-development/javascript/arrays/
weight: 11
---

## Code

{{< code lang="js" >}}
// luckyNumbers = [];
luckyNumbers = [4, 8, 15, 16, "twenty", false];
//  indexes:    0  1  2   3      4        5

luckyNumbers[0] = 90;
document.write(luckyNumbers[0] + "<br>");
document.write(luckyNumbers[1] + "<br>");
document.write(luckyNumbers.length);
{{< /code >}}