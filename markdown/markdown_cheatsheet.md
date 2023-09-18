# Markdown Cheatsheet
this document is intended as reference for some markdown files. The author does not claim completeness

## Table of contents

* [Headers](#headers)
* [Lists](#lists)
* [Text decoration](#text-decoration)
* [Links](#links)
* [Images](#images)
* [Code](#code)
* [Tables](#tables)
* [Block quotes](#block-quotes)
* [Horizontal Rule](#horizontal-rule)
* [Inline HTML](#inline-html)


## Headers

````md
# H1
## H2
### H3
#### H4
##### H5
###### H6
````

## Text decoration

````md
Italics: *asterisks* or _underscore_
Bold: **double asterisks** or __double underscore__
Mixed: **_mix both variants_** __*anyway u like*__
Underline: <u>use HTML u tag</u>
````

Italics: *asterisks* or _underscore_

Bold: **double asterisks** or __double underscore__

Mixed: **_mix both variants_** __*anyway u like*__

Underline: <u>use HTML u tag</u>

## Lists

### Ordered Lists

````md
1. Fist item
2. Second item
    1. Ordered sub list item must have four spaces
3. Third item
    * Unordered sub list item
4. etc.
````

1. First item
2. Second item
    1. Ordered sub list item must have four spaces
3. Third item
    * Unordered sub list item
4. etc.

### Unordered Lists

````md
* Unordered list can use asterisks
- Or minuses
+ Or pluses
````

* Unordered list can use asterisks
- Or minuses
+ Or pluses

## Links

````md
[External Link](https://www.google.com)
[Internal Link](#table-of-contents)
[Link to File](/directory/file.ext)
````
**NOTE:** Internal links must not have spaces and only one # sign although the section in the file might differ

[External Link](https://www.google.com)

[Internal Link](#table-of-contents)

[Link to File](/directory/file.ext)

## Images

````md
// schematic: start with ! then like a text link
![alt-text](url)
e.g.
![unsplash random image](https://source.unsplash.com/random/300x300)
````

![unsplash random image](https://source.unsplash.com/random/300x300)

## Code

````md
Inline code has backticks `like so`
````

Inline code has backticks `like so`

Blocks of code are either fenced by lines with four back-ticks ` ``` ` and snytax is added when the starting fence is provided wth the languafe like ` ```javascript`

````javascript
```javascript
const foo = 'bar';
console.log(foo);
```
````

## Tables

````md
Tables | Must | not
-- | --- | ---
be | pretty | !


| But       | a little   | effort |
| --------- | ---------- | ------ |
| increases | readability | a lot  |
````

Tables | Must | not
-- | --- | ---
be | pretty | !


| But       | a little   | effort |
| --------- | ---------- | ------ |
| increases | readability | a lot  |

## Block quotes

````md
> Block quotes can have
> multiple lines

This breaks the quote

> but will still be displayed as one line
>
> And cou can add **Markdown** inside a <u>Block quote</u>
````

> Block quotes can have
> multiple lines

This breaks the quote

> but will still be displayed as one line
> 
> And cou can add **Markdown** inside a <u>Block quote</u>


## Horizontal Rule

````md
Three or more...

---

Hyphens

***

Asterisks

___

Underscores
````

Three or more...

---

Hyphens

***

Asterisks

___

Underscores

## Inline HTML

For security reasons, not all Markdown applications support HTML in Markdown documents. When in doubt, check your Markdown application’s documentation. Some applications support only a subset of HTML tags.

