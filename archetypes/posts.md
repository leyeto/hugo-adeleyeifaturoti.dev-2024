+++
# Old template
# title = "{{ replace .File.ContentBaseName "-" " " | title }}"
# date = {{ .Date }}
# draft = true
# description = ""
# summary = ""
# showSummary = true
# slug = '{{ substr (md5 (printf "%s%s" .Date (replace .TranslationBaseName "-" " " | title))) 4 8 }}'
# tags = ['Others']
# keywords = ["SEO","Digital Marketing"]
# canonicalURL= 

# New template
# Use the title of the new post for SEO-friendly titles and URLs
title = "{{ replace .Name "-" " " | title }}"
date = {{ .Date }}
draft = true
description = "Add a short, compelling summary of the post here to improve SEO."
summary = "Provide a concise summary that will display on listings."
showSummary = true

# SEO Optimization
slug = "{{ .Name | urlize }}"  # Converts the title to a URL-friendly slug
canonicalURL = "{{ .Site.BaseURL }}posts/{{ .Name | urlize }}"  # Sets the canonical URL

# Categories, Tags, and Keywords for better SEO
categories = ["Category1", "Category2"]  # Replace with default categories or leave empty
tags = ["tag1", "tag2"]  # Replace with default tags
keywords = ["keyword1", "keyword2"]  # Add relevant keywords for better SEO

# Featured image for social media and previews
featuredImage = "/images/default.jpg"  # Replace with a default image path if you want
alt = "Add a descriptive alt text for the image"
+++

# H1

## H2

### H3

#### H4

##### H5

###### H6

**bold text**

_italics text_

> blockquote

Ordered list:

1. First item
2. Second item
3. Third item

Unordered list:

- List item
- List item
- List item

Code `code`

Horizontal rule

---

Link

[link text](https://example.com)

Image

![alt text](image.jpg)

Table with alignment:

| Syntax    | Description |   Test Text |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here's this |
| Paragraph |    Text     |    And more |

Fenced code block:

```
{
    "name": "John Doe",
    "age": 30,
    "city": "New York"
}
```

Footnote: |Heres's a sentence with a footnote. [^1]| [^1]: Here's the footnote.

Heading ID: | ### My Great Heading {#custom-id}

Definition List: term : definition

~~strikethrough~~

Task list:

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

Emoji: That is so funny! :joy:

Highlight:

I need to highlight these ==very important words==.

Subscript:

H~2~O

Superscript: X^2^
