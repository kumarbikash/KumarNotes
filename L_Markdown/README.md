# Writing Markdown files

## **Headings**

<br />

```Markdown
# First Title
```

# First Title

<br />

```Markdown
## Second Title
```

## Second Title

<br />

```Markdown
### Third Title
```

### Third Title

<br />

```Markdown
#### Fourth Title
```

#### Fourth Title

<br />

```Markdown
##### Fifth Title
```

##### Fifth Title

<br />

```Markdown
###### Sixth Title 
```

###### Sixth Title  

<br />
<br />

## **Text Styles**

<br />

| Code | Preview
| --- | ---
| `**Bold Text**` | **Bold Text**
| `__Bold Text__` | __Bold Text__
| `*Italic Text*` | *Italic Text*
| `_Italic Text_` | _Italic Text_
| `~~Strikethrough Text~~` | ~~Strikethrough Text~~
| `***Bold + Italic Text***` | ***Bold + Italic Text***
| `**_Bold + Italic Text_**` | **_Bold + Italic Text_**
| `Text<sub>Subscript</sub>` | Text<sub>Subscript</sub>
| `Text<sup>Superscript</sup>` | Text<sup>Superscript</sup>

<!--
**Bold Text**
__Bold Text__
*Italic Text*
_Italic Text_
~~Strikethrough Text~~
***Bold + Italic Text***
**_Bold + Italic Text_**
Text<sub>Subscript</sub>
Text<sup>Superscript</sup> -->

<br />
<br />

## **Quoting Text**

<br />

```Markdown
>Quoted Text
```

>Quoted Text

<br />
<br />

## **Quoting Code**

<br />

```Markdown
`single line code`
```

`single line code`

<br />

````Markdown
```Markdown
multi line code - line 1
multi line code - line 2
```
````

```Markdown
multi line code - line 1
multi line code - line 2
```

<br />
<br />

## **Color Models**

<br />

| Code | Preview
| --- | ---
| \`#FFFFFF\` | `#FFFFFF`
| \`#rgb(255,255,255)\` | `#rgb(255,255,255)`
| \`#hsl(255,255,255)\` | `#hsl(255,255,255)`

<br />
<br />

## **Links**

<br />

| Code | Preview
| --- | ---
| `[Link Text](http://localhost/)` | [Link Text](http://localhost/)

<br />
<br />

## **Section Links**

<br />
Link is visible on hovering the rendered text.

<br />
<br />

## **Relative Links**

<br />

Relative paths `./` and `../` can be used.

<br />
<br />

## **Images**

<br />

| Code | Preview
| --- | ---
| `![altText](assets/github.png)` | ![altText](assets/github.png)

<br />
<br />

## **Theme**

<br />

```HTML
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/darkmode.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/lightmode.png">
  <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="assets/lightmode.png">
</picture>
```

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/darkmode.png">
  <source media="(prefers-color-scheme: light)" srcset="assets/lightmode.png">
  <img alt="Shows an illustrated sun in light color mode and a moon with stars in dark color mode." src="assets/lightmode.png">
</picture>

<br />
<br />

## **Lists**

<br />

```Markdown
- item 1
- item 2
- item 3
```

- item 1
- item 2
- item 3

<br />

```Markdown
* item 1
* item 2
* item 3
```

* item 1
* item 2
* item 3

<br />

```Markdown
1. item 1
2. item 2
3. item 3
```

1. item 1
2. item 2
3. item 3

<br />
<br />

## **Nested Lists**

<br />

```Markdown
1. first list item 
   - first nested list item
     - second nested list item
```

1. first list item 
   - first nested list item
     - second nested list item

<br />

```Markdown
100. first list item 
     - first nested list item
       - second nested list item
```

100. first list item 
     - first nested list item
       - second nested list item

<br />
<br />

## **Task List**

<br />

```Markdown
- [x] task 1
- [ ] task 2
- [ ] task 3
```

- [x] task 1
- [ ] task 2
- [ ] task 3

<br />
<br />

## **Escape Character**

<br />

| Code | Preview
| --- | ---
| \\\`code\\\` | \`code\`
| \\\*code\\\* | \*code\*

<br />
<br />

## **Mention People & Team**

<br />

```Markdown
@github/support
```
@github/support

<br />
<br />

## **Referencing Issues and Pull**

<br />

Using the character `#`

<br />
<br />

## **Emoji**

<br />

```Markdown
:EMOJICODE:
```

<br />

| Code | Preview
| --- | ---
| `:+1:` | :+1:
| `:shipit:` | :shipit:

<br />
<br />

## **Paragraph**

<br />

```Markdown
A very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence.

Another very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence.
```

<br />

A very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence.

Another very long sentence, very long sentence, very long sentence, very long sentence, very long sentence, very long sentence.

<br />
<br />

## **Footnote**

<br />

```Markdown
Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.
```

<br />

Here is a simple footnote[^1].

A footnote can also have multiple lines[^2].  

You can also use words, to fit your writing style more closely[^note].

[^1]: My reference.
[^2]: Every new line should be prefixed with 2 spaces.  
  This allows you to have a footnote with multiple lines.
[^note]:
    Named footnotes will still render with numbers instead of the text but allow easier identification and linking.  
    This footnote also has been made with a different syntax using 4 spaces for new lines.

<br />
<br />

## **Comment**

<br />

| Code | Preview
| --- | ---
| `<!-- commented text -->` | <!-- commented text -->

<br />
<br />

## **Table**

<br />

```Markdown
| Heading 1 | Heading 2 | Heading 3
| --- | --- | ---
| Row 1 Cell 1 | Row 1 Cell 2 | Row 1 Cell 3
| Row 2 Cell 1 | Row 2 Cell 2 | Row 2 Cell 3
```

| Heading 1 | Heading 2 | Heading 3
| --- | --- | ---
| Row 1 Cell 1 | Row 1 Cell 2 | Row 1 Cell 3
| Row 2 Cell 1 | Row 2 Cell 2 | Row 2 Cell 3

<br />

```Markdown
| Heading 1 | Heading 2 | Heading 3
| :--- | :---: | ---:
| Left | Center | Right
```

| Heading 1 | Heading 2 | Heading 3
| :--- | :---: | ---:
| Left | Center | Right

<br />
<br />

## **Collapsed Section**

<br />

````Markdown
<details><summary>CLICK ME</summary>
<p>

#### We can hide anything, even code!

```ruby
   puts "Hello World"
```

</p>
</details>
````

<details><summary>CLICK ME</summary>
<p>

#### We can hide anything, even code!

```ruby
   puts "Hello World"
```

</p>
</details>

<br />
<br />

## **Code Block**

<br />

````
```
function test() {
  console.log("test function");
}
```
````

```
function test() {
  console.log("test function");
}
```

<br />

\`\`\`\`
````
```
function test() {
  console.log("test function");
}
```
````
\`\`\`\`

````
```
function test() {
  console.log("test function");
}
```
````

<br />

````
```SQL
select * from tblname
  where colname is not null;
```
````

```SQL
select * from tblname
  where colname is not null;
```

<br />
<br />

## **Diagram**

<br />

````
```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```
````

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

GeoJSON, TopoJSON, STL 3D, etc. also available

<br />
<br />

## **Mathematical Expressions**

<br />

```
Inline with text: $\sqrt{3x-1} + (1+x)^2$
```

Inline with text: $\sqrt{3x-1} + (1+x)^2$

<br />

```
As block:

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$
```

As block:

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

<br />

````
```math
\sqrt{3}
```
````

```math
sqrt{3}
```


<br />
<br />
<br />

<hr />

```
02 Sep 2022
```