# List of questions based on the written code

1. How do run the code the code in our project?
   <br>
   ```go
   go run main.go
   ```
   
   Go CLI
   | Command | Description |
   | ------- | ------------|
   | ```go build``` | Compiles a bunch of source code files|
   | ```go run``` | Compiles and executes one or two files |
   | ```go fmt``` | Formats all the code in each file in current directory|
   | ```go install``` | Compiles and "installs" a package |
   | ```go get``` | Downloads the raw source code of someone else's package|
   | ```go test``` | Runs any tests associated with the current project|
   <br> 
2. What does ```package main``` mean?
   <br>
   Package is collection of common source code files.

   Multiple files can be grouped under one package.
   There are two types of packages in go: executable and reusable  

   *executable* -> Generates a file that we can run  
   *reusable* -> Code used as 'helpers'. Good place to put reusable logic  

   ```go
   package main
   ```
   **main** here indicates that package is executable. And it must have function called main
   ```go
   func main()
   ```
   <br>
3. What does ```import "fmt"``` mean?
   <br>
   Import here means to give access from "fmt" to my current package main  
   We can find documentation on standard package on https://golang.org/pkg
4. What's that ```func``` thing?
   <br>
   Just like functions in other programming languages
5. How is the **main.go** file organized
   <br>
   ***Package declaration*** -> ***Import packages*** -> ***Do the magic***

