# Week-001 -- Build your own markdown to HTML CLI tool

Welcome to the first LOOP coding challenge, we will start our challenges with an extremely fun and educative project: `md2html`!

`md2html` will be a [CLI](https://en.wikipedia.org/wiki/Command-line_interface) tool that converts markdown to html. 

This might sound easy but parsing is a whole field within itself in computer science and i encourage you to research parsing techniques to help you
with this project.

Parsing is an extremely mature and widely used technique in software development, whenever you compile your code, a parser is used, whenever you read from a json file a parser is used, and you know how you can use `document.querySelector()` in your website? Well that's your browser parsing the HTML and returning the corresponding element depending on your query.

Once you learn parsing techniqes, you will have an extremely valuable new view at how compilers work and maybe even how to make your own special language!

## Guide to our tool

Our tool will have a few usecases and flags.

1. `-i [raw-md]` tells our tool that the next argument will be raw markdown.
2. `-if [md-file]` tells our tool that the next argument will be a markdown file.
3. `-of [{Optional} filename]` tells our tool to output the result html in a file,
    if no argument passed the html file will have the same name as the markdown file.

Our tool will only supports the following markdown features:

- bold text
- italic text
- bold italic text
- headings
- unordered lists
- ordered lists
- links
- images

The flavor of markdown we will be parsing is [github flavored markdown](https://github.github.com/gfm/) or (gfm).

However as a ***bonus*** you can add the flag `-flavor=` to configure which flavor of markdown our tool will parse.

## Example

### Example 1

```console
member@loop$ md2html -if README.md -of
```

results in the content of `README.md` file to be converted to `README.html` file

### Example 2

```console
member@loop$ md2html -if README.md -of document.html
```

results in `README.md` file being converted to `document.html` file

### Example 3

```console
member@loop$ md2html -i "# Hello world"
```

prints to the terminal `<html><body><h1>Hello world</h1></body></html>`

## Bonuses

- Add a `-flavor=` flag to specify which flavor of markdown to parse.
- Write the tool in a functional programming language.
- Use a [TDD](https://en.wikipedia.org/wiki/Test-driven_development#:~:text=Test%20Driven%20Development%20(TDD)%20is,leading%20to%20more%20robust%20software.) approach when writing your project.
- Support all different syntaxes of markdown.

## Submissions

When you finish the tool, upload your project to github and send us the link to it via our community whatsapp group chat.
Then when our admins are free, they will review your code and check if it's correct, if so your solution will be chosen to represent the solution
of this weeks challenge in the language you have chosen to solve it in.

## Useful links to help you with this challenge

- [Crafting interpreters (The parsing chapter) (recursive descent)](https://www.craftinginterpreters.com/parsing-expressions.html)
- [github flavored markdown](https://github.github.com/gfm/)
