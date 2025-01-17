# Taking Input

### Scanf&#x20;

<figure><img src="../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

Single Input&#x20;

```go
// code for single input 

package main 

import "fmt"

func main () {

    var name string 
    fmt.Print("Enter your name: ")
    fmt.Scanf("%s" , &name) // here instead of s we can also take v 
    fmt.Println("Hey there , ", name)
    fmt.Printf("Hey there , %s \n", name)
    fmt.Print("Hey there, " , name , " !!!")
}
```

Multiple Input&#x20;

```go
// code for taking multiple input from user 
package main

import ( " fmt " )

func main () {
    var name string
    var is_muggle bool

    fmt.Print("Enter your name & are you a muggle: ") 
    fmt.Scanf("%s %t" , &name , &is_muggle) 
    fmt.Println(name, is_muggle)
    fmt.Printf("%v  %t \n" , name , is_muggle)
    fmt.Print(name , " " , is_muggle)
 
}   
 
```

Scanf Return values&#x20;

count :- the number of arguments that the function writes to

err : - any error thrown during the execution of the function

Note :- This is kind of try and catch in other languages , the error generated will be stored in err.

```go
// How to generally use scanf and take input 
package main

import ("fmt")

func main () {

    var a string
    var b int
    fmt.Print("Enter a string and a number: ")
    count, err := fmt.Scanf("%s %d", &a , &b) 

    // sometimes when we don't want count or error we can do as below 
    
    // _, err := fmt.Scanf("%s %d", &a , &b) 
    
    // OR 
    
    // count, _ := fmt.Scanf("%s %d", &a , &b) 
    
    // OR 
    
    // _, _ := fmt.Scanf("%s %d", &a , &b) 
    // (This will not work , we have to atleast mention one of the above) 
    
    fmt.Println("count : " , count)
    fmt.Println("error : " , err )
    fmt.Println("a: " , a) 
    fmt.Println("b: " , b) 


}

```

