# Markdown Kullanım Örnekleri Sayfası

Bu sayfada sık kullanılan componentlerin örnekleri verilmiştir. Ne yapabiliyorduk, nasıl yapıyorduk
(1) diye bakmak için kullanılabilir.
{ .annotate }

1.  Başlık altında ilgili dokümantasyon linki verilmiştir. Ayrıca sayfanın kaynak koduna bakıp
    kullanım da incelenebilir.

## Admonitions

[squidfunk.github.io/mkdocs-material/reference/admonitions/](https://squidfunk.github.io/mkdocs-material/reference/admonitions/)

!!! info "Custom Başlık"

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

??? tip "Collapsable Admonition"

    Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod
    nulla. Curabitur feugiat, tortor non consequat finibus, justo purus auctor
    massa, nec semper lorem quam in massa.

## Annotataions

[squidfunk.github.io/mkdocs-material/reference/annotations/](https://squidfunk.github.io/mkdocs-material/reference/annotations/)

Metin içerisinde (1) annotation.
{ .annotate }

1.  :man_raising_hand: I'm an annotation! I can contain `code`, __formatted text__, images, ...
    basically anything that can be expressed in Markdown.

```py
def triangle(size: int): # (1)!
{ .annotate }
    for i in range(1, size+1):
        print("*" * i)
```

1.  Annotation için eklediğimiz `(1)!` yorum satırında olmalı.

## Code Blocks

[squidfunk.github.io/mkdocs-material/reference/code-blocks](https://squidfunk.github.io/mkdocs-material/reference/code-blocks/)

Başlıklı code block:

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

Line numbers:

``` py linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

``` py hl_lines="3-5"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```

## Content Tabs

[squidfunk.github.io/mkdocs-material/reference/content-tabs/](https://squidfunk.github.io/mkdocs-material/reference/content-tabs/)

=== "C"

    Bu C

    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

=== "C++"

    Bu da C++

    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```

=== "Python"

    Ooo yeni bir tab daha

    ```python
    print("Hello world!")
    ```

## Tables

[squidfunk.github.io/mkdocs-material/reference/data-tables/](https://squidfunk.github.io/mkdocs-material/reference/data-tables/)


|  Method  |             Description              |
| :------: | :----------------------------------: |
|  `GET`   | :material-check:     Fetch resource  |
|  `PUT`   | :material-check-all: Update resource |
| `DELETE` | :material-close:     Delete resource |

## Diagrams

[squidfunk.github.io/mkdocs-material/reference/diagrams/](https://squidfunk.github.io/mkdocs-material/reference/diagrams/)

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

## Footnote

[squidfunk.github.io/mkdocs-material/reference/footnotes/](https://squidfunk.github.io/mkdocs-material/reference/footnotes/)

Lorem ipsum[^1] dolor sit amet, consectetur adipiscing elit.[^2]

[^1]: Lorem ipsum dolor sit amet, consectetur adipiscing elit.

[^2]: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla et euismod nulla. Curabitur
    feugiat, tortor non consequat finibus, justo purus auctor massa, nec semper lorem quam in massa.

## Formatting

[squidfunk.github.io/mkdocs-material/reference/formatting/](https://squidfunk.github.io/mkdocs-material/reference/formatting/)

**bold text**, _italic text_

Text can be {--deleted--} and replacement text {++added++}. This can also be combined into {~~one~>a
single~~} operation. {==Highlighting==} is also possible {>>and comments can be added inline<<}.

{==

Formatting can also be applied to blocks by putting the opening and closing tags on separate lines
and adding new lines between the tags and the content.

==}

- ==This was marked==
- ^^This was inserted^^
- ~~This was deleted~~
- H~2~O
- A^T^A
- ++ctrl+alt+del++


## Emojis, Icons

[squidfunk.github.io/mkdocs-material/reference/icons-emojis/](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/)

Emojiler için Tweetmoji kullanıyoruz. Emoji kodu bulmak veya emoji aramak için
[burası](https://squidfunk.github.io/mkdocs-material/reference/icons-emojis/#search) var.

:smile: :keyboard:

Fontawesome icon örnekleri:

:fontawesome-brands-youtube: :fontawesome-brands-linux: :fontawesome-brands-fedora:

## Images

[squidfunk.github.io/mkdocs-material/reference/images](https://squidfunk.github.io/mkdocs-material/reference/images)


![Image title](https://dummyimage.com/600x400/f5f5f5/aaaaaa?text=–%20Image%20–)

## Lists

[squidfunk.github.io/mkdocs-material/reference/lists/](https://squidfunk.github.io/mkdocs-material/reference/lists/)

- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur accumsan nibh eu mattis.
  Vivamus tempus velit eros, porttitor placerat nibh lacinia sed. Aenean in finibus diam.

    * Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    * Nam vulputate tincidunt fringilla.
    * Nullam dignissim ultrices urna non auctor.

- Nulla et rhoncus turpis. Mauris ultricies elementum leo. Duis efficitur accumsan nibh eu mattis.
  Vivamus tempus velit eros, porttitor placerat nibh lacinia sed. Aenean in finibus diam.

Definition list:

`Lorem ipsum dolor sit amet`

:   Sed sagittis eleifend rutrum. Donec vitae suscipit est. Nullam tempus tellus non sem
    sollicitudin, quis rutrum leo facilisis.

`Cras arcu libero`

:   Aliquam metus eros, pretium sed nulla venenatis, faucibus auctor ex. Proin ut eros sed sapien
    ullamcorper consequat. Nunc ligula ante.

    Duis mollis est eget nibh volutpat, fermentum aliquet dui mollis.
    Nam vulputate tincidunt fringilla.
    Nullam dignissim ultrices urna non auctor.

Task list:

- [x] Lorem ipsum dolor sit amet, consectetur adipiscing elit
- [ ] Vestibulum convallis sit amet nisi a tincidunt
    * [x] In hac habitasse platea dictumst
    * [x] In scelerisque nibh non dolor mollis congue sed et metus
    * [ ] Praesent sed risus massa
- [ ] Aenean pretium efficitur erat, donec pharetra, ligula non scelerisque

## Tooltips

The HTML specification is maintained by the W3C.

*[HTML]: Hyper Text Markup Language *[W3C]: World Wide Web Consortium
