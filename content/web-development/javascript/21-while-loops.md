---
date: 2017-10-22T11:23:35-04:00
title: "While Loops"
seo_title: "While Loops | Javascript | Mike Dane"
subheader:
     greeting: Javascript - Program the Web
     description: This course covers the basics of programming in Javascript. Work your way through the videos and we'll teach you everything you need to know to make your website more responsive!
description: This tutorial covers while loops in Javascript.
author: Mike Dane
image: while-loops.png
video: 6fDBz8u1MkE
url: /web-development/javascript/while-loops/
weight: 21
---

## Code

{{< code lang="js" >}}
index = 1;
while(index <= 5){
     document.write(index);
     index++;
}

index = 1;
do{
	document.write(index);
	index++;
}while(index <= 5);
{{< /code >}}