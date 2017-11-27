# latex-cvinfo

By [ddspog](https://github.com/ddspog)

**cvinfo** package allows fetching data from a JSON file to insert on Latex files.

## License

You are free to copy, modify and distribute **cvinfo** with attribution under the terms of the MIT license. See the [LICENSE](https://github.com/ddspog/latex-cvinfo/blob/master/LICENSE) file for details.

## Installation

Before using **cvinfo** you need:

* LuaLaTeX Engine

Setup your way of reading and compiling Latex files. Then, on folder for public packages, put these files naming the folder as **cvinfo**. Update the packages, and you're ready to use this package.

## How to use

Import the package like this:

```latex
\usepackage{cvinfo}
```

Then you're ready to use it with the environment **loadinfo**:

```latex
\begin{loadinfo}{testinfo.json}%
    My name is \ctcname{3}
    and my phone is \ctccellphone%
\end{loadinfo}%
```

The *testinfo.json* must contain the fields used on cvinfo.sty file. Read it to understand how to structure your JSON data file.

## Contribution

This package has two objectives from now:

* Create a general function to access the fields, like:

```latex
\data{'contact'}{'name'}{3}
```

* Publish the package on Latex official repo.