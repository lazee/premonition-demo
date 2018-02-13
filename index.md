---
layout: default
---

[Premonition](https://github.com/amedia/premonition) is a Jekyll plugin that generates a various number of info boxes from plain and simple Markdown block quotes.

A block quote like this

~~~markdown
 > note "My note"
 > I love `Premonition` so much take a look [here](https://github.com/amedia/premonition)
~~~

can turn into

> note "My note"
> I love `Premonition` so much take a look [here](https://github.com/amedia/premonition)

in no time :)

You will find documentation [here](https://github.com/amedia/premonition) and get the
source code for this demo [here](https://github.com/amedia/premonition-demo).

## Examples

### Note with title

~~~markdown
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

~~~markdown
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

~~~markdown
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

~~~markdown
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

~~~markdown
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

~~~markdown
 > error "The information header"
 > [Premonition](https://github.com/amedia/premonition) allows you to add
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
> [Premonition](https://github.com/amedia/premonition) allows you to add
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
> Anything you can do in Markdown, you can do here. Expect from embeds Premonition boxes ;)
