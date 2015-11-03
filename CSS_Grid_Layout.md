CSS Grid Layout
===============
*By Rachel Andrew*

Remembers the "should we even use CSS" debate when Netscape still had a majority market share

Old-fashioned ways of doing layout

Flexbox isn't a grid solution. It's for one line or multi-line, so it's not just for one thing.

CSS Grid Layout first in IE10

CSS Properties
--------------

Display method
- display: grid or display: inline-grid

Column and row counts
- grid-template-columns
- grid-template-rows
- can use repeat keyword to multiply columns in an automated way
- can use subgrid keyword to leverage parent grid definition if used on a child

Gutters
- grid-column-gap
- grid-row-gap

Col/Row Properties
- grid-column (defaults to one column?)
- grid-row (defaults to one row)

Flow (packing)
- grid-flow: dense or sparse (sparse is default)

can span multiple rows/columns

shorthand uses "/" "start / end"

supports rtl/ltr writing modes

Terminology
-----------

Grid lines
- lines at the edge of columns or rows
- can be numbered
- can be named
``` CSS
.wrapper {
  display: grid;
  grid-template-columns: [col1-start] 100px [col1-end] 10px [col2-start] 100px [col2-end] 10px [col3-start] 100px [col3-end];
  grid-template-rows: [row1-start] auto [row1-end] 10px [row2-start] auto [row2-end];
}
```

Grid track
- space between two grid lines
Grid cells
- smallest unit, fits between four grid lines
Grid area
- any area on the grid bound by four grid lines, defined by setting start and end lines
- can be numbered
- can be named
``` CSS
.wrapper {
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer"
}
```

http://gridbyexample.com (only works in canary due to browser support)

fr unit - fraction unit, fraction of space in the available container
can mix fractions and pixels, applies px first then fr.

Allows for incredibly flexible prototyping, designing in the browser

Be aware of potential accessibility implications
Semantics must still be used
Grid does not change order in which source is read
Can have implications for tab order

Grid cells can become grids as well
Subgrid keyword
