+++
author = "Hugo Authors"
title = "Rich Content"
date = "2019-03-10"
description = "A brief description of Hugo Shortcodes"
tags = [
    "shortcodes",
    "privacy",
]
+++

Hugo ships with several [Built-in Shortcodes](https://gohugo.io/content-management/shortcodes/#use-hugo-s-built-in-shortcodes) for rich content, along with a [Privacy Config](https://gohugo.io/about/hugo-and-gdpr/) and a set of Simple Shortcodes that enable static and no-JS versions of various social media embeds.
<!--more-->
---

## Code Highlighting

{{< highlight go "linenos=inline, hl_lines=3 6-8, style=emacs" >}}
package main

import "fmt"

func main() {
    for i := 0; i < 3; i++ {
        fmt.Println("Value of i:", i)
    }
}
{{< /highlight >}}

## Instagram Shortcode

{{< instagram BGvuInzyFAe hidecaption >}}

<br>

---

## YouTube Shortcode

{{< youtube 0RKpf3rK57I >}}

<br>

---

## Twitter Shortcode

{{< x 1085870671291310081 >}}

<br>

---

## Vimeo Shortcode

{{< vimeo 48912912 >}}
