---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | Middleman | Giraffe Academy"
subheader:
     greeting: Middleman - Static Site Generator
     description: This course covers the basics of using Middleman - Static Site Generator. Work your way through the videos and we'll teach you everything you need to know to create a professional and scalable website or blog!
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in Middleman -  Static Site Generator.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 17
---
