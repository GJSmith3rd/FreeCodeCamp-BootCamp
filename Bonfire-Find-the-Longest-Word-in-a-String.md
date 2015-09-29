# Author
![@Rafase282](https://avatars0.githubusercontent.com/Rafase282?&s=128)

Submitted by Rafase282

[Github](https://github.com/Rafase282) | [FreeCodeCamp](http://www.freecodecamp.com/rafase282) | [CodePen](http://codepen.io/Rafase282/) | [LinkedIn](https://www.linkedin.com/in/rafase282) | [Blog/Site](https://rafase282.wordpress.com/) | [E-Mail](mailto:rafase282@gmail.com)

# Details
- Difficulty: 1/5

Return the length of the longest word in the provided sentence.

Your response should be a number.

Remember to use [ Read-Search-Ask](http://github.com/FreeCodeCamp/freecodecamp/wiki/How-to-get-help-when-you-get-stuck) if you get stuck. Try to pair program. Write your own code.

## Useful Links
- [String.split()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
- [String.length](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/length)

## Problem Script:

```js
function findLongestWord(str) {
  return str.length;
}

findLongestWord('The quick brown fox jumped over the lazy dog');
```

## Explanation:
You have to go through each word and figure out which one is the longest and return not the word, but how many characters does it has.

## Hint: 1
You should split the string into an array of words.

## Hint: 2
You will need to figure out a way to keep track globally of the greatest current length.

## Hint: 3
Remember how to get the length of elements on the array? `Array[index].length`

## My code:

```js
function findLongestWord(str) {
  var words = str.split(' ');
  var maxLength = 0;

  for (var i = 0; i < words.length; i++) {
    if (words[i].length > maxLength) {
      maxLength = words[i].length;
    }
  }

  return maxLength;
}
```

## My Code Explanation:
Take the string and convert it into an array of words. Declare a variable to keep track of the maximum length and loop from 0 to the length of the array of words.

Then check for the longest word by comparing the current word to the previous one and storing the new longest word. At the end of the loop just return the number value of the variable maxLength.

## [Go Home](https://github.com/Rafase282/My-FreeCodeCamp-Code/wiki)
