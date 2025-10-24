---
author:
- Camilo de Lellis
bibliography:
- sample.bib
title: Beginner at C
---

# Beginner at C

This is a repository for beginner-level code in the C programming
language. I am changing the target language from Golang to C after
having some thoughts and deciding what would be more useful for the
career path I intend to take and what I am passionate about.

# How to run C code

## Create the file

``` bash
    touch hello-world.c
```

## Write the code inside it

``` c
    #include <stdio.h>

    int main( ) {
        printf("hello, world");
        return 0;
    }
```

## Run it via command line

``` bash
    gcc hello-world.c 
    ./a.out 
```

# Rewriting this in LaTeX

I will now take notes using LaTeX and then convert them to Markdown.
Creating the file:

``` bash
    touch main.tex
```

After that, I’ll write everything that will be available through this
repo’s version control.

To convert it into my README.md again, I’ll just use the following:

``` bash
    pandoc main.tex -o README.md --from=latex --to=gfm --standalone
```
