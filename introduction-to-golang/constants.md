# Constants

```go
package main 

import "fmt" 

const age = 30 // Global constant 

func main () {
    const name := "golang" // once declared the value of constant cannot change" 
    fmt.Println(name) 
    fmt.Println(age)
    
    // Constant Grouping 
    const ( 
        port = 5000 
        host = " localhost"
    ) 
    
    fmt.Println(port,host) 
```
