## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

# Details
- Difficulty: 1/5

Return the remaining elements of an array after chopping off n elements from the head.

Remember to use [ Read-Search-Ask](http://github.com/FreeCodeCamp/freecodecamp/wiki/How-to-get-help-when-you-get-stuck) if you get stuck. Try to pair program. Write your own code.

## Useful Links
- [Array.slice()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice)
- [Array.splice()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)

## Problem Script:

```js
function slasher(arr, howMany) {
  // it doesn't always pay to be first
  return arr;
}

slasher([1, 2, 3], 2);
```

## Explanation:
We have to take an array and delete as many elements from the beginning as stated by the second parameter.

## Hint: 1
It can be done in one line with slice.

## Hint: 2
If you want you can try to use splice but slice is enough.

## Hint: 3
Really? Splice by the number of the second parameter.

## My code:

```js
function slasher(arr, howMany) {
  return arr.slice(howMany);
}
```

## My Code Explanation:
Slice the array by the about of the second parameter.

## [Go Home](https://github.com/Rafase282/My-FreeCodeCamp-Code/wiki)
