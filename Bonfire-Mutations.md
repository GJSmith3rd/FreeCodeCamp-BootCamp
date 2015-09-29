## Contact me
**Gilbert Joseph Smith III**

![@gjsmith3rd](https://avatars0.githubusercontent.com/gjsmith3rd?&s=128)

[Github](https://github.com/gjsmith3rd) | [FreeCodeCamp](http://www.freecodecamp.com/gjsmith3rd) |  [CodePen](http://codepen.io/gjsmith3rd/) | [LinkedIn](https://www.linkedin.com/in/gjsmith3rd) | [Blog/Site](https://gjsmith3rd.github.io/) | [E-Mail](mailto:contact@mobileCreature.com)

# Details
- Difficulty: 1/5

Return true if the string in the first element of the array contains all of the letters of the string in the second element of the array.

For example, ['hello', 'Hello'], should return true because all of the letters in the second string are present in the first, ignoring case.

The arguments ['hello', 'hey'] should return false because the string 'hello' does not contain a 'y'.

Lastly, ['Alien', 'line'], should return true because all of the letters in 'line' are present in 'Alien'.

Remember to use [ Read-Search-Ask](http://github.com/FreeCodeCamp/freecodecamp/wiki/How-to-get-help-when-you-get-stuck) if you get stuck. Try to pair program. Write your own code.

## Useful Links
- [Array.indexOf()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf)

## Problem Script:

```js
function mutation(arr) {
  return arr;
}

mutation(['hello', 'hey']);
```

## Explanation:
You basically have to check if the string in the first parameter contains all the characters found on the second parameter.

## Hint: 1
First make the arguments lowercase and arrays so we can compare without having to worry about the case.

## Hint: 2
Use `inndexOf()` to check if the letter of the second word is on the first.

## Hint: 3
You will need a way to check if all the words are in the first one, like keeping a counter and checking for a default value.

## My code:

```js
function mutation(arr) {

    var first = arr[0].toLowerCase().split('');
    var second = arr[1].toLowerCase().split('');
    var temp = 0;
    // Check every character and if the index is found add one
    for (var s in second){
        if (first.indexOf(second[s]) > -1) {
            temp+= 0;
        } else
            temp+=1;
        }
    if (temp === 0)
        return true;
    else
        return false;
}
```

## My Code Explanation:
- take the first and second parameter and make them lowercase and split them by characters.
- Create a temp variable to keep count.
- For each letter in the second parameter, check if it is found on the first, if so then add 0 to the tamp variable, otherwise add 1.
- Outside the loop, if temp is 0 then return true, otherwise false, this acts as an on and off. If all the letters were added then we just get 0, otherwise there will be at least a `1` which means one letter was not found.

## [Go Home](https://github.com/Rafase282/My-FreeCodeCamp-Code/wiki)
