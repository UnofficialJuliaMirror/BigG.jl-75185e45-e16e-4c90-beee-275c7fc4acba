# BigG.jl
A minimalistic Static Site Generator in Julia
Inspired by [this post](https://blog.thea.codes/a-small-static-site-generator/).


<!-- | **Build Status**                                                                                |
|:-----------------------------------------------------------------------------------------------:|
|[![Build Status](https://travis-ci.org/Moelf/Telegrambot.jl.svg?branch=master)](https://travis-ci.org/Moelf/Telegrambot.jl)| -->

## Installation

The package is not yet registered in `METADATA.jl` and can be installed with `Pkg.add`, or in `REPL` by pressing `] add Telegrambot`.
```julia
julia> Pkg.add("https://github.com/Moelf/BigG.jl")
```

## Basic Usage
Make two folders, `source` and `output`, put all `.md` files in `source` then:

```julia
using BigG

render_posts("./source", "./output", "BigG.jl/src/post.hbs")
render_index("./source", "./output", "BigG.jl/src/index.hbs")
```

This will generate an `index.html` where each `.md` will be rendered into a html and
linked in the index page.

## To-Do
- [ ] Allow directory structure (year/month/date/title.html)
