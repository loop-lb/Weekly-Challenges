# Week-001 -- Build your own markdown to HTML CLI tool

## Guide to our tool

Our tool will have a few usecases and flags.

1. `-i [raw-md]` tells our tool that the next argument will be raw markdown.
2. `-if [md-file]` tells our tool that the next argument will be a markdown file.
3. `-of [{Optional} filename]` tells our tool to output the result html in a file,
    if no argument passed the html file will have the same name as the markdown file.

## Example

### Example 1

```bash
md2html -if README.md -of
```

results in README.html

### Example 2

```bash
md2html -if README.md -of document.html
```

results in README.md being converted to document.html

### Example 3

```bash
md2html -i "# Hello world"
```

prints to the terminal `"<html><body><h1>Hello world</h1></body></html>"`
