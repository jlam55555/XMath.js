# xmath.js
JavaScript XMath library (and friends) for supplemental math functions (outside of the Math class) built for [Project Euler](https://projecteuler.net/) questions. These have both common and useful implementations

#### Usage
Download the `xmath.js` file into the desired directory, include in a regular `<script>` tag (before the script that uses the functions), and start math-ing away!

    <script src="xmath.js"></script>
    <script>
	    console.log(XMath.isPrime(313062169711));
	    // outputs "true"
    </script>

#### Sequence Generators
<table>
<tbody>
<tr>
	<td> <code>XMath.factorial(n);</code></td>
	<td>Return the factorial of <code>n</code></td>
</tr>
<tr>
	<td> <code>XMath.eSieve(n);</code></td>
	<td>Find primes up to `n` using the <a href="https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes>Sieve of Eratosthenes</a></td>
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
	<td>Return the factorial of `n`</td>
</tr>
</tbody>
</table>

#### Testers
<table>
<tbody>
<tr>
	<td> <code>XMath.isPrime(n);</code></td>
	<td>Returns <code>true</code> if <code>n</code> is prime, <code>false</code> if not</td>
</tr>
<tr>
	<td> <code>XMath.isPalindrome(n);</code></td>
	<td>Returns <code>true</code> if <code>n</code> (number or string) is a palindrome</td>
</tr>
</tbody>
</table>

#### Modifiers
<table>
<tbody>
<tr>
	<td> <code>XMath.merge(arr1, arr2, mergeBy);</code></td>
	<td>Returns an array of all possibilities of <code>arr1</code> and <code>arr2</code> values merged together when the last <code>mergeBy</code> characters of the <code>arr1</code> values equal the first <code>mergeBy</code> characters of the <code>arr2</code> values</td>
</tr>
<tr>
	<td> <code>XMath.pad(n, pad, length [, before]);</code></td>
	<td>Pads a number or string <code>n</code> with <code>pad</code> number of characters. <code>before</code> is an optional parameter determining whether or not to prepend the padding (<code>true</code>, default value) or append(<code>false</code>)</td>
</tr>
</tbody>
</table>
