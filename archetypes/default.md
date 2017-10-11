---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | Sass | Giraffe Academy"
subheader:
     greeting: Sass - Style a Website
     description: This course covers the basics of styling a website using Sass. Work your way through the videos and we'll teach you everything you need to know to style a basic website!
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in Sass.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 12
---
