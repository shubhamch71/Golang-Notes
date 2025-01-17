# Variables

• Go is statically typed. \
• Variables are assigned a type, either explicitly or implicitly.

### Syntax&#x20;

1\) var \<variable\_name> \<data-type> = \<value>  ( Here we are mentioning the data types explicitly)&#x20;

2\) var \<variable\_name> = "golang" ( Here the types is inferred by go)&#x20;

3\) name := "golang" ( this is shorthand operator , however this does not work outside a function)&#x20;



Note: - To declare a empty variable we can do it using 2nd syntax mentioned above :-&#x20;

```go
var name string // var name is intialised but not declared ie its value is 0
name = "golang" 
```

We can also declare mutliple variables at once :-&#x20;

```go
var s,t string = "foo", "bar" // here s,t are two variables 

// Another way of declaring multiple variables with diff data types 

var ( 
s string = "foo"
i int = 5
) 
```

