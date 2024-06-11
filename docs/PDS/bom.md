---
date: 2024-01-31
authors:
  - squidfunk
    ...
---
# BOM


[mkdocs.dotfiles]: Hyper Text Markup Language
[mkdocs]: World Wide Web Consortium


## Tabs

=== "Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Tab 2"
    More Markdown **content**.

    - list item a
    - list item b




$p(x|y) = \frac{p(y|x)p(x)}{p(y)}$, \(p(x|y) = \frac{p(y|x)p(x)}{p(y)}\).

$p(x|y) = \frac{p(y|x)p(x)}{p(y)}$, \(p(x|y) = \frac{p(y|x)p(x)}{p(y)}\).


==This was marked (highlight)==


- ~~This was deleted (strikethrough)~~


- H~2~O
- A^T^A

++ctrl+alt+del++

:smile:

``` title=".browserslistrc"
--8<-- ".browserslistrc"

Holca como estas
```

:fontawesome-regular-face-laugh-wink:

![Image title](https://dummyimage.com/600x400/eee/aaa){ align=left }

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Tablas

|           Id          	|      Valor     	| Cantidad 	|   URL   	|
|:---------------------:	|:--------------:	|:--------:	|:-------:	|
| C1,C2                 	| :material-check: 10uF-16V       	| 2        	|         	|
| C3,C11                	| 470nF-50V      	| 2        	|         	|
| C4,C9,C12,C17         	| 22uF-25V       	| 4        	|         	|
| C5,C6,C10,C13,C14,C18 	| 100nF-50V      	| 6        	|         	|
| C7,C8,C15,C16         	| 1000uF-35V     	| 4        	|         	|
| D1                    	| 1N4148         	| 1        	|         	|
| J1                    	| Conn_3x3.96mm  	| 1        	| Comprar 	|
| J2,J4                 	| Conn_02x2.54mm 	| 2        	| Comprar 	|
| J3                    	| Conn_03x2.54mm 	| 1        	| Comprar 	|
| JP1                   	| EN             	| 1        	|         	|
| R1,R2,R3              	| 10K            	| 3        	|         	|
| R4                    	| 20K            	| 1        	|         	|
| R5                    	| 30K            	| 1        	|         	|
| R6,R8,R10,R12         	| 22K            	| 4        	|         	|
| R7,R11                	| 680            	| 2        	|         	|
| R9,R13                	| 2.7-2W         	| 2        	|         	|
| U1,U2                 	| TDA7294        	| 2        	| Comprar 	|

## Alternativos

Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse
cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non
proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

## Listas

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque


## Ecuaciones 

$$
\operatorname{ker} f=\{g\in G:f(g)=e_{H}\}{\mbox{.}}
$$


### Tasklist

<!-- md:version 1.0.0 -->
<!-- md:extension [pymdownx.tasklist][Tasklist] -->

The [Tasklist] extension allows for the usage of [GitHub Flavored Markdown]
inspired [task lists][Tasklist specification], following the same syntactical
conventions. Enable it via `mkdocs.yml`:

``` yaml
markdown_extensions:
  - pymdownx.tasklist:
      custom_checkbox: true
```

The following configuration options are supported:

<!-- md:option pymdownx.tasklist.custom_checkbox -->

:   <!-- md:default `false` --> This option toggles the rendering
    style of checkboxes, replacing native checkbox styles with beautiful icons,
    and is therefore recommended:

    ``` yaml
    markdown_extensions:
      - pymdownx.tasklist:
          custom_checkbox: true
    ```

<!-- md:option pymdownx.tasklist.clickable_checkbox -->

:   <!-- md:default `false` --> This option toggles whether
    checkboxes are clickable. As the state is not persisted, the use of this
    option is _rather discouraged_ from a user experience perspective:

    ``` yaml
    markdown_extensions:
      - pymdownx.tasklist:
          clickable_checkbox: true
    ```

The other configuration options of this extension are not officially supported
by Material for MkDocs, which is why they may yield unexpected results. Use
them at your own risk.

See reference for usage:

- [Using task lists]

  [Tasklist]: https://facelessuser.github.io/pymdown-extensions/extensions/tasklist/
  [GitHub Flavored Markdown]: https://github.github.com/gfm/
  [Tasklist specification]: https://github.github.com/gfm/#task-list-items-extension-
  [Using task lists]: ../../reference/lists.md#using-task-lists



``` py title="hola.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```