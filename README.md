# xmath.js
XMath library (and friends) for supplemental math functions (outside of JS Math class) built for projecteuler questions. These have both common and useful implementations

- Sequence Generators
    - XMath.factorial(n);               // returns the factorial of `n`
    - XMath.eSieve(n);                  // finds primes up to `n` using the sieve of eratosthenes
    - XMath.fibonacci(n);               // finds the `n`th fibonacci sequence term
    - XMath.findCombos(arr [, str]);    // returns all permutations of `arr`'s values, starting with optional string `str`
- Testers
    - XMath.isPrime(n);                 // checks if a number `n` is prime using trial division
    - XMath.isPalindrome(n);            // checks if a number or string `n` is a palindrome
- Modifiers
    - XMath.merge(arr1, arr2, mergeBy)  // returns an array of all possibilities of `arr1` and `arr2` values merged together when the last `mergeBy` characters of the `arr1` values equal the first `mergeBy` characters of the `arr2` values
    - XMath.pad(n, pad, length, before) // pads a number or string `n` with `pad` characters. `before` is an optional variable determing whether to prepend ("true", default) or append ("false") 
