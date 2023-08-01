---

title: 锌指蛋白
description: Welcome to Plumocean's Blog
slug: Zinker-finger
date: 2023-08-01 00:00:00+0000
image: Zinc-finger.png
categories:
    - Transcription Factors
# tags:
#     - Tag

# links:
#   - title: GitHub
#     description: GitHub is the world's largest software development platform.
#     website: https://github.com
#     image: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
#   - title: TypeScript
#     description: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript.
#     website: https://www.typescriptlang.org
#     image: ts-logo-128.jpg



---


第一篇blog，matlab元素尝试

- [ ] Western材料list清单

Here is an example of headings. You can use this heading by the following markdown rules. For example: use `#` for heading 1 and use `######` for heading 6.

# Heading 1

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6


### Emphasis

The emphasis, aka italics, with _asterisks_ or _underscores_.

Strong emphasis, aka bold, with **asterisks** or **underscores**.

The combined emphasis with **asterisks and _underscores_**.

Strike through usesildes. ~~Scratch this.~~


### Link

[I'm an inline-style link](https://www.google.com)

[I'm an inline-style link with title](https://www.google.com "Google's Homepage")

[I'm a reference-style link][Arbitrary case-insensitive reference text]

[I'm a relative reference to a repository file](../blob/master/LICENSE)

[You can use numbers for reference-style link definitions][1]

Or leave it empty and use the [link text itself].

URLs and URLs in angle brackets will automatically get turned into links.
<http://www.example.com> or <http://www.example.com> and sometimes
example.com (but not on Github, for example).

Some text to show that the r [1] links can follow later.

[arbitrary case-insensitive reference text]: https://www.themefisher.commenu:
    main: 
        weight: 4```yaml
links:
  - title: GitHub
    description: GitHub is the world's largest software development platform.
    website: https://github.com
    image: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
  - title: TypeScript
    description: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript.
    website: https://www.typescriptlang.org
    image: ts-logo-128.jpg
```
### Ordered List

1. List item
2. List item
3. List item



### Unordered List

- List item
- List item
- List item




### Code and Syntax Highlighting

This is an `Inline code` sample.

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

```python
s = "Python syntax highlighting"
print s
```


### Blockquote

> Did you come here for something in particular or just general Riker-bashing? And blowing into maximum warp speed, you appeared for an instant to be in two places at once.



### Tables

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |   centered    |   $12 |
| zebra stripes |   are neat    |    $1 |



### video

<!-- {{< video src="https://www.w3schools.com/html/mov_bbb.mp4" width="100%" height="auto" autoplay="false" loop="false" muted="false" controls="true" class="rounded-lg" >}} -->

### linker follows

To use this feature, add `links` section to frontmatter.

```yaml
links:
  - title: GitHub
    description: GitHub is the world's largest software development platform.
    website: https://github.com
    image: https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png
  - title: TypeScript
    description: TypeScript is a typed superset of JavaScript that compiles to plain JavaScript.
    website: https://www.typescriptlang.org
    image: ts-logo-128.jpg
```

`image` field accepts both local and external images

### side bar insertion

To use this feature, add `links` section to frontmatter.

```yaml
menu:
    main: 
        weight: 4
        params:
            icon: link
```