## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

# Details
- Difficulty: 1/5

Reverse the provided string.

You may need to turn the string into an array before you can reverse it.

Your result must be a string.

Remember to use [ Read-Search-Ask](http://github.com/FreeCodeCamp/freecodecamp/wiki/How-to-get-help-when-you-get-stuck) if you get stuck. Try to pair program. Write your own code.

## Useful Links
- [Global String Object](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)
- [String.split()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)
- [Array.join()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)

## Problem Script:

```js
function reverseString(str) {
  return str;
}

reverseString('hello');
```

## Explanation:
You need to take the string and reverse it so if you had originally 'hello', it will turn into 'olleh'. Because you will need to split it, you will be working with Arrays too.

## Hint: 1
You should split the string by characters.

## Hint: 2
Find out about the built in function to reverse a string.

## Hint: 3
Once you have split and reversed, do not forget to join them back into one string.

## My code:

```js
function reverseString(str) {
  var strReverse = str.split('').reverse().join('');
  return strReverse;
}
```

## My Code Explanation:
This is a straightforward code. We create a variable that will hold the string split by characters, and then reversed and put back together.
