Command: gulp to run the fulp file


MAP-MERGE: 
------------------------------------------------
Sass map-merge() Function
The map-merge() function returns a new map with all the keys and values from both map1 and map2.

$colors: (
  primary: #BE0062,
  secondary: #D3A108
);

$custom: (
  myBlue: #20B7CE
);

$merge: map-merge($colors, $custom);

@debug map-has-key($merge, "primary"); // true
@debug map-has-key($merge, "secondary"); // true
@debug map-has-key($merge, "myBlue"); // true
@debug map-has-key($merge, "myRed"); // false

Syntax: map-merge($map1, $map2)

Parameter Value
Value	Type	Explanation
==============================================
$map1	Required	Specifies the first array.
$map2	Required	Specifies the second array.

Return Value
Value	Explanation
==============================================
array	Returns a new map with all the keys and values from both $map1 and $map2



GUTTER WIDTH
A gutter is the space between columns that helps separate content. Gutter widths are fixed values at each breakpoint range. To better adapt to a given screen size, gutter widths can change at different breakpoints. Wider gutters are more appropriate for larger screens, as they create more open space between columns.