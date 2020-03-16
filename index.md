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

> error "The information header"
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

Premonition also works within excerpts

{% for post in site.posts %}
  <h2>{{ post.title }}</h2>
  {{ post.excerpt }}
{% endfor %}

### Reference links 

> info "linked"
> This is a [reference link][example].

[example]: https://www.example.com/ "dd"

~~~markdown
> info "linked"
> This is a [reference link][example].

[example]: https://www.example.com/ "dd"
~~~
