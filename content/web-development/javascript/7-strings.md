---
date: 2017-10-22T11:23:34-04:00
title: "Strings"
seo_title: "Strings | Javascript | Giraffe Academy"
subheader:
     greeting: Javascript - Program the Web
     description: This course covers the basics of programming in Javascript. Work your way through the videos and we'll teach you everything you need to know to make your website more responsive!
description: This tutorial covers strings in Javascript.
author: Mike Dane
image: strings.png
video: 3JJyYmkXMSA
url: /web-development/javascript/strings/
weight: 7
---

## Code

{{< code lang="js" >}}
var greeting = "Hello";
//   indexes:   01234

document.write( greeting.length + "<br>" );
document.write( greeting.charAt(0) + "<br>"  );
document.write( greeting.indexOf("llo") + "<br>"  );
document.write( greeting.indexOf("z") + "<br>"  );
document.write( greeting.substring(2) + "<br>"  );
document.write( greeting.substring(1, 3) + "<br>"  );
{{< /code >}}