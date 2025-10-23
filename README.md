---
author:
- Camilo de Lellis
bibliography:
- sample.bib
title: Beginner at Golang
---

# Beginner at Golang

This is a repository for beginner-level code in the Go programming
language.

# How to run Golang code

## Create the file

``` bash
touch sandbox.go
```

## Write the code inside it

``` go
    package main
    
    import (
        "fmt"
        "time"
    )
    
    // this code was taken from Go's tour: https://go.dev/tour/welcome/4
    func main() {
        fmt.Println("this is running locally!")
    
        fmt.Println("current timestamp:", time.Now())
    }
```

## Run it via command line

``` bash
    go run sandbox.go
    this is running locally!
    current timestamp: 2025-10-22 22:38:43.145346871 -0300 -03 m=+0.000144101
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
