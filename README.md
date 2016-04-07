# xmath.js
JavaScript XMath library (and friends) for supplemental math functions (outside of the Math class) built for [Project Euler](https://projecteuler.net/) questions. These have both common and useful implementations.
<table>
<tr>
	<td><code>xmath.js</code></td>
	<td><code>XMath</code></td>
	<td>Main library. Common math operations</td>
</tr>
<tr>
	<td><code>xfraction.js</code></td>
	<td><code>XFraction</code></td>
	<td>Handles simple operations when working with fractions</td>
</tr>
<tr>
	<td><code>xbigfraction.js</code></td>
	<td><code>XBigFraction</code></td>
	<td>BigNumber implementation for <code>xfraction.js</code>. All input and output fractions are of the type <code>BigNumber</code> (therefore, needs dependency <a href="https://github.com/MikeMcl/bignumber.js/blob/master/bignumber.js"><code>bignumber.js</code</a>)</td>
</tr>
</table>

#### Usage
Download the desired file(s) into the desired directory (to do this, find the class of the function and match it to the corresponding file with the chart above). Include in a regular `<script>` tag (before the script that uses the functions). Start math-ing away!

Example: `isPrime()` usage:

`XMath.isPrime()` means it is in class `XMath`. `XMath` is located in file `xmath.js`. Download `xmath.js` and run it:

```javascript
<script src="xmath.js"></script>
<script>
    console.log(XMath.isPrime(313062169711));
    // outputs "true"
</script>
```

# Documentation
**Note**: A *ClassName* in italics represents an instance of a class. For example, make sure not to confuse the static function `XMath.factorial(n)` (which is a class function that performs an operation on `n`)) with an object method, such as <em>`XFraction`</em>`.reduce()` (which is performed on an `XFraction` instance).

#### Sequence Generators
<table>
<tr>
	<td> <code>XMath.factorial(n);</code></td>
	<td>Return the factorial of <code>n</code></td>
</tr>
<tr>
	<td> <code>XMath.eSieve(n);</code></td>
	<td>Find primes up to <code>n</code> using the <a href="https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes">Sieve of Eratosthenes</a></td>
</tr>
<tr>
	<td> <code>XMath.fibonacci(n);</code></td>
	<td>Find the <code>n</code>th <a href="https://en.wikipedia.org/wiki/Fibonacci_number">Fibonacci sequence</a> term</td>
</tr>
<tr>
	<td> <code>XMath.findCombos(arr [,str]);</code></td>
	<td>Get all permutations of <code>arr</code>'s values, starting with optional string <code>str</code></td>
</tr>
<tr>
	<td> <code>XMath.factorial(n);</code></td>
	<td>Return the factorial of <code>n</code></td>
</tr>
</table>

#### Testers
<table>
<tr>
	<td> <code>XMath.isPrime(n);</code></td>
	<td>Returns <code>true</code> if <code>n</code> is prime, <code>false</code> if not</td>
</tr>
<tr>
	<td> <code>XMath.isPalindrome(n);</code></td>
	<td>Returns <code>true</code> if <code>n</code> (number or string) is a palindrome</td>
</tr>
</table>

#### Modifiers
<table>
<tr>
	<td> <code>XMath.merge(arr1, arr2, mergeBy);</code></td>
	<td>Returns an array of all possibilities of <code>arr1</code> and <code>arr2</code> values merged together when the last <code>mergeBy</code> characters of the <code>arr1</code> values equal the first <code>mergeBy</code> characters of the <code>arr2</code> values</td>
</tr>
<tr>
	<td> <code>XMath.pad(n, pad, length [, before]);</code></td>
	<td>Pads a number or string <code>n</code> with <code>pad</code> number of characters. <code>before</code> is an optional parameter determining whether or not to prepend the padding (<code>true</code>, default value) or append(<code>false</code>)</td>
</tr>
</table>

#### Fractions
**Note**: For all of these, `XBigFraction` can replace `XFraction`; just make sure to include the right file (`xbigfraction.js`) and its dependency ([`bignumber.js`](https://github.com/MikeMcl/bignumber.js/blob/master/bignumber.js)).
<table>
<tr>
	<td><code>new XFraction(numerator, denominator)</code></td>
	<td>Create a new <code>XFraction</code> instance</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.multiply(fraction)</code></td>
	<td>Multiplies fraction with <code>fraction</code>.</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.divide(fraction)</code></td>
	<td>Divides fraction by <code>fraction</code>.</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.add(fraction)</code></td>
	<td>Adds fraction to <code>fraction</code>.</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.subtract(fraction)</code></td>
	<td>Subtracts <code>fraction</code> from fraction.</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.reduce()</code></td>
	<td>Simplifies fraction.</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.toString()</code></td>
	<td>Returns string representation of fraction (<code>"numerator/denominator"</code>).</td>
</tr>
<tr>
	<td><code><em>XFraction</em>.toDecimal()</code></td>
	<td>Returns decimal representation of fraction (<code>(Number) numerator/denominator</code>)</td>
</tr>
</table>
