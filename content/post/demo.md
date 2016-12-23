+++
categories = []
tags = [
    'demo', 'markdown', 'hugo'
]
thumbnail = ""
title = "Demo"
description = "Demo post for the blog theme"
date = "2016-12-21T21:37:55-07:00"
+++

# Section 1

Here's some `inline code` and below is some example html:

```html
<div id="wrapper">
    <header class="site-header">
        <div class="container">
            <div class="site-title-wrapper">
                <a class="site-logo" title="{{ .Title }}" href="{{ .Site.BaseURL }}">
                    <img src="{{ . }}" alt="{{ .Title }}" />
                </a>
                <h1 class="site-title">
                    <a title="{{ .Site.Title }}" href="{{ .Site.BaseURL }}">{{ .Site.Title }}</a>
                </h1>
            </div>
        </div>
    </header>
</div>    
```

# Section 2

A *bunch* of examples of different **typesetting** features:

## Bullet Lists and Numbered Lists

Some body paragraph text as well as a cute little bullet list of items:

- Raindrops on roses
- Whiskers on kittens
- Brown paper packages
    - Tied up with string
    - These are a few of my favorite things
- This is an extra long sentence designed to wrap around onto multiple lines
    when viewed on a desktop browser
- I am a reasonably happy and successful list item
    - I live in the shadow of the earlier list item

You know what's even cooler than a bullet list? An ordered list. I can prove it,
too: check out [this site][linkref] and [this one][linkref] and [this
site][linkref]. Totally credible!

1. When the dog barks
1. When the bee stings
1. When I'm feeling sad
    1. I simply remember my favorite things
    1. And then I don't feel...
1. ...So bad

## Equations and Math Typesetting

I use MathJax/LaTeX to write some compelling equations. For instance, consider
the `$Q$`-learning model for a simple aircraft avoidance problem:

<div>
\begin{align*}
Q^* (b,a_{+1}) &= R(b, a_{+1}) + \gamma \sum_{b'} T(s' | s,a)U^* (s') \\
&= \sum_{s} R(s,a)b(s) + \gamma \sum_{s'} T(s' | s,a)U^* (s') \\
&= R(s) +  R(a_{+1}) + \gamma \sum_{s'} T(s' | s,a)U^* (s')
\end{align*}
</div>

### Subsubsection to demonstrate tables

Since we are certain that `$h = 10$`, and we chose action `$a_{+1}$`, then `$\hat{h} = 10$`. We have the following possibilities for the next state:

h      | t     | r   | `$T(s' \vert s,a)$`
-------|-------|-----|-----------
10     | 0     | 1   | 0.5 + 0.25
9      | 0     | 1   | 0.25

## Figures and Images

I can either directly include an image without a caption, or make a 'figure'
that includes a caption. The figure is created using the shortcode syntax 
provided by [Hugo][hugo].

Here is an image included with the default Markdown syntax:

![My default image](../../../img/ee251_if_sim_result.png)

Here is a figure with a caption and title:

{{< figure src="/img/beautiful_mountains.png" caption="A screenshot of my lovely Desktop" title="Screenshot" >}}

## Embedded Videos

I can also easily embed YouTube videos with a shortcode.

{{< youtube dQw4w9WgXcQ >}}

Play it, I dare you.

[linkref]: https://example.org
[hugo]: https://gohugo.io
