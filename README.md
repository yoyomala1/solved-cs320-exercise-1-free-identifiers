Download Link: https://assignmentchef.com/product/solved-cs320-exercise-1-free-identifiers
<br>
<h2>1         Free Identifiers</h2>

Implement the function freeIds, which takes a WAE and produces a set of strings. The set should contain a string for each free identifier in the given WAE.

def freeIds(expr: WAE): Set[String] = ???

test(freeIds(WAE(“{with {x 1} {+ x y}}”)), Set(“y”)) test(freeIds(WAE(“{with {z 2} 1}”)), Set())

<h2>2          Binding Identifiers</h2>

Implement the function bindingIds, which is like freeIds, but the result set contains a string for each binding identifier in the given WAE (whether or not the binding identifier is ever referenced by a bound identifier).

def bindingIds(expr: WAE): Set[String] = ???

test(bindingIds(WAE(“{with {x 1} {+ x y}}”)), Set(“x”)) test(bindingIds(WAE(“{with {z 2} 1}”)), Set(“z”))

<h2>3         Bound Identifiers</h2>

Implement the function boundIds, which is like freeIds, but the result set contains a string for each bound identifier in the given WAE.

def boundIds(expr: WAE): Set[String] = ???

test(boundIds(WAE(“{with {x 1} {+ x y}}”)), Set(“x”)) test(boundIds(WAE(“{with {z 2} 1}”)), Set())