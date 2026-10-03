---
title: Expression Functions
parent: "Workspace"
nav_order: 2
---
# Expression Functions

Every function listed here can be called from any expression - in a [Variable Sheet](variable-sheet.md) cell or directly in an object's parameter field. Function names are not case sensitive, so `SQRT(2)` and `sqrt(2)` are the same call.

For the syntax around these functions - the leading `=`, operators, cell references and bracket tokens - see [Expressions](expressions.md).

## Text Arguments

A text argument is written in double quotes, and the usual escape sequences are honoured inside them: `\n` for a newline, `\r` for a carriage return, `\t` for a tab, `\\` for a backslash, `\"` for a double quote and `\'` for a single quote. Each reaches the function as the character it stands for, so any of them can be used as a delimiter:

```
=split(A1, "\n", 0)      the first line of a multi-line value
=count(A1, "\n")         how many lines that value has
=split(A1, "\"", 1)      splits on a double quote character
```

Escapes belong to the **formula text**, not to your data. A cell holding `C:\new\temp` reaches `split()`, `count()`, `substitute()` and `strcat()` exactly as the sheet stores it - the `\n` in the middle of it is two characters, not a newline.

## Math Functions

Any one- or two-argument method of the standard math library is available by name. The most useful ones:

| Function | Result |
| --- | --- |
| `abs(x)` | Absolute value: `=abs(-3)` is `3` |
| `sign(x)` | `-1`, `0` or `1` depending on the sign of `x` |
| `sqrt(x)` | Square root: `=sqrt(2)` is `1.4142135623730951` |
| `cbrt(x)` | Cube root |
| `pow(x, y)` | `x` raised to the power `y`: `=pow(2, 10)` is `1024` |
| `exp(x)` | `e` raised to the power `x` |
| `log(x)` | Natural logarithm. `log(x, base)` uses the base you give |
| `log10(x)`, `log2(x)` | Base 10 and base 2 logarithms |
| `min(a, b)`, `max(a, b)` | The smaller or larger of two values: `=max(wall, 1.2)` |
| `floor(x)`, `ceiling(x)` | Round down or up to a whole number |
| `round(x)` | Round to the nearest whole number |
| `truncate(x)` | Drop the fractional part |
| `sin(x)`, `cos(x)`, `tan(x)` | Trigonometry, in **radians** |
| `asin(x)`, `acos(x)`, `atan(x)` | Inverse trigonometry, returning radians |
| `atan2(y, x)` | The angle of the point (x, y), in radians |
| `sinh(x)`, `cosh(x)`, `tanh(x)` | Hyperbolic functions |

Two things to watch for:

- **Angles are radians.** Convert with `pi`: `=sin(30 * pi / 180)` is the sine of 30 degrees.
- **`round()` takes one argument.** There is no "round to 2 decimals" second argument. Scale instead: `=round(A1 * 100) / 100`.

`clamp(value, low, high)` also resolves, holding a value between two bounds.

## sum

```
sum(value, value, ...)
```

Adds its arguments. `=sum(A1, A2, A3)` totals three cells; `=sum(2, 3, 4)` is `9`.

## mod

```
mod(number, divisor)
```

The remainder of `number` divided by `divisor`: `=mod(7, 3)` is `1`.

The result always takes the sign of the **divisor**, the way a spreadsheet's `MOD` does — so `=mod(-1, 2)` is `1`, not `-1`. That is what makes it safe for "every other one" tests, which stay correct even where the counter goes negative:

```
=mod(index, 2) == 0
```

That is `1` on the even items and `0` on the odd ones, so multiplying by it turns a feature on for every other one.

The divisor does not have to be a whole number: `=mod(0.85, 0.05)` is `0`, and `=mod(0.9, 0.4)` is `0.1`.

A divisor of `0` has no answer, so it is an error — the cell shows the formula text instead of a value, the same as dividing by zero does.

## strcat / concat

```
strcat(value, value, ...)
concat(value, value, ...)
```

Joins its arguments into one piece of text. The two names do the same thing.

```
=strcat("MC-", A2, "-", B2)
```

With `A2` holding `MMQFQZ5S` and `B2` holding `12`, that produces `MC-MMQFQZ5S-12`. Escape sequences inside quoted arguments are honoured, so `=strcat(A1, "\n", A2)` puts the two values on separate lines.

## strlen

```
strlen(text)
```

The number of characters in a piece of text: `=strlen("MMQFQZ5S")` is `8`.

Measuring a cell works the same way: with `A2` holding `MMQFQZ5S`, `=strlen(A2)` is also `8` — what the cell shows is what gets counted.

## substring

```
substring(text, start, length)
```

Pulls `length` characters out of `text`, counting from `start` where the first character is `0`.

```
=substring("MMQFQZ5S", 0, 2)
```

gives `MM`. A start past the end of the text, or a length of zero or less, gives an empty result rather than an error.

## split

```
split(text, delimiter, index)
```

Splits `text` on `delimiter` and returns one piece, counting from `0`. The delimiter defaults to a comma and the index defaults to `0`. Each piece has its leading and trailing spaces trimmed, and an index past the end gives an empty result.

```
=split("10, 20, 30", ",", 1)
```

gives `20`.

## count

```
count(text, delimiter)
```

How many pieces `text` splits into - always one more than the number of delimiters found. The delimiter defaults to a comma.

```
=count("10, 20, 30", ",")
```

gives `3`. This is the natural partner to `split()` when the number of items is not known in advance, for example as an Array **Count**.

## substitute

```
substitute(text, old_text, new_text)
substitute(text, old_text, new_text, occurrence)
```

Replaces text. With three arguments every occurrence is replaced. With a fourth, only that one occurrence is, counting from `0`.

```
=substitute("a-b-c", "-", "_")        gives  a_b_c
=substitute("a-b-c", "-", "_", 1)     gives  a-b_c
```

## index

```
index(column, row)
```

Reads the cell at a column and a row - the one thing a written-out reference like `=A7` cannot do, because `index()` will take a **calculated** row.

The column is given in quotes and the row is the **one-based** number shown down the left of the sheet, exactly as in A1 notation. So `=index("A", 2)` and `=A2` are the same value.

The quoted column can be written two ways:

- **The name of a cell in that column.** If C1 is named `product_price`, `=index("product_price", 2)` reads `C2`. Naming the header cell is the natural way to do this, so a formula can say which column it means instead of counting letters across the top of the sheet.
- **Column letters** - `"A"`, `"ab"`. A full cell id is not a column: `"A1"` names a cell.

The name is read **first**, and column letters are what text no name claims falls back to. That is what lets a short name work: the columns run `A` to `XFD`, so a one, two or three letter name like `sku` is also column letters - for a column 13,000 columns off the right of any sheet you would build - and `=index("sku", 2)` means the cell you named. The two readings cannot collide, because a cell may not be **named** after a column of its own sheet: on a five column sheet the editor refuses `A` through `E` and accepts `F`, `sku` and `sku_id`.

The name is read as the formula is evaluated, so **renaming the cell does not rewrite it**. Rename `price` to `cost` and every `=price` in the design is rewritten, but `=index("price", 2)` still says `"price"` and has to be retyped. You are told which ones: a rename shows a message listing every formula left quoting the old name, so none of them go quietly stale. In a sheet whose names move about, column letters are the safer thing to write.

The point of the function is a row that is worked out rather than typed. Inside an [Array](../operations/array/index.md), each copy substitutes its own position for `[index]`:

```
=index("A", [index]+2)
```

The first copy reads `A2`, the second `A3`, the third `A4` - walking down column A while skipping the header in row 1. Put that in a Text object's text field and an array of it prints a different part number on every copy.

A quoted column that is neither column letters nor a name some cell has (`"A1"` is a cell, not a column), or a row past the bottom of the sheet, is treated exactly like a misspelled cell reference - the sheet shows `0` rather than inventing a value.

## xlookup

```
xlookup(lookup_value, lookup_column, return_column)
xlookup(lookup_value, lookup_column, return_column, if_not_found)
```

Searches down `lookup_column` for `lookup_value` and returns whatever `return_column` holds on that row. Where `index()` needs to be told the row, `xlookup()` finds it.

<!-- IMAGE_NEEDED: A sheet holding a small price list - ids in column A, names in column B, prices in column C - with a cell selected whose formula box shows =xlookup("Magenta thing", "B", "A") -->

Given a price list with ids in column A, names in column B and prices in column C:

```
=xlookup("Magenta thing", "B", "A")     gives  MMQFQZ5S
=xlookup("Magenta thing", "B", "C")     gives  19.99
```

The rules:

- **Both columns are quoted, and take either form `index()` takes** - the name of a cell in that column, or column letters (`"A"`, `"ab"`). Name A1 `sku_id` and B1 `sku_name` and the first example above can be written `=xlookup("Magenta thing", "sku_name", "sku_id")`. A full cell id is not a column, and neither is a bare `A` without the quotes. See [index](#index) for which of the two a quoted column is read as, and why a rename leaves it alone.
- **The search runs from row 1 down**, so a header row is scanned like any other.
- **The match is exact.** There is no partial or wildcard matching.
- **Text matches without regard to case**, so `"magenta THING"` finds `Magenta thing`.
- **Numbers match as numbers**, so `19.99` finds a cell holding `19.9900`.
- **The first matching row wins** when a value appears more than once.
- **Empty cells do not stop the search** - a gap in the middle of the column is scanned past.
- `if_not_found`, when given, is what you get when nothing matches: `=xlookup("no such thing", "B", "A", "unknown")`.
- **Without `if_not_found`, a miss behaves like a reference to a cell that does not exist** - the sheet shows `0`, and anything downstream is deferred rather than fed a made-up value.
- **A misspelled column - or a name no cell has - is a broken reference, not a miss.** `if_not_found` deliberately does not cover it, so a typo in a column shows up instead of being quietly answered.

## importdata

```
importdata(url_or_path)
```

Reads a whole URL or local file and returns its contents. A body that parses as a number comes back as a number; anything else comes back as text.

```
=importdata("https://example.com/current-length.txt")
=importdata("C:/Parts/sizes.csv")
```

Notes:

- **Use forward slashes in local paths.** A backslash starts an escape sequence inside a quoted argument, so write `"C:/Parts/sizes.csv"` rather than `"C:\Parts\sizes.csv"`.
- **Results are cached for the session.** The same URL or path is fetched once. To pick up a source that has changed, use **Refresh Imported Data** on the sheet editor's File menu - see [Editing a Variable Sheet](sheet-editing.md#refresh-imported-data).
- **A failure comes back as text** beginning with `Error:`, so a broken link shows in the cell instead of breaking the design.
- **`importdata` needs a desktop MatterCAD.** Neither source works in the browser build: a URL is refused outright, because the sheet evaluates synchronously and the browser has no synchronous fetch, and a local path fails on the sandbox that keeps a page away from your disk. Either way the cell shows an `Error:` message rather than a value.

### Designs From Someone Else Ask First

A design can use `importdata()` to read any file on your computer or send a web address anything it read, so a design you did not make here does not read anything until you say so. When you open one, its imported values are blank and a bar across the top of the 3D view says **This design reads files from your computer or the web. Only allow designs you trust.**

- **Allow** lets the design read, and its values fill in. MatterCAD remembers this for that file, so it does not ask again - unless someone changes the file.
- **The X** hides the bar and leaves the values blank.

Designs you make and save in MatterCAD on this computer never ask. Network shares (paths starting with `\\` or `//`) are never read, even after Allow.

Cells you copy out of a design that has not been allowed stay blocked when you paste them into another sheet. Text you paste from another program, and a CSV you import, arrive as typed formulas: an `importdata()` in them runs in your design like one you typed, so check what you paste.

### Reading a CSV Row by Row

`importdata()` hands back the whole file, so pull it apart with `split()` - once on newlines to pick a line, then again on commas to pick a field. The newline is written inline as `"\n"`, so the whole thing fits in one cell:

```
=split(split(importdata("C:/Parts/sizes.csv"), "\n", 2), ",", 0)
```

The inner `split()` takes line `2` (counting from 0, so the third line); the outer one takes field `0` of that line. Change the line number to `[index]+1` in an object's parameter field and each copy in an [Array](../operations/array/index.md) reads its own row of the file.

`count()` sizes the run for you - `=count(importdata("C:/Parts/sizes.csv"), "\n")` is the number of lines in the file, which is what an Array's **Count** wants. `importdata()` trims the whitespace off both ends of what it reads, so a file that ends with a newline does not leave an empty line on the end of the count, and `split()` trims each piece it hands back, so a Windows file's carriage returns do not come through either.

## rand

```
rand()
rand(seed)
```

A random number between 0 and 1. Called with no argument it is different every time the expression is evaluated. Called with a seed it is deterministic - the same seed always gives the same number, which is what you want for a design that has to look the same every time it is opened.

```
=rand(7) * 10
```

`[rand]` in square brackets does the same job as `rand()` and works in object parameter fields - see [Expressions](expressions.md).

## Related

- [Expressions](expressions.md) - Expression syntax, constants, cell references and bracket tokens
- [Variable Sheet](variable-sheet.md) - Where sheet values and named cells come from
- [Editing a Variable Sheet](sheet-editing.md) - Rows and columns, cell formats, and refreshing imported data
- [Object References](object-references.md) - Read another object's settings inside an expression
- [Array](../operations/array/index.md) - Drive each copy from its own row with `[index]`
