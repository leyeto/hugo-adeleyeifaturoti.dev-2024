+++
title = "{{ replace .File.ContentBaseName "-" " " | title }}"
date = {{ .Date }}
draft = true
description = ""
summary = ""
showSummary = false
slug = '{{ substr (md5 (printf "%s%s" .Date (replace .TranslationBaseName "-" " " | title))) 4 8 }}'
tags = ['Others']
technologies = ["JavaScript", "React", "Tailwind"]
projectObjective = "Build a new feature"
lessonsLearnt = "Learned how to do something"
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
