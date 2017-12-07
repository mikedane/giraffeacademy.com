---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | PHP | Giraffe Academy"
subheader:
     greeting: PHP - Programming Language
     description: This course covers the basics of programming in PHP. Work your way through the videos and we'll teach you everything you need to know to start your programming journey!
description: This tutorial covers {{ replace .TranslationBaseName "-" " " }} in PHP.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 33
---

## Code

{{< code lang="js" >}}

{{< /code >}}

