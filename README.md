# The Monkey Programming Language

Monkey is a programming language created by following [Writing an Interpreter in Go](https://interpreterbook.com/) by Thorsten Ball.

## To use it:

- [Download Go](https://golang.org/dl/)
- `git clone https://github.com/svwielga4/monkey.git`
- `cd monkey`
- `go run main.go`

## Language Features

- First class functions
- Arrays, Maps, Strings, Ints, Bools
- Control flow: if / else
- Macro system for meta-programming

## How to Use:

### Assignment

`let ten = 10;`
`let hi = "hello world";`
`let maybeTrue = 10 > 5`
`let luckyNumberArray = [33, 7];`
`let map = { "lovely": true, "dastardly": false };`
`let add = fn(x, y) { x + y; };`

### Control flow

`if (5 < 10) { return true; } else { return false; }`

### Macro System

`let unless = macro(condition, consequence, alternative) { quote(if (!(unquote(condition))) { unquote(consequence); } else { unquote(alternative); }); };`
