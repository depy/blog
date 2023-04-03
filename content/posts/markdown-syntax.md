---
title: "Markdown syntax"
date: 2023-03-31T14:44:51+02:00
draft: false
---


## Gist markdown examples

A collection of Markdown code and tricks that were tested to work in Gist.

This and all public gists in https://gist.github.com/ww9 are [Public Domain](https://en.wikipedia.org/wiki/Public_domain_equivalent_license). Do whatever you want with it including , no need to credit me.

I'm baby narwhal unicorn fit woke, neutral milk hotel PBR&B hella cupping gastropub plaid slow-carb. XOXO pickled health goth pok pok messenger bag. Raclette street art disrupt stumptown. Portland knausgaard lo-fi palo santo, sus fashion axe bespoke small batch tote bag readymade gochujang etsy.

Trust fund praxis neutral milk hotel af truffaut, gochujang sustainable deep v vice mukbang gatekeep photo booth hoodie. Green juice vaporware mixtape viral. Pickled church-key praxis selvage selfies brunch messenger bag, chartreuse occupy asymmetrical big mood pok pok craft beer vape. Gluten-free bicycle rights pop-up yr, iceland tonx banjo intelligentsia palo santo flexitarian artisan gastropub. Cloud bread single-origin coffee blackbird spyplane tacos whatever stumptown sartorial pinterest letterpress offal gluten-free before they sold out hammock.

### Lorem poopsom

Wayfarers selvage 8-bit trust fund marxism bodega boys sustainable. Keffiyeh fit migas sustainable activated charcoal swag big mood. Fixie banh mi pinterest bushwick. Cred lyft yr tattooed. Wayfarers woke narwhal single-origin coffee tote bag. Vibecession disrupt intelligentsia truffaut big mood af vexillologist put a bird on it before they sold out prism venmo whatever tilde irony everyday carry. Trust fund butcher neutra skateboard four dollar toast.

#### Porem loopsom

This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

Hello, world!

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

   Name | Age
--------|------
    Bob | 27
  Alice | 23
  Whoda | 37

#### Inline Markdown within tables

Table with no header...

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## Code Blocks

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.
