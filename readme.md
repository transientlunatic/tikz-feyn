Tikz-feyn
=========

Tikz-feyn is a LaTeX package which generates Feynman diagrams using
the PGF/TikZ package.

Usage
=====

Tikz-feyn can be loaded by
```tex
\usepackage{tikz-feyn}
```

A Feynman diagram can be constructed in one of two environments:

+ `tfeyn` produces display-style-like diagrams, which are suitable for
being used in part of a diagram, for example
![example1](https://raw.github.com/transientlunatic/tikz-feyn/docs/feyn1.png)
+ `tfeynin` produces inline Feynman diagrams which can be inserted
into text, or into an equation, for example
![example2](https://raw.githubusercontent.com/transientlunatic/tikz-feyn/develop/docs/feyn5.png)
In the current implementation of Tikz-feyn each Feynman diagram is
composed of a number of columns. For example,
![example1](https://raw.githubusercontent.com/transientlunatic/tikz-feyn/develop/docs/feyn4.png)
contains three columns. We construct a column using the `\tfcol` macro:

```tex
\tfcol(0,0){a, b, ..., z}[<vertical space>]
```

This creates a column of vertices, each equally-spaced, with the
names, a, b, through to z. The bottom of the column will be aligned to
the coordinates in the first argument.



