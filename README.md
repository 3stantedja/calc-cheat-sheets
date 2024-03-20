# `calc-cheat-sheets`

Cheat sheets for MATH 144 midterms (Winter 2024) at the University of Alberta.
The documents only contain stuff that I deemed pretty important to recall.

## Prerequisites and Building

You will need a fairly-complete TeX distribution — in my case I use MacTeX, which is TeX Live on macOS.
Make sure that `latexmk` is included in your TeX distribution (especially for MiKTeX distribution users.)

Clone this repository, and include the submodule[^1] as well; i.e.

```shell
$ git clone --recurse-submodules https://github.com/3stantedja/calc-cheat-sheets.git
```

After going into the repo, assuming you have a complete TeX distribution, run `latexmk` on the file you want to compile; e.g.

```shell
$ latexmk main.tex
```

The resulting PDF document should be at the `./outputs` folder, which should be generated by `latexmk` as part of the compiling process.
Note that it uses pdfTeX as its engine; as such I cannot guarantee that it'll compile on LuaTeX nor XeTeX.
I haven't had the time to test whether this will work with other TeX engines.

## Attributions

The cheat sheet is partly inspired by (and copied from) [Paul's Online Math Notes](https://tutorial.math.lamar.edu/); in particular his various cheat sheets for algebra and calculus, alongside my notes from this course.

[^1]: The reason that it's in a submodule is more so that I have a set of common packages that I use all in one place, and readily available, as soon as the LaTeX repo is cloned.