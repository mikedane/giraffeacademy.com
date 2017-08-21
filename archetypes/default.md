---
date: {{ .Date }}
title: "{{ replace .TranslationBaseName "-" " " | title }}"
seo_title: "{{ replace .TranslationBaseName "-" " " | title }} | Hugo | Giraffe Academy"
subheader:
   - greeting:
     description:
description: This tutorial covers how to use {{ replace .TranslationBaseName "-" " " }} in hugo static site generator.
author: Mike Dane
image: {{ .TranslationBaseName }}.png
video: {{ .TranslationBaseName }}.mp4
url: /{{.Dir}}{{ .TranslationBaseName }}/
weight: 4
---
