Markdown is a simple way to format text in documents without learning a complex piece of software or a large number of commands or techniques.

Markdown makes writing clear and readable notes easy.

## Titles
using a hash symbol `#` followed by a space and a name makes a title: `# Title`
## Headings
using two or more hash symbols `##` followed by a space and a name makes a heading 2, 3, 4 etc. depending on how many hashes are used. e.g.
`# Heading 1`
`## Heading 2`
`### Heading 3`
and so on...

## Italics
Italics can be done by surrounding a word with single asterisks `*` or underscores `_` for example *here's a sentence that has been italicised.* it looks like this `*emphasise these words*` or `_emphasise these words_`
## Bold
Bolding can be done by surrounding a word with double asterisks `**` or underscores `__` for example **here's a sentence that has been emboldened.** it looks like this `**bold these words**` or `__bold these words__`

## Code Fences
Code fences are a way to indicate that you want to have code highlighted with syntax highlighting in your notes, this is especially useful in Computer Science lessons!

code fences are made using backticks ``` ` ``` these can be found next to 1 on the keyboard and above tab.

A pair of backticks around a word will make it into a 'code fenced word' for example like `this` code fences change font to a mono font (so that letters are of equal width)

Three backtics indicates a block of text over multiple lines, you can also specify a language after the first set of backticks to use syntax highlighting. for example

``` python
def func():
	print("hello world")
```

this uses three backticks followed by the word python on the first line, then the code, then three backticks after the last line to indicate where the code ends.

how to write it:
```` markdown
``` python
def func():
	print("hello world")
```
````

here's an example for any shell application (bash, zsh, cmd etc.)

``` shell
mkdir test
cd test
touch test.txt
mv test.txt testing.txt
```

and here's how to write it:
```` markdown
``` shell
mkdir test
cd test
touch test.txt
mv test.txt testing.txt
```
````

