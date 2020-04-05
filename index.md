---
layout: default
---

[Premonition](https://github.com/lazee/premonition) is a [Jekyll](https://jekyllrb.com/) plugin
that can transform [Markdown](https://en.wikipedia.org/wiki/Markdown) [blockquotes](https://daringfireball.net/projects/markdown/syntax#blockquote)
into styled blocks of code. The default template and stylesheet focuses on creating info
boxes, but through the templating system you can modify it to suit your needs.With version 4 we also introduced
a new citation box.

Read the [documentation](https://github.com/lazee/premonition) to get started.

## Examples

### Citation (New in version 4)

~~~ markdown
 > citation "-- Mark Twain" [ cite = "twain" ]
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> citation "-- Mark Twain" [ cite = "twain" ]
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Note with title

~~~ markdown
 > note "My note"
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> note "My note"
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Note without title

~~~ markdown
 > note ""
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> note ""
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Info box

~~~ markdown
 > info "The information header"
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> info "The information header"
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Warning box

~~~ markdown
 > warning "The information header"
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> warning "The information header"
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Error box

~~~ markdown
 > error "The information header"
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

### Custom box

~~~ markdown
 > custom "A custom box with a Font Awesome icon"
 > Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
 > ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
 > Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.
~~~

> custom "A custom box with a Font Awesome icon"
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

### Error box with Markdown

~~~ markdown
 > error "The information header"
 > [Premonition](https://github.com/lazee/premonition) allows you to add
 >
 > * Lists
 > * like this
 >
 > Use *formatting* and add code blocks.
 >
 > ~~~~
 > Isn't that sweet?
 > ~~~~~
 > Anything you can do in Markdown, you can do here. Expect from embeds Premonition boxes ;)
~~~

> error "The information header"
> [Premonition](https://github.com/lazee/premonition) allows you to add
>
> * Lists
> * like this
>
> Use *formatting* and add code blocks.
>
>```
>Isn't that sweet?
>```
>
> Anything you can do in Markdown, you can do here.

### Post excerpts

Premonition also works within post excerpts. This is rendered from the
`2020-03-02-blog-post.md` post file in the source code of this
demo site:

{% for post in site.posts %}
  <h2>{{ post.title }}</h2>
  {{ post.excerpt }}
{% endfor %}

~~~markdown
---
layout: post
title:  "Welcome to Premonition!"
excerpt_separator: <!--more-->
---

> info "The information header"
> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean interdum, ligula in
> ultrices sodales, ante enim scelerisque diam, nec molestie lorem nulla sit amet dolor.
> Aenean id augue ante. Duis ut mi faucibus, pellentesque sem quis, gravida nisi. Nam cursus.

<!--more-->

## Not in excerpt

Hopefully
~~~

### Reference links 

> info "Linked"
> This is a [reference link][example].

[example]: https://www.example.com/ "dd"

~~~markdown
> info "Linked"
> This is a [reference link][example].

[example]: https://www.example.com/ "dd"
~~~

### Render error

If an unknown type is used, this error will appear:

> foo "Linked"
> Unknown type

~~~markdown
> foo "Linked"
> Unknown type
~~~
