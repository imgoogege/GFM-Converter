<div align="center">
    <img src="doc/LogoMakr_0AdsfK.png" width="200px">
</div>

<!-- GFM-TOC -->
* [Preview](#preview)
* [Introduction](#introduction)
* [Usage](#usage)
<!-- GFM-TOC -->


# Preview

[Output.md](https://github.com/CyC2018/GFM-Converter/blob/master/Output.md)

```text
[TOC]

# Formula

## Line

$$ f = \frac{a}{b} $$

## Inline

$ \vec{a} $ and $ \vec{b} $

# Center Tag

## Text

<center> What doesn't kill you makes you stronger. </center>

## Picture

<center> ![](pics/1.png) </center>
```


# Introduction

- Replace `[TOC]` tag into generated catalogue.
- Use CodeCogs to display Mathjax formula.
- Escape some spacial characters.

# Usage

You can just run App.java, and then specify the path of Markdown document. After that, a new file suffixed with `.gfm` will be generated.

```java
javac -encoding UTF-8 App.java
java App
```

You can also use below API in your program.

```java
GFM.convert(srcFilePath, detFilePath);
```