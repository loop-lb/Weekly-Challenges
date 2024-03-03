# Week-001 -- Build your own markdown to HTML CLI tool

## Guide to our tool

Our tool will have a few usecases and flags.

1. `-i [raw-md]` tells our tool that the next argument will be raw markdown.
2. `-if [md-file]` tells our tool that the next argument will be a markdown file.
3. `-of [{Optional} filename]` tells our tool to output the result html in a file,
    if no argument passed the html file will have the same name as the markdown file.

The flavor of markdown we will be parsing is [github flavored markdown](https://github.github.com/gfm/) or (gfm).

However as a ***bonus*** you can add the flag `-flavor=` to configure which flavor of markdown our tool will parse.

## Example

### Example 1

```console
member@loop$ md2html -if README.md -of
```

results in README.html

### Example 2

```console
member@loop$ md2html -if README.md -of document.html
```

results in README.md being converted to document.html

### Example 3

```console
member@loop$ md2html -i "# Hello world"
```

prints to the terminal `<html><body><h1>Hello world</h1></body></html>`

## Bonuses

- Add a `-flavor=` flag to specify which flavor of markdown to parse.
- Write the tool in a functional programming language.
- Use a [TDD](https://en.wikipedia.org/wiki/Test-driven_development#:~:text=Test%20Driven%20Development%20(TDD)%20is,leading%20to%20more%20robust%20software.) approach when writing your project.

## Submissions

When you finish the tool, send us a

## Useful links to help you with this challenge

- [Crafting interpreters (The parsing chapter) (recursive descent)](https://www.craftinginterpreters.com/parsing-expressions.html)
