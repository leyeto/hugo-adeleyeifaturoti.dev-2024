+++
date = '{{ .Date }}'
draft = true
title = '{{ replace .File.ContentBaseName "-" " " | title }}'
description = "{{ .Description }}"
author = "{{ .Site.Language.Params.Author.name }}"

+++
