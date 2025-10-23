# Beginner at Golang
This is an repo for beginner level code in Golang.

## How to run Golang code
Create the file:
```sh
touch sandbox.go
```

Write the code inside it:
```go
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

Run it via command line!
```sh
go run sandbox.go 
this is running locally!
current timestamp: 2025-10-22 22:38:43.145346871 -0300 -03 m=+0.000144101
```