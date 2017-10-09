---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | HTML | Giraffe Academy"
subheader:
     greeting: HTML - Build a Website
     description: This course covers the basics of building a website using HTML. Work your way through the videos and we'll teach you everything you need to know to create a basic website!
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in HTML.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 16
---
