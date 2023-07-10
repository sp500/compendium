# Markdown

Markdown is an easy-to-read, easy-to-write language for formatting plain text.


## Headings

``` title="headings"
# Markdown
## Headings
```

## Bold

** This is bold **

``` title="bold"
** This is bold **
```

## Italic

*This is italic*

``` title="italic"
*This is italic*
```

## Strikethrough

~~This is strikethrough~~

``` title="strikethrough"
~~This is strikethrough~~
```

## Subscript

Subscript<sub>1</sub>

``` title="subscript"
Subscript<sub>1</sub>
```

## Superscript

Superscript<sup>2</sup>

``` title="superscript"
Superscript<sup>2</sup>
```

## Quoting Text

> Quoted text


``` title="text"
> Quoted text
```


## Quoting Block


``` title="block"
line 1
line 2
line 3
```

## Links

Wrapping link text in brackets [ ], and then wrapping the URL or relative file in
parentheses ( ).

For example,

This site was built using [GitHub Pages](https://pages.github.com/)

``` title="url"
This site was built using [GitHub Pages](https://pages.github.com/)
```

This is [overview](./overview.md)

``` title="relative link"
This is [overview](./overview.md)
```


## Flowchart

``` title="flowchart mermaid"
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

``` mermaid
graph TD
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Root Cause];
  D --> B;
  B ---->|No| E[Yay!];
```

## Math
``` title="math equations" 
$$ 
\operatorname{ker} f=\{g\in G:f(g)=e_{H}\}{\mbox{.}}
$$
```
$$ 
\operatorname{ker} f=\{g\in G:f(g)=e_{H}\}{\mbox{.}}
$$

## More Information
- [Github: Basic Markdown Formatting](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [Github: Advanced Formatting](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
- [MkDocs Writing with Markdown](https://www.mkdocs.org/user-guide/writing-your-docs/#writing-with-markdown)
- [Docusaurus Markdown Features](https://docusaurus.io/docs/markdown-features)
- [Admonitions](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)
