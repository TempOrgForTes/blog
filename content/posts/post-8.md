---
title: Markdown Syntax Guide
date: 2023-06-20T00:00:00.000Z
description: Sample article showcasing basic Markdown syntax and formatting for
  HTML elements.
tags:
  - markdown
  - css
  - html
  - themes
categories:
  - themes
  - syntax
---
THIS TEXT EDIT BY NETLIFY DECAP content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme. <!--more-->

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

## H2

### H3

#### H4

##### H5

###### H6

## Paragraph

Тестовий абзац вау<br>Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae. **Note** that you can use *Markdown syntax* within a blockquote.

### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.
>
> — <cite>Rob Pike[^1]</cite>
>
> &nbsp;

[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

<table><thead><tr><th><p>Name</p></th><th><p>Age</p></th></tr></thead></table>

```
Bob | 27
```

Alice | 23

### Inline Markdown within tables

<table><thead><tr><th><p>Inline&nbsp;&nbsp;&nbsp;</p></th><th><p>Markdown&nbsp;&nbsp;&nbsp;</p></th><th><p>In&nbsp;&nbsp;&nbsp;</p></th><th><p>Table</p></th></tr></thead><tbody><tr><td><p><em>italics</em></p></td><td><p><strong>bold</strong></p></td><td><p><s>strikethrough</s>&nbsp;&nbsp;&nbsp;</p></td><td><p><code>code</code></p></td></tr></tbody></table>

## Code Blocks

### Code block with backticks

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

### Extra wide code block

```scala
def make[F[_]: Sync: Parallel: ThrowableMonadError](cfg: ServiceConfig, client: Client[F]): HealthMonitorService[F] =
  new HealthMonitorService[F] {

    override def checkWorkerStatus(workerCfg: WorkerConfig): F[WorkerStatus] = ???
  }
```

### Code block indented with four spaces

```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

### Code block with Hugo's internal highlight shortcode

{{< highlight html >}}

<!DOCTYPE html>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

### Inline code

`Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum`

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

* Item

1. First Sub-item
2. Second Sub-item

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press

<kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd>

to end the session.

Most

<mark>salamanders</mark>

are nocturnal, and hunt for insects, worms, and other small creatures.
