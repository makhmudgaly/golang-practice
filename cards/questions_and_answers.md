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

# Arrays and slices

*Array* - is fixed length list of things  
*Slice* - An array that can grow or shrink

Every element in a slice must be of same type

Ex:
```go
cards := []string{"Ace of Diamonds", "Five of Hearts"}
```

Adding more elements to slice
```go
cards = append(cards, "Jack of Spades")
```

How to iterate over slice

```go
cards := []string{"Ace of Diamonds", "Five of Hearts"}
	cards = append(cards, "Jack of Spades")

	for i, card := range cards {
		fmt.Println(i, card)
	}
```
Result
```
0 Ace of Diamonds
1 Five of Hearts
2 Jack of Spades
```

i -> index of this element in the array  
card -> current card we're iterating over  
range cards -> take the slice of 'cards' and loop over it

# Custom types

```go
package main

import "fmt"

// Create new type of 'deck'
// which is a slice of strings
type deck []string

func (d deck) print() {
	for idx, card := range d {
		fmt.Println(idx, card)
	}
}
```

# Receiver functions

```go
func (d deck) print() {
    for idx, card := range d {
		fmt.Println(idx, card)
	}
}
```
Any varible of type deck can access method ***print()***

d -> the actual copy of the deck we're working with is available in the function as a variable called d  
deck -> Every variable of type 'deck' can call this function on itself  

by convention we name d because it is one-two letter which indicates the type name