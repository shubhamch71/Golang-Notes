# Basics of Go

### Hello World&#x20;

```go
package main

import "fmt"

func main() {
    fmt.Println("hello world")
}
```

```
Output 

go run hello-world.go
hello world

go build hello-world.go 
// This will create a executable binary that we can execute anywhere 
ls
hello-world    hello-world.go

./hello-world
hello world


```

The go program always starts with package main and the func main&#x20;
