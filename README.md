---
author:
- Camilo de Lellis
bibliography:
- sample.bib
title: Beginner at C/C++
---

# Introduction to C++

## What is C++

C++ is a object oriented programming language being used in the most
diverse applications. For this reason it is called a **general purpose
language**. It is a superset of C, being a extension including object
oriented features that C lacks.

## Why use C++

I’ve taken a liking to C/C++ because of the career path I intend to
take. I want to work with GPU development, with the development of
software much more closely to hardware. I like machine learning and want
to work with algorithm optimization aswell. We’ll see how this will turn
out. I intend to write these notes with C++ in mind because it seems the
more suitable from a market perspective, but I want to compare the code
to C as much as possible and say where it would be better to implement
something in C and when it would be better to do so in C++.

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
