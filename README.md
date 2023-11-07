# _Perfectness_
The perfectest programming language
## Comments
Many programming languages use `//` for comments, but that's kind of confusing.<br>
To fix this, _Perfectness_ uses two of the "Speech Balloon" emoji, like `💬💬` (which makes much more sense).
```
💬💬 This is a comment!
```
This is similar for multiline comments. You just use `💬* *💬`.
```
💬*
This is a multiline comment!
*💬
💬**
* This is a PerfectDoc comment!
*💬
```
## Semicolons
Because people always seem to forget semicolons, _Perfectness_ has a simple fix: Semicolons are not allowed.
```java
x = 1; 💬💬 Syntax Error: Semicolons are not allowed
```
## Variables
When creating a variable, you can type: 
- `var` (optional)
- Modifiers (optional)
- A Type (optional)
- The name of the variable
-  `=` followed by a value (optional)
```java
a = 1
Int b 2
var c = 3
var Int d = 4
```
### Modifiers
There are many modifiers you can use:
```java
const e = 5 💬💬no editing
const Int f = 6
final g 💬💬
public h
protected i
private j
package k
static l
readonly m 💬💬no assigning
let n 💬💬no recreating
```
You can also combine modifiers:
```java
public static final readonly const let var Int x = 100
```
### Naming
You can name variables with almost any characters:
```java
var a = 1
var FRUIT = 'banana'
```
This includes spaces, special characters, and Unicode characters:
```java
var String my name = 'Bob'
var 1/2 = 0.5
var 😀 = 'Smiley Face'
```
You can also name variables with primitive values like numbers:
```java
var 1 = 2
output(1) = 2
output(2 - 1) = 0
output(3 - 2) = 1
output(-1) = -2
```
## Types
### Basic Types
#### Booleans
A bit can be `0` or `1`.

A boolean can be `true`, `false`, or `maybe` (just like in [DreamBerd](https://github.com/TodePond/DreamBerd)).<br>
These are all valid booleans: `false`, `maybe`, `true`.

**Info:** Booleans are stored as one and a half bits (just like in [DreamBerd](https://github.com/TodePond/DreamBerd)).
##### Maybe
`maybe` will be `true` half of the time, and `false` the other half.
```java
if (maybe) {
 output('The maybe was true.')
} else {
 output('The maybe was false.')
}
```
However, this does not apply to `if/else/perhaps` statements:
```java
if (maybe) {
 output('This will never run.')
} else {
 output('This will never run.')
} perhaps {
 output('This will always run.')
}
```
In an `if/perhaps` statement, `false` won't run anything, `true` will run the `if` part, and `maybe` will run the `perhaps` part.
```java
if (condition) {
 output('This will run when true.')
} perhaps {
 output('This will run when maybe.')
}
```
##### Chance
The `chance(n)` function returns a `Chance`, which is basically a boolean with about an `n` chance of being `true`.<br>
In the following code, the if statement will only run 10% of the time:
```java
if (chance(0.1)) {
 output('There was a 1/10 chance of this happening!')
}
```
You can also set a variable to a chance:
```java
var Chance ch = chance(0.25)
output(ch) 💬💬This will be true 25% of the time, and false 75% of the time.
```
`Chance`s will never be `maybe`.
**Note:** the behavior of a `Chance` in an `if/perhaps` or `if/else/perhaps` statement is undefined.
#### Numbers
- Bytes - `10`
- Integers - `123456`
- Longs - `10000000000l`
- Floats - `123.45`
- Doubles - `123.45`
#### Strings
Because Windows does not allow double quotes in file names, all strings must use single quotes:
```java
output("Hi") 💬💬 Syntax Error: Windows filenames can't contain double quotes
output('Hello') = 'Hello'
```
### Casting
To cast a
### Note about Types
```java
expect Boolean = Bit[8] = Byte
expect Byte = Bit[1.5]
expect Int = Bit[32] = Byte[4]
expect Long = Bit[64] = Byte[8] = Int[2]
expect Float = Bit[32] = Byte[4] = Int
expect Double = Bit[64] = Byte[8] = Float[2] = Long
```
## Objects
### Lists
You can make an array of values:
```java
Array x = [1, 'apple', false]
Int[] y = [1, 2, 3]
```
When creating an array, you can specify a length of the created array. This can also include floats, strings, and other arrays:
```java
Boolean[] a = new Boolean[3]
Int[5] b = [1, 2, 3, 4] 💬💬 Type Error: Array [1, 2, 3, 4] has wrong length for Int[5]

Float[] c = new Float[2.4]
Double[] d = new Double['cat']
String[] e = new String[[1, 2, 3]]
```
You will still get the correct lengths:
```java
output(c.length) 💬💬 2.4
output(d.length) 💬💬 'cat'
output(e.length) 💬💬 [1, 2, 3]
```
### Maps
You can create maps in a similar way to arrays:
```java
Map f = [a = 1, b = 2, c = 'dog']
Map<Int>
```

## Console
```java
console.say(message)
console.warn(message)
console.error(message)

output(123 * 456)
```
## Assertions
In some programming languges, you can use the `assert` keyword to confirm that something is true. However, this word is very rarely used in real life. Instead, _Perfectness_ uses the `expect` keyword.
```java
expect 1 + 1 = 2
```
If the value of the condition is not what you expected, just use the `assume` keyword to make it true for you.
All of these are true.
```java
assume 1 + 2 = 5
output(1 + 1) = 2
output(1 + 2) = 5
output(1 + (1 + 1)) = 5
output(1 + 3) = 4
output(3) = 3
output(2 + 1) = 3

assume false
output(false) = true
output(1 = 2) = true
output(1 > 2) = true
output(!true) = true
assume false = !true
output(false) = true
output(true = false) = true
```
## Math
Addition and subtraction are the same as in most other programming languages:
```java
output(1 + 1) = 2
output(1 - 1) = 0
```
However, this is not the case for multiplication and division:
```java
output(1 * 1) 💬💬 Syntax Error: Unknown symbol '*'
output(1 / 1) 💬💬 Syntax Error: Unknown symbol '/'
```
Because the meaning of `*` for multiplying and `/` for dividing is not very obvious, use the characters meant for those operations instead:
```java
output(1 × 2) = 1
output(1 ÷ 2) = 0.5
```

## Classes
class Example
 
!
