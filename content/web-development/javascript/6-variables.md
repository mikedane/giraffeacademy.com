---
date: 2017-10-22T11:23:34-04:00
title: "Variables"
seo_title: "Variables | Javascript | Mike Dane"
subheader:
     greeting: Javascript - Program the Web
     description: This course covers the basics of programming in Javascript. Work your way through the videos and we'll teach you everything you need to know to make your website more responsive!
description: This tutorial covers variables in Javascript.
author: Mike Dane
image: variables.png
video: YptrAq5O-jQ
url: /web-development/javascript/variables/
weight: 6
---

## Code

{{< code lang="js" >}}
/*
Names are case-sensitive and may begin with:
     letters, $, _
After, may include
     letters, numbers, $, _
Convention says
     Start with a lowercase word, then additional words are capitalized
     ex. myFirstVariable
*/

var name = "Mike";                 // String w/ double quotes
var occupation = 'programmer';     // String w/ single quotes

var age = 20;                      // Integer
var gpa = 2.5;                     // Floating point number

var isTall;                        // boolean true/false
isTall = true;

name = "John";

document.write("Your name is " + name);
{{< /code >}}