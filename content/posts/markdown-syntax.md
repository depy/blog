---
title: "Markdown syntax"
date: 2023-03-31T14:44:51+02:00
publishDate: 2023-04-02
draft: false
---


## Gist markdown examples

A collection of Markdown code and tricks that were tested to work in Gist.

This and all public gists in https://gist.github.com/ww9 are [Public Domain](https://en.wikipedia.org/wiki/Public_domain_equivalent_license). Do whatever you want with it including , no need to credit me.

I'm baby narwhal unicorn fit woke, neutral milk hotel PBR&B hella cupping gastropub plaid slow-carb. XOXO pickled health goth pok pok messenger bag. Raclette street art disrupt stumptown. Portland knausgaard lo-fi palo santo, sus fashion axe bespoke small batch tote bag readymade gochujang etsy.

-----

Trust fund praxis neutral milk hotel af truffaut, gochujang sustainable deep v vice mukbang gatekeep photo booth hoodie. Green juice vaporware mixtape viral. Pickled church-key praxis selvage selfies brunch messenger bag, chartreuse occupy asymmetrical big mood pok pok craft beer vape. Gluten-free bicycle rights pop-up yr, iceland tonx banjo intelligentsia palo santo flexitarian artisan gastropub. Cloud bread single-origin coffee blackbird spyplane tacos whatever stumptown sartorial pinterest letterpress offal gluten-free before they sold out hammock.

### Lorem poopsom

Wayfarers selvage 8-bit trust fund marxism bodega boys sustainable. Keffiyeh fit migas sustainable activated charcoal swag big mood. Fixie banh mi pinterest bushwick. Cred lyft yr tattooed. Wayfarers woke narwhal single-origin coffee tote bag. Vibecession disrupt intelligentsia truffaut big mood af vexillologist put a bird on it before they sold out prism venmo whatever tilde irony everyday carry. Trust fund butcher neutra skateboard four dollar toast.

#### Porem loopsom

This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.

Hello, world!

<small>small text</small>

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.

### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Images

![Red Mage Gopher](/images/rdmgopher.png)

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

   Name | Age
--------|------
    Bob | 27
  Alice | 23
  Whoda | 37

### Inline Markdown within tables

Table with no header...

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

## Code Blocks

### Code block with backticks

```
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

{{< highlight js >}}
var x, y, z;  // Declare 3 variables
x = 5;    // Assign the value 5 to x
y = 6;    // Assign the value 6 to y
z = x + y;  // Assign the sum of x and y to z

document.getElementById("demo").innerHTML =
"The value of z is " + z + ".";
{{< /highlight >}}

{{< highlight ruby >}}
def sum_eq_n?(arr, n)
  return true if arr.empty? && n == 0

  arr.product(arr).reject { |a,b| a == b }.any? { |a,b| a + b == n }
end
{{< /highlight >}}

{{< highlight python >}}
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def myfunc(self):
    print("Hello my name is " + self.name)

p1 = Person("John", 36)

p1.age = 40

print(p1.age)
{{< /highlight >}}

{{< highlight j >}}
dna =: +/"1 @: ('ACGT'=/])
rna =: (] ` (]&'U') @. ('T'=]))"0
revc =: |. @ ('TCAG' {~ 'AGTC' i."1 ])
{{< /highlight >}}

{{< highlight forth >}}
\ "No Weighting" from Starting Forth Chapter 12
VARIABLE DENSITY
VARIABLE THETA
VARIABLE ID

: " ( -- addr )   [CHAR] " WORD DUP C@ 1+ ALLOT ;

: MATERIAL ( addr n1 n2 -- )    \ addr=string, n1=density, n2=theta
   CREATE  , , , 
   DOES> ( -- )   DUP @ THETA !
   CELL+ DUP @ DENSITY !  CELL+ @ ID ! ;

: .SUBSTANCE ( -- )   ID @ COUNT TYPE ;
: FOOT ( n1 -- n2 )   10 * ;
: INCH ( n1 -- n2 )   100 12 */  5 +  10 /  + ;
: /TAN ( n1 -- n2 )   1000 THETA @ */ ;

: PILE ( n -- )         \ n=scaled height
   DUP DUP 10 */ 1000 */  355 339 */  /TAN /TAN
   DENSITY @ 200 */  ." = " . ." tons of "  .SUBSTANCE ;

\ table of materials
\   string-address  density  tan[theta] 
   " cement"           131        700  MATERIAL CEMENT
   " loose gravel"      93        649  MATERIAL LOOSE-GRAVEL
   " packed gravel"    100        700  MATERIAL PACKED-GRAVEL
   " dry sand"          90        754  MATERIAL DRY-SAND
   " wet sand"         118        900  MATERIAL WET-SAND
   " clay"             120        727  MATERIAL CLAY
{{< /highlight >}}

### Code block indented with four spaces

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

### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title><br/><br/>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

## List Types

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

* List item
* Another item
* And another item

### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese