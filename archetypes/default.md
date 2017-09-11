---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | Hugo | Giraffe Academy"
subheader:
     greeting: Hugo - Static Site Generator
     description: This course covers the basics of using Hugo - Static Site Generator. Work your way through the articles and we'll teach you everything you need to know to create a professional and scalable website or blog!
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in Hugo -  Static Site Generator.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 23
---
