# Gonum Plot  [![Build Status](https://travis-ci.org/gonum/plot.svg?branch=master)](https://travis-ci.org/gonum/plot) [![Coverage Status](https://img.shields.io/coveralls/gonum/plot.svg)](https://coveralls.io/r/gonum/plot) [![GoDoc](https://godoc.org/github.com/gonum/plot?status.svg)](https://godoc.org/github.com/gonum/plot)

`gonum/plot` is the new, official fork of code.google.com/p/plotinum.
It provides an API for building and drawing plots in Go.
*Note* that this new API is still in flux and may change.
See the wiki for some [example plots](http://github.com/gonum/plot/wiki/Example-plots).

There is a discussion list on Google Groups: gonum-dev@googlegroups.com.

`gonum/plot` is split into a few packages:

* The `plot` package provides simple interface for laying out a plot and provides primitives for drawing to it.
* The `plotter` package provides a standard set of `Plotter`s which use the primitives provided by the `plot` package for drawing lines, scatter plots, box plots, error bars, etc. to a plot. You do not need to use the `plotter` package to make use of `gonum/plot`, however: see the wiki for a tutorial on making your own custom plotters.
* The `plotutil` package contains a few routines that allow some common plot types to be made very easily. This package is quite new so it is not as well tested as the others and it is bound to change.
* The `vg` package provides a generic vector graphics API that sits on top of other vector graphics back-ends such as a custom EPS back-end, draw2d, SVGo, X-Window and gopdf.

## Documentation

Documentation is available at:

  https://godoc.org/github.com/gonum/plot

## Installation

You can get `gonum/plot` using go get:

`go get github.com/gonum/plot/...`

If you write a cool plotter that you think others may be interested in using, please post to the list so that we can link to it in the `gonum/plot` wiki or possibly integrate it into the `plotter` package.
