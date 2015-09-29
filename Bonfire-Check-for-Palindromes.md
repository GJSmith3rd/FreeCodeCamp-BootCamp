# Author
![@Rafase282](https://avatars0.githubusercontent.com/Rafase282?&s=128)

Submitted by Rafase282

[Github](https://github.com/Rafase282) | [FreeCodeCamp](http://www.freecodecamp.com/rafase282) | [CodePen](http://codepen.io/Rafase282/) | [LinkedIn](https://www.linkedin.com/in/rafase282) | [Blog/Site](https://rafase282.wordpress.com/) | [E-Mail](mailto:rafase282@gmail.com)

# Details
- Difficulty: 1/5

Return true if the given string is a palindrome. Otherwise, return false.

A palindrome is a word or sentence that's spelled the same way both forward and backward, ignoring punctuation, case, and spacing.

You'll need to remove punctuation and turn everything lower case in order to check for palindromes.

We'll pass strings with varying formats, such as "racecar", "RaceCar", and "race CAR" among others.

Remember to use [ Read-Search-Ask](http://github.com/FreeCodeCamp/freecodecamp/wiki/How-to-get-help-when-you-get-stuck) if you get stuck. Try to pair program. Write your own code.

## Useful Links
- [String.replace()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace)
- [String.toLowerCase()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/toLowerCase)

## Problem Script:

```js
function palindrome(str) {
  // Good luck!
  return true;
}
palindrome("eye");
```

## Explanation:
You have to check if the string you get as an input is a palindrome and return true if it is, and false otherwise.

## Hint: 1
Make sure to turn the string to lowercase.

## Hint: 2
You will need to use split() and join()

## Hint: 3
Using regular expressions to change to lowercase will make things easier and the code simpler.

## My code:

```Javascript
function palindrome(str) {
  var normalizedStr = str.replace(/[\W_]/g, '').toLowerCase();
  var reverseStr = normalizedStr.split('').reverse().join('');
  return normalizedStr === reverseStr;
}
```

## My Code Explanation:
We use regular expressions to replace any uppercase letter into a lowercase. Then we check if the string is the same as the reversed string using `split()` to split the original string by characters, then reverse and then join it back together.

## [Go Home](https://github.com/Rafase282/My-FreeCodeCamp-Code/wiki)
