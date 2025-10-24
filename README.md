---
author:
- Camilo de Lellis
bibliography:
- sample.bib
title: Beginner at C/C++
---

# Beginner at C/C++

This is a repository for beginner-level code in the C/C++ programming
languages. I am changing the target language from Golang to C after
having some thoughts and deciding what would be more useful for the
career path I intend to take and what I am passionate about.

# How to run C code

Running C code is a fairly simple process. We shall now see the steps
needed for doing so.

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

# How to run C++ code

The process is extremely similar to running C code, as we should see
below.

## Create the file

``` bash
    touch hello-world.c
```

## Write the code inside it

``` c
    #include <iostream>

    using namespace std;

    int main(){
        cout << "hello world from cpp" << endl;
        return 0;
    }
```

## Run it via command line

``` bash
    g++ hello-world.cpp
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
