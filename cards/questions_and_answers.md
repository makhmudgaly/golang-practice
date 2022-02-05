# Variables

```go
var card string = "Ace of Spades"
```
var -> create new variable
card -> name of variable
string -> type of variable

Another way of creating of variable is 
```go
card := "Ace of Spades"
```

Compiler figures out the type by itself
Use ***:=*** only for creating new variable
```go
card = "Five of Diamonds"
```

# Functions

```go
func newCard() string {
	return "Five of Diamonds"
}
```

func -> indicates that it is function  
newCard -> name of function  
string -> data type function returns  

If function returns something you have to put **return type**