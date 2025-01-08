# Golang Learning Notes

## Go With Habib

## Course conducted by Habibur Rahman (Senior Software Engineer)

## Table of Contents

1. [Golang [007] - Hello World](#golang-007---hello-world)
2. [Golang [008] - Variables and Data Types](#golang-008---variables-and-data-types)
3. [Golang [009] - If else and switch](#golang-009---if-else-and-switch)

## Golang [007] - Hello World

-   Every Go file must have a `package` declaration.
-   The package of the main function Go file should be `main`.
-   The built-in package `fmt` is used for formatting output in Go. The full form of `fmt` is "formatter."
-   Using `fmt.Println`, you can print lines to the console.

### Example Code:

```go
package main

import "fmt"

func main() {
    fmt.Println("Hello gophers!")
}
```

## Golang [008] - Variables and Data Types

-   A variable is like a container where you can store data. In programming, a variable is used to hold data.
-   In Go, variables can be declared like this: `a := 10`.
-   Go has various data types, and variables are used to hold values of specific types such as integers, strings, floats, etc.
-   Variables are stored in memory cells in a key-value pair manner. For example, if you declare `b := 10`, the computer stores the value 10 against the key `b` in the memory cell. When the variable `b` is called, the value is retrieved from memory.
-   Data types in Go include Numeric, Boolean, and String.
    -   Numeric data types are further divided into integers and floating-point numbers:
        -   Integers: `int` (e.g., `int8`, `int16`, `int32`, `int64`, `uint`, `uint8`, `uint16`, `uint32`, `uint64`)
        -   Floating-point numbers: `float32`, `float64`
    -   Boolean data type is represented as `bool`.
    -   Strings are represented as `string`.
-   When declaring a variable for the first time, use `:=` (e.g., `a := 10`). To update its value, use `=` (e.g., `a = 20`).
-   Constants (`const`) are immutable and cannot be updated once declared.

### Variable Declaration Syntax

```go
a := 10 // Short declaration with type inference
a = 20 // Updating data
var a = 10
var x int = 10

const x = "Hello"
```

## Golang [009] - If else and switch

-   Control flow in Go can be handled using `if-else` and `switch` statements.
-   `if-else` is used to execute code blocks based on conditions.
-   Comparison operators include: `>`, `<`, `<=`, `>=`, `==`, `!=`.
-   Logical operators include: `&&` (AND), `||` (OR), `!` (NOT).
-   `switch` is used to select one of many code blocks to execute.

### Example Code:

#### If-Else Example:

```go
package main

import "fmt"

func main() {
    age := 18

    if age > 18 {
        fmt.Println("You are eligible to be married")
    } else if age < 18 {
        fmt.Println("You are not eligible to be married but you can love someone")
    } else {
        fmt.Println("You are just a teenager, not eligible to be married")
    }
}
```

#### Logical Operators Example:

```go
package main

import "fmt"

func main() {
    age := 18
    sex := "male"

    if age > 18 && sex == "male" {
        fmt.Println("You are eligible to be married")
    } else if age > 60 || sex == "male" {
        fmt.Println("You are old")
    } else {
        fmt.Println("You are just a teenager, not eligible to be married")
    }
}
```

#### Switch Example:

```go
package main

import "fmt"

func main() {
    a := 3

    switch a {
    case 1:
        fmt.Println("a is 1")
    case 2, 3:
        fmt.Println("a is either 2 or 3")
    default:
        fmt.Println("a is neither 1 nor 2 or 3")
    }
}
```

### To Be Continued...

-   More details on control flow and best practices will be added later.
