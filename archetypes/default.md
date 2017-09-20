---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | Gatsby | Giraffe Academy"
subheader:
     greeting: Gatsby - Static Site Generator
     description: This course covers the basics of using Gatsby - Static Site Generator. Work your way through the videos and we'll teach you everything you need to know to create a professional and scalable website or blog!
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in Gatsby -  Static Site Generator.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 13
---
